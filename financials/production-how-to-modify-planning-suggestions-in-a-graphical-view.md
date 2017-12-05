---
title: How to Modify Planning Suggestions in a Graphical View | Microsoft Docs
description: A typical planning activity is to change or add planning worksheet lines to modify the suggested supply orders before you commit them by running the **Carry out Action Message** function. An alternative to doing this in the planning worksheet is to use a graphical view.
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
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 4bc8694fc1da6caab88c3b462e5b50306d08271b
ms.contentlocale: en-ca
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-modify-planning-suggestions-in-a-graphical-view"></a><span data-ttu-id="27fa7-104">How to: Modify Planning Suggestions in a Graphical View</span><span class="sxs-lookup"><span data-stu-id="27fa7-104">How to: Modify Planning Suggestions in a Graphical View</span></span>
<span data-ttu-id="27fa7-105">A typical planning activity is to change or add planning worksheet lines to modify the suggested supply orders before you commit them by running the **Carry out Action Message** function.</span><span class="sxs-lookup"><span data-stu-id="27fa7-105">A typical planning activity is to change or add planning worksheet lines to modify the suggested supply orders before you commit them by running the **Carry out Action Message** function.</span></span> <span data-ttu-id="27fa7-106">An alternative to doing this in the planning worksheet is to use a graphical view.</span><span class="sxs-lookup"><span data-stu-id="27fa7-106">An alternative to doing this in the planning worksheet is to use a graphical view.</span></span>

<span data-ttu-id="27fa7-107">In the **Item Availability by Timeline** window, you can modify certain supply orders and suggestions by dragging elements on the x-axis to change quantity or dragging elements on the y-axis to change due date.</span><span class="sxs-lookup"><span data-stu-id="27fa7-107">In the **Item Availability by Timeline** window, you can modify certain supply orders and suggestions by dragging elements on the x-axis to change quantity or dragging elements on the y-axis to change due date.</span></span>  

 <span data-ttu-id="27fa7-108">In the **Item Availability by Timeline** window and the **Planning Worksheet** window you can make the following changes:</span><span class="sxs-lookup"><span data-stu-id="27fa7-108">In the **Item Availability by Timeline** window and the **Planning Worksheet** window you can make the following changes:</span></span>  

-   <span data-ttu-id="27fa7-109">Modify a suggested supply order that only exists as a planning line.</span><span class="sxs-lookup"><span data-stu-id="27fa7-109">Modify a suggested supply order that only exists as a planning line.</span></span>  
-   <span data-ttu-id="27fa7-110">Modify an existing supply order that the planning system suggests to change.</span><span class="sxs-lookup"><span data-stu-id="27fa7-110">Modify an existing supply order that the planning system suggests to change.</span></span>  
-   <span data-ttu-id="27fa7-111">Create a new suggested supply order and modify it.</span><span class="sxs-lookup"><span data-stu-id="27fa7-111">Create a new suggested supply order and modify it.</span></span>  

<span data-ttu-id="27fa7-112">For more information about the planning line types that are shown, see the Description field on the **Event Changes** FastTab.</span><span class="sxs-lookup"><span data-stu-id="27fa7-112">For more information about the planning line types that are shown, see the Description field on the **Event Changes** FastTab.</span></span>  

<span data-ttu-id="27fa7-113">When you choose **Save Changes** in the **Item Availability by Timeline** window, the modifications that you have made are copied to the planning or requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="27fa7-113">When you choose **Save Changes** in the **Item Availability by Timeline** window, the modifications that you have made are copied to the planning or requisition worksheet.</span></span> <span data-ttu-id="27fa7-114">You can now implement them using the **Carry Out Action Msg.-Plan.** function.</span><span class="sxs-lookup"><span data-stu-id="27fa7-114">You can now implement them using the **Carry Out Action Msg.-Plan.** function.</span></span>  

