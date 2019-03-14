---
title: How to Create Put-aways from Internal Put-aways | Microsoft Docs
description: After items have been put away and before they are picked to fulfill the needs of a production order or shipment, they are stored in the warehouse as part of available inventory.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 5cafcc32874187ae787279c20256c11cadaff6a1
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="pick-and-put-away-without-a-source-document"></a><span data-ttu-id="a5c03-103">Pick and Put Away Without a Source Document</span><span class="sxs-lookup"><span data-stu-id="a5c03-103">Pick and Put Away Without a Source Document</span></span>
<span data-ttu-id="a5c03-104">After items have been put away and before they are picked to fulfill the needs of a production order or shipment, they are stored in the warehouse as part of available inventory.</span><span class="sxs-lookup"><span data-stu-id="a5c03-104">After items have been put away and before they are picked to fulfill the needs of a production order or shipment, they are stored in the warehouse as part of available inventory.</span></span>  

<span data-ttu-id="a5c03-105">Situations can arise where items must be taken out of the warehouse pick bins temporarily, perhaps to serve as demonstration models in a sales presentation.</span><span class="sxs-lookup"><span data-stu-id="a5c03-105">Situations can arise where items must be taken out of the warehouse pick bins temporarily, perhaps to serve as demonstration models in a sales presentation.</span></span> <span data-ttu-id="a5c03-106">These items are still owned by the company and are part of inventory, but they are not available for picking.</span><span class="sxs-lookup"><span data-stu-id="a5c03-106">These items are still owned by the company and are part of inventory, but they are not available for picking.</span></span> <span data-ttu-id="a5c03-107">They are registered in a special purpose bin that you create for this purpose; technically, the items are in the warehouse, but physically, they could be in a conference or demonstration room.</span><span class="sxs-lookup"><span data-stu-id="a5c03-107">They are registered in a special purpose bin that you create for this purpose; technically, the items are in the warehouse, but physically, they could be in a conference or demonstration room.</span></span>  

<span data-ttu-id="a5c03-108">In other situations, the production unit might unexpectedly need a few parts for a process.</span><span class="sxs-lookup"><span data-stu-id="a5c03-108">In other situations, the production unit might unexpectedly need a few parts for a process.</span></span> <span data-ttu-id="a5c03-109">You can pick items for the production bins using the internal pick.</span><span class="sxs-lookup"><span data-stu-id="a5c03-109">You can pick items for the production bins using the internal pick.</span></span> <span data-ttu-id="a5c03-110">When the process is over and output is created, you post the consumption of the items and empty the production bin, which in turn decreases the quantity of the item at your location.</span><span class="sxs-lookup"><span data-stu-id="a5c03-110">When the process is over and output is created, you post the consumption of the items and empty the production bin, which in turn decreases the quantity of the item at your location.</span></span>  

<span data-ttu-id="a5c03-111">Likewise, items can be returned to the warehouse to be put away.</span><span class="sxs-lookup"><span data-stu-id="a5c03-111">Likewise, items can be returned to the warehouse to be put away.</span></span> <span data-ttu-id="a5c03-112">The items may have been taken out of available inventory for a production order, and then not used at all.</span><span class="sxs-lookup"><span data-stu-id="a5c03-112">The items may have been taken out of available inventory for a production order, and then not used at all.</span></span> <span data-ttu-id="a5c03-113">To make them part of available inventory again, they must be put away in the bin.</span><span class="sxs-lookup"><span data-stu-id="a5c03-113">To make them part of available inventory again, they must be put away in the bin.</span></span>  

<span data-ttu-id="a5c03-114">The **Internal Put-aways** enables you to perform put-aways without having to refer to a particular source document.</span><span class="sxs-lookup"><span data-stu-id="a5c03-114">The **Internal Put-aways** enables you to perform put-aways without having to refer to a particular source document.</span></span> <span data-ttu-id="a5c03-115">You can easily set up all the information you need to create a put-away warehouse instruction.</span><span class="sxs-lookup"><span data-stu-id="a5c03-115">You can easily set up all the information you need to create a put-away warehouse instruction.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a5c03-116">If you are not using internal picks and internal put-aways, these adjustments can be performed using the methods to move items from bin to bin or to post quantity adjustments in a bin.</span><span class="sxs-lookup"><span data-stu-id="a5c03-116">If you are not using internal picks and internal put-aways, these adjustments can be performed using the methods to move items from bin to bin or to post quantity adjustments in a bin.</span></span>  
>   
>  <span data-ttu-id="a5c03-117">When the location uses directed put-away and pick, and therefore uses bin types, you cannot manually move items in or out of a bin of bin type RECEIVE, because items that are in a RECEIVE-type bin must be registered as being put away before they are part of available inventory.</span><span class="sxs-lookup"><span data-stu-id="a5c03-117">When the location uses directed put-away and pick, and therefore uses bin types, you cannot manually move items in or out of a bin of bin type RECEIVE, because items that are in a RECEIVE-type bin must be registered as being put away before they are part of available inventory.</span></span>  

