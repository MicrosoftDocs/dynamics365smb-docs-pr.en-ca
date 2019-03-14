---
title: Design Details - Variance | Microsoft Docs
description: Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 36062fc6fa40c3fc2b928ffad7e3b242634149fc
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="design-details-variance"></a><span data-ttu-id="5fba5-103">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="5fba5-103">Design Details: Variance</span></span>
<span data-ttu-id="5fba5-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span><span class="sxs-lookup"><span data-stu-id="5fba5-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span></span>  

 <span data-ttu-id="5fba5-105">actual cost – standard cost = variance</span><span class="sxs-lookup"><span data-stu-id="5fba5-105">actual cost – standard cost = variance</span></span>  

 <span data-ttu-id="5fba5-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span><span class="sxs-lookup"><span data-stu-id="5fba5-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5fba5-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span><span class="sxs-lookup"><span data-stu-id="5fba5-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span></span>  

## <a name="example"></a><span data-ttu-id="5fba5-108">Example</span><span class="sxs-lookup"><span data-stu-id="5fba5-108">Example</span></span>  
 <span data-ttu-id="5fba5-109">The following example illustrates how variance is calculated for purchased items.</span><span class="sxs-lookup"><span data-stu-id="5fba5-109">The following example illustrates how variance is calculated for purchased items.</span></span> <span data-ttu-id="5fba5-110">It is based on the following scenario:</span><span class="sxs-lookup"><span data-stu-id="5fba5-110">It is based on the following scenario:</span></span>  

1.  <span data-ttu-id="5fba5-111">The user purchases an item at $ 90.00, but the standard cost is $ 100.00.</span><span class="sxs-lookup"><span data-stu-id="5fba5-111">The user purchases an item at LCY 90.00, but the standard cost is LCY 100.00.</span></span> <span data-ttu-id="5fba5-112">Accordingly, the purchase variance is $ –10.00.</span><span class="sxs-lookup"><span data-stu-id="5fba5-112">Accordingly, the purchase variance is LCY –10.00.</span></span>  
2.  <span data-ttu-id="5fba5-113">$ 10.00 is credited to the purchase variance account.</span><span class="sxs-lookup"><span data-stu-id="5fba5-113">LCY 10.00 is credited to the purchase variance account.</span></span>  
3.  <span data-ttu-id="5fba5-114">The user posts an item charge of $ 20.00.</span><span class="sxs-lookup"><span data-stu-id="5fba5-114">The user posts an item charge of LCY 20.00.</span></span> <span data-ttu-id="5fba5-115">Accordingly, the actual cost is increased to $ 110.00, and the value of the purchase variance becomes $ 10.00.</span><span class="sxs-lookup"><span data-stu-id="5fba5-115">Accordingly, the actual cost is increased to LCY 110.00, and the value of the purchase variance becomes LCY 10.00.</span></span>  
4.  <span data-ttu-id="5fba5-116">$ 20.00 is debited to the purchase variance account.</span><span class="sxs-lookup"><span data-stu-id="5fba5-116">LCY 20.00 is debited to the purchase variance account.</span></span> <span data-ttu-id="5fba5-117">Accordingly, the net purchase variance becomes $ 10.00.</span><span class="sxs-lookup"><span data-stu-id="5fba5-117">Accordingly, the net purchase variance becomes LCY 10.00.</span></span>  
5.  <span data-ttu-id="5fba5-118">The user revalues the item from $ 100.00 to $ 70.00.</span><span class="sxs-lookup"><span data-stu-id="5fba5-118">The user revalues the item from LCY 100.00 to LCY 70.00.</span></span> <span data-ttu-id="5fba5-119">This does not affect the variance calculation, only the inventory value.</span><span class="sxs-lookup"><span data-stu-id="5fba5-119">This does not affect the variance calculation, only the inventory value.</span></span>  

 <span data-ttu-id="5fba5-120">The following table shows the resulting value entries.</span><span class="sxs-lookup"><span data-stu-id="5fba5-120">The following table shows the resulting value entries.</span></span>  

 <span data-ttu-id="5fba5-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "Purchase variance calculation")</span><span class="sxs-lookup"><span data-stu-id="5fba5-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "Purchase variance calculation")</span></span>  

## <a name="determining-the-standard-cost"></a><span data-ttu-id="5fba5-122">Determining the Standard Cost</span><span class="sxs-lookup"><span data-stu-id="5fba5-122">Determining the Standard Cost</span></span>  
 <span data-ttu-id="5fba5-123">The standard cost is used when calculating variance and the amount to capitalize.</span><span class="sxs-lookup"><span data-stu-id="5fba5-123">The standard cost is used when calculating variance and the amount to capitalize.</span></span> <span data-ttu-id="5fba5-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span><span class="sxs-lookup"><span data-stu-id="5fba5-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span></span> <span data-ttu-id="5fba5-125">This point is when the inventory increase is invoiced.</span><span class="sxs-lookup"><span data-stu-id="5fba5-125">This point is when the inventory increase is invoiced.</span></span> <span data-ttu-id="5fba5-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span><span class="sxs-lookup"><span data-stu-id="5fba5-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span></span>  

 <span data-ttu-id="5fba5-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span><span class="sxs-lookup"><span data-stu-id="5fba5-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span></span>  

