---
title: Picking and Shipping in Basic Warehouse Configurations | Microsoft Docs
description: In Business Central, the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 01/31/2019
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a94c4f2f8d622a91b74ba0de6f0f18e7eb84a5ef
ms.openlocfilehash: 1b07a3b064f1bc45a183d0a2d27b810312007a22
ms.contentlocale: en-ca
ms.lasthandoff: 01/31/2019

---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="4c29b-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="4c29b-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>

<span data-ttu-id="4c29b-104">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="4c29b-104">**Note**: This walkthrough must be performed on a demonstration company with the **Full Evaluation - Complete Sample Data** option, which is available in the Sandbox environment.</span></span> <span data-ttu-id="4c29b-105">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span><span class="sxs-lookup"><span data-stu-id="4c29b-105">For more information, see [Creating a Sandbox Environment](across-how-create-sandbox-environment.md).</span></span>

<span data-ttu-id="4c29b-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="4c29b-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="4c29b-107">Method</span><span class="sxs-lookup"><span data-stu-id="4c29b-107">Method</span></span>|<span data-ttu-id="4c29b-108">Inbound process</span><span class="sxs-lookup"><span data-stu-id="4c29b-108">Inbound process</span></span>|<span data-ttu-id="4c29b-109">Bins</span><span class="sxs-lookup"><span data-stu-id="4c29b-109">Bins</span></span>|<span data-ttu-id="4c29b-110">Picks</span><span class="sxs-lookup"><span data-stu-id="4c29b-110">Picks</span></span>|<span data-ttu-id="4c29b-111">Shipments</span><span class="sxs-lookup"><span data-stu-id="4c29b-111">Shipments</span></span>|<span data-ttu-id="4c29b-112">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="4c29b-112">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="4c29b-113">A</span><span class="sxs-lookup"><span data-stu-id="4c29b-113">A</span></span>|<span data-ttu-id="4c29b-114">Post pick and shipment from the order line</span><span class="sxs-lookup"><span data-stu-id="4c29b-114">Post pick and shipment from the order line</span></span>|<span data-ttu-id="4c29b-115">X</span><span class="sxs-lookup"><span data-stu-id="4c29b-115">X</span></span>|||<span data-ttu-id="4c29b-116">2</span><span class="sxs-lookup"><span data-stu-id="4c29b-116">2</span></span>|  
|<span data-ttu-id="4c29b-117">B</span><span class="sxs-lookup"><span data-stu-id="4c29b-117">B</span></span>|<span data-ttu-id="4c29b-118">Post pick and shipment from an inventory pick document</span><span class="sxs-lookup"><span data-stu-id="4c29b-118">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="4c29b-119">X</span><span class="sxs-lookup"><span data-stu-id="4c29b-119">X</span></span>||<span data-ttu-id="4c29b-120">3</span><span class="sxs-lookup"><span data-stu-id="4c29b-120">3</span></span>|  
|<span data-ttu-id="4c29b-121">C</span><span class="sxs-lookup"><span data-stu-id="4c29b-121">C</span></span>|<span data-ttu-id="4c29b-122">Post pick and shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="4c29b-122">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="4c29b-123">X</span><span class="sxs-lookup"><span data-stu-id="4c29b-123">X</span></span>|<span data-ttu-id="4c29b-124">4/5/6</span><span class="sxs-lookup"><span data-stu-id="4c29b-124">4/5/6</span></span>|  
|<span data-ttu-id="4c29b-125">D</span><span class="sxs-lookup"><span data-stu-id="4c29b-125">D</span></span>|<span data-ttu-id="4c29b-126">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="4c29b-126">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="4c29b-127">X</span><span class="sxs-lookup"><span data-stu-id="4c29b-127">X</span></span>|<span data-ttu-id="4c29b-128">X</span><span class="sxs-lookup"><span data-stu-id="4c29b-128">X</span></span>|<span data-ttu-id="4c29b-129">4/5/6</span><span class="sxs-lookup"><span data-stu-id="4c29b-129">4/5/6</span></span>|  

<span data-ttu-id="4c29b-130">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="4c29b-130">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="4c29b-131">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="4c29b-131">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="4c29b-132">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="4c29b-132">About This Walkthrough</span></span>  
<span data-ttu-id="4c29b-133">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span><span class="sxs-lookup"><span data-stu-id="4c29b-133">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** page to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="4c29b-134">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span><span class="sxs-lookup"><span data-stu-id="4c29b-134">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="4c29b-135">This walkthrough demonstrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="4c29b-135">This walkthrough demonstrates the following tasks:</span></span>  

