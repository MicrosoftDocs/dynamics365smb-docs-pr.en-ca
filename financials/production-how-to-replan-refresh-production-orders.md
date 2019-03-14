---
title: How to Replan or Refresh Production Orders Directly| Microsoft Docs
description: The production order lines contain the items that are to be produced in the production order.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 9b839b26814f730febc384ae1bca432a7c26852f
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="replan-or-refresh-production-orders-directly"></a><span data-ttu-id="421ee-103">Replan or Refresh Production Orders Directly</span><span class="sxs-lookup"><span data-stu-id="421ee-103">Replan or Refresh Production Orders Directly</span></span>
<span data-ttu-id="421ee-104">The **Replan** function on production orders is typically used after you have added or changed components that constitute underlying production orders.</span><span class="sxs-lookup"><span data-stu-id="421ee-104">The **Replan** function on production orders is typically used after you have added or changed components that constitute underlying production orders.</span></span> <span data-ttu-id="421ee-105">The function calculates changes made to components and routings lines, and it includes items on lower production BOM levels for which it may generate new production orders.</span><span class="sxs-lookup"><span data-stu-id="421ee-105">The function calculates changes made to components and routings lines, and it includes items on lower production BOM levels for which it may generate new production orders.</span></span>  

<span data-ttu-id="421ee-106">Based on the changes you have made to the components and routing lines, the Replan function calculates and plans for any new demand for the production order.</span><span class="sxs-lookup"><span data-stu-id="421ee-106">Based on the changes you have made to the components and routing lines, the Replan function calculates and plans for any new demand for the production order.</span></span>  

<span data-ttu-id="421ee-107">The **Refresh** function on production orders is typically used after you have done one of the following:</span><span class="sxs-lookup"><span data-stu-id="421ee-107">The **Refresh** function on production orders is typically used after you have done one of the following:</span></span>

- <span data-ttu-id="421ee-108">Created a production order header manually to calculate and create line data for the first time.</span><span class="sxs-lookup"><span data-stu-id="421ee-108">Created a production order header manually to calculate and create line data for the first time.</span></span>
- <span data-ttu-id="421ee-109">Made changes to the production order header to recalculate all the line data.</span><span class="sxs-lookup"><span data-stu-id="421ee-109">Made changes to the production order header to recalculate all the line data.</span></span>

<span data-ttu-id="421ee-110">The Refresh function calculates changes made to a production order header and does not involve production BOM levels.</span><span class="sxs-lookup"><span data-stu-id="421ee-110">The Refresh function calculates changes made to a production order header and does not involve production BOM levels.</span></span> <span data-ttu-id="421ee-111">The function calculates and initiates the values of the component lines and routing lines based on the master data defined in the assigned production BOM and routing, according to the order quantity and due date on the production order’s header.</span><span class="sxs-lookup"><span data-stu-id="421ee-111">The function calculates and initiates the values of the component lines and routing lines based on the master data defined in the assigned production BOM and routing, according to the order quantity and due date on the production order’s header.</span></span>

<span data-ttu-id="421ee-112">You can either insert the production order lines manually or use the function that calculates the production order lines from the header.</span><span class="sxs-lookup"><span data-stu-id="421ee-112">You can either insert the production order lines manually or use the function that calculates the production order lines from the header.</span></span>  

> [!NOTE]
 <span data-ttu-id="421ee-113">If you use the Refresh function to recalculate production order lines, the old production order lines are deleted and new lines are calculated.</span><span class="sxs-lookup"><span data-stu-id="421ee-113">If you use the Refresh function to recalculate production order lines, the old production order lines are deleted and new lines are calculated.</span></span>  

