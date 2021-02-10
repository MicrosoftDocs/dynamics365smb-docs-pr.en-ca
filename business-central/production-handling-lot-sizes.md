---
title: Handling Lot Sizes | Microsoft Docs
description: This topic describes different ways to handle lot sizes.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 6f07828e969d5a8394657bc1e05d44156ada5411
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749027"
---
# <a name="handling-lot-sizes-in-production"></a><span data-ttu-id="f75e2-103">Handling Lot Sizes in Production</span><span class="sxs-lookup"><span data-stu-id="f75e2-103">Handling Lot Sizes in Production</span></span>
<span data-ttu-id="f75e2-104">In terms of quantity, the number of items you produce in a production operation might not correlate to how sell them.</span><span class="sxs-lookup"><span data-stu-id="f75e2-104">In terms of quantity, the number of items you produce in a production operation might not correlate to how sell them.</span></span> <span data-ttu-id="f75e2-105">For example, you might produce hundreds of items in a single lot, but sell each item individually.</span><span class="sxs-lookup"><span data-stu-id="f75e2-105">For example, you might produce hundreds of items in a single lot, but sell each item individually.</span></span> <span data-ttu-id="f75e2-106">When you configure your production routes and bills of materials (BOMs), there are few nuances you should consider with regards to lot sizes.</span><span class="sxs-lookup"><span data-stu-id="f75e2-106">When you configure your production routes and bills of materials (BOMs), there are few nuances you should consider with regards to lot sizes.</span></span> <span data-ttu-id="f75e2-107">This topic describes how lot sizes impact cost calculations and resource planning.</span><span class="sxs-lookup"><span data-stu-id="f75e2-107">This topic describes how lot sizes impact cost calculations and resource planning.</span></span>

## <a name="units-of-measure-in-production-bill-of-materials"></a><span data-ttu-id="f75e2-108">Units of Measure in Production Bill of Materials</span><span class="sxs-lookup"><span data-stu-id="f75e2-108">Units of Measure in Production Bill of Materials</span></span>
<span data-ttu-id="f75e2-109">Although you specify the base unit of measure (UOM) for an item, your BOM might use a different UOM for the finished product.</span><span class="sxs-lookup"><span data-stu-id="f75e2-109">Although you specify the base unit of measure (UOM) for an item, your BOM might use a different UOM for the finished product.</span></span> <span data-ttu-id="f75e2-110">For example, the base UOM for an item might be PCS, but your BOM might call for pallet or tonne.</span><span class="sxs-lookup"><span data-stu-id="f75e2-110">For example, the base UOM for an item might be PCS, but your BOM might call for pallet or ton.</span></span> <span data-ttu-id="f75e2-111">This comes in handy when your machines or raw components dictate the volume.</span><span class="sxs-lookup"><span data-stu-id="f75e2-111">This comes in handy when your machines or raw components dictate the volume.</span></span> <span data-ttu-id="f75e2-112">For example, you probably wouldn't want to bake a single muffin because it is difficult to use a portion of an egg.</span><span class="sxs-lookup"><span data-stu-id="f75e2-112">For example, you probably wouldn't want to bake a single muffin because it is difficult to use a portion of an egg.</span></span> <span data-ttu-id="f75e2-113">Instead, you bake a batch of muffins to reduce waste.</span><span class="sxs-lookup"><span data-stu-id="f75e2-113">Instead, you bake a batch of muffins to reduce waste.</span></span> <span data-ttu-id="f75e2-114">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="f75e2-114">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span></span>

## <a name="lot-size-on-routing-lines"></a><span data-ttu-id="f75e2-115">Lot size on routing lines</span><span class="sxs-lookup"><span data-stu-id="f75e2-115">Lot size on routing lines</span></span>
<span data-ttu-id="f75e2-116">From a routing perspective, you can specify a lot size on routing lines to align with the capacity of the machines that produce the items.</span><span class="sxs-lookup"><span data-stu-id="f75e2-116">From a routing perspective, you can specify a lot size on routing lines to align with the capacity of the machines that produce the items.</span></span> <span data-ttu-id="f75e2-117">The run time on routing lines is reduced proportionally to the lot size.</span><span class="sxs-lookup"><span data-stu-id="f75e2-117">The run time on routing lines is reduced proportionally to the lot size.</span></span> 

