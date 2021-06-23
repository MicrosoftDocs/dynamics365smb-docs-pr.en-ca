---
title: Picking and Shipping in Basic Warehouse Configurations
description: In Business Central, the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: jill-kotel-andersson
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: e1763e6288c8b8218955049ba7ef4c461ee5164e
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214662"
---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="8b0fc-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="8b0fc-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>

<!-- [!INCLUDE[complete_sample_data](includes/complete_sample_data.md)] -->

<span data-ttu-id="8b0fc-104">In [!INCLUDE[prod_short](includes/prod_short.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-104">In [!INCLUDE[prod_short](includes/prod_short.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="8b0fc-105">Method</span><span class="sxs-lookup"><span data-stu-id="8b0fc-105">Method</span></span>|<span data-ttu-id="8b0fc-106">Inbound process</span><span class="sxs-lookup"><span data-stu-id="8b0fc-106">Inbound process</span></span>|<span data-ttu-id="8b0fc-107">Bins</span><span class="sxs-lookup"><span data-stu-id="8b0fc-107">Bins</span></span>|<span data-ttu-id="8b0fc-108">Picks</span><span class="sxs-lookup"><span data-stu-id="8b0fc-108">Picks</span></span>|<span data-ttu-id="8b0fc-109">Shipments</span><span class="sxs-lookup"><span data-stu-id="8b0fc-109">Shipments</span></span>|<span data-ttu-id="8b0fc-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="8b0fc-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="8b0fc-111">A</span><span class="sxs-lookup"><span data-stu-id="8b0fc-111">A</span></span>|<span data-ttu-id="8b0fc-112">Post pick and shipment from the order line</span><span class="sxs-lookup"><span data-stu-id="8b0fc-112">Post pick and shipment from the order line</span></span>|<span data-ttu-id="8b0fc-113">X</span><span class="sxs-lookup"><span data-stu-id="8b0fc-113">X</span></span>|||<span data-ttu-id="8b0fc-114">2</span><span class="sxs-lookup"><span data-stu-id="8b0fc-114">2</span></span>|  
|<span data-ttu-id="8b0fc-115">B</span><span class="sxs-lookup"><span data-stu-id="8b0fc-115">B</span></span>|<span data-ttu-id="8b0fc-116">Post pick and shipment from an inventory pick document</span><span class="sxs-lookup"><span data-stu-id="8b0fc-116">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="8b0fc-117">X</span><span class="sxs-lookup"><span data-stu-id="8b0fc-117">X</span></span>||<span data-ttu-id="8b0fc-118">3</span><span class="sxs-lookup"><span data-stu-id="8b0fc-118">3</span></span>|  
|<span data-ttu-id="8b0fc-119">C</span><span class="sxs-lookup"><span data-stu-id="8b0fc-119">C</span></span>|<span data-ttu-id="8b0fc-120">Post pick and shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="8b0fc-120">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="8b0fc-121">X</span><span class="sxs-lookup"><span data-stu-id="8b0fc-121">X</span></span>|<span data-ttu-id="8b0fc-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="8b0fc-122">4/5/6</span></span>|  
|<span data-ttu-id="8b0fc-123">D</span><span class="sxs-lookup"><span data-stu-id="8b0fc-123">D</span></span>|<span data-ttu-id="8b0fc-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="8b0fc-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="8b0fc-125">X</span><span class="sxs-lookup"><span data-stu-id="8b0fc-125">X</span></span>|<span data-ttu-id="8b0fc-126">X</span><span class="sxs-lookup"><span data-stu-id="8b0fc-126">X</span></span>|<span data-ttu-id="8b0fc-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="8b0fc-127">4/5/6</span></span>|  

<span data-ttu-id="8b0fc-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="8b0fc-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="8b0fc-129">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="8b0fc-130">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="8b0fc-130">About This Walkthrough</span></span>

<span data-ttu-id="8b0fc-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="8b0fc-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="8b0fc-133">This walkthrough demonstrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="8b0fc-133">This walkthrough demonstrates the following tasks:</span></span>  

- <span data-ttu-id="8b0fc-134">Setting up SOUTH location for inventory picks.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-134">Setting up SOUTH location for inventory picks.</span></span>  
- <span data-ttu-id="8b0fc-135">Creating a sales order for customer 10000 for 30 Amsterdam Lamps.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-135">Creating a sales order for customer 10000 for 30 Amsterdam Lamps.</span></span>  
- <span data-ttu-id="8b0fc-136">Releasing the sales order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-136">Releasing the sales order for warehouse handling.</span></span>  
- <span data-ttu-id="8b0fc-137">Creating an inventory pick based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-137">Creating an inventory pick based on a released source document.</span></span>  
- <span data-ttu-id="8b0fc-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="8b0fc-139">Roles</span><span class="sxs-lookup"><span data-stu-id="8b0fc-139">Roles</span></span>

<span data-ttu-id="8b0fc-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="8b0fc-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

- <span data-ttu-id="8b0fc-141">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="8b0fc-141">Warehouse Manager</span></span>  
- <span data-ttu-id="8b0fc-142">Order Processor</span><span class="sxs-lookup"><span data-stu-id="8b0fc-142">Order Processor</span></span>  
- <span data-ttu-id="8b0fc-143">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="8b0fc-143">Warehouse Worker</span></span>  

<!-- ## Prerequisites

To complete this walkthrough, you will need:  

- For [!INCLUDE[prod_short](includes/prod_short.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, CRONUS installed.
 -->

## <a name="story"></a><span data-ttu-id="8b0fc-144">Story</span><span class="sxs-lookup"><span data-stu-id="8b0fc-144">Story</span></span>

<span data-ttu-id="8b0fc-145">Ellen, the warehouse manager at CRONUS, sets up SOUTH warehouse for basic pick handling where warehouse workers process outbound orders individually.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-145">Ellen, the warehouse manager at CRONUS, sets up SOUTH warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="8b0fc-146">Susan, the order processor, creates a sales order for 30 units of item 1928-S to be shipped to customer 10000 from the SOUTH Warehouse.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-146">Susan, the order processor, creates a sales order for 30 units of item 1928-S to be shipped to customer 10000 from the SOUTH Warehouse.</span></span> <span data-ttu-id="8b0fc-147">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-147">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="8b0fc-148">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where 1928-S is stored.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-148">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where 1928-S is stored.</span></span>

[!INCLUDE[set_up_location.md](includes/set_up_location.md)]

### <a name="setting-up-the-bin-codes"></a><span data-ttu-id="8b0fc-149">Setting Up the Bin Codes</span><span class="sxs-lookup"><span data-stu-id="8b0fc-149">Setting Up the Bin Codes</span></span>
<span data-ttu-id="8b0fc-150">Once you have the location set up, you must add two bins.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-150">Once you have the location set up, you must add two bins.</span></span>

#### <a name="to-setup-the-bin-codes"></a><span data-ttu-id="8b0fc-151">To setup the bin codes</span><span class="sxs-lookup"><span data-stu-id="8b0fc-151">To setup the bin codes</span></span>

1. <span data-ttu-id="8b0fc-152">Select the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-152">Select the **Bins** action.</span></span>
2. <span data-ttu-id="8b0fc-153">Create two bins, with the codes *S-01-0001* and *S-01-0002*.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-153">Create two bins, with the codes *S-01-0001* and *S-01-0002*.</span></span>

### <a name="making-yourself-a-warehouse-employee-at-location-south"></a><span data-ttu-id="8b0fc-154">Making Yourself a Warehouse Employee at Location SOUTH</span><span class="sxs-lookup"><span data-stu-id="8b0fc-154">Making Yourself a Warehouse Employee at Location SOUTH</span></span>

<span data-ttu-id="8b0fc-155">In order to use this functionality, you must add yourself to the location as a warehouse worker.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-155">In order to use this functionality, you must add yourself to the location as a warehouse worker.</span></span> 

#### <a name="to-make-yourself-a-warehouse-employee"></a><span data-ttu-id="8b0fc-156">To make yourself a warehouse employee</span><span class="sxs-lookup"><span data-stu-id="8b0fc-156">To make yourself a warehouse employee</span></span>

  1. <span data-ttu-id="8b0fc-157">Choose the ![Lightbulb that opens the Tell Me feature first](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-157">Choose the ![Lightbulb that opens the Tell Me feature first](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="8b0fc-158">Choose the **User ID** field, and select your own user account on the **Warehouse Employees** page.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-158">Choose the **User ID** field, and select your own user account on the **Warehouse Employees** page.</span></span>
  3. <span data-ttu-id="8b0fc-159">In the **Location Code** field, choose SOUTH.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-159">In the **Location Code** field, choose SOUTH.</span></span>  
  4. <span data-ttu-id="8b0fc-160">Select the **Default** field, and then select the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-160">Select the **Default** field, and then select the **Yes** button.</span></span>  

### <a name="making-item-1928-s-available"></a><span data-ttu-id="8b0fc-161">Making Item 1928-S Available</span><span class="sxs-lookup"><span data-stu-id="8b0fc-161">Making Item 1928-S Available</span></span>

<span data-ttu-id="8b0fc-162">To make item 1928-S available at the SOUTH location follow these steps:</span><span class="sxs-lookup"><span data-stu-id="8b0fc-162">To make item 1928-S available at the SOUTH location follow these steps:</span></span>  

  1. <span data-ttu-id="8b0fc-163">Choose the ![Lightbulb that opens the Tell Me feature second](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-163">Choose the ![Lightbulb that opens the Tell Me feature second](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span></span>  
  2. <span data-ttu-id="8b0fc-164">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span><span class="sxs-lookup"><span data-stu-id="8b0fc-164">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="8b0fc-165">Entry Type</span><span class="sxs-lookup"><span data-stu-id="8b0fc-165">Entry Type</span></span>|<span data-ttu-id="8b0fc-166">Item Number</span><span class="sxs-lookup"><span data-stu-id="8b0fc-166">Item Number</span></span>|<span data-ttu-id="8b0fc-167">Location Code</span><span class="sxs-lookup"><span data-stu-id="8b0fc-167">Location Code</span></span>|<span data-ttu-id="8b0fc-168">Bin Code</span><span class="sxs-lookup"><span data-stu-id="8b0fc-168">Bin Code</span></span>|<span data-ttu-id="8b0fc-169">Quantity</span><span class="sxs-lookup"><span data-stu-id="8b0fc-169">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="8b0fc-170">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-170">Positive Adjmt.</span></span>|<span data-ttu-id="8b0fc-171">1928-S</span><span class="sxs-lookup"><span data-stu-id="8b0fc-171">1928-S</span></span>|<span data-ttu-id="8b0fc-172">SOUTH</span><span class="sxs-lookup"><span data-stu-id="8b0fc-172">SOUTH</span></span>|<span data-ttu-id="8b0fc-173">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="8b0fc-173">S-01-0001</span></span>|<span data-ttu-id="8b0fc-174">20</span><span class="sxs-lookup"><span data-stu-id="8b0fc-174">20</span></span>|  
        |<span data-ttu-id="8b0fc-175">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-175">Positive Adjmt.</span></span>|<span data-ttu-id="8b0fc-176">1928-S</span><span class="sxs-lookup"><span data-stu-id="8b0fc-176">1928-S</span></span>|<span data-ttu-id="8b0fc-177">SOUTH</span><span class="sxs-lookup"><span data-stu-id="8b0fc-177">SOUTH</span></span>|<span data-ttu-id="8b0fc-178">S-01-0002</span><span class="sxs-lookup"><span data-stu-id="8b0fc-178">S-01-0002</span></span>|<span data-ttu-id="8b0fc-179">20</span><span class="sxs-lookup"><span data-stu-id="8b0fc-179">20</span></span>|  

        <span data-ttu-id="8b0fc-180">By default, the **Bin Code** field on the sales lines are hidden, so you must display it.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-180">By default, the **Bin Code** field on the sales lines are hidden, so you must display it.</span></span> <span data-ttu-id="8b0fc-181">To do this you need to personalize the page.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-181">To do this you need to personalize the page.</span></span> <span data-ttu-id="8b0fc-182">For more information, see [To start personalizing a page through the Personalizing banner](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).</span><span class="sxs-lookup"><span data-stu-id="8b0fc-182">For more information, see [To start personalizing a page through the Personalizing banner](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).</span></span>

  3. <span data-ttu-id="8b0fc-183">Choose **Actions**, then **Posting**, and then choose **Post**.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-183">Choose **Actions**, then **Posting**, and then choose **Post**.</span></span>  
  4. <span data-ttu-id="8b0fc-184">Select the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-184">Select the **Yes** button.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="8b0fc-185">Creating the Sales Order</span><span class="sxs-lookup"><span data-stu-id="8b0fc-185">Creating the Sales Order</span></span>

<span data-ttu-id="8b0fc-186">Sales orders are the most common type of outbound source document.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-186">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="8b0fc-187">To create the sales order</span><span class="sxs-lookup"><span data-stu-id="8b0fc-187">To create the sales order</span></span>

1. <span data-ttu-id="8b0fc-188">Choose the ![Lightbulb that opens the Tell Me feature third](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-188">Choose the ![Lightbulb that opens the Tell Me feature third](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8b0fc-189">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-189">Choose the **New** action.</span></span>  
3. <span data-ttu-id="8b0fc-190">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-190">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="8b0fc-191">Item</span><span class="sxs-lookup"><span data-stu-id="8b0fc-191">Item</span></span>|<span data-ttu-id="8b0fc-192">Location Code</span><span class="sxs-lookup"><span data-stu-id="8b0fc-192">Location Code</span></span>|<span data-ttu-id="8b0fc-193">Quantity</span><span class="sxs-lookup"><span data-stu-id="8b0fc-193">Quantity</span></span>|  
    |----|-------------|--------|  
    |<span data-ttu-id="8b0fc-194">1928-S</span><span class="sxs-lookup"><span data-stu-id="8b0fc-194">1928-S</span></span>|<span data-ttu-id="8b0fc-195">SOUTH</span><span class="sxs-lookup"><span data-stu-id="8b0fc-195">SOUTH</span></span>|<span data-ttu-id="8b0fc-196">30</span><span class="sxs-lookup"><span data-stu-id="8b0fc-196">30</span></span>|  

     <span data-ttu-id="8b0fc-197">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-197">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4. <span data-ttu-id="8b0fc-198">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-198">Choose the **Release** action.</span></span>  

    <span data-ttu-id="8b0fc-199">John proceeds to pick and ship the sold items.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-199">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="8b0fc-200">Picking and Shipping Items</span><span class="sxs-lookup"><span data-stu-id="8b0fc-200">Picking and Shipping Items</span></span>

<span data-ttu-id="8b0fc-201">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-201">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="8b0fc-202">To pick and ship items</span><span class="sxs-lookup"><span data-stu-id="8b0fc-202">To pick and ship items</span></span>

1. <span data-ttu-id="8b0fc-203">Choose the ![Lightbulb that opens the Tell Me feature fourth](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-203">Choose the ![Lightbulb that opens the Tell Me feature fourth](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8b0fc-204">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-204">Choose the **New** action.</span></span>  

    <span data-ttu-id="8b0fc-205">Make sure that the **No.**</span><span class="sxs-lookup"><span data-stu-id="8b0fc-205">Make sure that the **No.**</span></span> <span data-ttu-id="8b0fc-206">field on the **General** FastTab is filled in.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-206">field on the **General** FastTab is filled in.</span></span>
3. <span data-ttu-id="8b0fc-207">Select the **Source Document** field, and then select **Sales Order**.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-207">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4. <span data-ttu-id="8b0fc-208">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-208">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="8b0fc-209">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-209">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5. <span data-ttu-id="8b0fc-210">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-210">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="8b0fc-211">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-211">Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two inventory pick lines.</span></span>  
6. <span data-ttu-id="8b0fc-212">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-212">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="8b0fc-213">The 30 Amsterdam Lamps are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span><span class="sxs-lookup"><span data-stu-id="8b0fc-213">The 30 Amsterdam Lamps are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8b0fc-214">See Also</span><span class="sxs-lookup"><span data-stu-id="8b0fc-214">See Also</span></span>

[<span data-ttu-id="8b0fc-215">Pick Items with Inventory Picks</span><span class="sxs-lookup"><span data-stu-id="8b0fc-215">Pick Items with Inventory Picks</span></span>](warehouse-how-to-pick-items-with-inventory-picks.md)  
[<span data-ttu-id="8b0fc-216">Pick Items for Warehouse Shipment</span><span class="sxs-lookup"><span data-stu-id="8b0fc-216">Pick Items for Warehouse Shipment</span></span>](warehouse-how-to-pick-items-for-warehouse-shipment.md)  
[<span data-ttu-id="8b0fc-217">Set Up Basic Warehouses with Operations Areas</span><span class="sxs-lookup"><span data-stu-id="8b0fc-217">Set Up Basic Warehouses with Operations Areas</span></span>](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)  
[<span data-ttu-id="8b0fc-218">Move Components to an Operation Area in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="8b0fc-218">Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  
[<span data-ttu-id="8b0fc-219">Pick for Production or Assembly</span><span class="sxs-lookup"><span data-stu-id="8b0fc-219">Pick for Production or Assembly</span></span>](warehouse-how-to-pick-for-production.md)  
[<span data-ttu-id="8b0fc-220">Move Items Ad Hoc in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="8b0fc-220">Move Items Ad Hoc in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)  
[<span data-ttu-id="8b0fc-221">Design Details: Outbound Warehouse Flow</span><span class="sxs-lookup"><span data-stu-id="8b0fc-221">Design Details: Outbound Warehouse Flow</span></span>](design-details-outbound-warehouse-flow.md)  
[<span data-ttu-id="8b0fc-222">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="8b0fc-222">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
<span data-ttu-id="8b0fc-223">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8b0fc-223">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]
