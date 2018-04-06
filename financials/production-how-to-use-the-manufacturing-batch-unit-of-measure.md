---
title: How to Use the Manufacturing Batch Unit of Measure | Microsoft Docs
description: If an item is stocked in one unit of measure but produced in another, then the production order must be use a manufacturing batch unit of measure to calculate the correct quantity of components. An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 7dafbb96b4ce4f5ad525ab299edd8549c7aa600e
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-manufacturing-batch-units-of-measure"></a><span data-ttu-id="d5b36-104">Work with Manufacturing Batch Units of Measure</span><span class="sxs-lookup"><span data-stu-id="d5b36-104">Work with Manufacturing Batch Units of Measure</span></span>
<span data-ttu-id="d5b36-105">If an item is stocked in one unit of measure but produced in another, a production order is created that uses a manufacturing batch unit of measure to calculate the correct quantity of the components during the **Refresh Production Order** batch job.</span><span class="sxs-lookup"><span data-stu-id="d5b36-105">If an item is stocked in one unit of measure but produced in another, a production order is created that uses a manufacturing batch unit of measure to calculate the correct quantity of the components during the **Refresh Production Order** batch job.</span></span> <span data-ttu-id="d5b36-106">An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.</span><span class="sxs-lookup"><span data-stu-id="d5b36-106">An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.</span></span>  

## <a name="to-create-a-production-bom-using-a-batch-unit-of-measure"></a><span data-ttu-id="d5b36-107">To create a production BOM using a batch unit of measure</span><span class="sxs-lookup"><span data-stu-id="d5b36-107">To create a production BOM using a batch unit of measure</span></span>  
1.  <span data-ttu-id="d5b36-108">The manufacturing batch unit of measure is set up as an alternative unit of measure in the **Item Units of Measure** window on the item to be produced.</span><span class="sxs-lookup"><span data-stu-id="d5b36-108">The manufacturing batch unit of measure is set up as an alternative unit of measure in the **Item Units of Measure** window on the item to be produced.</span></span> <span data-ttu-id="d5b36-109">The batch unit of measure will not replace the base unit of measure on the item.</span><span class="sxs-lookup"><span data-stu-id="d5b36-109">The batch unit of measure will not replace the base unit of measure on the item.</span></span>  
2.  <span data-ttu-id="d5b36-110">Create a production BOM for the item set up with the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-110">Create a production BOM for the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="d5b36-111">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="d5b36-111">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span></span>  
3.  <span data-ttu-id="d5b36-112">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-112">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure.</span></span>  
4.  <span data-ttu-id="d5b36-113">For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-113">For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measure.</span></span>  
5.  <span data-ttu-id="d5b36-114">Open the **Item Card** for the related item.</span><span class="sxs-lookup"><span data-stu-id="d5b36-114">Open the **Item Card** for the related item.</span></span>  

    <span data-ttu-id="d5b36-115">On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.</span><span class="sxs-lookup"><span data-stu-id="d5b36-115">On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.</span></span>  
6.  <span data-ttu-id="d5b36-116">Create a production order header using the item set up with the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-116">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="d5b36-117">For more information, see [Create Production Orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="d5b36-117">For more information, see [Create Production Orders](production-how-to-create-production-orders.md).</span></span>  
7.  <span data-ttu-id="d5b36-118">Choose the **Refresh** action, and then choose  the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d5b36-118">Choose the **Refresh** action, and then choose  the **OK** button.</span></span>  

<span data-ttu-id="d5b36-119">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span><span class="sxs-lookup"><span data-stu-id="d5b36-119">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="d5b36-120">The program calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-120">The program calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measure.</span></span>  

## <a name="to-calculate-a-manufacturing-batch-unit-of-measure-on-a-production-order"></a><span data-ttu-id="d5b36-121">To calculate a manufacturing batch unit of measure on a production order</span><span class="sxs-lookup"><span data-stu-id="d5b36-121">To calculate a manufacturing batch unit of measure on a production order</span></span>  
1.  <span data-ttu-id="d5b36-122">Create a production order header using the item set up with the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-122">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span>  
2.  <span data-ttu-id="d5b36-123">In the **Item No.** field in the Production Order line, type the same item number used in the header.</span><span class="sxs-lookup"><span data-stu-id="d5b36-123">In the **Item No.** field in the Production Order line, type the same item number used in the header.</span></span>  
3.  <span data-ttu-id="d5b36-124">In the **Quantity** field, enter the same quantity used in the header.</span><span class="sxs-lookup"><span data-stu-id="d5b36-124">In the **Quantity** field, enter the same quantity used in the header.</span></span>  
4.  <span data-ttu-id="d5b36-125">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure code.</span><span class="sxs-lookup"><span data-stu-id="d5b36-125">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure code.</span></span>  
5.  <span data-ttu-id="d5b36-126">Choose the **Refresh** action.</span><span class="sxs-lookup"><span data-stu-id="d5b36-126">Choose the **Refresh** action.</span></span>
6.  <span data-ttu-id="d5b36-127">On the **Calculate** FastTab, clear the **Lines** check box.</span><span class="sxs-lookup"><span data-stu-id="d5b36-127">On the **Calculate** FastTab, clear the **Lines** check box.</span></span>  
7.  <span data-ttu-id="d5b36-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d5b36-128">Choose the **OK** button.</span></span>  
8.  <span data-ttu-id="d5b36-129">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span><span class="sxs-lookup"><span data-stu-id="d5b36-129">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="d5b36-130">The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="d5b36-130">The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measure.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d5b36-131">See Also</span><span class="sxs-lookup"><span data-stu-id="d5b36-131">See Also</span></span>  
[<span data-ttu-id="d5b36-132">Create Routings</span><span class="sxs-lookup"><span data-stu-id="d5b36-132">Create Routings</span></span>](production-how-to-create-routings.md)  
<span data-ttu-id="d5b36-133">[Create Production BOMs](production-how-to-create-production-boms.md)   </span><span class="sxs-lookup"><span data-stu-id="d5b36-133">[Create Production BOMs](production-how-to-create-production-boms.md)   </span></span>  
[<span data-ttu-id="d5b36-134">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="d5b36-134">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="d5b36-135">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="d5b36-135">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="d5b36-136">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="d5b36-136">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="d5b36-137">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="d5b36-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="d5b36-138">Purchasing</span><span class="sxs-lookup"><span data-stu-id="d5b36-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="d5b36-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d5b36-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

