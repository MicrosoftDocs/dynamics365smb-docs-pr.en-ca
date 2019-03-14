---
title: Manage Fixed Assets| Microsoft Docs
description: Learn about the fixed assets functionality and get an overview of how to work with fixed assets.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: machinery, buildings
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 9569f01f286008b76667e3a524257ba1aac61f91
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="fixed-assets"></a><span data-ttu-id="0b3d8-103">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-103">Fixed Assets</span></span>
<span data-ttu-id="0b3d8-104">The Fixed Assets functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides an overview of your fixed assets and ensures correct periodic depreciation.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-104">The Fixed Assets functionality in [!INCLUDE[d365fin](includes/d365fin_md.md)] provides an overview of your fixed assets and ensures correct periodic depreciation.</span></span> <span data-ttu-id="0b3d8-105">It also enables you to keep track of your maintenance costs, manage insurance policies, post fixed asset transactions, and generate various reports and statistics.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-105">It also enables you to keep track of your maintenance costs, manage insurance policies, post fixed asset transactions, and generate various reports and statistics.</span></span>

<span data-ttu-id="0b3d8-106">For each fixed asset, you must set up a card containing information about the asset.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-106">For each fixed asset, you must set up a card containing information about the asset.</span></span> <span data-ttu-id="0b3d8-107">You can set up buildings or production equipment as a main asset with a component list, and you can group them in various ways, such as by class, department, or location.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-107">You can set up buildings or production equipment as a main asset with a component list, and you can group them in various ways, such as by class, department, or location.</span></span> <span data-ttu-id="0b3d8-108">Then you can begin to acquire, maintain, and sell the fixed assets.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-108">Then you can begin to acquire, maintain, and sell the fixed assets.</span></span> <span data-ttu-id="0b3d8-109">You can also set up budgeted assets.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-109">You can also set up budgeted assets.</span></span> <span data-ttu-id="0b3d8-110">This makes it possible to include any anticipated acquisitions and sales in reports.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-110">This makes it possible to include any anticipated acquisitions and sales in reports.</span></span>

<span data-ttu-id="0b3d8-111">To keep track of fixed asset depreciations as well as other financial transactions related to fixed assets, you set up one or more depreciation books for each fixed asset in your company.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-111">To keep track of fixed asset depreciations as well as other financial transactions related to fixed assets, you set up one or more depreciation books for each fixed asset in your company.</span></span> <span data-ttu-id="0b3d8-112">Depreciation is done by running a report to calculate periodic depreciation and fill in a journal with the resulting entries, ready to be posted.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-112">Depreciation is done by running a report to calculate periodic depreciation and fill in a journal with the resulting entries, ready to be posted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="0b3d8-113">supports several depreciation methods.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-113">supports several depreciation methods.</span></span> <span data-ttu-id="0b3d8-114">For more information, see [Depreciation Methods](fa-depreciation-methods.md).</span><span class="sxs-lookup"><span data-stu-id="0b3d8-114">For more information, see [Depreciation Methods](fa-depreciation-methods.md).</span></span> <span data-ttu-id="0b3d8-115">You can set up multiple depreciation books per fixed asset for different purposes, such as one for tax reporting and another for internal reporting.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-115">You can set up multiple depreciation books per fixed asset for different purposes, such as one for tax reporting and another for internal reporting.</span></span>

<span data-ttu-id="0b3d8-116">For each asset, you can record maintenance costs and the next service date.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-116">For each asset, you can record maintenance costs and the next service date.</span></span> <span data-ttu-id="0b3d8-117">Keeping track of maintenance expenses can be important for budgeting purposes and for making decisions about whether to replace a fixed asset.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-117">Keeping track of maintenance expenses can be important for budgeting purposes and for making decisions about whether to replace a fixed asset.</span></span>

<span data-ttu-id="0b3d8-118">Each fixed asset can be attached to one or more insurance policies.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-118">Each fixed asset can be attached to one or more insurance policies.</span></span> <span data-ttu-id="0b3d8-119">You can therefore easily verify that insurance policy amounts are in accordance with the value of the assets that are linked to the policy.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-119">You can therefore easily verify that insurance policy amounts are in accordance with the value of the assets that are linked to the policy.</span></span> <span data-ttu-id="0b3d8-120">This also makes it easy to monitor annual insurance premiums.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-120">This also makes it easy to monitor annual insurance premiums.</span></span>