<span data-ttu-id="f75e2-118">This works well when the quantity on a production order is a factor of the lot size on the route.</span><span class="sxs-lookup"><span data-stu-id="f75e2-118">This works well when the quantity on a production order is a factor of the lot size on the route.</span></span> <span data-ttu-id="f75e2-119">For example, if your baking sheet can hold 10 muffins, you should bake 10, 20, 30, and so on, and not 5 nor 15.</span><span class="sxs-lookup"><span data-stu-id="f75e2-119">For example, if your baking sheet can hold 10 muffins, you should bake 10, 20, 30, and so on, and not 5 nor 15.</span></span>  <span data-ttu-id="f75e2-120">This is much less of an issue if you are dealing with large quantities.</span><span class="sxs-lookup"><span data-stu-id="f75e2-120">This is much less of an issue if you are dealing with large quantities.</span></span>

<span data-ttu-id="f75e2-121">Lot size is also popular in manufacturing environments where output is measured as quantity you can make during fixed amount of time.</span><span class="sxs-lookup"><span data-stu-id="f75e2-121">Lot size is also popular in manufacturing environments where output is measured as quantity you can make during fixed amount of time.</span></span> <span data-ttu-id="f75e2-122">Example, if Volume per 9 hour shift is 25000 cubic feet, you can set run time as 9 hours and lot size as 25000.</span><span class="sxs-lookup"><span data-stu-id="f75e2-122">Example, if Volume per 9 hour shift is 25000 cubic feet, you can set run time as 9 hours and lot size as 25000.</span></span>
<span data-ttu-id="f75e2-123">The production order quantity becomes less important as on the production order the run time gets calculated as the Run time / Lot size to get the run time per piece.</span><span class="sxs-lookup"><span data-stu-id="f75e2-123">The production order quantity becomes less important as on the production order the run time gets calculated as the Run time / Lot size to get the run time per piece.</span></span>
 
> [!NOTE]
> <span data-ttu-id="f75e2-124">The value defined in Lot size doesn't have impact on time specified in **Setup Time** field of the routing line.</span><span class="sxs-lookup"><span data-stu-id="f75e2-124">The value defined in Lot size doesn't have impact on time specified in **Setup Time** field of the routing line.</span></span> <span data-ttu-id="f75e2-125">The setup will happen only one time, even if there are several lots.</span><span class="sxs-lookup"><span data-stu-id="f75e2-125">The setup will happen only one time, even if there are several lots.</span></span> <span data-ttu-id="f75e2-126">For example, so that you don’t need to warm the oven for the second lot of muffins.</span><span class="sxs-lookup"><span data-stu-id="f75e2-126">For example, so that you don’t need to warm the oven for the second lot of muffins.</span></span> <span data-ttu-id="f75e2-127">For more information, see [Create Routings](production-how-to-create-routings.md).</span><span class="sxs-lookup"><span data-stu-id="f75e2-127">For more information, see [Create Routings](production-how-to-create-routings.md).</span></span>

## <a name="lot-sizes-for-items-and-stockkeeping-units"></a><span data-ttu-id="f75e2-128">Lot Sizes for Items and Stockkeeping Units</span><span class="sxs-lookup"><span data-stu-id="f75e2-128">Lot Sizes for Items and Stockkeeping Units</span></span>
<span data-ttu-id="f75e2-129">Lot sizes defined for routings are not the same as lot sizes for items or stockkeeping units.</span><span class="sxs-lookup"><span data-stu-id="f75e2-129">Lot sizes defined for routings are not the same as lot sizes for items or stockkeeping units.</span></span> <span data-ttu-id="f75e2-130">Those values are used for a different purpose, and do not affect production capacity.</span><span class="sxs-lookup"><span data-stu-id="f75e2-130">Those values are used for a different purpose, and do not affect production capacity.</span></span> 

## <a name="lot-size-on-item-and-stockkeeping-units"></a><span data-ttu-id="f75e2-131">Lot size on item and stockkeeping units</span><span class="sxs-lookup"><span data-stu-id="f75e2-131">Lot size on item and stockkeeping units</span></span>
<span data-ttu-id="f75e2-132">For items and stockkeeping units, lot sizes have the following effects on cost calculation and supply planning:</span><span class="sxs-lookup"><span data-stu-id="f75e2-132">For items and stockkeeping units, lot sizes have the following effects on cost calculation and supply planning:</span></span>