<span data-ttu-id="27fa7-115">The following procedure shows how to modify supply suggestions by drag and drop.</span><span class="sxs-lookup"><span data-stu-id="27fa7-115">The following procedure shows how to modify supply suggestions by drag and drop.</span></span> <span data-ttu-id="27fa7-116">As an alternative, you can change the **Due Date** and **Quantity** fields on the **Event Changes** FastTab and immediately see the changes graphically on the **Timeline** FastTab in the **Planning Worksheet** window.</span><span class="sxs-lookup"><span data-stu-id="27fa7-116">As an alternative, you can change the **Due Date** and **Quantity** fields on the **Event Changes** FastTab and immediately see the changes graphically on the **Timeline** FastTab in the **Planning Worksheet** window.</span></span>  

## <a name="to-modify-suggested-supply-orders-in-the-graphical-view"></a><span data-ttu-id="27fa7-117">To modify suggested supply orders in the graphical view</span><span class="sxs-lookup"><span data-stu-id="27fa7-117">To modify suggested supply orders in the graphical view</span></span>  
1.  <span data-ttu-id="27fa7-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Availability by Timeline**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="27fa7-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Availability by Timeline**, and then choose the related link.</span></span>  

    <span data-ttu-id="27fa7-119">The **Item Availability by Timeline** window opens with the item number, location, and variant of the item on the selected planning line prefilled in the **Options** FastTab.</span><span class="sxs-lookup"><span data-stu-id="27fa7-119">The **Item Availability by Timeline** window opens with the item number, location, and variant of the item on the selected planning line prefilled in the **Options** FastTab.</span></span> <span data-ttu-id="27fa7-120">The **Timeline** FastTab shows a graphical representation of the item’s projected inventory, including planning suggestions.</span><span class="sxs-lookup"><span data-stu-id="27fa7-120">The **Timeline** FastTab shows a graphical representation of the item’s projected inventory, including planning suggestions.</span></span>  

