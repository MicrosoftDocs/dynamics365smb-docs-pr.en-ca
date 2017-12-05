---
title: Design Details - Closing Demand and Supply | Microsoft Docs
description: This topic provides a suggestion for what to do after you perform supply balancing procedures.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, planning, example, closing, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0796865fa5b04630cc3ac68a63cc8113664a2d24
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-closing-demand-and-supply"></a><span data-ttu-id="3fe61-103">Design Details: Closing Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="3fe61-103">Design Details: Closing Demand and Supply</span></span>
<span data-ttu-id="3fe61-104">When the supply balancing procedures have been performed, there are three possible end situations:</span><span class="sxs-lookup"><span data-stu-id="3fe61-104">When the supply balancing procedures have been performed, there are three possible end situations:</span></span>  
  
* <span data-ttu-id="3fe61-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span><span class="sxs-lookup"><span data-stu-id="3fe61-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span></span> <span data-ttu-id="3fe61-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span><span class="sxs-lookup"><span data-stu-id="3fe61-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span></span>  
* <span data-ttu-id="3fe61-107">The supply order cannot be modified to cover all of the demand.</span><span class="sxs-lookup"><span data-stu-id="3fe61-107">The supply order cannot be modified to cover all of the demand.</span></span> <span data-ttu-id="3fe61-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span><span class="sxs-lookup"><span data-stu-id="3fe61-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span></span> <span data-ttu-id="3fe61-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span><span class="sxs-lookup"><span data-stu-id="3fe61-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span></span>  
* <span data-ttu-id="3fe61-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span><span class="sxs-lookup"><span data-stu-id="3fe61-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span></span> <span data-ttu-id="3fe61-111">If there is any surplus supply, it may be decreased (or cancelled) and then closed.</span><span class="sxs-lookup"><span data-stu-id="3fe61-111">If there is any surplus supply, it may be decreased (or canceled) and then closed.</span></span> <span data-ttu-id="3fe61-112">It is possible that additional supply events exist further along in the chain, and they should also be cancelled.</span><span class="sxs-lookup"><span data-stu-id="3fe61-112">It is possible that additional supply events exist further along in the chain, and they should also be canceled.</span></span>  
  
<span data-ttu-id="3fe61-113">Last, the planning system will create an order tracking link between the supply and the demand.</span><span class="sxs-lookup"><span data-stu-id="3fe61-113">Last, the planning system will create an order tracking link between the supply and the demand.</span></span>  
  
## <a name="creating-the-planning-line-suggested-action"></a><span data-ttu-id="3fe61-114">Creating the Planning Line (Suggested Action)</span><span class="sxs-lookup"><span data-stu-id="3fe61-114">Creating the Planning Line (Suggested Action)</span></span>  
<span data-ttu-id="3fe61-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span><span class="sxs-lookup"><span data-stu-id="3fe61-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span></span> <span data-ttu-id="3fe61-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span><span class="sxs-lookup"><span data-stu-id="3fe61-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span></span> <span data-ttu-id="3fe61-117">This means that when first created, the planning line may be changed again.</span><span class="sxs-lookup"><span data-stu-id="3fe61-117">This means that when first created, the planning line may be changed again.</span></span>  
  
<span data-ttu-id="3fe61-118">To minimize database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span><span class="sxs-lookup"><span data-stu-id="3fe61-118">To minimize database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span></span>  
  
* <span data-ttu-id="3fe61-119">Create only the planning line with the current due date and quantity but without the routing and components.</span><span class="sxs-lookup"><span data-stu-id="3fe61-119">Create only the planning line with the current due date and quantity but without the routing and components.</span></span>  
* <span data-ttu-id="3fe61-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span><span class="sxs-lookup"><span data-stu-id="3fe61-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span></span> <span data-ttu-id="3fe61-121">This is demanding in terms of database accesses.</span><span class="sxs-lookup"><span data-stu-id="3fe61-121">This is demanding in terms of database accesses.</span></span> <span data-ttu-id="3fe61-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span><span class="sxs-lookup"><span data-stu-id="3fe61-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span></span>  
* <span data-ttu-id="3fe61-123">Include BOM explosion: this can wait until just before the supply event is closed.</span><span class="sxs-lookup"><span data-stu-id="3fe61-123">Include BOM explosion: this can wait until just before the supply event is closed.</span></span>  
  
<span data-ttu-id="3fe61-124">This concludes the descriptions of how demand and supply is loaded, prioritized, and balanced by the planning system.</span><span class="sxs-lookup"><span data-stu-id="3fe61-124">This concludes the descriptions of how demand and supply is loaded, prioritized, and balanced by the planning system.</span></span> <span data-ttu-id="3fe61-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span><span class="sxs-lookup"><span data-stu-id="3fe61-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="3fe61-126">See Also</span><span class="sxs-lookup"><span data-stu-id="3fe61-126">See Also</span></span>  
<span data-ttu-id="3fe61-127">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="3fe61-127">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="3fe61-128">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="3fe61-128">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="3fe61-129">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="3fe61-129">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)