* <span data-ttu-id="f75e2-133">For standard cost calculation, if you enable **Cost Incl Setup** on the **Manufacturing Setup** page, the cost for the setup is added to the standard cost.</span><span class="sxs-lookup"><span data-stu-id="f75e2-133">For standard cost calculation, if you enable **Cost Incl Setup** on the **Manufacturing Setup** page, the cost for the setup is added to the standard cost.</span></span> <span data-ttu-id="f75e2-134">If you specify a lot size, the setup cost for routing operation will be reduced according to one lot size.</span><span class="sxs-lookup"><span data-stu-id="f75e2-134">If you specify a lot size, the setup cost for routing operation will be reduced according to one lot size.</span></span> <span data-ttu-id="f75e2-135">For example, if your lot size defined on item card is 10, and it takes 15 minutes to heat the oven, the cost of the fuel will be allocated to the 10 muffins as roughly 1.5 minutes.</span><span class="sxs-lookup"><span data-stu-id="f75e2-135">For example, if your lot size defined on item card is 10, and it takes 15 minutes to heat the oven, the cost of the fuel will be allocated to the 10 muffins as roughly 1.5 minutes.</span></span> 

> [!NOTE]
> <span data-ttu-id="f75e2-136">Setup costs are handled differently from a standard cost and capacity allocation perspectives.</span><span class="sxs-lookup"><span data-stu-id="f75e2-136">Setup costs are handled differently from a standard cost and capacity allocation perspectives.</span></span> <span data-ttu-id="f75e2-137">If produced quantity doesn't match lot size defined in the item card that will lead to variation.</span><span class="sxs-lookup"><span data-stu-id="f75e2-137">If produced quantity doesn't match lot size defined in the item card that will lead to variation.</span></span> <span data-ttu-id="f75e2-138">For more information, see [Managing Inventory Costs](finance-manage-inventory-costs.md).</span><span class="sxs-lookup"><span data-stu-id="f75e2-138">For more information, see [Managing Inventory Costs](finance-manage-inventory-costs.md).</span></span> <!--not sure that I got this part right seems to repeat the first example.-->

<span data-ttu-id="f75e2-139">For supply planning, the lot size setting on items works with the **Default Dampener %** on the **Manufacturing Setup** page.</span><span class="sxs-lookup"><span data-stu-id="f75e2-139">For supply planning, the lot size setting on items works with the **Default Dampener %** on the **Manufacturing Setup** page.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="f75e2-140">will ignore changes in demand that are below the dampener percentage and will not create planning suggestions.</span><span class="sxs-lookup"><span data-stu-id="f75e2-140">will ignore changes in demand that are below the dampener percentage and will not create planning suggestions.</span></span> <span data-ttu-id="f75e2-141">For example, 15 is specified in the Default Dampener % field, and we have a production order for 20 muffins to feed 20 guests, but one guest cannot attend.</span><span class="sxs-lookup"><span data-stu-id="f75e2-141">For example, 15 is specified in the Default Dampener % field, and we have a production order for 20 muffins to feed 20 guests, but one guest cannot attend.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="f75e2-142">will ignore the single missing guest because it's only 10% of the lot size 10 defined on the item.</span><span class="sxs-lookup"><span data-stu-id="f75e2-142">will ignore the single missing guest because it's only 10% of the lot size 10 defined on the item.</span></span> <span data-ttu-id="f75e2-143">However, if two guests cannot make it, [!INCLUDE[prod_short](includes/prod_short.md)] will suggest that we reduce the order quantity because two is 20% of the lot size.</span><span class="sxs-lookup"><span data-stu-id="f75e2-143">However, if two guests cannot make it, [!INCLUDE[prod_short](includes/prod_short.md)] will suggest that we reduce the order quantity because two is 20% of the lot size.</span></span> <span data-ttu-id="f75e2-144">For more information about planning, see [Planning](production-planning.md).</span><span class="sxs-lookup"><span data-stu-id="f75e2-144">For more information about planning, see [Planning](production-planning.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="f75e2-145">See Also</span><span class="sxs-lookup"><span data-stu-id="f75e2-145">See Also</span></span>
[<span data-ttu-id="f75e2-146">Create Production BOMs</span><span class="sxs-lookup"><span data-stu-id="f75e2-146">Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
<span data-ttu-id="f75e2-147">[Work with Manufacturing Batch Units of Measure](production-how-to-use-the-manufacturing-batch-unit-of-measure.md)
[Create Routings](production-how-to-create-routings.md)</span><span class="sxs-lookup"><span data-stu-id="f75e2-147">[Work with Manufacturing Batch Units of Measure](production-how-to-use-the-manufacturing-batch-unit-of-measure.md)
[Create Routings](production-how-to-create-routings.md)</span></span>  
[<span data-ttu-id="f75e2-148">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="f75e2-148">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)