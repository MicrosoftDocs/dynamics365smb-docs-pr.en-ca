---
title: How to Pick for Production in Basic Warehouse Configurations | Microsoft Docs
description: When your warehouse location requires pick processing but does not require shipment processing, use the **Inventory Pick** window to organize and record the picking of components.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 35eb4fdb15eded48510a232ed26aa02b4f5700c2
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-pick-for-production-or-assembly"></a><span data-ttu-id="b30ef-103">How to: Pick for Production or Assembly</span><span class="sxs-lookup"><span data-stu-id="b30ef-103">How to: Pick for Production or Assembly</span></span>
<span data-ttu-id="b30ef-104">How you put away your pick components for production or assembly orders depends on how your warehouse is set up as a location.</span><span class="sxs-lookup"><span data-stu-id="b30ef-104">How you put away your pick components for production or assembly orders depends on how your warehouse is set up as a location.</span></span> <span data-ttu-id="b30ef-105">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-105">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

<span data-ttu-id="b30ef-106">In basic warehouse configurations where the location requires pick processing but not shipment processing, you use the **Inventory Pick** window to organize and record the picking of components.</span><span class="sxs-lookup"><span data-stu-id="b30ef-106">In basic warehouse configurations where the location requires pick processing but not shipment processing, you use the **Inventory Pick** window to organize and record the picking of components.</span></span>  

