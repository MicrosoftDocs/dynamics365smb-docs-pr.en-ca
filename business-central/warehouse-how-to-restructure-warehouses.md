---
title: How to Restructure Warehouses | Microsoft Docs
description: You may want to restructure your warehouse with new bin codes and new bin characteristics.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 06233abf9eef229ac86ee31857352af1de5e34e2
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="restructure-warehouses"></a><span data-ttu-id="8ba45-103">Restructure Warehouses</span><span class="sxs-lookup"><span data-stu-id="8ba45-103">Restructure Warehouses</span></span>
<span data-ttu-id="8ba45-104">You may want to restructure your warehouse with new bin codes and new bin characteristics.</span><span class="sxs-lookup"><span data-stu-id="8ba45-104">You may want to restructure your warehouse with new bin codes and new bin characteristics.</span></span> <span data-ttu-id="8ba45-105">You will not undertake this kind of activity very often, but situations can occur where a reclassification is necessary to achieve or maintain a more efficient operation.</span><span class="sxs-lookup"><span data-stu-id="8ba45-105">You will not undertake this kind of activity very often, but situations can occur where a reclassification is necessary to achieve or maintain a more efficient operation.</span></span> <span data-ttu-id="8ba45-106">For example:</span><span class="sxs-lookup"><span data-stu-id="8ba45-106">For example:</span></span>  

- <span data-ttu-id="8ba45-107">You might want to switch to bin codes that support the use of automatic data capture, for example, with hand-held devices.</span><span class="sxs-lookup"><span data-stu-id="8ba45-107">You might want to switch to bin codes that support the use of automatic data capture, for example, with hand-held devices.</span></span>  
- <span data-ttu-id="8ba45-108">The warehouse may have purchased a new rack system that gives new possibilities in item storage.</span><span class="sxs-lookup"><span data-stu-id="8ba45-108">The warehouse may have purchased a new rack system that gives new possibilities in item storage.</span></span>  
- <span data-ttu-id="8ba45-109">The company may have altered its item assortment and moved the warehouse to a new physical location to accommodate this change.</span><span class="sxs-lookup"><span data-stu-id="8ba45-109">The company may have altered its item assortment and moved the warehouse to a new physical location to accommodate this change.</span></span>  

<span data-ttu-id="8ba45-110">If your warehouse is set up to use bins but not directed put-away and pick, restructure your warehouse by creating the new bins that you want to use in the future.</span><span class="sxs-lookup"><span data-stu-id="8ba45-110">If your warehouse is set up to use bins but not directed put-away and pick, restructure your warehouse by creating the new bins that you want to use in the future.</span></span>  

## <a name="to-restructure-a-basic-warehouse-that-uses-bins-only"></a><span data-ttu-id="8ba45-111">To restructure a basic warehouse that uses bins only</span><span class="sxs-lookup"><span data-stu-id="8ba45-111">To restructure a basic warehouse that uses bins only</span></span>  
1.  <span data-ttu-id="8ba45-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ba45-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8ba45-113">On the **Warehouse** FastTab, set the **Default Bin Selection** field to **Last-Used Bin**.</span><span class="sxs-lookup"><span data-stu-id="8ba45-113">On the **Warehouse** FastTab, set the **Default Bin Selection** field to **Last-Used Bin**.</span></span>  
3.  <span data-ttu-id="8ba45-114">Move all the contents of your current bins to the new bins that you have just created.</span><span class="sxs-lookup"><span data-stu-id="8ba45-114">Move all the contents of your current bins to the new bins that you have just created.</span></span>  

    1.  <span data-ttu-id="8ba45-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Reclassification Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ba45-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Reclassification Journal**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="8ba45-116">Select a journal line, and then choose the **Get Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="8ba45-116">Select a journal line, and then choose the **Get Bin Content** action.</span></span>  
    3.  <span data-ttu-id="8ba45-117">On the **Bin Content** FastTab, set filters in the **Location Code**, **Bin Code**, and **Item No.** fields to specify the content that you want to move.</span><span class="sxs-lookup"><span data-stu-id="8ba45-117">On the **Bin Content** FastTab, set filters in the **Location Code**, **Bin Code**, and **Item No.** fields to specify the content that you want to move.</span></span>  
    4.  <span data-ttu-id="8ba45-118">Choose the **OK** button to fill a journal line.</span><span class="sxs-lookup"><span data-stu-id="8ba45-118">Choose the **OK** button to fill a journal line.</span></span>  
    5.  <span data-ttu-id="8ba45-119">In the **New Bin Code** field, select the bin to which the items should be moved.</span><span class="sxs-lookup"><span data-stu-id="8ba45-119">In the **New Bin Code** field, select the bin to which the items should be moved.</span></span>  
    6.  <span data-ttu-id="8ba45-120">Repeat steps b through e for all bin content that you want to move.</span><span class="sxs-lookup"><span data-stu-id="8ba45-120">Repeat steps b through e for all bin content that you want to move.</span></span>  
    7.  <span data-ttu-id="8ba45-121">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="8ba45-121">Choose the **Post** action.</span></span>  

