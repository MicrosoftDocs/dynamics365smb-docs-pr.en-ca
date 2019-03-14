---
title: How to Assign Default Bins to Items | Microsoft Docs
description: If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 826e1392143b166566619c5aef8c28ac2b09bc22
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="assign-default-bins-to-items"></a><span data-ttu-id="ffa17-104">Assign Default Bins to Items</span><span class="sxs-lookup"><span data-stu-id="ffa17-104">Assign Default Bins to Items</span></span>
<span data-ttu-id="ffa17-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span><span class="sxs-lookup"><span data-stu-id="ffa17-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="ffa17-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span><span class="sxs-lookup"><span data-stu-id="ffa17-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="ffa17-107">Default bins are defined in the **Bin Content** window.</span><span class="sxs-lookup"><span data-stu-id="ffa17-107">Default bins are defined in the **Bin Content** window.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="ffa17-108">To assign a default bin to an item</span><span class="sxs-lookup"><span data-stu-id="ffa17-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="ffa17-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ffa17-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="ffa17-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span><span class="sxs-lookup"><span data-stu-id="ffa17-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="ffa17-111">Make sure to select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="ffa17-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="ffa17-112">Choose the **Create Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="ffa17-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="ffa17-113">Default bins are now assigned for your item.</span><span class="sxs-lookup"><span data-stu-id="ffa17-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ffa17-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span><span class="sxs-lookup"><span data-stu-id="ffa17-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="ffa17-115">To change the default bin for an item</span><span class="sxs-lookup"><span data-stu-id="ffa17-115">To change the default bin for an item</span></span>  
<span data-ttu-id="ffa17-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span><span class="sxs-lookup"><span data-stu-id="ffa17-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="ffa17-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Contents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ffa17-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ffa17-118">In the **Location Filter** field, select the appropriate location code.</span><span class="sxs-lookup"><span data-stu-id="ffa17-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="ffa17-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="ffa17-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="ffa17-120">Find the bin content line for the bin that you would like as the new default bin.</span><span class="sxs-lookup"><span data-stu-id="ffa17-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="ffa17-121">Select the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="ffa17-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ffa17-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span><span class="sxs-lookup"><span data-stu-id="ffa17-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ffa17-123">See Also</span><span class="sxs-lookup"><span data-stu-id="ffa17-123">See Also</span></span>  
[<span data-ttu-id="ffa17-124">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="ffa17-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="ffa17-125">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="ffa17-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="ffa17-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="ffa17-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="ffa17-127">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="ffa17-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="ffa17-128">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="ffa17-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="ffa17-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ffa17-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