## <a name="to-replan-a-production-order"></a><span data-ttu-id="421ee-114">To replan a production order</span><span class="sxs-lookup"><span data-stu-id="421ee-114">To replan a production order</span></span>  
1.  <span data-ttu-id="421ee-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="421ee-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="421ee-116">Open the production order you want to replan.</span><span class="sxs-lookup"><span data-stu-id="421ee-116">Open the production order you want to replan.</span></span>  
3.  <span data-ttu-id="421ee-117">On the **Lines** FastTab, choose the **Lines** action, and then choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="421ee-117">On the **Lines** FastTab, choose the **Lines** action, and then choose the **Components** action.</span></span>  
4.  <span data-ttu-id="421ee-118">Add a component, which is a produced item or subassembly.</span><span class="sxs-lookup"><span data-stu-id="421ee-118">Add a component, which is a produced item or subassembly.</span></span>  
5.  <span data-ttu-id="421ee-119">From the production order, choose the **Replan** action.</span><span class="sxs-lookup"><span data-stu-id="421ee-119">From the production order, choose the **Replan** action.</span></span>  

    <span data-ttu-id="421ee-120">In the **Replan Production Order** window, proceed to define how and what to replan.</span><span class="sxs-lookup"><span data-stu-id="421ee-120">In the **Replan Production Order** window, proceed to define how and what to replan.</span></span>  
6.  <span data-ttu-id="421ee-121">In the **Scheduling Direction** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="421ee-121">In the **Scheduling Direction** field, select one of the following options.</span></span>  

    |<span data-ttu-id="421ee-122">Option</span><span class="sxs-lookup"><span data-stu-id="421ee-122">Option</span></span>|<span data-ttu-id="421ee-123">Description</span><span class="sxs-lookup"><span data-stu-id="421ee-123">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="421ee-124">**Back**</span><span class="sxs-lookup"><span data-stu-id="421ee-124">**Back**</span></span>|<span data-ttu-id="421ee-125">Calculates the operation sequence backwards from the earliest possible ending date, defined by due date and/or other scheduled orders, to the latest possible starting date.</span><span class="sxs-lookup"><span data-stu-id="421ee-125">Calculates the operation sequence backwards from the earliest possible ending date, defined by due date and/or other scheduled orders, to the latest possible starting date.</span></span> <span data-ttu-id="421ee-126">**Note:**  This default option is relevant in the majority of situations.</span><span class="sxs-lookup"><span data-stu-id="421ee-126">**Note:**  This default option is relevant in the majority of situations.</span></span>|  
    |<span data-ttu-id="421ee-127">**Forward**</span><span class="sxs-lookup"><span data-stu-id="421ee-127">**Forward**</span></span>|<span data-ttu-id="421ee-128">Calculates the operation sequence forward from the earliest latest possible starting date, defined by due date and/or other scheduled orders, to the earliest possible ending date.</span><span class="sxs-lookup"><span data-stu-id="421ee-128">Calculates the operation sequence forward from the earliest latest possible starting date, defined by due date and/or other scheduled orders, to the earliest possible ending date.</span></span> <span data-ttu-id="421ee-129">**Note:**  This option is only relevant for expedite orders.</span><span class="sxs-lookup"><span data-stu-id="421ee-129">**Note:**  This option is only relevant for expedite orders.</span></span>|  

7.  <span data-ttu-id="421ee-130">In the **Plan** field, select whether to calculate production requirements for produced items on the production BOM, as follows.</span><span class="sxs-lookup"><span data-stu-id="421ee-130">In the **Plan** field, select whether to calculate production requirements for produced items on the production BOM, as follows.</span></span>  

    |<span data-ttu-id="421ee-131">Option</span><span class="sxs-lookup"><span data-stu-id="421ee-131">Option</span></span>|<span data-ttu-id="421ee-132">Description</span><span class="sxs-lookup"><span data-stu-id="421ee-132">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="421ee-133">**No Levels**</span><span class="sxs-lookup"><span data-stu-id="421ee-133">**No Levels**</span></span>|<span data-ttu-id="421ee-134">Do not consider lower level production.</span><span class="sxs-lookup"><span data-stu-id="421ee-134">Do not consider lower level production.</span></span> <span data-ttu-id="421ee-135">This only updates the item’s schedule, like refresh.</span><span class="sxs-lookup"><span data-stu-id="421ee-135">This only updates the item’s schedule, like refresh.</span></span>|  
    |<span data-ttu-id="421ee-136">**One Level**</span><span class="sxs-lookup"><span data-stu-id="421ee-136">**One Level**</span></span>|<span data-ttu-id="421ee-137">Plan for first-level production demand.</span><span class="sxs-lookup"><span data-stu-id="421ee-137">Plan for first-level production demand.</span></span> <span data-ttu-id="421ee-138">First-level production orders may be created.</span><span class="sxs-lookup"><span data-stu-id="421ee-138">First-level production orders may be created.</span></span>|  
    |<span data-ttu-id="421ee-139">**All Levels**</span><span class="sxs-lookup"><span data-stu-id="421ee-139">**All Levels**</span></span>|<span data-ttu-id="421ee-140">Plan for all-level production demand.</span><span class="sxs-lookup"><span data-stu-id="421ee-140">Plan for all-level production demand.</span></span> <span data-ttu-id="421ee-141">All-level production orders may be created.</span><span class="sxs-lookup"><span data-stu-id="421ee-141">All-level production orders may be created.</span></span>|  