## <a name="to-create-an-internal-pick"></a><span data-ttu-id="a5c03-118">To create an internal pick</span><span class="sxs-lookup"><span data-stu-id="a5c03-118">To create an internal pick</span></span>  
1.  <span data-ttu-id="a5c03-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Pick**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a5c03-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Pick**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a5c03-120">Fill in the **No.**</span><span class="sxs-lookup"><span data-stu-id="a5c03-120">Fill in the **No.**</span></span> <span data-ttu-id="a5c03-121">field and the **To Bin Code** field on the **General** FastTab.</span><span class="sxs-lookup"><span data-stu-id="a5c03-121">field and the **To Bin Code** field on the **General** FastTab.</span></span> <span data-ttu-id="a5c03-122">The **To Bin Code** field specifies the bin from which you want to get the items.</span><span class="sxs-lookup"><span data-stu-id="a5c03-122">The **To Bin Code** field specifies the bin from which you want to get the items.</span></span> <span data-ttu-id="a5c03-123">For production purposes, this bin would be the inbound production bin or the open shop bin.</span><span class="sxs-lookup"><span data-stu-id="a5c03-123">For production purposes, this bin would be the inbound production bin or the open shop bin.</span></span> <span data-ttu-id="a5c03-124">For other purposes, choose a To Bin Code of a bin type that is not used for picking, most likely a staging, shipping or special purpose bin.</span><span class="sxs-lookup"><span data-stu-id="a5c03-124">For other purposes, choose a To Bin Code of a bin type that is not used for picking, most likely a staging, shipping or special purpose bin.</span></span>  
3.  <span data-ttu-id="a5c03-125">Select an item in the **Item No.** field, and fill in the quantities you want to pick.</span><span class="sxs-lookup"><span data-stu-id="a5c03-125">Select an item in the **Item No.** field, and fill in the quantities you want to pick.</span></span>  
4. <span data-ttu-id="a5c03-126">Choose the **Create Pick** action.</span><span class="sxs-lookup"><span data-stu-id="a5c03-126">Choose the **Create Pick** action.</span></span> <span data-ttu-id="a5c03-127">A warehouse pick instruction is now ready for a warehouse employee to perform.</span><span class="sxs-lookup"><span data-stu-id="a5c03-127">A warehouse pick instruction is now ready for a warehouse employee to perform.</span></span>  

## <a name="to-create-an-internal-put-away"></a><span data-ttu-id="a5c03-128">To create an internal put-away</span><span class="sxs-lookup"><span data-stu-id="a5c03-128">To create an internal put-away</span></span>  
1.  <span data-ttu-id="a5c03-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Put-away**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a5c03-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Put-away**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a5c03-130">Fill in the **No.**</span><span class="sxs-lookup"><span data-stu-id="a5c03-130">Fill in the **No.**</span></span> <span data-ttu-id="a5c03-131">and **From Bin Code** fields on the **General** FastTab.</span><span class="sxs-lookup"><span data-stu-id="a5c03-131">and **From Bin Code** fields on the **General** FastTab.</span></span> <span data-ttu-id="a5c03-132">The **From Bin Code** field specifies the bin where the items being returned to the warehouse, perhaps from production, are located.</span><span class="sxs-lookup"><span data-stu-id="a5c03-132">The **From Bin Code** field specifies the bin where the items being returned to the warehouse, perhaps from production, are located.</span></span>  
3.  <span data-ttu-id="a5c03-133">Fill in the item numbers and quantities on the lines.</span><span class="sxs-lookup"><span data-stu-id="a5c03-133">Fill in the item numbers and quantities on the lines.</span></span>  
4.  <span data-ttu-id="a5c03-134">Choose the **Create Put-away** action.</span><span class="sxs-lookup"><span data-stu-id="a5c03-134">Choose the **Create Put-away** action.</span></span> <span data-ttu-id="a5c03-135">A warehouse put-away instruction is now ready for a warehouse employee to perform.</span><span class="sxs-lookup"><span data-stu-id="a5c03-135">A warehouse put-away instruction is now ready for a warehouse employee to perform.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a5c03-136">See Also</span><span class="sxs-lookup"><span data-stu-id="a5c03-136">See Also</span></span>  
[<span data-ttu-id="a5c03-137">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="a5c03-137">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="a5c03-138">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="a5c03-138">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="a5c03-139">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="a5c03-139">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="a5c03-140">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="a5c03-140">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="a5c03-141">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="a5c03-141">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="a5c03-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a5c03-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
