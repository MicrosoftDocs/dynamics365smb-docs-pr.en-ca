---
title: How to Put Items Away with Inventory Put-aways | Microsoft Docs
description: When your location is setup to require put-away processing but not receive processing, you use the **Inventory Put-away** document to record and post put-away and receipt information for your source documents. The inbound source document can be a purchase order, a sales return order, an inbound transfer order, or a production order whose output is ready for put-away.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 92eae2f24daf8181e39b3d22ea23c31a9ee85347
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="put-items-away-with-inventory-put-aways"></a><span data-ttu-id="6b0b7-104">Put Items Away with Inventory Put-aways</span><span class="sxs-lookup"><span data-stu-id="6b0b7-104">Put Items Away with Inventory Put-aways</span></span>
<span data-ttu-id="6b0b7-105">When your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** document to record and post put-away and receipt information for your source documents.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-105">When your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** document to record and post put-away and receipt information for your source documents.</span></span> <span data-ttu-id="6b0b7-106">The inbound source document can be a purchase order, a sales return order, an inbound transfer order, or an assembly or production order whose output is ready to be put away.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-106">The inbound source document can be a purchase order, a sales return order, an inbound transfer order, or an assembly or production order whose output is ready to be put away.</span></span>  

<span data-ttu-id="6b0b7-107">You can create an inventory put-away in three ways:</span><span class="sxs-lookup"><span data-stu-id="6b0b7-107">You can create an inventory put-away in three ways:</span></span>  

- <span data-ttu-id="6b0b7-108">Create the put-away in two steps by first creating a warehouse request from the source document, which acts as a signal to the warehouse that the source document is ready for put-away.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-108">Create the put-away in two steps by first creating a warehouse request from the source document, which acts as a signal to the warehouse that the source document is ready for put-away.</span></span> <span data-ttu-id="6b0b7-109">The inventory put-away can then be created from the **Inventory Put-away** window based on the source document.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-109">The inventory put-away can then be created from the **Inventory Put-away** window based on the source document.</span></span>  
- <span data-ttu-id="6b0b7-110">Create the inventory put-away directly from the source document itself.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-110">Create the inventory put-away directly from the source document itself.</span></span>  
- <span data-ttu-id="6b0b7-111">Create inventory put-aways for several source documents at once by using a batch job.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-111">Create inventory put-aways for several source documents at once by using a batch job.</span></span>  

## <a name="to-request-an-inventory-put-away-by-releasing-the-source-document"></a><span data-ttu-id="6b0b7-112">To request an inventory put-away by releasing the source document</span><span class="sxs-lookup"><span data-stu-id="6b0b7-112">To request an inventory put-away by releasing the source document</span></span>
<span data-ttu-id="6b0b7-113">For purchase orders, sales return orders, inbound transfer orders, and assembly orders, you create the warehouse request by releasing the order.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-113">For purchase orders, sales return orders, inbound transfer orders, and assembly orders, you create the warehouse request by releasing the order.</span></span> <span data-ttu-id="6b0b7-114">The following describes how to do this from a purchase order.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-114">The following describes how to do this from a purchase order.</span></span>  

1.  <span data-ttu-id="6b0b7-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="6b0b7-116">Select the purchase order that you want to release, and then choose the **Release** action.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-116">Select the purchase order that you want to release, and then choose the **Release** action.</span></span>  

    <span data-ttu-id="6b0b7-117">For production orders, you create the warehouse request by creating an inbound request from the released production order.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-117">For production orders, you create the warehouse request by creating an inbound request from the released production order.</span></span>  
3.  <span data-ttu-id="6b0b7-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Released Production Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Released Production Orders**, and then choose the related link.</span></span>  
4. <span data-ttu-id="6b0b7-119">Choose the **Create Inbound Whse. Request** action.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-119">Choose the **Create Inbound Whse. Request** action.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6b0b7-120">You can also create the inbound warehouse request by selecting the **Create Inbound Request** check box when you refresh the production order.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-120">You can also create the inbound warehouse request by selecting the **Create Inbound Request** check box when you refresh the production order.</span></span> <span data-ttu-id="6b0b7-121">For more information, see [Refresh or Replan Production Orders](production-how-to-replan-refresh-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b7-121">For more information, see [Refresh or Replan Production Orders](production-how-to-replan-refresh-production-orders.md).</span></span>  

<span data-ttu-id="6b0b7-122">When the warehouse request is created, a warehouse employee assigned to putting items away can see that the source document is ready and can create an inventory put-away document.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-122">When the warehouse request is created, a warehouse employee assigned to putting items away can see that the source document is ready and can create an inventory put-away document.</span></span>  

## <a name="to-create-an-inventory-put-away-based-on-the-source-document"></a><span data-ttu-id="6b0b7-123">To create an inventory put-away based on the source document</span><span class="sxs-lookup"><span data-stu-id="6b0b7-123">To create an inventory put-away based on the source document</span></span>
<span data-ttu-id="6b0b7-124">Now that the request is created, the warehouse employee can create a new inventory put-away based on the released source document.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-124">Now that the request is created, the warehouse employee can create a new inventory put-away based on the released source document.</span></span>   
1.  <span data-ttu-id="6b0b7-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Put-away**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Put-away**, and then select the related link.</span></span>  
2. <span data-ttu-id="6b0b7-126">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-126">Choose the **New** action.</span></span>  
3. <span data-ttu-id="6b0b7-127">In the **Source Document** field, select the type of source document you are putting away for.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-127">In the **Source Document** field, select the type of source document you are putting away for.</span></span>  
4. <span data-ttu-id="6b0b7-128">In the **Source No.** field, select the source document.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-128">In the **Source No.** field, select the source document.</span></span>  
5. <span data-ttu-id="6b0b7-129">Alternatively, choose the **Get Source Document** action to select the document from a list of inbound source documents that are ready for put-away at the location.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-129">Alternatively, choose the **Get Source Document** action to select the document from a list of inbound source documents that are ready for put-away at the location.</span></span>  
6. <span data-ttu-id="6b0b7-130">Choose the **OK** button to fill the put-away lines according to the selected source document.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-130">Choose the **OK** button to fill the put-away lines according to the selected source document.</span></span>  

