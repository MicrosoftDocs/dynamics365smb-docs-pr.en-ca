---
title: Design Details - Demand and Supply | Microsoft Docs
description: Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order. In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 983fbb1a4ce652900185010800474b80350f193d
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="1c688-104">Design Details: Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="1c688-104">Design Details: Demand and Supply</span></span>
<span data-ttu-id="1c688-105">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span><span class="sxs-lookup"><span data-stu-id="1c688-105">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="1c688-106">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span><span class="sxs-lookup"><span data-stu-id="1c688-106">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
 <span data-ttu-id="1c688-107">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span><span class="sxs-lookup"><span data-stu-id="1c688-107">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="1c688-108">In addition, a sales return may also represent supply.</span><span class="sxs-lookup"><span data-stu-id="1c688-108">In addition, a sales return may also represent supply.</span></span>  
  
 <span data-ttu-id="1c688-109">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span><span class="sxs-lookup"><span data-stu-id="1c688-109">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="1c688-110">One profile holds demand events, and the other holds the corresponding supply events.</span><span class="sxs-lookup"><span data-stu-id="1c688-110">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="1c688-111">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span><span class="sxs-lookup"><span data-stu-id="1c688-111">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
 <span data-ttu-id="1c688-112">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span><span class="sxs-lookup"><span data-stu-id="1c688-112">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
 <span data-ttu-id="1c688-113">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span><span class="sxs-lookup"><span data-stu-id="1c688-113">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="1c688-114">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="1c688-114">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="1c688-115">See Also</span><span class="sxs-lookup"><span data-stu-id="1c688-115">See Also</span></span>  
 <span data-ttu-id="1c688-116">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="1c688-116">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="1c688-117">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="1c688-117">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="1c688-118">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="1c688-118">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)