8.  <span data-ttu-id="421ee-142">Select **One Level**, and choose the **OK** button to replan the production order, and calculate and create a new underlying production order for the introduced subassembly, if it is not fully available.</span><span class="sxs-lookup"><span data-stu-id="421ee-142">Select **One Level**, and choose the **OK** button to replan the production order, and calculate and create a new underlying production order for the introduced subassembly, if it is not fully available.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="421ee-143">Changes implemented with the **Replan** function are very likely to change the capacity need of the production order and you may therefore have to reschedule operations afterwards.</span><span class="sxs-lookup"><span data-stu-id="421ee-143">Changes implemented with the **Replan** function are very likely to change the capacity need of the production order and you may therefore have to reschedule operations afterwards.</span></span>  

## <a name="to-refresh-a-production-order"></a><span data-ttu-id="421ee-144">To refresh a production order</span><span class="sxs-lookup"><span data-stu-id="421ee-144">To refresh a production order</span></span>  
<span data-ttu-id="421ee-145">If you have amended production order lines, components, or routing lines, you must also refresh the information on the production order.</span><span class="sxs-lookup"><span data-stu-id="421ee-145">If you have amended production order lines, components, or routing lines, you must also refresh the information on the production order.</span></span> <span data-ttu-id="421ee-146">In the following procedure, the components are calculated for a firm planned production order.</span><span class="sxs-lookup"><span data-stu-id="421ee-146">In the following procedure, the components are calculated for a firm planned production order.</span></span> <span data-ttu-id="421ee-147">The steps are similar for routing lines.</span><span class="sxs-lookup"><span data-stu-id="421ee-147">The steps are similar for routing lines.</span></span>