2.  <span data-ttu-id="27fa7-121">Make sure that the **Include Planning Suggestions** field is selected.</span><span class="sxs-lookup"><span data-stu-id="27fa7-121">Make sure that the **Include Planning Suggestions** field is selected.</span></span>  
3.  <span data-ttu-id="27fa7-122">Find the suggested supply order that you want to modify.</span><span class="sxs-lookup"><span data-stu-id="27fa7-122">Find the suggested supply order that you want to modify.</span></span> <span data-ttu-id="27fa7-123">You can identify modifiable elements by the green circle and the disk icon.</span><span class="sxs-lookup"><span data-stu-id="27fa7-123">You can identify modifiable elements by the green circle and the disk icon.</span></span> <span data-ttu-id="27fa7-124">For more information about the different symbols, see the "Symbols and Icons on the Timeline FastTab" section.</span><span class="sxs-lookup"><span data-stu-id="27fa7-124">For more information about the different symbols, see the "Symbols and Icons on the Timeline FastTab" section.</span></span>  
4.  <span data-ttu-id="27fa7-125">Place the pointer over the green circle until it enlarges and the pointer changes to Move shape (four arrows).</span><span class="sxs-lookup"><span data-stu-id="27fa7-125">Place the pointer over the green circle until it enlarges and the pointer changes to Move shape (four arrows).</span></span>  
5.  <span data-ttu-id="27fa7-126">Press and hold the mouse button while you drag the pointer up or down to modify the quantity.</span><span class="sxs-lookup"><span data-stu-id="27fa7-126">Press and hold the mouse button while you drag the pointer up or down to modify the quantity.</span></span> <span data-ttu-id="27fa7-127">Press and hold the mouse button while you drag the pointer left or right to modify the due date.</span><span class="sxs-lookup"><span data-stu-id="27fa7-127">Press and hold the mouse button while you drag the pointer left or right to modify the due date.</span></span>  
6.  <span data-ttu-id="27fa7-128">In addition to moving elements by drag and drop, you can modify planning suggestions by using a number of drop-down menu functions.</span><span class="sxs-lookup"><span data-stu-id="27fa7-128">In addition to moving elements by drag and drop, you can modify planning suggestions by using a number of drop-down menu functions.</span></span> <span data-ttu-id="27fa7-129">Access the drop-down menu for the green circle of a suggested supply element and select one the following functions</span><span class="sxs-lookup"><span data-stu-id="27fa7-129">Access the drop-down menu for the green circle of a suggested supply element and select one the following functions</span></span>  

    |<span data-ttu-id="27fa7-130">Function</span><span class="sxs-lookup"><span data-stu-id="27fa7-130">Function</span></span>|<span data-ttu-id="27fa7-131">Description</span><span class="sxs-lookup"><span data-stu-id="27fa7-131">Description</span></span>|  
    |--------------|---------------------------------------|  
    |<span data-ttu-id="27fa7-132">**Create New Supply**</span><span class="sxs-lookup"><span data-stu-id="27fa7-132">**Create New Supply**</span></span>|<span data-ttu-id="27fa7-133">Creates a new element point where you access the drop-down menu, which represents a new suggested supply order.</span><span class="sxs-lookup"><span data-stu-id="27fa7-133">Creates a new element point where you access the drop-down menu, which represents a new suggested supply order.</span></span> <span data-ttu-id="27fa7-134">It becomes a new line in the planning worksheet when you choose **Save Changes**.</span><span class="sxs-lookup"><span data-stu-id="27fa7-134">It becomes a new line in the planning worksheet when you choose **Save Changes**.</span></span><br /><br /> <span data-ttu-id="27fa7-135">**NOTE:** If the **Location Filter** or **Variant Filter** fields on the **Options** FastTab are empty or have more than one filter value, then the new supply is created and later saved to the planning or requisition worksheet with the following codes:</span><span class="sxs-lookup"><span data-stu-id="27fa7-135">**NOTE:** If the **Location Filter** or **Variant Filter** fields on the **Options** FastTab are empty or have more than one filter value, then the new supply is created and later saved to the planning or requisition worksheet with the following codes:</span></span><br /><br /> <span data-ttu-id="27fa7-136">* If the filter field is empty, then the new supply is created without a location or variant code.</span><span class="sxs-lookup"><span data-stu-id="27fa7-136">* If the filter field is empty, then the new supply is created without a location or variant code.</span></span><br /><br /> <span data-ttu-id="27fa7-137">* If more than one filter value is defined, then the new supply is created for the first filter value according to the sorting method.</span><span class="sxs-lookup"><span data-stu-id="27fa7-137">* If more than one filter value is defined, then the new supply is created for the first filter value according to the sorting method.</span></span><br /><br /> <span data-ttu-id="27fa7-138">If you want another variant or location code, then you must manually change it on the new planning line.</span><span class="sxs-lookup"><span data-stu-id="27fa7-138">If you want another variant or location code, then you must manually change it on the new planning line.</span></span>|  
    |<span data-ttu-id="27fa7-139">**Auto-Adjust Supply**</span><span class="sxs-lookup"><span data-stu-id="27fa7-139">**Auto-Adjust Supply**</span></span>|<span data-ttu-id="27fa7-140">Optimizes a new supply that you have created in the graph by making sure that it results in zero inventory before the next supply.</span><span class="sxs-lookup"><span data-stu-id="27fa7-140">Optimizes a new supply that you have created in the graph by making sure that it results in zero inventory before the next supply.</span></span>|  
    |<span data-ttu-id="27fa7-141">**Delete Supply**</span><span class="sxs-lookup"><span data-stu-id="27fa7-141">**Delete Supply**</span></span>|<span data-ttu-id="27fa7-142">Deletes the element in the **Timeline** FastTab and deletes the planning line when you choose **Save Changes**.</span><span class="sxs-lookup"><span data-stu-id="27fa7-142">Deletes the element in the **Timeline** FastTab and deletes the planning line when you choose **Save Changes**.</span></span> <span data-ttu-id="27fa7-143">The icon changes to a disk that has a red cross when the supply has been deleted.</span><span class="sxs-lookup"><span data-stu-id="27fa7-143">The icon changes to a disk that has a red cross when the supply has been deleted.</span></span><br /><br /> <span data-ttu-id="27fa7-144">**NOTE:** You can only delete a supply of action message type **New**.</span><span class="sxs-lookup"><span data-stu-id="27fa7-144">**NOTE:** You can only delete a supply of action message type **New**.</span></span> <span data-ttu-id="27fa7-145">After you choose **Save Changes**, you must manually delete the planning line in question in the planning or requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="27fa7-145">After you choose **Save Changes**, you must manually delete the planning line in question in the planning or requisition worksheet.</span></span>|  