-   <span data-ttu-id="4c29b-136">Setting up SILVER location for inventory picks.</span><span class="sxs-lookup"><span data-stu-id="4c29b-136">Setting up SILVER location for inventory picks.</span></span>  
-   <span data-ttu-id="4c29b-137">Creating a sales order for customer 10000 for 30 loudspeakers.</span><span class="sxs-lookup"><span data-stu-id="4c29b-137">Creating a sales order for customer 10000 for 30 loudspeakers.</span></span>  
-   <span data-ttu-id="4c29b-138">Releasing the sales order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="4c29b-138">Releasing the sales order for warehouse handling.</span></span>  
-   <span data-ttu-id="4c29b-139">Creating an inventory pick based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="4c29b-139">Creating an inventory pick based on a released source document.</span></span>  
-   <span data-ttu-id="4c29b-140">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span><span class="sxs-lookup"><span data-stu-id="4c29b-140">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="4c29b-141">Roles</span><span class="sxs-lookup"><span data-stu-id="4c29b-141">Roles</span></span>  
<span data-ttu-id="4c29b-142">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="4c29b-142">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="4c29b-143">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="4c29b-143">Warehouse Manager</span></span>  
-   <span data-ttu-id="4c29b-144">Order Processor</span><span class="sxs-lookup"><span data-stu-id="4c29b-144">Order Processor</span></span>  
-   <span data-ttu-id="4c29b-145">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="4c29b-145">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="4c29b-146">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="4c29b-146">Prerequisites</span></span>  
<span data-ttu-id="4c29b-147">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="4c29b-147">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="4c29b-148">CRONUS International Ltd. installed.</span><span class="sxs-lookup"><span data-stu-id="4c29b-148">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="4c29b-149">To make yourself a warehouse employee at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="4c29b-149">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="4c29b-150">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c29b-150">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="4c29b-151">Choose the **User ID** field, and select your own user account on the **Users** page.</span><span class="sxs-lookup"><span data-stu-id="4c29b-151">Choose the **User ID** field, and select your own user account on the **Users** page.</span></span>  
    3.  <span data-ttu-id="4c29b-152">In the **Location Code** field, enter SILVER.</span><span class="sxs-lookup"><span data-stu-id="4c29b-152">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="4c29b-153">Select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="4c29b-153">Select the **Default** field.</span></span>  

-   <span data-ttu-id="4c29b-154">Make item LS-81 available at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="4c29b-154">Make item LS-81 available at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="4c29b-155">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c29b-155">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="4c29b-156">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span><span class="sxs-lookup"><span data-stu-id="4c29b-156">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="4c29b-157">Entry Type</span><span class="sxs-lookup"><span data-stu-id="4c29b-157">Entry Type</span></span>|<span data-ttu-id="4c29b-158">Item Number</span><span class="sxs-lookup"><span data-stu-id="4c29b-158">Item Number</span></span>|<span data-ttu-id="4c29b-159">Location Code</span><span class="sxs-lookup"><span data-stu-id="4c29b-159">Location Code</span></span>|<span data-ttu-id="4c29b-160">Bin Code</span><span class="sxs-lookup"><span data-stu-id="4c29b-160">Bin Code</span></span>|<span data-ttu-id="4c29b-161">Quantity</span><span class="sxs-lookup"><span data-stu-id="4c29b-161">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="4c29b-162">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="4c29b-162">Positive Adjmt.</span></span>|<span data-ttu-id="4c29b-163">LS-81</span><span class="sxs-lookup"><span data-stu-id="4c29b-163">LS-81</span></span>|<span data-ttu-id="4c29b-164">SILVER</span><span class="sxs-lookup"><span data-stu-id="4c29b-164">SILVER</span></span>|<span data-ttu-id="4c29b-165">S-01-0001 **Note:**  The item’s default bin in CRONUS</span><span class="sxs-lookup"><span data-stu-id="4c29b-165">S-01-0001 **Note:**  The item’s default bin in CRONUS</span></span>|<span data-ttu-id="4c29b-166">20</span><span class="sxs-lookup"><span data-stu-id="4c29b-166">20</span></span>|  
        |<span data-ttu-id="4c29b-167">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="4c29b-167">Positive Adjmt.</span></span>|<span data-ttu-id="4c29b-168">LS-81</span><span class="sxs-lookup"><span data-stu-id="4c29b-168">LS-81</span></span>|<span data-ttu-id="4c29b-169">SILVER</span><span class="sxs-lookup"><span data-stu-id="4c29b-169">SILVER</span></span>|<span data-ttu-id="4c29b-170">S-01-0002</span><span class="sxs-lookup"><span data-stu-id="4c29b-170">S-01-0002</span></span>|<span data-ttu-id="4c29b-171">20</span><span class="sxs-lookup"><span data-stu-id="4c29b-171">20</span></span>|  

    3.  <span data-ttu-id="4c29b-172">Choose the **Post** action, and then select the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="4c29b-172">Choose the **Post** action, and then select the **Yes** button.</span></span>  