1.  <span data-ttu-id="421ee-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="421ee-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="421ee-149">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="421ee-149">Choose the **New** action.</span></span> <span data-ttu-id="421ee-150">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="421ee-150">For more information, see [Create Production orders](production-how-to-create-production-orders.md).</span></span>  
3.  <span data-ttu-id="421ee-151">Choose the **Refresh** action.</span><span class="sxs-lookup"><span data-stu-id="421ee-151">Choose the **Refresh** action.</span></span>
4. <span data-ttu-id="421ee-152">In the **Refresh Production Order** window, select one of the following options:</span><span class="sxs-lookup"><span data-stu-id="421ee-152">In the **Refresh Production Order** window, select one of the following options:</span></span>

    |<span data-ttu-id="421ee-153">Option</span><span class="sxs-lookup"><span data-stu-id="421ee-153">Option</span></span>|<span data-ttu-id="421ee-154">Description</span><span class="sxs-lookup"><span data-stu-id="421ee-154">Description</span></span>|  
    |----------------------------------|---------------|---------------------------------------|  
    |<span data-ttu-id="421ee-155">**Scheduling Direction**</span><span class="sxs-lookup"><span data-stu-id="421ee-155">**Scheduling Direction**</span></span>|<span data-ttu-id="421ee-156">**Forward**</span><span class="sxs-lookup"><span data-stu-id="421ee-156">**Forward**</span></span>|<span data-ttu-id="421ee-157">Scheduling starts from the starting date and proceeds forward to the finishing date.</span><span class="sxs-lookup"><span data-stu-id="421ee-157">Scheduling starts from the starting date and proceeds forward to the finishing date.</span></span> <span data-ttu-id="421ee-158">You must fill in the starting date to use this option.</span><span class="sxs-lookup"><span data-stu-id="421ee-158">You must fill in the starting date to use this option.</span></span>|  
    ||<span data-ttu-id="421ee-159">**Backward**</span><span class="sxs-lookup"><span data-stu-id="421ee-159">**Backward**</span></span>|<span data-ttu-id="421ee-160">Scheduling starts from the ending date and proceeds backward to the starting date.</span><span class="sxs-lookup"><span data-stu-id="421ee-160">Scheduling starts from the ending date and proceeds backward to the starting date.</span></span>|  
    |<span data-ttu-id="421ee-161">**Calculate**</span><span class="sxs-lookup"><span data-stu-id="421ee-161">**Calculate**</span></span>|<span data-ttu-id="421ee-162">**Lines**</span><span class="sxs-lookup"><span data-stu-id="421ee-162">**Lines**</span></span>|<span data-ttu-id="421ee-163">Select this field to calculate the production order lines.</span><span class="sxs-lookup"><span data-stu-id="421ee-163">Select this field to calculate the production order lines.</span></span>|  
    ||<span data-ttu-id="421ee-164">**Routings**</span><span class="sxs-lookup"><span data-stu-id="421ee-164">**Routings**</span></span>|<span data-ttu-id="421ee-165">This field has no influence on calculating the production lines.</span><span class="sxs-lookup"><span data-stu-id="421ee-165">This field has no influence on calculating the production lines.</span></span>|  
    ||<span data-ttu-id="421ee-166">**Component Need**</span><span class="sxs-lookup"><span data-stu-id="421ee-166">**Component Need**</span></span>|<span data-ttu-id="421ee-167">This field has no influence on calculating the production lines.</span><span class="sxs-lookup"><span data-stu-id="421ee-167">This field has no influence on calculating the production lines.</span></span>|  
    |<span data-ttu-id="421ee-168">**Warehouse**</span><span class="sxs-lookup"><span data-stu-id="421ee-168">**Warehouse**</span></span>|<span data-ttu-id="421ee-169">**Create Inbound Request**</span><span class="sxs-lookup"><span data-stu-id="421ee-169">**Create Inbound Request**</span></span>|<span data-ttu-id="421ee-170">This field has no influence on calculating the production lines.</span><span class="sxs-lookup"><span data-stu-id="421ee-170">This field has no influence on calculating the production lines.</span></span>|  

5. <span data-ttu-id="421ee-171">Choose the **OK** button to confirm your selection.</span><span class="sxs-lookup"><span data-stu-id="421ee-171">Choose the **OK** button to confirm your selection.</span></span> <span data-ttu-id="421ee-172">Now the production order lines are calculated.</span><span class="sxs-lookup"><span data-stu-id="421ee-172">Now the production order lines are calculated.</span></span>

> [!NOTE]  
>  <span data-ttu-id="421ee-173">Calculating production order components deletes previous changes in the components.</span><span class="sxs-lookup"><span data-stu-id="421ee-173">Calculating production order components deletes previous changes in the components.</span></span>

## <a name="see-also"></a><span data-ttu-id="421ee-174">See Also</span><span class="sxs-lookup"><span data-stu-id="421ee-174">See Also</span></span>  
[<span data-ttu-id="421ee-175">Planning</span><span class="sxs-lookup"><span data-stu-id="421ee-175">Planning</span></span>](production-planning.md)  
[<span data-ttu-id="421ee-176">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="421ee-176">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="421ee-177">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="421ee-177">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="421ee-178">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="421ee-178">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="421ee-179">Purchasing</span><span class="sxs-lookup"><span data-stu-id="421ee-179">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="421ee-180">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="421ee-180">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="421ee-181">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="421ee-181">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="421ee-182">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="421ee-182">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
