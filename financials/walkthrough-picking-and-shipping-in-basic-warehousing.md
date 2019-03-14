---
title: Walkthrough - Picking and Shipping in Basic Warehouse Configurations | Microsoft Docs
description: In Finance and Operations, Business edition, the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 41a23df0e19bda1262dafbfaf89df7518b2b40b6
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a><span data-ttu-id="b2356-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="b2356-103">Walkthrough: Picking and Shipping in Basic Warehouse Configurations</span></span>
<span data-ttu-id="b2356-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span><span class="sxs-lookup"><span data-stu-id="b2356-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="b2356-105">Method</span><span class="sxs-lookup"><span data-stu-id="b2356-105">Method</span></span>|<span data-ttu-id="b2356-106">Inbound process</span><span class="sxs-lookup"><span data-stu-id="b2356-106">Inbound process</span></span>|<span data-ttu-id="b2356-107">Bins</span><span class="sxs-lookup"><span data-stu-id="b2356-107">Bins</span></span>|<span data-ttu-id="b2356-108">Picks</span><span class="sxs-lookup"><span data-stu-id="b2356-108">Picks</span></span>|<span data-ttu-id="b2356-109">Shipments</span><span class="sxs-lookup"><span data-stu-id="b2356-109">Shipments</span></span>|<span data-ttu-id="b2356-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="b2356-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="b2356-111">A</span><span class="sxs-lookup"><span data-stu-id="b2356-111">A</span></span>|<span data-ttu-id="b2356-112">Post pick and shipment from the order line</span><span class="sxs-lookup"><span data-stu-id="b2356-112">Post pick and shipment from the order line</span></span>|<span data-ttu-id="b2356-113">X</span><span class="sxs-lookup"><span data-stu-id="b2356-113">X</span></span>|||<span data-ttu-id="b2356-114">2</span><span class="sxs-lookup"><span data-stu-id="b2356-114">2</span></span>|  
|<span data-ttu-id="b2356-115">B</span><span class="sxs-lookup"><span data-stu-id="b2356-115">B</span></span>|<span data-ttu-id="b2356-116">Post pick and shipment from an inventory pick document</span><span class="sxs-lookup"><span data-stu-id="b2356-116">Post pick and shipment from an inventory pick document</span></span>||<span data-ttu-id="b2356-117">X</span><span class="sxs-lookup"><span data-stu-id="b2356-117">X</span></span>||<span data-ttu-id="b2356-118">3</span><span class="sxs-lookup"><span data-stu-id="b2356-118">3</span></span>|  
|<span data-ttu-id="b2356-119">C</span><span class="sxs-lookup"><span data-stu-id="b2356-119">C</span></span>|<span data-ttu-id="b2356-120">Post pick and shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="b2356-120">Post pick and shipment from a warehouse shipment document</span></span>|||<span data-ttu-id="b2356-121">X</span><span class="sxs-lookup"><span data-stu-id="b2356-121">X</span></span>|<span data-ttu-id="b2356-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="b2356-122">4/5/6</span></span>|  
|<span data-ttu-id="b2356-123">D</span><span class="sxs-lookup"><span data-stu-id="b2356-123">D</span></span>|<span data-ttu-id="b2356-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span><span class="sxs-lookup"><span data-stu-id="b2356-124">Post pick from a warehouse pick document and post shipment from a warehouse shipment document</span></span>||<span data-ttu-id="b2356-125">X</span><span class="sxs-lookup"><span data-stu-id="b2356-125">X</span></span>|<span data-ttu-id="b2356-126">X</span><span class="sxs-lookup"><span data-stu-id="b2356-126">X</span></span>|<span data-ttu-id="b2356-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="b2356-127">4/5/6</span></span>|  

<span data-ttu-id="b2356-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="b2356-128">For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="b2356-129">The following walkthrough demonstrates method B in the previous table.</span><span class="sxs-lookup"><span data-stu-id="b2356-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="b2356-130">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="b2356-130">About This Walkthrough</span></span>  
<span data-ttu-id="b2356-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** window to record and post pick and ship information for your outbound source documents.</span><span class="sxs-lookup"><span data-stu-id="b2356-131">In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Inventory Pick** window to record and post pick and ship information for your outbound source documents.</span></span> <span data-ttu-id="b2356-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span><span class="sxs-lookup"><span data-stu-id="b2356-132">The outbound source document can be a sales order, purchase return order, outbound transfer order, or a production order with component need.</span></span>  

