---
title: Design Details - Monitoring the Projected Inventory Level and the Reorder Point | Microsoft Docs
description: Learn how inventory planning distinguishes between projected inventory and projected available inventory levels.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: a0e64d96389739c67a9e9f548958fac12e3aca2a
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-monitoring-the-projected-inventory-level-and-the-reorder-point"></a><span data-ttu-id="85524-103">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span><span class="sxs-lookup"><span data-stu-id="85524-103">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>
<span data-ttu-id="85524-104">Inventory is a type of supply, but for inventory planning, the planning system distinguishes between two inventory levels:</span><span class="sxs-lookup"><span data-stu-id="85524-104">Inventory is a type of supply, but for inventory planning, the planning system distinguishes between two inventory levels:</span></span>  

* <span data-ttu-id="85524-105">Projected inventory</span><span class="sxs-lookup"><span data-stu-id="85524-105">Projected inventory</span></span>  
* <span data-ttu-id="85524-106">Projected available inventory</span><span class="sxs-lookup"><span data-stu-id="85524-106">Projected available inventory</span></span>  

## <a name="projected-inventory"></a><span data-ttu-id="85524-107">Projected Inventory</span><span class="sxs-lookup"><span data-stu-id="85524-107">Projected Inventory</span></span>  
<span data-ttu-id="85524-108">Initially, projected inventory is the quantity of gross inventory, including supply and demand in the past even if not posted, when starting the planning process.</span><span class="sxs-lookup"><span data-stu-id="85524-108">Initially, projected inventory is the quantity of gross inventory, including supply and demand in the past even if not posted, when starting the planning process.</span></span> <span data-ttu-id="85524-109">In the future, this becomes a moving projected inventory level that is maintained by gross quantities from future supply and demand because those are introduced along the time line (whether reserved or in other ways allocated).</span><span class="sxs-lookup"><span data-stu-id="85524-109">In the future, this becomes a moving projected inventory level that is maintained by gross quantities from future supply and demand because those are introduced along the time line (whether reserved or in other ways allocated).</span></span>  

<span data-ttu-id="85524-110">The projected inventory is used by the planning system to monitor the reorder point and to determine the reorder quantity when using the Maximum Qty. reordering policy.</span><span class="sxs-lookup"><span data-stu-id="85524-110">The projected inventory is used by the planning system to monitor the reorder point and to determine the reorder quantity when using the Maximum Qty. reordering policy.</span></span>  

## <a name="projected-available-inventory"></a><span data-ttu-id="85524-111">Projected Available Inventory</span><span class="sxs-lookup"><span data-stu-id="85524-111">Projected Available Inventory</span></span>  
<span data-ttu-id="85524-112">The projected available inventory is the part of the projected inventory that at a given point in time is available to fulfill demand.</span><span class="sxs-lookup"><span data-stu-id="85524-112">The projected available inventory is the part of the projected inventory that at a given point in time is available to fulfill demand.</span></span> <span data-ttu-id="85524-113">The projected available inventory is used by the planning engine when monitoring the safety stock level.</span><span class="sxs-lookup"><span data-stu-id="85524-113">The projected available inventory is used by the planning engine when monitoring the safety stock level.</span></span>  

<span data-ttu-id="85524-114">The projected available inventory is used by the planning system to monitor the safety stock level, since the safety stock must always be available to serve unexpected demand.</span><span class="sxs-lookup"><span data-stu-id="85524-114">The projected available inventory is used by the planning system to monitor the safety stock level, since the safety stock must always be available to serve unexpected demand.</span></span>  

## <a name="time-buckets"></a><span data-ttu-id="85524-115">Time Buckets</span><span class="sxs-lookup"><span data-stu-id="85524-115">Time Buckets</span></span>  
<span data-ttu-id="85524-116">Having a tight control of the projected inventory is crucial to detect when the reorder point is reached or crossed and to calculate the right order quantity when using the Maximum Qty. reordering policy.</span><span class="sxs-lookup"><span data-stu-id="85524-116">Having a tight control of the projected inventory is crucial to detect when the reorder point is reached or crossed and to calculate the right order quantity when using the Maximum Qty. reordering policy.</span></span>  