> [!NOTE]  
>   <span data-ttu-id="0b3d8-121">You can record fixed asset transactions on the **Fixed Asset G/L Journal** page or on the **Fixed Asset Journal** page, depending on whether the transactions are for financial reporting or for internal management.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-121">You can record fixed asset transactions on the **Fixed Asset G/L Journal** page or on the **Fixed Asset Journal** page, depending on whether the transactions are for financial reporting or for internal management.</span></span> <span data-ttu-id="0b3d8-122">Help for Fixed Assets only describes how to use the **Fixed Asset G/L Journal** page.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-122">Help for Fixed Assets only describes how to use the **Fixed Asset G/L Journal** page.</span></span> <span data-ttu-id="0b3d8-123">For more information, see [Set Up Fixed Asset Depreciation](fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="0b3d8-123">For more information, see [Set Up Fixed Asset Depreciation](fa-how-setup-depreciation.md).</span></span>

<span data-ttu-id="0b3d8-124">Before you can begin to manage fixed assets, you must set up default values, fixed asset accounting, posting groups, allocation keys, journals, and posting types.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-124">Before you can begin to manage fixed assets, you must set up default values, fixed asset accounting, posting groups, allocation keys, journals, and posting types.</span></span> <span data-ttu-id="0b3d8-125">For more information, see [Setting Up Fixed Assets](fa-setup.md).</span><span class="sxs-lookup"><span data-stu-id="0b3d8-125">For more information, see [Setting Up Fixed Assets](fa-setup.md).</span></span>

<span data-ttu-id="0b3d8-126">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-126">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="0b3d8-127">To</span><span class="sxs-lookup"><span data-stu-id="0b3d8-127">To</span></span> | <span data-ttu-id="0b3d8-128">See</span><span class="sxs-lookup"><span data-stu-id="0b3d8-128">See</span></span> |
| --- | --- |
| <span data-ttu-id="0b3d8-129">Create fixed assets, assign depreciation methods, post acquisitions, salvage values, and print fixed asset lists.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-129">Create fixed assets, assign depreciation methods, post acquisitions, salvage values, and print fixed asset lists.</span></span> |[<span data-ttu-id="0b3d8-130">Acquire Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-130">Acquire Fixed Assets</span></span>](fa-how-acquire.md) |
| <span data-ttu-id="0b3d8-131">Record service visits, post maintenance costs, and monitor maintenance costs.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-131">Record service visits, post maintenance costs, and monitor maintenance costs.</span></span> |[<span data-ttu-id="0b3d8-132">Maintain Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-132">Maintain Fixed Assets</span></span>](fa-how-maintain.md) |
| <span data-ttu-id="0b3d8-133">Update insurance information, post acquisition costs to insurance policies, modify insurance coverage, view insurance statistics, and list insurance policies.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-133">Update insurance information, post acquisition costs to insurance policies, modify insurance coverage, view insurance statistics, and list insurance policies.</span></span> |[<span data-ttu-id="0b3d8-134">Insure Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-134">Insure Fixed Assets</span></span>](fa-how-insure.md) |
| <span data-ttu-id="0b3d8-135">Reclassify fixed assets, transfer fixed assets to different locations, split up or combine assets.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-135">Reclassify fixed assets, transfer fixed assets to different locations, split up or combine assets.</span></span> |[<span data-ttu-id="0b3d8-136">Transfer, Split, or Combine Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-136">Transfer, Split, or Combine Fixed Assets</span></span>](fa-how-trans-split-combine.md) |
| <span data-ttu-id="0b3d8-137">Adjust values of fixed assets, post appreciation, and post write-down transactions.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-137">Adjust values of fixed assets, post appreciation, and post write-down transactions.</span></span> |[<span data-ttu-id="0b3d8-138">Revalue Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-138">Revalue Fixed Assets</span></span>](fa-how-revalue.md) |
| <span data-ttu-id="0b3d8-139">Calculate depreciation, post depreciation, and analyse depreciation in fixed assets reports.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-139">Calculate depreciation, post depreciation, and  analyze depreciation in fixed assets reports.</span></span> |[<span data-ttu-id="0b3d8-140">Depreciate or Amortize Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-140">Depreciate or Amortize Fixed Assets</span></span>](fa-how-depreciate-amortize.md) |
| <span data-ttu-id="0b3d8-141">Post disposal transactions, view disposal ledger entries, and post partial disposals.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-141">Post disposal transactions, view disposal ledger entries, and post partial disposals.</span></span> |[<span data-ttu-id="0b3d8-142">Dispose of or Retire Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-142">Dispose of or Retire Fixed Assets</span></span>](fa-how-dispose-retire.md) |
| <span data-ttu-id="0b3d8-143">Manage fixed asset budgets, budget acquisition costs, budget disposals of fixed assets, and budget depreciation.</span><span class="sxs-lookup"><span data-stu-id="0b3d8-143">Manage fixed asset budgets, budget acquisition costs, budget disposals of fixed assets, and budget depreciation.</span></span> |[<span data-ttu-id="0b3d8-144">Manage Budgets for Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-144">Manage Budgets for Fixed Assets</span></span>](fa-how-manage-budgets.md) |

## <a name="see-also"></a><span data-ttu-id="0b3d8-145">See Also</span><span class="sxs-lookup"><span data-stu-id="0b3d8-145">See Also</span></span>
[<span data-ttu-id="0b3d8-146">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="0b3d8-146">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="0b3d8-147">Changing Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="0b3d8-147">Changing Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="0b3d8-148">Finance</span><span class="sxs-lookup"><span data-stu-id="0b3d8-148">Finance</span></span>](finance.md)  
[<span data-ttu-id="0b3d8-149">Getting Started</span><span class="sxs-lookup"><span data-stu-id="0b3d8-149">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="0b3d8-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0b3d8-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 