7.  <span data-ttu-id="27fa7-146">Choose the **Reload** action if you want to reset all the changes that you have made after you last opened the **Item Availability by Timeline** window or selected **Reload**.</span><span class="sxs-lookup"><span data-stu-id="27fa7-146">Choose the **Reload** action if you want to reset all the changes that you have made after you last opened the **Item Availability by Timeline** window or selected **Reload**.</span></span>  
8. <span data-ttu-id="27fa7-147">When the elements are placed where you want them in the diagram, choose **Save Changes** to copy modified quantity and date changes to the planning or requisition lines that represent the graphical elements.</span><span class="sxs-lookup"><span data-stu-id="27fa7-147">When the elements are placed where you want them in the diagram, choose **Save Changes** to copy modified quantity and date changes to the planning or requisition lines that represent the graphical elements.</span></span>  

<span data-ttu-id="27fa7-148">To implement the supply plan changes, you must follow the resulting action messages from the planning or requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="27fa7-148">To implement the supply plan changes, you must follow the resulting action messages from the planning or requisition worksheet.</span></span> <span data-ttu-id="27fa7-149">For more information, see Carry Out Action Msg.-Plan..</span><span class="sxs-lookup"><span data-stu-id="27fa7-149">For more information, see Carry Out Action Msg.-Plan..</span></span>