<span data-ttu-id="85524-117">As stated earlier, the projected inventory level is calculated at the start of the planning period.</span><span class="sxs-lookup"><span data-stu-id="85524-117">As stated earlier, the projected inventory level is calculated at the start of the planning period.</span></span> <span data-ttu-id="85524-118">It is a gross level that does not consider reservations and similar allocations.</span><span class="sxs-lookup"><span data-stu-id="85524-118">It is a gross level that does not consider reservations and similar allocations.</span></span> <span data-ttu-id="85524-119">To monitor this inventory level during the planning sequence, the system monitors the aggregated changes over a period of time, a time bucket.</span><span class="sxs-lookup"><span data-stu-id="85524-119">To monitor this inventory level during the planning sequence, the system monitors the aggregated changes over a period of time, a time bucket.</span></span> <span data-ttu-id="85524-120">The system ensures that the time bucket is at least one day since it is the most precise unit of time for a demand or supply event.</span><span class="sxs-lookup"><span data-stu-id="85524-120">The system ensures that the time bucket is at least one day since it is the most precise unit of time for a demand or supply event.</span></span>  

## <a name="determining-the-projected-inventory-level"></a><span data-ttu-id="85524-121">Determining the Projected Inventory Level</span><span class="sxs-lookup"><span data-stu-id="85524-121">Determining the Projected Inventory Level</span></span>  
<span data-ttu-id="85524-122">The following sequence describes how the projected inventory level is determined:</span><span class="sxs-lookup"><span data-stu-id="85524-122">The following sequence describes how the projected inventory level is determined:</span></span>  

* <span data-ttu-id="85524-123">When a supply event, such as a purchase order has been totally planned, it will increase the projected inventory on its due date.</span><span class="sxs-lookup"><span data-stu-id="85524-123">When a supply event, such as a purchase order has been totally planned, it will increase the projected inventory on its due date.</span></span>  
* <span data-ttu-id="85524-124">When a demand event has been fully satisfied, it will not decrease the projected inventory right away.</span><span class="sxs-lookup"><span data-stu-id="85524-124">When a demand event has been fully satisfied, it will not decrease the projected inventory right away.</span></span> <span data-ttu-id="85524-125">Instead, it posts a decrease reminder, which is an internal record that holds the date and quantity of the contribution to the projected inventory.</span><span class="sxs-lookup"><span data-stu-id="85524-125">Instead, it posts a decrease reminder, which is an internal record that holds the date and quantity of the contribution to the projected inventory.</span></span>  
* <span data-ttu-id="85524-126">When a subsequent supply event is planned and placed on the time line, the posted decrease reminders are investigated one by one up until the planned date of the supply while updating the projected inventory.</span><span class="sxs-lookup"><span data-stu-id="85524-126">When a subsequent supply event is planned and placed on the time line, the posted decrease reminders are investigated one by one up until the planned date of the supply while updating the projected inventory.</span></span> <span data-ttu-id="85524-127">During this process, the reorder point level of the internal increase reminder may be reached or crossed.</span><span class="sxs-lookup"><span data-stu-id="85524-127">During this process, the reorder point level of the internal increase reminder may be reached or crossed.</span></span>  
* <span data-ttu-id="85524-128">If a new supply order is introduced, the system checks if it is entered before the current supply.</span><span class="sxs-lookup"><span data-stu-id="85524-128">If a new supply order is introduced, the system checks if it is entered before the current supply.</span></span> <span data-ttu-id="85524-129">If it is, the new supply becomes current supply and the balancing procedure starts over.</span><span class="sxs-lookup"><span data-stu-id="85524-129">If it is, the new supply becomes current supply and the balancing procedure starts over.</span></span>  

<span data-ttu-id="85524-130">The following shows a graphical illustration of this principle:</span><span class="sxs-lookup"><span data-stu-id="85524-130">The following shows a graphical illustration of this principle:</span></span>  

