---
title: Understanding Item Types| Microsoft Docs
description: You can adjust the inventory valuation of an item using the FIFO or Average costing methods, for example, when item costs change for reasons other than transactions.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/18/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 2240840e977bcd1186c74972ce0457deb03058a0
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="about-item-types"></a><span data-ttu-id="777e7-103">About Item Types</span><span class="sxs-lookup"><span data-stu-id="777e7-103">About Item Types</span></span>
<span data-ttu-id="777e7-104">In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system.</span><span class="sxs-lookup"><span data-stu-id="777e7-104">In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system.</span></span> <span data-ttu-id="777e7-105">Three options exist:</span><span class="sxs-lookup"><span data-stu-id="777e7-105">Three options exist:</span></span>

|<span data-ttu-id="777e7-106">Option</span><span class="sxs-lookup"><span data-stu-id="777e7-106">Option</span></span>|<span data-ttu-id="777e7-107">Typical Purpose</span><span class="sxs-lookup"><span data-stu-id="777e7-107">Typical Purpose</span></span>|
|------|-----------|
|<span data-ttu-id="777e7-108">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="777e7-108">Inventory</span></span>|<span data-ttu-id="777e7-109">A physical unit, such as a bicycle, for full business support.</span><span class="sxs-lookup"><span data-stu-id="777e7-109">A physical unit, such as a bicycle, for full business support.</span></span>|
|<span data-ttu-id="777e7-110">Non-Inventory</span><span class="sxs-lookup"><span data-stu-id="777e7-110">Non-Inventory</span></span>|<span data-ttu-id="777e7-111">A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.</span><span class="sxs-lookup"><span data-stu-id="777e7-111">A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.</span></span>|
|<span data-ttu-id="777e7-112">Service</span><span class="sxs-lookup"><span data-stu-id="777e7-112">Service</span></span>|<span data-ttu-id="777e7-113">A labour time unit, such as a consultancy hour, for limited business support.</span><span class="sxs-lookup"><span data-stu-id="777e7-113">A labor time unit, such as a consultancy hour, for limited business support.</span></span>|

<span data-ttu-id="777e7-114">The **Inventory** type involves full tracking of inventory quantity and value.</span><span class="sxs-lookup"><span data-stu-id="777e7-114">The **Inventory** type involves full tracking of inventory quantity and value.</span></span> <span data-ttu-id="777e7-115">Therefore, all item transaction types are supported, and items of type Inventory can be used with all item-handling features.</span><span class="sxs-lookup"><span data-stu-id="777e7-115">Therefore, all item transaction types are supported, and items of type Inventory can be used with all item-handling features.</span></span>

<span data-ttu-id="777e7-116">The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value.</span><span class="sxs-lookup"><span data-stu-id="777e7-116">The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value.</span></span> <span data-ttu-id="777e7-117">Therefore, only selected item transaction types and features are supported.</span><span class="sxs-lookup"><span data-stu-id="777e7-117">Therefore, only selected item transaction types and features are supported.</span></span>

<span data-ttu-id="777e7-118">The three item types support the following features respectively.</span><span class="sxs-lookup"><span data-stu-id="777e7-118">The three item types support the following features respectively.</span></span>