## <a name="symbols-and-icons-on-the-timeline-fasttab"></a><span data-ttu-id="27fa7-150">Symbols and Icons on the Timeline FastTab</span><span class="sxs-lookup"><span data-stu-id="27fa7-150">Symbols and Icons on the Timeline FastTab</span></span>
 |<span data-ttu-id="27fa7-151">Symbol/Icon</span><span class="sxs-lookup"><span data-stu-id="27fa7-151">Symbol/Icon</span></span>|<span data-ttu-id="27fa7-152">Description</span><span class="sxs-lookup"><span data-stu-id="27fa7-152">Description</span></span>|  
 |------------------|---------------------------------------|  
 |<span data-ttu-id="27fa7-153">Black cross</span><span class="sxs-lookup"><span data-stu-id="27fa7-153">Black cross</span></span>|<span data-ttu-id="27fa7-154">Orders (both supply and demand).</span><span class="sxs-lookup"><span data-stu-id="27fa7-154">Orders (both supply and demand).</span></span><br /><br /> <span data-ttu-id="27fa7-155">-   Cannot be modified.</span><span class="sxs-lookup"><span data-stu-id="27fa7-155">-   Cannot be modified.</span></span><br /><span data-ttu-id="27fa7-156">-   Visible when the **Show Projected Inventory** field is selected (orange graph).</span><span class="sxs-lookup"><span data-stu-id="27fa7-156">-   Visible when the **Show Projected Inventory** field is selected (orange graph).</span></span>|  
 |<span data-ttu-id="27fa7-157">Red circle</span><span class="sxs-lookup"><span data-stu-id="27fa7-157">Red circle</span></span>|<span data-ttu-id="27fa7-158">Existing supply orders that are not in planning suggestions.</span><span class="sxs-lookup"><span data-stu-id="27fa7-158">Existing supply orders that are not in planning suggestions.</span></span><br /><br /> <span data-ttu-id="27fa7-159">-   Cannot be modified.</span><span class="sxs-lookup"><span data-stu-id="27fa7-159">-   Cannot be modified.</span></span><br /><span data-ttu-id="27fa7-160">-   Visible when the **Show Projected Inventory** field is selected (orange graph).</span><span class="sxs-lookup"><span data-stu-id="27fa7-160">-   Visible when the **Show Projected Inventory** field is selected (orange graph).</span></span>|  
 |<span data-ttu-id="27fa7-161">Yellow star</span><span class="sxs-lookup"><span data-stu-id="27fa7-161">Yellow star</span></span>|<span data-ttu-id="27fa7-162">Forecast demand.</span><span class="sxs-lookup"><span data-stu-id="27fa7-162">Forecast demand.</span></span><br /><br /> <span data-ttu-id="27fa7-163">-   Cannot be modified.</span><span class="sxs-lookup"><span data-stu-id="27fa7-163">-   Cannot be modified.</span></span><br /><span data-ttu-id="27fa7-164">-   Visible when the **Forecast Name** field has a value.</span><span class="sxs-lookup"><span data-stu-id="27fa7-164">-   Visible when the **Forecast Name** field has a value.</span></span><br /><br /> <span data-ttu-id="27fa7-165">When both the **Show Projected Inventory** and the **Include Planning Suggestions** fields are selected, then each yellow star has a linked counterpart in the opposite graph.</span><span class="sxs-lookup"><span data-stu-id="27fa7-165">When both the **Show Projected Inventory** and the **Include Planning Suggestions** fields are selected, then each yellow star has a linked counterpart in the opposite graph.</span></span> <span data-ttu-id="27fa7-166">This illustrates how a suggested supply fulfills the forecasted demand.</span><span class="sxs-lookup"><span data-stu-id="27fa7-166">This illustrates how a suggested supply fulfills the forecasted demand.</span></span>|  
 |<span data-ttu-id="27fa7-167">Green circle with an icon shaped as a disk that has a red cross</span><span class="sxs-lookup"><span data-stu-id="27fa7-167">Green circle with an icon shaped as a disk that has a red cross</span></span>|<span data-ttu-id="27fa7-168">Suggested supply order with action message *Cancel*.</span><span class="sxs-lookup"><span data-stu-id="27fa7-168">Suggested supply order with action message *Cancel*.</span></span><br /><br /> <span data-ttu-id="27fa7-169">-   Cannot be modified.</span><span class="sxs-lookup"><span data-stu-id="27fa7-169">-   Cannot be modified.</span></span><br /><span data-ttu-id="27fa7-170">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span><span class="sxs-lookup"><span data-stu-id="27fa7-170">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span></span>|  
 |<span data-ttu-id="27fa7-171">Green circle with an icon shaped as a disk that has a star</span><span class="sxs-lookup"><span data-stu-id="27fa7-171">Green circle with an icon shaped as a disk that has a star</span></span>|<span data-ttu-id="27fa7-172">Suggested supply orders with action message *New*.</span><span class="sxs-lookup"><span data-stu-id="27fa7-172">Suggested supply orders with action message *New*.</span></span><br /><br /> <span data-ttu-id="27fa7-173">-   Can be modified.</span><span class="sxs-lookup"><span data-stu-id="27fa7-173">-   Can be modified.</span></span><br /><span data-ttu-id="27fa7-174">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span><span class="sxs-lookup"><span data-stu-id="27fa7-174">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span></span>|  
 |<span data-ttu-id="27fa7-175">Green circle with an icon shaped as a disk that has one or two arrows</span><span class="sxs-lookup"><span data-stu-id="27fa7-175">Green circle with an icon shaped as a disk that has one or two arrows</span></span>|<span data-ttu-id="27fa7-176">Suggested supply orders with action message *Reschedule*, *Change Qty.*, or *Resched. and Chg. Qty.*</span><span class="sxs-lookup"><span data-stu-id="27fa7-176">Suggested supply orders with action message *Reschedule*, *Change Qty.*, or *Resched. and Chg. Qty.*</span></span><br /><br /> <span data-ttu-id="27fa7-177">-   Can be modified.</span><span class="sxs-lookup"><span data-stu-id="27fa7-177">-   Can be modified.</span></span><br /><span data-ttu-id="27fa7-178">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span><span class="sxs-lookup"><span data-stu-id="27fa7-178">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span></span><br /><br /> <span data-ttu-id="27fa7-179">The arrows reflect the direction of the planning suggestion.</span><span class="sxs-lookup"><span data-stu-id="27fa7-179">The arrows reflect the direction of the planning suggestion.</span></span> <span data-ttu-id="27fa7-180">For example, a left arrow together with an up arrow reflects a *Resched. and Chg. Qty.* action message that consists of a backward rescheduling and a quantity increase.</span><span class="sxs-lookup"><span data-stu-id="27fa7-180">For example, a left arrow together with an up arrow reflects a *Resched. and Chg. Qty.* action message that consists of a backward rescheduling and a quantity increase.</span></span>|  

