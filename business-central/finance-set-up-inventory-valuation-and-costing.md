---
title: Set Up Inventory Valuation and Costing | Microsoft Docs
description: The following table describes a sequence of tasks, with links to the topics that describe them.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 26b7f280afa61bc42af7b728272116731e6947b1
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 10/01/2019
ms.locfileid: "2305677"
---
# <a name="setting-up-inventory-valuation-and-costing"></a><span data-ttu-id="bb6f5-103">Setting Up Inventory Valuation and Costing</span><span class="sxs-lookup"><span data-stu-id="bb6f5-103">Setting Up Inventory Valuation and Costing</span></span>
<span data-ttu-id="bb6f5-104">To make sure that inventory costs are recorded correctly, you must set up various fields and pages before you begin to make item transactions.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-104">To make sure that inventory costs are recorded correctly, you must set up various fields and pages before you begin to make item transactions.</span></span>

<span data-ttu-id="bb6f5-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="bb6f5-106">**To**</span><span class="sxs-lookup"><span data-stu-id="bb6f5-106">**To**</span></span>|<span data-ttu-id="bb6f5-107">**See**</span><span class="sxs-lookup"><span data-stu-id="bb6f5-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="bb6f5-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span></span>|[<span data-ttu-id="bb6f5-109">Register New Items</span><span class="sxs-lookup"><span data-stu-id="bb6f5-109">Register New Items</span></span>](inventory-how-register-new-items.md)|  
|<span data-ttu-id="bb6f5-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span></span>|<span data-ttu-id="bb6f5-111">**Automatic Cost Posting** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-111">**Automatic Cost Posting** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bb6f5-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span></span>|<span data-ttu-id="bb6f5-113">**Expected Cost Posting to G/L** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-113">**Expected Cost Posting to G/L** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bb6f5-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span></span>|[<span data-ttu-id="bb6f5-115">Adjust Item Costs</span><span class="sxs-lookup"><span data-stu-id="bb6f5-115">Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|  
|<span data-ttu-id="bb6f5-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span></span>|<span data-ttu-id="bb6f5-117">**Average Cost Calc. Type** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-117">**Average Cost Calc. Type** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bb6f5-118">Select the period of time you would like application to use for calculating the weighted average cost of items that use the average costing method.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-118">Select the period of time you would like application to use for calculating the weighted average cost of items that use the average costing method.</span></span>|<span data-ttu-id="bb6f5-119">**Average Cost Period** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-119">**Average Cost Period** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="bb6f5-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span></span>|[<span data-ttu-id="bb6f5-121">Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="bb6f5-121">Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="bb6f5-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="bb6f5-123">**Exact Cost Reversing Mandatory** field on the **Sales & Receivables** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-123">**Exact Cost Reversing Mandatory** field on the **Sales & Receivables** page</span></span>|  
|<span data-ttu-id="bb6f5-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="bb6f5-125">**Exact Cost Reversing Mandatory** field on the **´Purchases & Payables** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-125">**Exact Cost Reversing Mandatory** field on the **´Purchases & Payables** page</span></span>|
|<span data-ttu-id="bb6f5-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span></span>|<span data-ttu-id="bb6f5-127">**Rounding Method** page</span><span class="sxs-lookup"><span data-stu-id="bb6f5-127">**Rounding Method** page</span></span>|  

## <a name="see-also"></a><span data-ttu-id="bb6f5-128">See Also</span><span class="sxs-lookup"><span data-stu-id="bb6f5-128">See Also</span></span>  
[<span data-ttu-id="bb6f5-129">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="bb6f5-129">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="bb6f5-130">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="bb6f5-130">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="bb6f5-131">Finance</span><span class="sxs-lookup"><span data-stu-id="bb6f5-131">Finance</span></span>](finance.md)  