<span data-ttu-id="b2356-133">This walkthrough demonstrates the following tasks:</span><span class="sxs-lookup"><span data-stu-id="b2356-133">This walkthrough demonstrates the following tasks:</span></span>  

-   <span data-ttu-id="b2356-134">Setting up SILVER location for inventory picks.</span><span class="sxs-lookup"><span data-stu-id="b2356-134">Setting up SILVER location for inventory picks.</span></span>  
-   <span data-ttu-id="b2356-135">Creating a sales order for customer 10000 for 30 loudspeakers.</span><span class="sxs-lookup"><span data-stu-id="b2356-135">Creating a sales order for customer 10000 for 30 loudspeakers.</span></span>  
-   <span data-ttu-id="b2356-136">Releasing the sales order for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="b2356-136">Releasing the sales order for warehouse handling.</span></span>  
-   <span data-ttu-id="b2356-137">Creating an inventory pick based on a released source document.</span><span class="sxs-lookup"><span data-stu-id="b2356-137">Creating an inventory pick based on a released source document.</span></span>  
-   <span data-ttu-id="b2356-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span><span class="sxs-lookup"><span data-stu-id="b2356-138">Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.</span></span>  

## <a name="roles"></a><span data-ttu-id="b2356-139">Roles</span><span class="sxs-lookup"><span data-stu-id="b2356-139">Roles</span></span>  
<span data-ttu-id="b2356-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span><span class="sxs-lookup"><span data-stu-id="b2356-140">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="b2356-141">Warehouse Manager</span><span class="sxs-lookup"><span data-stu-id="b2356-141">Warehouse Manager</span></span>  
-   <span data-ttu-id="b2356-142">Order Processor</span><span class="sxs-lookup"><span data-stu-id="b2356-142">Order Processor</span></span>  
-   <span data-ttu-id="b2356-143">Warehouse Worker</span><span class="sxs-lookup"><span data-stu-id="b2356-143">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="b2356-144">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="b2356-144">Prerequisites</span></span>  
<span data-ttu-id="b2356-145">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="b2356-145">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="b2356-146">CRONUS International Ltd. installed.</span><span class="sxs-lookup"><span data-stu-id="b2356-146">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="b2356-147">To make yourself a warehouse employee at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="b2356-147">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="b2356-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Employees**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b2356-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="b2356-149">Choose the **User ID** field, and select your own user account in the **Users** window.</span><span class="sxs-lookup"><span data-stu-id="b2356-149">Choose the **User ID** field, and select your own user account in the **Users** window.</span></span>  
    3.  <span data-ttu-id="b2356-150">In the **Location Code** field, enter SILVER.</span><span class="sxs-lookup"><span data-stu-id="b2356-150">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="b2356-151">Select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="b2356-151">Select the **Default** field.</span></span>  