|<span data-ttu-id="777e7-119">Item Type</span><span class="sxs-lookup"><span data-stu-id="777e7-119">Item Type</span></span>|<span data-ttu-id="777e7-120">Sales</span><span class="sxs-lookup"><span data-stu-id="777e7-120">Sales</span></span>|<span data-ttu-id="777e7-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="777e7-121">Purchasing</span></span>|<span data-ttu-id="777e7-122">Job Consumption</span><span class="sxs-lookup"><span data-stu-id="777e7-122">Job Consumption</span></span>|<span data-ttu-id="777e7-123">Service Consumption</span><span class="sxs-lookup"><span data-stu-id="777e7-123">Service Consumption</span></span>|<span data-ttu-id="777e7-124">Assembly Consumption</span><span class="sxs-lookup"><span data-stu-id="777e7-124">Assembly Consumption</span></span>|<span data-ttu-id="777e7-125">Production Consumption</span><span class="sxs-lookup"><span data-stu-id="777e7-125">Production Consumption</span></span>|<span data-ttu-id="777e7-126">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="777e7-126">Assembly Output</span></span>|<span data-ttu-id="777e7-127">Production Output</span><span class="sxs-lookup"><span data-stu-id="777e7-127">Production Output</span></span>|<span data-ttu-id="777e7-128">Location Transfer</span><span class="sxs-lookup"><span data-stu-id="777e7-128">Location Transfer</span></span>|<span data-ttu-id="777e7-129">Physical Counting</span><span class="sxs-lookup"><span data-stu-id="777e7-129">Physical Counting</span></span>|<span data-ttu-id="777e7-130">Inventory Revaluation</span><span class="sxs-lookup"><span data-stu-id="777e7-130">Inventory Revaluation</span></span>|<span data-ttu-id="777e7-131">Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="777e7-131">Inventory Costing</span></span>|<span data-ttu-id="777e7-132">Item Tracking</span><span class="sxs-lookup"><span data-stu-id="777e7-132">Item Tracking</span></span>|<span data-ttu-id="777e7-133">Reservation</span><span class="sxs-lookup"><span data-stu-id="777e7-133">Reservation</span></span>|<span data-ttu-id="777e7-134">Warehousing</span><span class="sxs-lookup"><span data-stu-id="777e7-134">Warehousing</span></span>|<span data-ttu-id="777e7-135">Planning</span><span class="sxs-lookup"><span data-stu-id="777e7-135">Planning</span></span>|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|<span data-ttu-id="777e7-136">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="777e7-136">Inventory</span></span>|<span data-ttu-id="777e7-137">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-137">Yes</span></span>|<span data-ttu-id="777e7-138">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-138">Yes</span></span>|<span data-ttu-id="777e7-139">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-139">Yes</span></span>|<span data-ttu-id="777e7-140">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-140">Yes</span></span>|<span data-ttu-id="777e7-141">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-141">Yes</span></span>|<span data-ttu-id="777e7-142">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-142">Yes</span></span>|<span data-ttu-id="777e7-143">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-143">Yes</span></span>|<span data-ttu-id="777e7-144">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-144">Yes</span></span>|<span data-ttu-id="777e7-145">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-145">Yes</span></span>|<span data-ttu-id="777e7-146">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-146">Yes</span></span>|<span data-ttu-id="777e7-147">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-147">Yes</span></span>|<span data-ttu-id="777e7-148">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-148">Yes</span></span>|<span data-ttu-id="777e7-149">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-149">Yes</span></span>|<span data-ttu-id="777e7-150">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-150">Yes</span></span>|<span data-ttu-id="777e7-151">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-151">Yes</span></span>|<span data-ttu-id="777e7-152">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-152">Yes</span></span>|
|<span data-ttu-id="777e7-153">Non-Inventory</span><span class="sxs-lookup"><span data-stu-id="777e7-153">Non-Inventory</span></span>|<span data-ttu-id="777e7-154">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-154">Yes</span></span>|<span data-ttu-id="777e7-155">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-155">Yes</span></span>|<span data-ttu-id="777e7-156">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-156">Yes</span></span>|<span data-ttu-id="777e7-157">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-157">Yes</span></span>|<span data-ttu-id="777e7-158">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-158">Yes</span></span>|<span data-ttu-id="777e7-159">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-159">Yes</span></span>|<span data-ttu-id="777e7-160">No</span><span class="sxs-lookup"><span data-stu-id="777e7-160">No</span></span>|<span data-ttu-id="777e7-161">No</span><span class="sxs-lookup"><span data-stu-id="777e7-161">No</span></span>|<span data-ttu-id="777e7-162">No</span><span class="sxs-lookup"><span data-stu-id="777e7-162">No</span></span>|<span data-ttu-id="777e7-163">No</span><span class="sxs-lookup"><span data-stu-id="777e7-163">No</span></span>|<span data-ttu-id="777e7-164">No</span><span class="sxs-lookup"><span data-stu-id="777e7-164">No</span></span>|<span data-ttu-id="777e7-165">No</span><span class="sxs-lookup"><span data-stu-id="777e7-165">No</span></span>|<span data-ttu-id="777e7-166">No</span><span class="sxs-lookup"><span data-stu-id="777e7-166">No</span></span>|<span data-ttu-id="777e7-167">No</span><span class="sxs-lookup"><span data-stu-id="777e7-167">No</span></span>|<span data-ttu-id="777e7-168">No</span><span class="sxs-lookup"><span data-stu-id="777e7-168">No</span></span>|<span data-ttu-id="777e7-169">No</span><span class="sxs-lookup"><span data-stu-id="777e7-169">No</span></span>|
|<span data-ttu-id="777e7-170">Service</span><span class="sxs-lookup"><span data-stu-id="777e7-170">Service</span></span>|<span data-ttu-id="777e7-171">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-171">Yes</span></span>|<span data-ttu-id="777e7-172">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-172">Yes</span></span>|<span data-ttu-id="777e7-173">Yes</span><span class="sxs-lookup"><span data-stu-id="777e7-173">Yes</span></span>|<span data-ttu-id="777e7-174">No</span><span class="sxs-lookup"><span data-stu-id="777e7-174">No</span></span>|<span data-ttu-id="777e7-175">No</span><span class="sxs-lookup"><span data-stu-id="777e7-175">No</span></span>|<span data-ttu-id="777e7-176">No</span><span class="sxs-lookup"><span data-stu-id="777e7-176">No</span></span>|<span data-ttu-id="777e7-177">No</span><span class="sxs-lookup"><span data-stu-id="777e7-177">No</span></span>|<span data-ttu-id="777e7-178">No</span><span class="sxs-lookup"><span data-stu-id="777e7-178">No</span></span>|<span data-ttu-id="777e7-179">No</span><span class="sxs-lookup"><span data-stu-id="777e7-179">No</span></span>|<span data-ttu-id="777e7-180">No</span><span class="sxs-lookup"><span data-stu-id="777e7-180">No</span></span>|<span data-ttu-id="777e7-181">No</span><span class="sxs-lookup"><span data-stu-id="777e7-181">No</span></span>|<span data-ttu-id="777e7-182">No</span><span class="sxs-lookup"><span data-stu-id="777e7-182">No</span></span>|<span data-ttu-id="777e7-183">No</span><span class="sxs-lookup"><span data-stu-id="777e7-183">No</span></span>|<span data-ttu-id="777e7-184">No</span><span class="sxs-lookup"><span data-stu-id="777e7-184">No</span></span>|<span data-ttu-id="777e7-185">No</span><span class="sxs-lookup"><span data-stu-id="777e7-185">No</span></span>|<span data-ttu-id="777e7-186">No</span><span class="sxs-lookup"><span data-stu-id="777e7-186">No</span></span>|