## <a name="story"></a><span data-ttu-id="4c29b-173">Story</span><span class="sxs-lookup"><span data-stu-id="4c29b-173">Story</span></span>  
<span data-ttu-id="4c29b-174">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span><span class="sxs-lookup"><span data-stu-id="4c29b-174">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="4c29b-175">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span><span class="sxs-lookup"><span data-stu-id="4c29b-175">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span></span> <span data-ttu-id="4c29b-176">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span><span class="sxs-lookup"><span data-stu-id="4c29b-176">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="4c29b-177">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where LS-81 is stored.</span><span class="sxs-lookup"><span data-stu-id="4c29b-177">John manages all involved tasks on the **Inventory Pick** page, which automatically points to the bins where LS-81 is stored.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="4c29b-178">Setting Up the Location</span><span class="sxs-lookup"><span data-stu-id="4c29b-178">Setting Up the Location</span></span>  
<span data-ttu-id="4c29b-179">The setup of the **Location Card** page defines the company’s warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="4c29b-179">The setup of the **Location Card** page defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="4c29b-180">To set up the location</span><span class="sxs-lookup"><span data-stu-id="4c29b-180">To set up the location</span></span>  
1.  <span data-ttu-id="4c29b-181">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c29b-181">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4c29b-182">Open the SILVER location card.</span><span class="sxs-lookup"><span data-stu-id="4c29b-182">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="4c29b-183">Select the **Require Pick** check box.</span><span class="sxs-lookup"><span data-stu-id="4c29b-183">Select the **Require Pick** check box.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="4c29b-184">Creating the Sales Order</span><span class="sxs-lookup"><span data-stu-id="4c29b-184">Creating the Sales Order</span></span>  
<span data-ttu-id="4c29b-185">Sales orders are the most common type of outbound source document.</span><span class="sxs-lookup"><span data-stu-id="4c29b-185">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="4c29b-186">To create the sales order</span><span class="sxs-lookup"><span data-stu-id="4c29b-186">To create the sales order</span></span>  
1.  <span data-ttu-id="4c29b-187">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c29b-187">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4c29b-188">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="4c29b-188">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="4c29b-189">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span><span class="sxs-lookup"><span data-stu-id="4c29b-189">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="4c29b-190">Item</span><span class="sxs-lookup"><span data-stu-id="4c29b-190">Item</span></span>|<span data-ttu-id="4c29b-191">Location Code</span><span class="sxs-lookup"><span data-stu-id="4c29b-191">Location Code</span></span>|<span data-ttu-id="4c29b-192">Quantity</span><span class="sxs-lookup"><span data-stu-id="4c29b-192">Quantity</span></span>|  
    |----------|-------------------|--------------|  
    |<span data-ttu-id="4c29b-193">LS_81</span><span class="sxs-lookup"><span data-stu-id="4c29b-193">LS_81</span></span>|<span data-ttu-id="4c29b-194">SILVER</span><span class="sxs-lookup"><span data-stu-id="4c29b-194">SILVER</span></span>|<span data-ttu-id="4c29b-195">30</span><span class="sxs-lookup"><span data-stu-id="4c29b-195">30</span></span>|  

     <span data-ttu-id="4c29b-196">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="4c29b-196">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4.  <span data-ttu-id="4c29b-197">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="4c29b-197">Choose the **Release** action.</span></span>  

    <span data-ttu-id="4c29b-198">John proceeds to pick and ship the sold items.</span><span class="sxs-lookup"><span data-stu-id="4c29b-198">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="4c29b-199">Picking and Shipping Items</span><span class="sxs-lookup"><span data-stu-id="4c29b-199">Picking and Shipping Items</span></span>  
<span data-ttu-id="4c29b-200">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span><span class="sxs-lookup"><span data-stu-id="4c29b-200">On the **Inventory Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span>  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="4c29b-201">To pick and ship items</span><span class="sxs-lookup"><span data-stu-id="4c29b-201">To pick and ship items</span></span>  
1.  <span data-ttu-id="4c29b-202">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c29b-202">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4c29b-203">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="4c29b-203">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="4c29b-204">Select the **Source Document** field, and then select **Sales Order**.</span><span class="sxs-lookup"><span data-stu-id="4c29b-204">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4.  <span data-ttu-id="4c29b-205">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4c29b-205">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="4c29b-206">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span><span class="sxs-lookup"><span data-stu-id="4c29b-206">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5.  <span data-ttu-id="4c29b-207">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="4c29b-207">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="4c29b-208">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory pick lines.</span><span class="sxs-lookup"><span data-stu-id="4c29b-208">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory pick lines.</span></span>  
6.  <span data-ttu-id="4c29b-209">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4c29b-209">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="4c29b-210">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span><span class="sxs-lookup"><span data-stu-id="4c29b-210">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4c29b-211">See Also</span><span class="sxs-lookup"><span data-stu-id="4c29b-211">See Also</span></span>  
 <span data-ttu-id="4c29b-212">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-212">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
 <span data-ttu-id="4c29b-213">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-213">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
 <span data-ttu-id="4c29b-214">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-214">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="4c29b-215">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-215">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="4c29b-216">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-216">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="4c29b-217">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-217">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="4c29b-218">[Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="4c29b-218">[Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="4c29b-219">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="4c29b-219">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="4c29b-220">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4c29b-220">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