-   <span data-ttu-id="b2356-152">Make item LS-81 available at SILVER location by following these steps:</span><span class="sxs-lookup"><span data-stu-id="b2356-152">Make item LS-81 available at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="b2356-153">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b2356-153">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Journals**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="b2356-154">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span><span class="sxs-lookup"><span data-stu-id="b2356-154">Open the default journal, and then create two item journal lines with the following information about the work date (January 23).</span></span>  

        |<span data-ttu-id="b2356-155">Entry Type</span><span class="sxs-lookup"><span data-stu-id="b2356-155">Entry Type</span></span>|<span data-ttu-id="b2356-156">Item Number</span><span class="sxs-lookup"><span data-stu-id="b2356-156">Item Number</span></span>|<span data-ttu-id="b2356-157">Location Code</span><span class="sxs-lookup"><span data-stu-id="b2356-157">Location Code</span></span>|<span data-ttu-id="b2356-158">Bin Code</span><span class="sxs-lookup"><span data-stu-id="b2356-158">Bin Code</span></span>|<span data-ttu-id="b2356-159">Quantity</span><span class="sxs-lookup"><span data-stu-id="b2356-159">Quantity</span></span>|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |<span data-ttu-id="b2356-160">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="b2356-160">Positive Adjmt.</span></span>|<span data-ttu-id="b2356-161">LS-81</span><span class="sxs-lookup"><span data-stu-id="b2356-161">LS-81</span></span>|<span data-ttu-id="b2356-162">SILVER</span><span class="sxs-lookup"><span data-stu-id="b2356-162">SILVER</span></span>|<span data-ttu-id="b2356-163">S-01-0001 **Note:**  The item’s default bin in CRONUS</span><span class="sxs-lookup"><span data-stu-id="b2356-163">S-01-0001 **Note:**  The item’s default bin in CRONUS</span></span>|<span data-ttu-id="b2356-164">20</span><span class="sxs-lookup"><span data-stu-id="b2356-164">20</span></span>|  
        |<span data-ttu-id="b2356-165">Positive Adjmt.</span><span class="sxs-lookup"><span data-stu-id="b2356-165">Positive Adjmt.</span></span>|<span data-ttu-id="b2356-166">LS-81</span><span class="sxs-lookup"><span data-stu-id="b2356-166">LS-81</span></span>|<span data-ttu-id="b2356-167">SILVER</span><span class="sxs-lookup"><span data-stu-id="b2356-167">SILVER</span></span>|<span data-ttu-id="b2356-168">S-01-0002</span><span class="sxs-lookup"><span data-stu-id="b2356-168">S-01-0002</span></span>|<span data-ttu-id="b2356-169">20</span><span class="sxs-lookup"><span data-stu-id="b2356-169">20</span></span>|  

    3.  <span data-ttu-id="b2356-170">Choose the **Post** action, and then select the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="b2356-170">Choose the **Post** action, and then select the **Yes** button.</span></span>  

## <a name="story"></a><span data-ttu-id="b2356-171">Story</span><span class="sxs-lookup"><span data-stu-id="b2356-171">Story</span></span>  
<span data-ttu-id="b2356-172">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span><span class="sxs-lookup"><span data-stu-id="b2356-172">Ellen, the warehouse manager at CRONUS, sets up SILVER warehouse for basic pick handling where warehouse workers process outbound orders individually.</span></span> <span data-ttu-id="b2356-173">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span><span class="sxs-lookup"><span data-stu-id="b2356-173">Susan, the order processor, creates a sales order for 30 units of item LS-81 to be shipped to customer 10000 from the SILVER Warehouse.</span></span> <span data-ttu-id="b2356-174">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span><span class="sxs-lookup"><span data-stu-id="b2356-174">John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer.</span></span> <span data-ttu-id="b2356-175">John manages all involved tasks in the **Inventory Pick** window, which automatically points to the bins where LS-81 is stored.</span><span class="sxs-lookup"><span data-stu-id="b2356-175">John manages all involved tasks in the **Inventory Pick** window, which automatically points to the bins where LS-81 is stored.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="b2356-176">Setting Up the Location</span><span class="sxs-lookup"><span data-stu-id="b2356-176">Setting Up the Location</span></span>  
<span data-ttu-id="b2356-177">The setup of the **Location Card** window defines the company’s warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="b2356-177">The setup of the **Location Card** window defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="b2356-178">To set up the location</span><span class="sxs-lookup"><span data-stu-id="b2356-178">To set up the location</span></span>  
1.  <span data-ttu-id="b2356-179">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b2356-179">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b2356-180">Open the SILVER location card.</span><span class="sxs-lookup"><span data-stu-id="b2356-180">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="b2356-181">Select the **Require Pick** check box.</span><span class="sxs-lookup"><span data-stu-id="b2356-181">Select the **Require Pick** check box.</span></span>  

## <a name="creating-the-sales-order"></a><span data-ttu-id="b2356-182">Creating the Sales Order</span><span class="sxs-lookup"><span data-stu-id="b2356-182">Creating the Sales Order</span></span>  
<span data-ttu-id="b2356-183">Sales orders are the most common type of outbound source document.</span><span class="sxs-lookup"><span data-stu-id="b2356-183">Sales orders are the most common type of outbound source document.</span></span>  