|<span data-ttu-id="5fba5-128">Cost Share</span><span class="sxs-lookup"><span data-stu-id="5fba5-128">Cost Share</span></span>|<span data-ttu-id="5fba5-129">Purchased Item</span><span class="sxs-lookup"><span data-stu-id="5fba5-129">Purchased Item</span></span>|<span data-ttu-id="5fba5-130">Produced/Assembled Item</span><span class="sxs-lookup"><span data-stu-id="5fba5-130">Produced/Assembled Item</span></span>|  
|----------------|--------------------|------------------------------|  
|<span data-ttu-id="5fba5-131">**Standard Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-131">**Standard Cost**</span></span>||<span data-ttu-id="5fba5-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span><span class="sxs-lookup"><span data-stu-id="5fba5-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span></span>|  
|<span data-ttu-id="5fba5-133">**Single-Level Material Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-133">**Single-Level Material Cost**</span></span>|<span data-ttu-id="5fba5-134">Unit Cost</span><span class="sxs-lookup"><span data-stu-id="5fba5-134">Unit Cost</span></span>|<span data-ttu-id="5fba5-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "Equation 1")</span><span class="sxs-lookup"><span data-stu-id="5fba5-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "Equation 1")</span></span>|  
|<span data-ttu-id="5fba5-136">**Single-Level Capacity Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-136">**Single-Level Capacity Cost**</span></span>|<span data-ttu-id="5fba5-137">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-137">Not applicable</span></span>|<span data-ttu-id="5fba5-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "Equation 2")</span><span class="sxs-lookup"><span data-stu-id="5fba5-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "Equation 2")</span></span>|  
|<span data-ttu-id="5fba5-139">**Single-Level Subcontrd. Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-139">**Single-Level Subcontrd. Cost**</span></span>|<span data-ttu-id="5fba5-140">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-140">Not applicable</span></span>|<span data-ttu-id="5fba5-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "Equation 3")</span><span class="sxs-lookup"><span data-stu-id="5fba5-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "Equation 3")</span></span>|  
|<span data-ttu-id="5fba5-142">**Single-Level Cap. Ovhd Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-142">**Single-Level Cap. Ovhd Cost**</span></span>|<span data-ttu-id="5fba5-143">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-143">Not applicable</span></span>|<span data-ttu-id="5fba5-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "Equation 4")</span><span class="sxs-lookup"><span data-stu-id="5fba5-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "Equation 4")</span></span>|  
|<span data-ttu-id="5fba5-145">**Single-Level Mfg. Ovhd Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-145">**Single-Level Mfg. Ovhd Cost**</span></span>|<span data-ttu-id="5fba5-146">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-146">Not applicable</span></span>|<span data-ttu-id="5fba5-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) \* Indirect Cost % / 100 + Overhead Rate</span><span class="sxs-lookup"><span data-stu-id="5fba5-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) \* Indirect Cost % / 100 + Overhead Rate</span></span>|  
|<span data-ttu-id="5fba5-148">**Rolled-up Material Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-148">**Rolled-up Material Cost**</span></span>|<span data-ttu-id="5fba5-149">Unit Cost</span><span class="sxs-lookup"><span data-stu-id="5fba5-149">Unit Cost</span></span>|<span data-ttu-id="5fba5-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "Equation 5")</span><span class="sxs-lookup"><span data-stu-id="5fba5-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "Equation 5")</span></span>|  
|<span data-ttu-id="5fba5-151">**Rolled-up Capacity Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-151">**Rolled-up Capacity Cost**</span></span>|<span data-ttu-id="5fba5-152">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-152">Not applicable</span></span>|<span data-ttu-id="5fba5-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "Equation 6")</span><span class="sxs-lookup"><span data-stu-id="5fba5-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "Equation 6")</span></span>|  
|<span data-ttu-id="5fba5-154">**Rolled-Up Subcontracted Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-154">**Rolled-Up Subcontracted Cost**</span></span>|<span data-ttu-id="5fba5-155">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-155">Not applicable</span></span>|<span data-ttu-id="5fba5-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "Equation 7")</span><span class="sxs-lookup"><span data-stu-id="5fba5-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "Equation 7")</span></span>|  
|<span data-ttu-id="5fba5-157">**Rolled-up Capacity Ovhd. Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-157">**Rolled-up Capacity Ovhd. Cost**</span></span>|<span data-ttu-id="5fba5-158">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-158">Not applicable</span></span>|<span data-ttu-id="5fba5-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "Equation 8")</span><span class="sxs-lookup"><span data-stu-id="5fba5-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "Equation 8")</span></span>|  
|<span data-ttu-id="5fba5-160">**Rolled-up Mfg. Ovhd. Cost**</span><span class="sxs-lookup"><span data-stu-id="5fba5-160">**Rolled-up Mfg. Ovhd. Cost**</span></span>|<span data-ttu-id="5fba5-161">Not applicable</span><span class="sxs-lookup"><span data-stu-id="5fba5-161">Not applicable</span></span>|<span data-ttu-id="5fba5-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "Equation 9")</span><span class="sxs-lookup"><span data-stu-id="5fba5-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "Equation 9")</span></span>|  

## <a name="see-also"></a><span data-ttu-id="5fba5-163">See Also</span><span class="sxs-lookup"><span data-stu-id="5fba5-163">See Also</span></span>  
 <span data-ttu-id="5fba5-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="5fba5-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="5fba5-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span><span class="sxs-lookup"><span data-stu-id="5fba5-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span></span>  
 [<span data-ttu-id="5fba5-166">Finance</span><span class="sxs-lookup"><span data-stu-id="5fba5-166">Finance</span></span>](finance.md)  
 <span data-ttu-id="5fba5-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5fba5-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