<span data-ttu-id="27fa7-181">When you access the drop-down menu for the **Timeline** FastTab, the following functions appear depending what you choose</span><span class="sxs-lookup"><span data-stu-id="27fa7-181">When you access the drop-down menu for the **Timeline** FastTab, the following functions appear depending what you choose</span></span>  

 |<span data-ttu-id="27fa7-182">Function</span><span class="sxs-lookup"><span data-stu-id="27fa7-182">Function</span></span>|<span data-ttu-id="27fa7-183">Description</span><span class="sxs-lookup"><span data-stu-id="27fa7-183">Description</span></span>|  
 |--------------|---------------------------------------|  
 |<span data-ttu-id="27fa7-184">**Create New Supply**</span><span class="sxs-lookup"><span data-stu-id="27fa7-184">**Create New Supply**</span></span>|<span data-ttu-id="27fa7-185">Creates a new element on the point where you access the drop-down menu, which represents a new suggested supply order.</span><span class="sxs-lookup"><span data-stu-id="27fa7-185">Creates a new element on the point where you access the drop-down menu, which represents a new suggested supply order.</span></span> <span data-ttu-id="27fa7-186">It becomes a new line in the planning worksheet when you choose **Save Changes** on the **Process** tab.</span><span class="sxs-lookup"><span data-stu-id="27fa7-186">It becomes a new line in the planning worksheet when you choose **Save Changes** on the **Process** tab.</span></span><br /><br /> <span data-ttu-id="27fa7-187">Any filter values that are defined in the **Location Filter** or **Variant Filter** fields on the **Options** FastTab will be applied to the new supply order.</span><span class="sxs-lookup"><span data-stu-id="27fa7-187">Any filter values that are defined in the **Location Filter** or **Variant Filter** fields on the **Options** FastTab will be applied to the new supply order.</span></span> <span data-ttu-id="27fa7-188">**Note:**  If the filter fields are empty or have more than one filter value, then the new supply order is created by using the following codes:</span><span class="sxs-lookup"><span data-stu-id="27fa7-188">**Note:**  If the filter fields are empty or have more than one filter value, then the new supply order is created by using the following codes:</span></span> <ul><li><span data-ttu-id="27fa7-189">If the filter field is empty, then the new supply is created without a location or variant code.</span><span class="sxs-lookup"><span data-stu-id="27fa7-189">If the filter field is empty, then the new supply is created without a location or variant code.</span></span></li><li><span data-ttu-id="27fa7-190">If more than one filter value is defined, then the new supply is created by using the first filter value according to the sorting order.</span><span class="sxs-lookup"><span data-stu-id="27fa7-190">If more than one filter value is defined, then the new supply is created by using the first filter value according to the sorting order.</span></span></li></ul> <span data-ttu-id="27fa7-191">If you want another variant or location code in the new supply order, then you must manually change it on the new planning line.</span><span class="sxs-lookup"><span data-stu-id="27fa7-191">If you want another variant or location code in the new supply order, then you must manually change it on the new planning line.</span></span>|  
 |<span data-ttu-id="27fa7-192">**Auto-Adjust Supply**</span><span class="sxs-lookup"><span data-stu-id="27fa7-192">**Auto-Adjust Supply**</span></span>|<span data-ttu-id="27fa7-193">Optimizes a new supply that you have created in the graph by making sure that it creates zero inventory before the next supply.</span><span class="sxs-lookup"><span data-stu-id="27fa7-193">Optimizes a new supply that you have created in the graph by making sure that it creates zero inventory before the next supply.</span></span>|  
 |<span data-ttu-id="27fa7-194">**Delete Supply**</span><span class="sxs-lookup"><span data-stu-id="27fa7-194">**Delete Supply**</span></span>|<span data-ttu-id="27fa7-195">Deletes the element in the **Timeline** FastTab and deletes the planning line when you choose **Save Changes** on the **Process** tab. The icon changes to a disk that has a red cross when the supply has been deleted.</span><span class="sxs-lookup"><span data-stu-id="27fa7-195">Deletes the element in the **Timeline** FastTab and deletes the planning line when you choose **Save Changes** on the **Process** tab. The icon changes to a disk that has a red cross when the supply has been deleted.</span></span> <span data-ttu-id="27fa7-196">**Note:**  You can only delete a supply of action message type *New*.</span><span class="sxs-lookup"><span data-stu-id="27fa7-196">**Note:**  You can only delete a supply of action message type *New*.</span></span> <span data-ttu-id="27fa7-197">After you choose **Save Changes** on the **Process** tab, you must manually delete the planning line in question in the planning or requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="27fa7-197">After you choose **Save Changes** on the **Process** tab, you must manually delete the planning line in question in the planning or requisition worksheet.</span></span>|  
 |<span data-ttu-id="27fa7-198">**Show Document**</span><span class="sxs-lookup"><span data-stu-id="27fa7-198">**Show Document**</span></span>|<span data-ttu-id="27fa7-199">Opens the order, planning line, or forecast that the element represents.</span><span class="sxs-lookup"><span data-stu-id="27fa7-199">Opens the order, planning line, or forecast that the element represents.</span></span>|  
 |<span data-ttu-id="27fa7-200">**Zoom Out (Ctrl++)**</span><span class="sxs-lookup"><span data-stu-id="27fa7-200">**Zoom Out (Ctrl++)**</span></span>|<span data-ttu-id="27fa7-201">Makes the scale of the x-axis larger, so that fewer days are shown.</span><span class="sxs-lookup"><span data-stu-id="27fa7-201">Makes the scale of the x-axis larger, so that fewer days are shown.</span></span> <span data-ttu-id="27fa7-202">**Note:**  You can also do this by pressing Ctrl + scroll mouse wheel.</span><span class="sxs-lookup"><span data-stu-id="27fa7-202">**Note:**  You can also do this by pressing Ctrl + scroll mouse wheel.</span></span>|  
 |<span data-ttu-id="27fa7-203">**Zoom In (Ctrl+-)**</span><span class="sxs-lookup"><span data-stu-id="27fa7-203">**Zoom In (Ctrl+-)**</span></span>|<span data-ttu-id="27fa7-204">Makes the scale of the x-axis smaller, so that more days are shown.</span><span class="sxs-lookup"><span data-stu-id="27fa7-204">Makes the scale of the x-axis smaller, so that more days are shown.</span></span> <span data-ttu-id="27fa7-205">**Note:**  You can also do this by pressing Ctrl + scroll mouse wheel.</span><span class="sxs-lookup"><span data-stu-id="27fa7-205">**Note:**  You can also do this by pressing Ctrl + scroll mouse wheel.</span></span>|  
 |<span data-ttu-id="27fa7-206">**Reset Zoom (Ctrl+0)**</span><span class="sxs-lookup"><span data-stu-id="27fa7-206">**Reset Zoom (Ctrl+0)**</span></span>|<span data-ttu-id="27fa7-207">Reverts the scale of the x-axis to what was used before you zoomed.</span><span class="sxs-lookup"><span data-stu-id="27fa7-207">Reverts the scale of the x-axis to what was used before you zoomed.</span></span>|  