### <a name="to-create-the-sales-order"></a><span data-ttu-id="b2356-184">To create the sales order</span><span class="sxs-lookup"><span data-stu-id="b2356-184">To create the sales order</span></span>  
1.  <span data-ttu-id="b2356-185">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b2356-185">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b2356-186">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="b2356-186">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="b2356-187">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span><span class="sxs-lookup"><span data-stu-id="b2356-187">Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.</span></span>  

    |<span data-ttu-id="b2356-188">Item</span><span class="sxs-lookup"><span data-stu-id="b2356-188">Item</span></span>|<span data-ttu-id="b2356-189">Location Code</span><span class="sxs-lookup"><span data-stu-id="b2356-189">Location Code</span></span>|<span data-ttu-id="b2356-190">Quantity</span><span class="sxs-lookup"><span data-stu-id="b2356-190">Quantity</span></span>|  
    |----------|-------------------|--------------|  
    |<span data-ttu-id="b2356-191">LS_81</span><span class="sxs-lookup"><span data-stu-id="b2356-191">LS_81</span></span>|<span data-ttu-id="b2356-192">SILVER</span><span class="sxs-lookup"><span data-stu-id="b2356-192">SILVER</span></span>|<span data-ttu-id="b2356-193">30</span><span class="sxs-lookup"><span data-stu-id="b2356-193">30</span></span>|  

     <span data-ttu-id="b2356-194">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span><span class="sxs-lookup"><span data-stu-id="b2356-194">Proceed to notify the warehouse that the sales order is ready for warehouse handling.</span></span>  

4.  <span data-ttu-id="b2356-195">Choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="b2356-195">Choose the **Release** action.</span></span>  

    <span data-ttu-id="b2356-196">John proceeds to pick and ship the sold items.</span><span class="sxs-lookup"><span data-stu-id="b2356-196">John proceeds to pick and ship the sold items.</span></span>  

## <a name="picking-and-shipping-items"></a><span data-ttu-id="b2356-197">Picking and Shipping Items</span><span class="sxs-lookup"><span data-stu-id="b2356-197">Picking and Shipping Items</span></span>  
<span data-ttu-id="b2356-198">In the **Inventory Pick** window, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span><span class="sxs-lookup"><span data-stu-id="b2356-198">In the **Inventory Pick** window, you can manage all outbound warehouse activities for a specific source document, such as a sales order.</span></span>  

### <a name="to-pick-and-ship-items"></a><span data-ttu-id="b2356-199">To pick and ship items</span><span class="sxs-lookup"><span data-stu-id="b2356-199">To pick and ship items</span></span>  
1.  <span data-ttu-id="b2356-200">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Picks**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b2356-200">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Picks**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b2356-201">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="b2356-201">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="b2356-202">Select the **Source Document** field, and then select **Sales Order**.</span><span class="sxs-lookup"><span data-stu-id="b2356-202">Select the **Source Document** field, and then select **Sales Order**.</span></span>  
4.  <span data-ttu-id="b2356-203">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b2356-203">Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="b2356-204">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span><span class="sxs-lookup"><span data-stu-id="b2356-204">Alternatively, choose the **Get Source Document** action, and then select the sales order.</span></span>  
5.  <span data-ttu-id="b2356-205">Choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="b2356-205">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="b2356-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory pick lines.</span><span class="sxs-lookup"><span data-stu-id="b2356-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory pick lines.</span></span>  
6.  <span data-ttu-id="b2356-207">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b2356-207">Choose the **Post** action, select **Ship**, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="b2356-208">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span><span class="sxs-lookup"><span data-stu-id="b2356-208">The 30 loudspeakers are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b2356-209">See Also</span><span class="sxs-lookup"><span data-stu-id="b2356-209">See Also</span></span>  
 <span data-ttu-id="b2356-210">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-210">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
 <span data-ttu-id="b2356-211">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-211">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
 <span data-ttu-id="b2356-212">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-212">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="b2356-213">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-213">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="b2356-214">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-214">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="b2356-215">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-215">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="b2356-216">[Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="b2356-216">[Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="b2356-217">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="b2356-217">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="b2356-218">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2356-218">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