> [!NOTE]
> <span data-ttu-id="777e7-187">Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalogue items.</span><span class="sxs-lookup"><span data-stu-id="777e7-187">Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalog items.</span></span> <span data-ttu-id="777e7-188">Catalogue items are not to be mistaken with regular items of type Non-Inventory.</span><span class="sxs-lookup"><span data-stu-id="777e7-188">Catalog items are not to be mistaken with regular items of type Non-Inventory.</span></span> <span data-ttu-id="777e7-189">For more information, see [Work with Catalogue Items](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="777e7-189">For more information, see [Work with Catalog Items](inventory-how-work-nonstock-items.md).</span></span>

> [!NOTE]
> <span data-ttu-id="777e7-190">Customers' items that you perform service on, such as a printer, are called service items.</span><span class="sxs-lookup"><span data-stu-id="777e7-190">Customers' items that you perform service on, such as a printer, are called service items.</span></span> <span data-ttu-id="777e7-191">Service items have nothing to do with regular or catalogue items.</span><span class="sxs-lookup"><span data-stu-id="777e7-191">Service items have nothing to do with regular or catalog items.</span></span> <span data-ttu-id="777e7-192">However, service components can be regular items.</span><span class="sxs-lookup"><span data-stu-id="777e7-192">However, service components can be regular items.</span></span> <span data-ttu-id="777e7-193">For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).</span><span class="sxs-lookup"><span data-stu-id="777e7-193">For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="777e7-194">See Also</span><span class="sxs-lookup"><span data-stu-id="777e7-194">See Also</span></span>
[<span data-ttu-id="777e7-195">Register New Items</span><span class="sxs-lookup"><span data-stu-id="777e7-195">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="777e7-196">Setting Up Inventory</span><span class="sxs-lookup"><span data-stu-id="777e7-196">Setting Up Inventory</span></span>](inventory-setup-inventory.md)  
[<span data-ttu-id="777e7-197">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="777e7-197">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="777e7-198">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="777e7-198">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="777e7-199">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="777e7-199">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