<span data-ttu-id="8ba45-122">You have now emptied the bins where the items used to be.</span><span class="sxs-lookup"><span data-stu-id="8ba45-122">You have now emptied the bins where the items used to be.</span></span> <span data-ttu-id="8ba45-123">The default bins for your items have now been changed to the new bins.</span><span class="sxs-lookup"><span data-stu-id="8ba45-123">The default bins for your items have now been changed to the new bins.</span></span>  

## <a name="to-restructure-an-advanced-warehouse-that-uses-directed-put-away-and-pick"></a><span data-ttu-id="8ba45-124">To restructure an advanced warehouse that uses directed put-away and pick</span><span class="sxs-lookup"><span data-stu-id="8ba45-124">To restructure an advanced warehouse that uses directed put-away and pick</span></span>  

1.  <span data-ttu-id="8ba45-125">Create the new bins that you want to use in the future.</span><span class="sxs-lookup"><span data-stu-id="8ba45-125">Create the new bins that you want to use in the future.</span></span> <span data-ttu-id="8ba45-126">For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md).</span><span class="sxs-lookup"><span data-stu-id="8ba45-126">For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md).</span></span>  
2.  <span data-ttu-id="8ba45-127">Move all the contents of your current bins to the new bins that you just created.</span><span class="sxs-lookup"><span data-stu-id="8ba45-127">Move all the contents of your current bins to the new bins that you just created.</span></span>  

    1.  <span data-ttu-id="8ba45-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Reclassification Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ba45-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Reclassification Journal**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="8ba45-129">For the bins where no real movement of items is involved, create a line for each of your current bins in the **Warehouse Reclassification Journal** with the old bin code, **From Bin Code**, and the new bin code, **To Bin Code**.</span><span class="sxs-lookup"><span data-stu-id="8ba45-129">For the bins where no real movement of items is involved, create a line for each of your current bins in the **Warehouse Reclassification Journal** with the old bin code, **From Bin Code**, and the new bin code, **To Bin Code**.</span></span>  
    3.  <span data-ttu-id="8ba45-130">If some of the movements involve actual physical movements that you want employees to perform, use **Movement Worksheets** to prepare movement instructions instead of using the warehouse reclassification journal.</span><span class="sxs-lookup"><span data-stu-id="8ba45-130">If some of the movements involve actual physical movements that you want employees to perform, use **Movement Worksheets** to prepare movement instructions instead of using the warehouse reclassification journal.</span></span> <span data-ttu-id="8ba45-131">For more information, see [Move Items in Advanced Warehouse Configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="8ba45-131">For more information, see [Move Items in Advanced Warehouse Configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span></span>  

3.  <span data-ttu-id="8ba45-132">When the old bins are emptied, reclassify them as **QC** type bins to ensure that they are not included in item flows.</span><span class="sxs-lookup"><span data-stu-id="8ba45-132">When the old bins are emptied, reclassify them as **QC** type bins to ensure that they are not included in item flows.</span></span>  

    1.  <span data-ttu-id="8ba45-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ba45-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="8ba45-134">Select the line with the location, and then choose the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="8ba45-134">Select the line with the location, and then choose the **Bins** action.</span></span>  
    3.  <span data-ttu-id="8ba45-135">On the **Bins** page, in the **Bin Type Code** field, enter **QC** for each of the old bins that you emptied in step 3 in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="8ba45-135">On the **Bins** page, in the **Bin Type Code** field, enter **QC** for each of the old bins that you emptied in step 3 in the previous procedure.</span></span>  

<span data-ttu-id="8ba45-136">You have now removed the bins from the warehouse flow, and reclassified them as QC bins. QC bins have none of the activity fields on the **Bin Types** page selected and are therefore not considered by the item flow.</span><span class="sxs-lookup"><span data-stu-id="8ba45-136">You have now removed the bins from the warehouse flow, and reclassified them as QC bins. QC bins have none of the activity fields on the **Bin Types** page selected and are therefore not considered by the item flow.</span></span> <span data-ttu-id="8ba45-137">For more information, see [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).</span><span class="sxs-lookup"><span data-stu-id="8ba45-137">For more information, see [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).</span></span>  

## <a name="to-delete-a-bin"></a><span data-ttu-id="8ba45-138">To delete a bin</span><span class="sxs-lookup"><span data-stu-id="8ba45-138">To delete a bin</span></span>  

1.  <span data-ttu-id="8ba45-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ba45-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8ba45-140">Select the location where you want to delete bins. Choose the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="8ba45-140">Select the location where you want to delete bins. Choose the **Bins** action.</span></span>  
3.  <span data-ttu-id="8ba45-141">Select the lines for the bins that you want to delete.</span><span class="sxs-lookup"><span data-stu-id="8ba45-141">Select the lines for the bins that you want to delete.</span></span>  
4.  <span data-ttu-id="8ba45-142">Choose the **Delete** action.</span><span class="sxs-lookup"><span data-stu-id="8ba45-142">Choose the **Delete** action.</span></span>  

<span data-ttu-id="8ba45-143">If you choose the **Yes** button, the bin is deleted for use in the future, but the bin code in all warehouse entries remains the same.</span><span class="sxs-lookup"><span data-stu-id="8ba45-143">If you choose the **Yes** button, the bin is deleted for use in the future, but the bin code in all warehouse entries remains the same.</span></span>  

<span data-ttu-id="8ba45-144">If you want to rename a bin so that all records associated with the bin are also renamed, including bin contents, warehouse activity lines, registered warehouse activity lines, warehouse worksheet lines, warehouse receipt lines, posted warehouse receipt lines, warehouse shipment lines, posted warehouse shipment lines, and warehouse entries, you can do so on the **Bins** page.</span><span class="sxs-lookup"><span data-stu-id="8ba45-144">If you want to rename a bin so that all records associated with the bin are also renamed, including bin contents, warehouse activity lines, registered warehouse activity lines, warehouse worksheet lines, warehouse receipt lines, posted warehouse receipt lines, warehouse shipment lines, posted warehouse shipment lines, and warehouse entries, you can do so on the **Bins** page.</span></span>  

## <a name="to-rename-a-bin-and-change-the-bin-code-in-all-records"></a><span data-ttu-id="8ba45-145">To rename a bin and change the bin code in all records</span><span class="sxs-lookup"><span data-stu-id="8ba45-145">To rename a bin and change the bin code in all records</span></span>  

1.  <span data-ttu-id="8ba45-146">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8ba45-146">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8ba45-147">Select the location where you want to rename a bin or change the bin code, and then choose the **Bins** action.</span><span class="sxs-lookup"><span data-stu-id="8ba45-147">Select the location where you want to rename a bin or change the bin code, and then choose the **Bins** action.</span></span>  
3.  <span data-ttu-id="8ba45-148">Select the bin that you want to change and enter a new bin code in the **Code** field.</span><span class="sxs-lookup"><span data-stu-id="8ba45-148">Select the bin that you want to change and enter a new bin code in the **Code** field.</span></span>  
4.  <span data-ttu-id="8ba45-149">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="8ba45-149">Choose the **Yes** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8ba45-150">If you choose **Yes** and there are many entries concerning this bin, for example, because you have not deleted warehouse documents for some time, it may take some time to rename all the records.</span><span class="sxs-lookup"><span data-stu-id="8ba45-150">If you choose **Yes** and there are many entries concerning this bin, for example, because you have not deleted warehouse documents for some time, it may take some time to rename all the records.</span></span> <span data-ttu-id="8ba45-151">Therefore, if you use this method, consider running the batch job **Delete Registered Whse. Documents** before you start the renaming process.</span><span class="sxs-lookup"><span data-stu-id="8ba45-151">Therefore, if you use this method, consider running the batch job **Delete Registered Whse. Documents** before you start the renaming process.</span></span> <span data-ttu-id="8ba45-152">Also note that the only documents that are deleted in this batch job are put-aways, picks, and movements.</span><span class="sxs-lookup"><span data-stu-id="8ba45-152">Also note that the only documents that are deleted in this batch job are put-aways, picks, and movements.</span></span>  
>   
>  <span data-ttu-id="8ba45-153">If you are renaming a receiving bin or a shipping bin, all the posted receipts or shipments that refer to the bin in question are renamed.</span><span class="sxs-lookup"><span data-stu-id="8ba45-153">If you are renaming a receiving bin or a shipping bin, all the posted receipts or shipments that refer to the bin in question are renamed.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8ba45-154">See Also</span><span class="sxs-lookup"><span data-stu-id="8ba45-154">See Also</span></span>  
[<span data-ttu-id="8ba45-155">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="8ba45-155">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="8ba45-156">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="8ba45-156">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="8ba45-157">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="8ba45-157">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="8ba45-158">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="8ba45-158">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="8ba45-159">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="8ba45-159">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="8ba45-160">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8ba45-160">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
