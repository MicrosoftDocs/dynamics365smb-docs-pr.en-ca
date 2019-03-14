---
title: How to Enable Picking by FEFO | Microsoft Docs
description: First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.
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
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: e21ff28a472391ea19bc393ecfee017e7aa668f1
ms.contentlocale: en-ca
ms.lasthandoff: 04/16/2018

---
# <a name="enable-picking-items-by-fefo"></a><span data-ttu-id="c6056-103">Enable Picking Items by FEFO</span><span class="sxs-lookup"><span data-stu-id="c6056-103">Enable Picking Items by FEFO</span></span>
<span data-ttu-id="c6056-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span><span class="sxs-lookup"><span data-stu-id="c6056-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span></span>  

 <span data-ttu-id="c6056-105">This functionality only works when the following criteria are met:</span><span class="sxs-lookup"><span data-stu-id="c6056-105">This functionality only works when the following criteria are met:</span></span>  

- <span data-ttu-id="c6056-106">The item must have a serial/lot number.</span><span class="sxs-lookup"><span data-stu-id="c6056-106">The item must have a serial/lot number.</span></span>  
- <span data-ttu-id="c6056-107">On the item’s item tracking code setup, the **SN-Specific Warehouse Tracking** field or the **Lot-Specific Warehouse Tracking** field must be selected.</span><span class="sxs-lookup"><span data-stu-id="c6056-107">On the item’s item tracking code setup, the **SN-Specific Warehouse Tracking** field or the **Lot-Specific Warehouse Tracking** field must be selected.</span></span>  
- <span data-ttu-id="c6056-108">The item must be posted to inventory with an expiration date.</span><span class="sxs-lookup"><span data-stu-id="c6056-108">The item must be posted to inventory with an expiration date.</span></span>  
- <span data-ttu-id="c6056-109">On the location card, the **Require Pick** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="c6056-109">On the location card, the **Require Pick** check box must be selected.</span></span>  
- <span data-ttu-id="c6056-110">On the location card, the **Pick According to FEFO** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="c6056-110">On the location card, the **Pick According to FEFO** check box must be selected.</span></span>  
- <span data-ttu-id="c6056-111">On the location card, the **Bin Mandatory** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="c6056-111">On the location card, the **Bin Mandatory** check box must be selected.</span></span>  

  <span data-ttu-id="c6056-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span><span class="sxs-lookup"><span data-stu-id="c6056-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c6056-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="c6056-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span></span>  

 <span data-ttu-id="c6056-114">If two serial/lot-numbered items have the same expiration date, then the program selects the item with the lowest serial or lot number.</span><span class="sxs-lookup"><span data-stu-id="c6056-114">If two serial/lot-numbered items have the same expiration date, then the program selects the item with the lowest serial or lot number.</span></span> <span data-ttu-id="c6056-115">If the serial or lot numbers are the same, then the program selects the item that was registered first.</span><span class="sxs-lookup"><span data-stu-id="c6056-115">If the serial or lot numbers are the same, then the program selects the item that was registered first.</span></span>  

> [!NOTE]
> - <span data-ttu-id="c6056-116">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="c6056-116">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span></span>  
>   -   <span data-ttu-id="c6056-117">To enable movements according to FEFO, either in the **Inventory Movement** window or the **Movement Worksheet** window, you must leave the **From Bin** field empty.</span><span class="sxs-lookup"><span data-stu-id="c6056-117">To enable movements according to FEFO, either in the **Inventory Movement** window or the **Movement Worksheet** window, you must leave the **From Bin** field empty.</span></span>  
>   -   <span data-ttu-id="c6056-118">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span><span class="sxs-lookup"><span data-stu-id="c6056-118">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span></span> <span data-ttu-id="c6056-119">This applies even if you are not using Pick according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="c6056-119">This applies even if you are not using Pick according to FEFO.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c6056-120">See Also</span><span class="sxs-lookup"><span data-stu-id="c6056-120">See Also</span></span>  
<span data-ttu-id="c6056-121">[Picking Items](warehouse-pick-items.md) </span><span class="sxs-lookup"><span data-stu-id="c6056-121">[Picking Items](warehouse-pick-items.md) </span></span>  
<span data-ttu-id="c6056-122">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="c6056-122">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
<span data-ttu-id="c6056-123">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="c6056-123">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
[<span data-ttu-id="c6056-124">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="c6056-124">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
[<span data-ttu-id="c6056-125">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="c6056-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="c6056-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c6056-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
