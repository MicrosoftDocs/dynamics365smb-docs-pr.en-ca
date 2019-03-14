---
title: How to Move Items in advanced warehouse configurations | Microsoft Docs
description: In advanced warehouse configurations, that is, locations with directed put-away and pick, warehouse movements between bins are performed by a senior employee preparing warehouse movements in the movement worksheet and then creating the warehouse movements for warehouse employees to perform.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/232017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 4caa041c6b3acef5d0cbf6c037f0ec535cd3176e
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="move-items-in-advanced-warehouse-configurations"></a><span data-ttu-id="960a2-103">Move Items in Advanced Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="960a2-103">Move Items in Advanced Warehouse Configurations</span></span>
<span data-ttu-id="960a2-104">In advanced warehouse configurations, that is, locations with directed put-away and pick, warehouse movements between bins are performed by a senior employee preparing warehouse movements in the movement worksheet and then creating the warehouse movements for warehouse employees to perform.</span><span class="sxs-lookup"><span data-stu-id="960a2-104">In advanced warehouse configurations, that is, locations with directed put-away and pick, warehouse movements between bins are performed by a senior employee preparing warehouse movements in the movement worksheet and then creating the warehouse movements for warehouse employees to perform.</span></span>  

## <a name="to-move-items-with-the-warehouse-movement-worksheet"></a><span data-ttu-id="960a2-105">To move items with the warehouse movement worksheet</span><span class="sxs-lookup"><span data-stu-id="960a2-105">To move items with the warehouse movement worksheet</span></span>
<span data-ttu-id="960a2-106">The **Movement Worksheet** window has two functions that can assist in automatically filling in the lines.</span><span class="sxs-lookup"><span data-stu-id="960a2-106">The **Movement Worksheet** window has two functions that can assist in automatically filling in the lines.</span></span> <span data-ttu-id="960a2-107">The first is the **Calculate Bin Replenishment** function.</span><span class="sxs-lookup"><span data-stu-id="960a2-107">The first is the **Calculate Bin Replenishment** function.</span></span> <span data-ttu-id="960a2-108">This function uses the bin rankings to suggest replenishment for high-ranking bins from low-ranking bins. The second is the **Get Bin Content** function, which fills in the worksheet lines with the entire bin contents of the bin or bins you specify.</span><span class="sxs-lookup"><span data-stu-id="960a2-108">This function uses the bin rankings to suggest replenishment for high-ranking bins from low-ranking bins. The second is the **Get Bin Content** function, which fills in the worksheet lines with the entire bin contents of the bin or bins you specify.</span></span>

1.  <span data-ttu-id="960a2-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="960a2-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="960a2-110">Enter the warehouse movement information on the worksheet lines as appropriate.</span><span class="sxs-lookup"><span data-stu-id="960a2-110">Enter the warehouse movement information on the worksheet lines as appropriate.</span></span>  
3. <span data-ttu-id="960a2-111">Choose the **Create Movement** action to create a warehouse movement document which can then be registered when the warehouse movement is completed.</span><span class="sxs-lookup"><span data-stu-id="960a2-111">Choose the **Create Movement** action to create a warehouse movement document which can then be registered when the warehouse movement is completed.</span></span>  

### <a name="to-register-the-warehouse-movement"></a><span data-ttu-id="960a2-112">To register the warehouse movement</span><span class="sxs-lookup"><span data-stu-id="960a2-112">To register the warehouse movement</span></span>  
1.  <span data-ttu-id="960a2-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movements**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="960a2-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movements**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="960a2-114">Open the warehouse movement that you want to process.</span><span class="sxs-lookup"><span data-stu-id="960a2-114">Open the warehouse movement that you want to process.</span></span>  
3.  <span data-ttu-id="960a2-115">On lines of action type **Place**, specify where, which, and when to move the item in question by editing the **Zone Code**, **Bin Code**, **Qty. to Handle**, or **Due Date** fields.</span><span class="sxs-lookup"><span data-stu-id="960a2-115">On lines of action type **Place**, specify where, which, and when to move the item in question by editing the **Zone Code**, **Bin Code**, **Qty. to Handle**, or **Due Date** fields.</span></span>  

    <span data-ttu-id="960a2-116">If your warehouse has been set up so the bin codes follow the physical structure of the warehouse, you can take quantities of several items from successive bulk bins and then place them in forward picking bins, which also might be close to one another.</span><span class="sxs-lookup"><span data-stu-id="960a2-116">If your warehouse has been set up so the bin codes follow the physical structure of the warehouse, you can take quantities of several items from successive bulk bins and then place them in forward picking bins, which also might be close to one another.</span></span>  