## <a name="to-create-an-inventory-put-away-from-the-source-document"></a><span data-ttu-id="6b0b7-131">To create an inventory put-away from the source document</span><span class="sxs-lookup"><span data-stu-id="6b0b7-131">To create an inventory put-away from the source document</span></span>  
1.  <span data-ttu-id="6b0b7-132">In the source document, which can be a purchase order, sales return order, inbound transfer order, or production order, choose the **Create Inventory Put-away/Pick** action.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-132">In the source document, which can be a purchase order, sales return order, inbound transfer order, or production order, choose the **Create Inventory Put-away/Pick** action.</span></span>  
2. <span data-ttu-id="6b0b7-133">Select the **Create Invt. Put-away** check box.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-133">Select the **Create Invt. Put-away** check box.</span></span>
3. <span data-ttu-id="6b0b7-134">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-134">Choose the **OK** button.</span></span> <span data-ttu-id="6b0b7-135">A new inventory put-away is created.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-135">A new inventory put-away is created.</span></span>

## <a name="to-create-multiple-inventory-put-aways-with-a-batch-job"></a><span data-ttu-id="6b0b7-136">To create multiple inventory put-aways with a batch job</span><span class="sxs-lookup"><span data-stu-id="6b0b7-136">To create multiple inventory put-aways with a batch job</span></span>  
1.  <span data-ttu-id="6b0b7-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Invt. Put-away / Pick**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Invt. Put-away / Pick**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6b0b7-138">On the **Warehouse Request** FastTab of the request window, use the **Source Document** and **Source No.** fields to filter on certain types of documents or ranges of document numbers.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-138">On the **Warehouse Request** FastTab of the request window, use the **Source Document** and **Source No.** fields to filter on certain types of documents or ranges of document numbers.</span></span>  
3.  <span data-ttu-id="6b0b7-139">On the **Options** FastTab, select the **Create Invt. Put-away** check box.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-139">On the **Options** FastTab, select the **Create Invt. Put-away** check box.</span></span>
4.  <span data-ttu-id="6b0b7-140">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-140">Choose the **OK** button.</span></span> <span data-ttu-id="6b0b7-141">The specified inventory put-aways are created.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-141">The specified inventory put-aways are created.</span></span>

## <a name="to-record-the-inventory-put-away"></a><span data-ttu-id="6b0b7-142">To record the inventory put-away</span><span class="sxs-lookup"><span data-stu-id="6b0b7-142">To record the inventory put-away</span></span>  
1. <span data-ttu-id="6b0b7-143">Open a previously created put-away document by selecting one from the **Inventory Put-aways** window.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-143">Open a previously created put-away document by selecting one from the **Inventory Put-aways** window.</span></span>  
2. <span data-ttu-id="6b0b7-144">In the **Bin Code** field on the put-away lines, the bin where the items must be put away is suggesting per the item's default bin.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-144">In the **Bin Code** field on the put-away lines, the bin where the items must be put away is suggesting per the item's default bin.</span></span> <span data-ttu-id="6b0b7-145">You can change the bin in this window if necessary.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-145">You can change the bin in this window if necessary.</span></span>  
3. <span data-ttu-id="6b0b7-146">Perform the put-away and enter the information for the actual quantity put away in the **Qty. to Handle** field.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-146">Perform the put-away and enter the information for the actual quantity put away in the **Qty. to Handle** field.</span></span>

    <span data-ttu-id="6b0b7-147">If it is necessary to place the items for one line in more than one bin, for example because the designated bin is full, then use the **Split Line** function on the **Lines** FastTab.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-147">If it is necessary to place the items for one line in more than one bin, for example because the designated bin is full, then use the **Split Line** function on the **Lines** FastTab.</span></span> <span data-ttu-id="6b0b7-148">For more information about splitting lines, see [Split Warehouse Activity Lines](warehouse-how-to-split-warehouse-activity-lines.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b7-148">For more information about splitting lines, see [Split Warehouse Activity Lines](warehouse-how-to-split-warehouse-activity-lines.md).</span></span>  
4. <span data-ttu-id="6b0b7-149">When you have performed the put-away, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-149">When you have performed the put-away, choose the **Post** action.</span></span>  

<span data-ttu-id="6b0b7-150">The posting process will post the receipt, or for production orders, the output, of the source document lines that have been put away, and if the location uses bins, the posting will also create warehouse entries to post the bin quantity changes.</span><span class="sxs-lookup"><span data-stu-id="6b0b7-150">The posting process will post the receipt, or for production orders, the output, of the source document lines that have been put away, and if the location uses bins, the posting will also create warehouse entries to post the bin quantity changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="6b0b7-151">See Also</span><span class="sxs-lookup"><span data-stu-id="6b0b7-151">See Also</span></span>  
[<span data-ttu-id="6b0b7-152">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="6b0b7-152">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="6b0b7-153">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="6b0b7-153">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="6b0b7-154">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="6b0b7-154">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="6b0b7-155">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="6b0b7-155">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="6b0b7-156">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="6b0b7-156">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="6b0b7-157">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6b0b7-157">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