<span data-ttu-id="b30ef-107">In basic warehouse configurations, you must pick for assembly orders with the **Inventory Movement** window.</span><span class="sxs-lookup"><span data-stu-id="b30ef-107">In basic warehouse configurations, you must pick for assembly orders with the **Inventory Movement** window.</span></span> <span data-ttu-id="b30ef-108">For more information, see the "Handling Assemble-to-Order Item with Inventory Picks" section in [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-108">For more information, see the "Handling Assemble-to-Order Item with Inventory Picks" section in [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span></span>  

<span data-ttu-id="b30ef-109">In advanced warehouse configurations where locations require both picks and shipments, you use the **Warehouse Pick** window to bring components to production or assembly orders.</span><span class="sxs-lookup"><span data-stu-id="b30ef-109">In advanced warehouse configurations where locations require both picks and shipments, you use the **Warehouse Pick** window to bring components to production or assembly orders.</span></span>

> [!NOTE]  
>  <span data-ttu-id="b30ef-110">The following important differences exist between inventory picks and inventory movements:</span><span class="sxs-lookup"><span data-stu-id="b30ef-110">The following important differences exist between inventory picks and inventory movements:</span></span>  
>   
>  -   <span data-ttu-id="b30ef-111">When you register an inventory pick for an internal operation, such as production, the consumption of the picked components is posted at the same time.</span><span class="sxs-lookup"><span data-stu-id="b30ef-111">When you register an inventory pick for an internal operation, such as production, the consumption of the picked components is posted at the same time.</span></span> <span data-ttu-id="b30ef-112">When you register an inventory movement for an internal operation, you only record the physical movement of the required components to a bin in the operation area without posting the consumption.</span><span class="sxs-lookup"><span data-stu-id="b30ef-112">When you register an inventory movement for an internal operation, you only record the physical movement of the required components to a bin in the operation area without posting the consumption.</span></span>  
> -   <span data-ttu-id="b30ef-113">When you use inventory picks, the **Bin Code** field on a production order component line defines the *take* bin from where components are decreased when posting consumption.</span><span class="sxs-lookup"><span data-stu-id="b30ef-113">When you use inventory picks, the **Bin Code** field on a production order component line defines the *take* bin from where components are decreased when posting consumption.</span></span> <span data-ttu-id="b30ef-114">When you use inventory movements, the **Bin Code** field on production order component lines defines the *place* bin in the operation area where the warehouse worker must place the components.</span><span class="sxs-lookup"><span data-stu-id="b30ef-114">When you use inventory movements, the **Bin Code** field on production order component lines defines the *place* bin in the operation area where the warehouse worker must place the components.</span></span>  

<span data-ttu-id="b30ef-115">A system precondition for picking, or moving, components for source documents is that an outbound warehouse request exists to notify the warehouse area of the component need.</span><span class="sxs-lookup"><span data-stu-id="b30ef-115">A system precondition for picking, or moving, components for source documents is that an outbound warehouse request exists to notify the warehouse area of the component need.</span></span> <span data-ttu-id="b30ef-116">The outbound warehouse request is created whenever the production order status is changed to Released or when a released production order is created.</span><span class="sxs-lookup"><span data-stu-id="b30ef-116">The outbound warehouse request is created whenever the production order status is changed to Released or when a released production order is created.</span></span>  

## <a name="to-pick-components-in-basic-warehouse-configurations"></a><span data-ttu-id="b30ef-117">To pick components in basic warehouse configurations</span><span class="sxs-lookup"><span data-stu-id="b30ef-117">To pick components in basic warehouse configurations</span></span>
<span data-ttu-id="b30ef-118">In basic warehouse configurations where the location is set up to use picking only, you can pick components for production activities with the **Inventory Pick** window.</span><span class="sxs-lookup"><span data-stu-id="b30ef-118">In basic warehouse configurations where the location is set up to use picking only, you can pick components for production activities with the **Inventory Pick** window.</span></span> <span data-ttu-id="b30ef-119">For more information, see [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-119">For more information, see [How to: Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md).</span></span>

1.  <span data-ttu-id="b30ef-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Picks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b30ef-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b30ef-121">To access the production order components, choose the **Get Source Documents** action, and then select the released production order.</span><span class="sxs-lookup"><span data-stu-id="b30ef-121">To access the production order components, choose the **Get Source Documents** action, and then select the released production order.</span></span>  
3.  <span data-ttu-id="b30ef-122">Perform the pick, and then record the actual picking information in the **Qty. Picked** field.</span><span class="sxs-lookup"><span data-stu-id="b30ef-122">Perform the pick, and then record the actual picking information in the **Qty. Picked** field.</span></span>  
4.  <span data-ttu-id="b30ef-123">When the lines are ready for posting, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="b30ef-123">When the lines are ready for posting, choose the **Post** action.</span></span> <span data-ttu-id="b30ef-124">The posting creates the necessary warehouse entries and posts the consumption of the items.</span><span class="sxs-lookup"><span data-stu-id="b30ef-124">The posting creates the necessary warehouse entries and posts the consumption of the items.</span></span>  

<span data-ttu-id="b30ef-125">You can also create an **Inventory Pick** directly from the released production order.</span><span class="sxs-lookup"><span data-stu-id="b30ef-125">You can also create an **Inventory Pick** directly from the released production order.</span></span> <span data-ttu-id="b30ef-126">Choose the **Create Inventory Put-away/Pick** action, select the **Create Invt. Pick** check box, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b30ef-126">Choose the **Create Inventory Put-away/Pick** action, select the **Create Invt. Pick** check box, and then choose the **OK** button.</span></span>

<span data-ttu-id="b30ef-127">Alternatively, you can use the **Inventory Movement** window to move items between bins ad hoc, meaning without reference to a source document.</span><span class="sxs-lookup"><span data-stu-id="b30ef-127">Alternatively, you can use the **Inventory Movement** window to move items between bins ad hoc, meaning without reference to a source document.</span></span>
<span data-ttu-id="b30ef-128">For more information, see [How to: Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-128">For more information, see [How to: Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span></span>

### <a name="handling-assemble-to-order-items-with-inventory-picks"></a><span data-ttu-id="b30ef-129">Handling Assemble-to-Order Items with Inventory Picks</span><span class="sxs-lookup"><span data-stu-id="b30ef-129">Handling Assemble-to-Order Items with Inventory Picks</span></span>
<span data-ttu-id="b30ef-130">The **Inventory Pick** window is also used to pick and ship for sales where items must be assembled before they can be shipped.</span><span class="sxs-lookup"><span data-stu-id="b30ef-130">The **Inventory Pick** window is also used to pick and ship for sales where items must be assembled before they can be shipped.</span></span> <span data-ttu-id="b30ef-131">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-131">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>

<span data-ttu-id="b30ef-132">Items to be shipped are not physically present in a bin until they are assembled and posted as output to a bin in the assembly area.</span><span class="sxs-lookup"><span data-stu-id="b30ef-132">Items to be shipped are not physically present in a bin until they are assembled and posted as output to a bin in the assembly area.</span></span> <span data-ttu-id="b30ef-133">This means that picking assemble-to-order items for shipment follows a special flow.</span><span class="sxs-lookup"><span data-stu-id="b30ef-133">This means that picking assemble-to-order items for shipment follows a special flow.</span></span> <span data-ttu-id="b30ef-134">From a bin, warehouse workers take the assembly items to the shipping dock and then post the inventory pick.</span><span class="sxs-lookup"><span data-stu-id="b30ef-134">From a bin, warehouse workers take the assembly items to the shipping dock and then post the inventory pick.</span></span> <span data-ttu-id="b30ef-135">The posted inventory pick then posts the assembly output, the component consumption, and the sales shipment.</span><span class="sxs-lookup"><span data-stu-id="b30ef-135">The posted inventory pick then posts the assembly output, the component consumption, and the sales shipment.</span></span>

<span data-ttu-id="b30ef-136">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to automatically create an inventory movement when the inventory pick for the assembly item is created.</span><span class="sxs-lookup"><span data-stu-id="b30ef-136">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to automatically create an inventory movement when the inventory pick for the assembly item is created.</span></span> <span data-ttu-id="b30ef-137">To enable this, you must select the **Create Movements Automatically** field in the **Assembly Setup** window.</span><span class="sxs-lookup"><span data-stu-id="b30ef-137">To enable this, you must select the **Create Movements Automatically** field in the **Assembly Setup** window.</span></span> <span data-ttu-id="b30ef-138">For more information, see [How to: Move Components to an Operation Area in Basic Warehousing](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-138">For more information, see [How to: Move Components to an Operation Area in Basic Warehousing](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span></span>

<span data-ttu-id="b30ef-139">Inventory pick lines for sales items are created in different ways depending on whether none, some, or all of the sales line quantities are assembled to order.</span><span class="sxs-lookup"><span data-stu-id="b30ef-139">Inventory pick lines for sales items are created in different ways depending on whether none, some, or all of the sales line quantities are assembled to order.</span></span>

<span data-ttu-id="b30ef-140">In regular sales where you use inventory picks to post shipment of inventory quantities, one inventory pick line, or several if the item is placed in different bins, is created for each sales order line.</span><span class="sxs-lookup"><span data-stu-id="b30ef-140">In regular sales where you use inventory picks to post shipment of inventory quantities, one inventory pick line, or several if the item is placed in different bins, is created for each sales order line.</span></span> <span data-ttu-id="b30ef-141">This pick line is based on the quantity in the **Qty. to Ship** field.</span><span class="sxs-lookup"><span data-stu-id="b30ef-141">This pick line is based on the quantity in the **Qty. to Ship** field.</span></span>

<span data-ttu-id="b30ef-142">In assemble-to-order sales where the full quantity on the sales order line is assembled to order, one inventory pick line is created for that quantity.</span><span class="sxs-lookup"><span data-stu-id="b30ef-142">In assemble-to-order sales where the full quantity on the sales order line is assembled to order, one inventory pick line is created for that quantity.</span></span> <span data-ttu-id="b30ef-143">This means that the value in the Quantity to Assemble field is the same as the value in the **Qty. to Ship** field.</span><span class="sxs-lookup"><span data-stu-id="b30ef-143">This means that the value in the Quantity to Assemble field is the same as the value in the **Qty. to Ship** field.</span></span> <span data-ttu-id="b30ef-144">The **Assemble to Order** field is selected on the line.</span><span class="sxs-lookup"><span data-stu-id="b30ef-144">The **Assemble to Order** field is selected on the line.</span></span>

<span data-ttu-id="b30ef-145">If an assembly output flow is set up for the location, then the value in the **Asm.-to-Order Shpt. Bin Code** field or the value in the **From-Assembly Bin Code** field, in that order, is inserted in the **Bin Code** field on the inventory pick line.</span><span class="sxs-lookup"><span data-stu-id="b30ef-145">If an assembly output flow is set up for the location, then the value in the **Asm.-to-Order Shpt. Bin Code** field or the value in the **From-Assembly Bin Code** field, in that order, is inserted in the **Bin Code** field on the inventory pick line.</span></span>

<span data-ttu-id="b30ef-146">If no bin code is specified on the sales order line, and no assembly output flow is set up for the location, then the **Bin Code** field on the inventory pick line is empty.</span><span class="sxs-lookup"><span data-stu-id="b30ef-146">If no bin code is specified on the sales order line, and no assembly output flow is set up for the location, then the **Bin Code** field on the inventory pick line is empty.</span></span> <span data-ttu-id="b30ef-147">The warehouse worker must open the **Bin Contents** window and select the bin where the assembly items are assembled.</span><span class="sxs-lookup"><span data-stu-id="b30ef-147">The warehouse worker must open the **Bin Contents** window and select the bin where the assembly items are assembled.</span></span>

<span data-ttu-id="b30ef-148">In combination scenarios, where a part of the quantity must first be assembled and another must be picked from inventory, a minimum of two inventory pick lines are created.</span><span class="sxs-lookup"><span data-stu-id="b30ef-148">In combination scenarios, where a part of the quantity must first be assembled and another must be picked from inventory, a minimum of two inventory pick lines are created.</span></span> <span data-ttu-id="b30ef-149">One pick line is for the assemble-to-order quantity.</span><span class="sxs-lookup"><span data-stu-id="b30ef-149">One pick line is for the assemble-to-order quantity.</span></span> <span data-ttu-id="b30ef-150">The other pick line depends on which bins can fulfill the remaining quantity from inventory.</span><span class="sxs-lookup"><span data-stu-id="b30ef-150">The other pick line depends on which bins can fulfill the remaining quantity from inventory.</span></span> <span data-ttu-id="b30ef-151">Bin codes on the two lines are filled in different ways as described for the two different sales types respectively.</span><span class="sxs-lookup"><span data-stu-id="b30ef-151">Bin codes on the two lines are filled in different ways as described for the two different sales types respectively.</span></span> <span data-ttu-id="b30ef-152">For more information, see the “Combination Scenarios” section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-152">For more information, see the “Combination Scenarios” section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).</span></span>

## <a name="to-pick-components-in-advanced-warehouse-configurations"></a><span data-ttu-id="b30ef-153">To pick components in advanced warehouse configurations</span><span class="sxs-lookup"><span data-stu-id="b30ef-153">To pick components in advanced warehouse configurations</span></span>
<span data-ttu-id="b30ef-154">In advanced warehouse configurations where the location is set up to use picking as well as shipping, you can pick components for production and assembly activities with the **Warehouse Pick** window.</span><span class="sxs-lookup"><span data-stu-id="b30ef-154">In advanced warehouse configurations where the location is set up to use picking as well as shipping, you can pick components for production and assembly activities with the **Warehouse Pick** window.</span></span> <span data-ttu-id="b30ef-155">For more information, see [How to: Pick Items with Warehouse Picks](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-155">For more information, see [How to: Pick Items with Warehouse Picks](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span></span>

<span data-ttu-id="b30ef-156">Alternatively, you can use the **Movement Worksheet** window to move items between bins ad hoc, meaning without reference to a source document.</span><span class="sxs-lookup"><span data-stu-id="b30ef-156">Alternatively, you can use the **Movement Worksheet** window to move items between bins ad hoc, meaning without reference to a source document.</span></span> <span data-ttu-id="b30ef-157">For more information, see [How to: Move Items in Advanced Warehouse Configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-157">For more information, see [How to: Move Items in Advanced Warehouse Configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span></span>  

<span data-ttu-id="b30ef-158">You cannot create a warehouse pick document from scratch because a pick activity is always part of a workflow, either in a pull or a push scenario.</span><span class="sxs-lookup"><span data-stu-id="b30ef-158">You cannot create a warehouse pick document from scratch because a pick activity is always part of a workflow, either in a pull or a push scenario.</span></span>  

<span data-ttu-id="b30ef-159">You can create the warehouse pick document in a push fashion by selecting the **Create Whse. Pick** action on the source document, such as a released assembly order or warehouse shipment.</span><span class="sxs-lookup"><span data-stu-id="b30ef-159">You can create the warehouse pick document in a push fashion by selecting the **Create Whse. Pick** action on the source document, such as a released assembly order or warehouse shipment.</span></span> <span data-ttu-id="b30ef-160">For more information, see [How to: Pick Items with Warehouse Picks](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-160">For more information, see [How to: Pick Items with Warehouse Picks](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span></span>  

<span data-ttu-id="b30ef-161">Alternatively, you can create the warehouse pick document in a pull fashion by using the **Pick Worksheet** window to detect pick requests, both for shipment and internal operations, and then create the required warehouse pick documents.</span><span class="sxs-lookup"><span data-stu-id="b30ef-161">Alternatively, you can create the warehouse pick document in a pull fashion by using the **Pick Worksheet** window to detect pick requests, both for shipment and internal operations, and then create the required warehouse pick documents.</span></span>  

<span data-ttu-id="b30ef-162">The following procedure explains a pull scenario where you pick components for a released production order through the **Pick Worksheet** window.</span><span class="sxs-lookup"><span data-stu-id="b30ef-162">The following procedure explains a pull scenario where you pick components for a released production order through the **Pick Worksheet** window.</span></span> <span data-ttu-id="b30ef-163">The procedure also applies to assembly orders.</span><span class="sxs-lookup"><span data-stu-id="b30ef-163">The procedure also applies to assembly orders.</span></span>  

<span data-ttu-id="b30ef-164">To create pick requests, both for pull and for push scenarios, the source documents in question must be released.</span><span class="sxs-lookup"><span data-stu-id="b30ef-164">To create pick requests, both for pull and for push scenarios, the source documents in question must be released.</span></span> <span data-ttu-id="b30ef-165">Release source documents for internal operations in the following ways.</span><span class="sxs-lookup"><span data-stu-id="b30ef-165">Release source documents for internal operations in the following ways.</span></span>  

 |<span data-ttu-id="b30ef-166">Source Document</span><span class="sxs-lookup"><span data-stu-id="b30ef-166">Source Document</span></span>|<span data-ttu-id="b30ef-167">Release Method</span><span class="sxs-lookup"><span data-stu-id="b30ef-167">Release Method</span></span>|  
 |---------------------|--------------------|  
 |<span data-ttu-id="b30ef-168">Production Order</span><span class="sxs-lookup"><span data-stu-id="b30ef-168">Production Order</span></span>|<span data-ttu-id="b30ef-169">Change order type to released production order.</span><span class="sxs-lookup"><span data-stu-id="b30ef-169">Change order type to released production order.</span></span>|  
 |<span data-ttu-id="b30ef-170">Assembly Order</span><span class="sxs-lookup"><span data-stu-id="b30ef-170">Assembly Order</span></span>|<span data-ttu-id="b30ef-171">Change status to Released.</span><span class="sxs-lookup"><span data-stu-id="b30ef-171">Change status to Released.</span></span>|  

## <a name="to-pick-components-using-the-pick-worksheet"></a><span data-ttu-id="b30ef-172">To pick components using the pick worksheet</span><span class="sxs-lookup"><span data-stu-id="b30ef-172">To pick components using the pick worksheet</span></span>  

1.  <span data-ttu-id="b30ef-173">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Pick Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b30ef-173">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Pick Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b30ef-174">Choose the **Get Warehouse Documents** action, and then select the component lines from the released production order.</span><span class="sxs-lookup"><span data-stu-id="b30ef-174">Choose the **Get Warehouse Documents** action, and then select the component lines from the released production order.</span></span>  
3.  <span data-ttu-id="b30ef-175">Inspect the lines, sort them to ensure an efficient picking round, and combine them with other worksheet lines if necessary to make best use of employee time.</span><span class="sxs-lookup"><span data-stu-id="b30ef-175">Inspect the lines, sort them to ensure an efficient picking round, and combine them with other worksheet lines if necessary to make best use of employee time.</span></span>  
4.  <span data-ttu-id="b30ef-176">Choose the **Create Pick** action.</span><span class="sxs-lookup"><span data-stu-id="b30ef-176">Choose the **Create Pick** action.</span></span>  
5.  <span data-ttu-id="b30ef-177">Define how to create the warehouse pick documents and how to sort pick lines by filling fields in the **Create Pick** window.</span><span class="sxs-lookup"><span data-stu-id="b30ef-177">Define how to create the warehouse pick documents and how to sort pick lines by filling fields in the **Create Pick** window.</span></span>  
6.  <span data-ttu-id="b30ef-178">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b30ef-178">Choose the **OK** button.</span></span>

<span data-ttu-id="b30ef-179">Warehouse pick documents are now created with pick lines for each component that is required in the internal operation.</span><span class="sxs-lookup"><span data-stu-id="b30ef-179">Warehouse pick documents are now created with pick lines for each component that is required in the internal operation.</span></span>

<span data-ttu-id="b30ef-180">If the internal operation area, such as a production shop floor, is set up with a default bin for placement of components to be used in the operation, then that bin code is inserted in the Place lines on the warehouse pick document to instruct warehouse workers where to place the items.</span><span class="sxs-lookup"><span data-stu-id="b30ef-180">If the internal operation area, such as a production shop floor, is set up with a default bin for placement of components to be used in the operation, then that bin code is inserted in the Place lines on the warehouse pick document to instruct warehouse workers where to place the items.</span></span> <span data-ttu-id="b30ef-181">For more information, see [How to: Set Up Basic Warehouses with Operation Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md).</span><span class="sxs-lookup"><span data-stu-id="b30ef-181">For more information, see [How to: Set Up Basic Warehouses with Operation Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md).</span></span>

## <a name="filling-the-consumption-bin"></a><span data-ttu-id="b30ef-182">Filling the Consumption Bin</span><span class="sxs-lookup"><span data-stu-id="b30ef-182">Filling the Consumption Bin</span></span>
<span data-ttu-id="b30ef-183">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span><span class="sxs-lookup"><span data-stu-id="b30ef-183">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span></span>

<span data-ttu-id="b30ef-184">![Bin flow chart](media/binflow.png "BinFlow")</span><span class="sxs-lookup"><span data-stu-id="b30ef-184">![Bin flow chart](media/binflow.png "BinFlow")</span></span>

## <a name="see-also"></a><span data-ttu-id="b30ef-185">See Also</span><span class="sxs-lookup"><span data-stu-id="b30ef-185">See Also</span></span>
[<span data-ttu-id="b30ef-186">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b30ef-186">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="b30ef-187">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="b30ef-187">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="b30ef-188">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="b30ef-188">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="b30ef-189">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="b30ef-189">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="b30ef-190">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b30ef-190">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b30ef-191">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b30ef-191">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