4.  <span data-ttu-id="960a2-117">On lines of action type **Take**, specify in the **Qty. to Handle** field a part quantity of the bin content that you want to move.</span><span class="sxs-lookup"><span data-stu-id="960a2-117">On lines of action type **Take**, specify in the **Qty. to Handle** field a part quantity of the bin content that you want to move.</span></span> <span data-ttu-id="960a2-118">All other fields on lines of action type **Take** are read-only.</span><span class="sxs-lookup"><span data-stu-id="960a2-118">All other fields on lines of action type **Take** are read-only.</span></span>  
5.  <span data-ttu-id="960a2-119">To move all suggested quantities as specified in the **Quantity** field, choose the **Autofill Qty. to Handle** action.</span><span class="sxs-lookup"><span data-stu-id="960a2-119">To move all suggested quantities as specified in the **Quantity** field, choose the **Autofill Qty. to Handle** action.</span></span>  
6. <span data-ttu-id="960a2-120">Choose the **Register** action.</span><span class="sxs-lookup"><span data-stu-id="960a2-120">Choose the **Register** action.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="960a2-121">If the location uses directed put-away and pick, then you cannot manually move items in or out of bins of bin type RECEIVE, because items in such bins must be registered as being put away before they are part of available inventory.</span><span class="sxs-lookup"><span data-stu-id="960a2-121">If the location uses directed put-away and pick, then you cannot manually move items in or out of bins of bin type RECEIVE, because items in such bins must be registered as being put away before they are part of available inventory.</span></span>

## <a name="to-register-the-movement-of-an-item-that-has-already-occurred"></a><span data-ttu-id="960a2-122">To register the movement of an item that has already occurred</span><span class="sxs-lookup"><span data-stu-id="960a2-122">To register the movement of an item that has already occurred</span></span>  
<span data-ttu-id="960a2-123">If your location uses directed put-away and pick, and you need to move items to other bins without a pre-existing warehouse put-away, pick, or movement, you can register the correct placement of the items in the warehouse using the **Whse. Reclassification Journal**.</span><span class="sxs-lookup"><span data-stu-id="960a2-123">If your location uses directed put-away and pick, and you need to move items to other bins without a pre-existing warehouse put-away, pick, or movement, you can register the correct placement of the items in the warehouse using the **Whse. Reclassification Journal**.</span></span>

1.  <span data-ttu-id="960a2-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Reclassification Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="960a2-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Reclassification Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="960a2-125">Fill in the **Item No.**, **From Zone Code**, **From Bin Code**, **To Zone Code**, and **To Bin Code** fields.</span><span class="sxs-lookup"><span data-stu-id="960a2-125">Fill in the **Item No.**, **From Zone Code**, **From Bin Code**, **To Zone Code**, and **To Bin Code** fields.</span></span>  
3.  <span data-ttu-id="960a2-126">Choose the **Register** action.</span><span class="sxs-lookup"><span data-stu-id="960a2-126">Choose the **Register** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="960a2-127">See Also</span><span class="sxs-lookup"><span data-stu-id="960a2-127">See Also</span></span>  
[<span data-ttu-id="960a2-128">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="960a2-128">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="960a2-129">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="960a2-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="960a2-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="960a2-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="960a2-131">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="960a2-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="960a2-132">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="960a2-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="960a2-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="960a2-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
