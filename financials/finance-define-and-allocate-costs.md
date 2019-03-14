---
title: Defining and Allocating Costs | Microsoft Docs
description: Cost allocations move costs and revenues between cost types, cost centres, and cost objects. You can define as many allocations as you need.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 04e5a95b7a926528cc26c254390d08e3bce6ad8a
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="defining-and-allocating-costs"></a><span data-ttu-id="449b4-104">Defining and Allocating Costs</span><span class="sxs-lookup"><span data-stu-id="449b4-104">Defining and Allocating Costs</span></span>
<span data-ttu-id="449b4-105">Cost allocations move costs and revenues between cost types, cost centres, and cost objects.</span><span class="sxs-lookup"><span data-stu-id="449b4-105">Cost allocations move costs and revenues between cost types, cost centers, and cost objects.</span></span> <span data-ttu-id="449b4-106">You can define as many allocations as you need.</span><span class="sxs-lookup"><span data-stu-id="449b4-106">You can define as many allocations as you need.</span></span> <span data-ttu-id="449b4-107">Each allocation consists of:</span><span class="sxs-lookup"><span data-stu-id="449b4-107">Each allocation consists of:</span></span>  

-   <span data-ttu-id="449b4-108">An allocation source.</span><span class="sxs-lookup"><span data-stu-id="449b4-108">An allocation source.</span></span>  
-   <span data-ttu-id="449b4-109">One or more allocation targets.</span><span class="sxs-lookup"><span data-stu-id="449b4-109">One or more allocation targets.</span></span>  

<span data-ttu-id="449b4-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span><span class="sxs-lookup"><span data-stu-id="449b4-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span></span> <span data-ttu-id="449b4-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span><span class="sxs-lookup"><span data-stu-id="449b4-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span></span> <span data-ttu-id="449b4-112">You allocate all electricity and heating costs to three cost centres: Workshop, Production, and Sales.</span><span class="sxs-lookup"><span data-stu-id="449b4-112">You allocate all electricity and heating costs to three cost centers: Workshop, Production, and Sales.</span></span> <span data-ttu-id="449b4-113">These cost centres are your allocation targets.</span><span class="sxs-lookup"><span data-stu-id="449b4-113">These cost centers are your allocation targets.</span></span>  

<span data-ttu-id="449b4-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span><span class="sxs-lookup"><span data-stu-id="449b4-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span></span> <span data-ttu-id="449b4-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span><span class="sxs-lookup"><span data-stu-id="449b4-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span></span>  

<span data-ttu-id="449b4-116">For each allocation target, you define an allocation base.</span><span class="sxs-lookup"><span data-stu-id="449b4-116">For each allocation target, you define an allocation base.</span></span> <span data-ttu-id="449b4-117">The allocation base can be either static or dynamic.</span><span class="sxs-lookup"><span data-stu-id="449b4-117">The allocation base can be either static or dynamic.</span></span>  

-   <span data-ttu-id="449b4-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="449b4-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span></span>  
-   <span data-ttu-id="449b4-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost centre or sales revenue of a cost object throughout a certain time period.</span><span class="sxs-lookup"><span data-stu-id="449b4-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost center or sales revenue of a cost object throughout a certain time period.</span></span>  

<span data-ttu-id="449b4-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="449b4-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="449b4-121">To</span><span class="sxs-lookup"><span data-stu-id="449b4-121">To</span></span>|<span data-ttu-id="449b4-122">See</span><span class="sxs-lookup"><span data-stu-id="449b4-122">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="449b4-123">Set up allocation source and its targets.</span><span class="sxs-lookup"><span data-stu-id="449b4-123">Set up allocation source and its targets.</span></span>|[<span data-ttu-id="449b4-124">Set Up Allocation Source and Targets</span><span class="sxs-lookup"><span data-stu-id="449b4-124">Set Up Allocation Source and Targets</span></span>](finance-how-to-set-up-allocation-source-and-targets.md)|  
|<span data-ttu-id="449b4-125">Set up various filters for dynamic allocation bases.</span><span class="sxs-lookup"><span data-stu-id="449b4-125">Set up various filters for dynamic allocation bases.</span></span>|[<span data-ttu-id="449b4-126">Setting Filters for Dynamic Allocation Bases</span><span class="sxs-lookup"><span data-stu-id="449b4-126">Setting Filters for Dynamic Allocation Bases</span></span>](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|<span data-ttu-id="449b4-127">See an example of how to define a static allocation.</span><span class="sxs-lookup"><span data-stu-id="449b4-127">See an example of how to define a static allocation.</span></span>|[<span data-ttu-id="449b4-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span><span class="sxs-lookup"><span data-stu-id="449b4-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|<span data-ttu-id="449b4-129">See an example of how to define a dynamic allocation.</span><span class="sxs-lookup"><span data-stu-id="449b4-129">See an example of how to define a dynamic allocation.</span></span>|[<span data-ttu-id="449b4-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span><span class="sxs-lookup"><span data-stu-id="449b4-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a><span data-ttu-id="449b4-131">See Also</span><span class="sxs-lookup"><span data-stu-id="449b4-131">See Also</span></span>  
 <span data-ttu-id="449b4-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="449b4-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="449b4-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="449b4-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="449b4-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="449b4-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span></span>  
 <span data-ttu-id="449b4-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="449b4-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="449b4-136">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="449b4-136">About Cost Accounting</span></span>](finance-about-cost-accounting.md)