<span data-ttu-id="27fa7-208">In addition to the keyboard actions that were mentioned earlier, you can also use the following keyboard actions in the **TimeLine** FastTab.</span><span class="sxs-lookup"><span data-stu-id="27fa7-208">In addition to the keyboard actions that were mentioned earlier, you can also use the following keyboard actions in the **TimeLine** FastTab.</span></span>  

 |<span data-ttu-id="27fa7-209">Keyboard Action</span><span class="sxs-lookup"><span data-stu-id="27fa7-209">Keyboard Action</span></span>|<span data-ttu-id="27fa7-210">Description</span><span class="sxs-lookup"><span data-stu-id="27fa7-210">Description</span></span>|  
 |---------------------|---------------------------------------|  
 |<span data-ttu-id="27fa7-211">Ctrl + scroll mouse wheel</span><span class="sxs-lookup"><span data-stu-id="27fa7-211">Ctrl + scroll mouse wheel</span></span>|<span data-ttu-id="27fa7-212">Changes the scale of the x-axis.</span><span class="sxs-lookup"><span data-stu-id="27fa7-212">Changes the scale of the x-axis.</span></span>|  
 |<span data-ttu-id="27fa7-213">Select an element, then press Shift+Arrow</span><span class="sxs-lookup"><span data-stu-id="27fa7-213">Select an element, then press Shift+Arrow</span></span>|<span data-ttu-id="27fa7-214">Moves the element in the direction of the arrow stroke.</span><span class="sxs-lookup"><span data-stu-id="27fa7-214">Moves the element in the direction of the arrow stroke.</span></span>|  
 |<span data-ttu-id="27fa7-215">Tab</span><span class="sxs-lookup"><span data-stu-id="27fa7-215">Tab</span></span>|<span data-ttu-id="27fa7-216">Moves to the next element.</span><span class="sxs-lookup"><span data-stu-id="27fa7-216">Moves to the next element.</span></span>|  
 |<span data-ttu-id="27fa7-217">Shift+Tab</span><span class="sxs-lookup"><span data-stu-id="27fa7-217">Shift+Tab</span></span>|<span data-ttu-id="27fa7-218">Moves to the previous element.</span><span class="sxs-lookup"><span data-stu-id="27fa7-218">Moves to the previous element.</span></span>|  
 |<span data-ttu-id="27fa7-219">While moving an element, press Esc.</span><span class="sxs-lookup"><span data-stu-id="27fa7-219">While moving an element, press Esc.</span></span>|<span data-ttu-id="27fa7-220">Cancels the move.</span><span class="sxs-lookup"><span data-stu-id="27fa7-220">Cancels the move.</span></span> <span data-ttu-id="27fa7-221">**Note:**  Does not work if you have released the mouse button.</span><span class="sxs-lookup"><span data-stu-id="27fa7-221">**Note:**  Does not work if you have released the mouse button.</span></span>|

## <a name="see-also"></a><span data-ttu-id="27fa7-222">See Also</span><span class="sxs-lookup"><span data-stu-id="27fa7-222">See Also</span></span>  
<span data-ttu-id="27fa7-223">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="27fa7-223">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="27fa7-224">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="27fa7-224">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="27fa7-225">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="27fa7-225">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="27fa7-226">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="27fa7-226">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="27fa7-227">Purchasing</span><span class="sxs-lookup"><span data-stu-id="27fa7-227">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="27fa7-228">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="27fa7-228">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="27fa7-229">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="27fa7-229">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="27fa7-230">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="27fa7-230">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