![](media/nav_app_supply_planning_2_projected_inventory.png "NAV_APP_supply_planning_2_projected_inventory")  

1. <span data-ttu-id="85524-131">Supply **Sa** of 4 (fixed) closes Demand **Da** of -3.</span><span class="sxs-lookup"><span data-stu-id="85524-131">Supply **Sa** of 4 (fixed) closes Demand **Da** of -3.</span></span>  
2. <span data-ttu-id="85524-132">CloseDemand: Create a decrease reminder of -3 (not shown).</span><span class="sxs-lookup"><span data-stu-id="85524-132">CloseDemand: Create a decrease reminder of -3 (not shown).</span></span>  
3. <span data-ttu-id="85524-133">Supply **Sa** is closed with a surplus of 1 (no more demand exists).</span><span class="sxs-lookup"><span data-stu-id="85524-133">Supply **Sa** is closed with a surplus of 1 (no more demand exists).</span></span>  

     <span data-ttu-id="85524-134">This increases the projected inventory level to +4, while the projected **available** inventory becomes -1.</span><span class="sxs-lookup"><span data-stu-id="85524-134">This increases the projected inventory level to +4, while the projected **available** inventory becomes -1.</span></span>  

4. <span data-ttu-id="85524-135">The next supply **Sb** of 2 (another order) has already been placed on the timeline.</span><span class="sxs-lookup"><span data-stu-id="85524-135">The next supply **Sb** of 2 (another order) has already been placed on the timeline.</span></span>  
5. <span data-ttu-id="85524-136">System checks if there is any decrease reminder preceding **Sb** (there is not, so no action is taken).</span><span class="sxs-lookup"><span data-stu-id="85524-136">System checks if there is any decrease reminder preceding **Sb** (there is not, so no action is taken).</span></span>  
6. <span data-ttu-id="85524-137">System closes supply **Sb** (no more demand exists)—either A: by reducing it to 0 (cancel) or B: by leaving as is.</span><span class="sxs-lookup"><span data-stu-id="85524-137">System closes supply **Sb** (no more demand exists)—either A: by reducing it to 0 (cancel) or B: by leaving as is.</span></span>  

     <span data-ttu-id="85524-138">This increases the projected inventory level (A: +0 => +4 or B: +2 = +6).</span><span class="sxs-lookup"><span data-stu-id="85524-138">This increases the projected inventory level (A: +0 => +4 or B: +2 = +6).</span></span>  

7. <span data-ttu-id="85524-139">System makes a final check: Is there any decrease reminder?</span><span class="sxs-lookup"><span data-stu-id="85524-139">System makes a final check: Is there any decrease reminder?</span></span> <span data-ttu-id="85524-140">Yes, there is one on the date of **Da**.</span><span class="sxs-lookup"><span data-stu-id="85524-140">Yes, there is one on the date of **Da**.</span></span>  
8. <span data-ttu-id="85524-141">System adds the decrease reminder of -3 reminder to the projected inventory level, either A: +4 -3 = 1 or B: +6 -3 = +3.</span><span class="sxs-lookup"><span data-stu-id="85524-141">System adds the decrease reminder of -3 reminder to the projected inventory level, either A: +4 -3 = 1 or B: +6 -3 = +3.</span></span>  
9. <span data-ttu-id="85524-142">In case of A, the system creates a forward-scheduled order starting on date **Da**.</span><span class="sxs-lookup"><span data-stu-id="85524-142">In case of A, the system creates a forward-scheduled order starting on date **Da**.</span></span>  

     <span data-ttu-id="85524-143">In case of B, the reorder point is reached and a new order is created.</span><span class="sxs-lookup"><span data-stu-id="85524-143">In case of B, the reorder point is reached and a new order is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="85524-144">See Also</span><span class="sxs-lookup"><span data-stu-id="85524-144">See Also</span></span>  
<span data-ttu-id="85524-145">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="85524-145">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="85524-146">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="85524-146">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="85524-147">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="85524-147">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="85524-148">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="85524-148">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
