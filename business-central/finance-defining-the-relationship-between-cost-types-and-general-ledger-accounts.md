---
title: Defining the Relationship Between Cost Types and General Ledger Accounts | Microsoft Docs
description: Learn how to define the relationship between the cost type and the general ledger account.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 7709edb214804f52ee9b495c43b5302e2a23bd6b
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="a1bff-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span><span class="sxs-lookup"><span data-stu-id="a1bff-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="a1bff-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span><span class="sxs-lookup"><span data-stu-id="a1bff-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="a1bff-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span><span class="sxs-lookup"><span data-stu-id="a1bff-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="a1bff-106">The **Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="a1bff-106">The **Cost Type No.**</span></span> <span data-ttu-id="a1bff-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span><span class="sxs-lookup"><span data-stu-id="a1bff-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="a1bff-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span><span class="sxs-lookup"><span data-stu-id="a1bff-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="a1bff-109">Relationship Between General Ledger Accounts and Cost Types</span><span class="sxs-lookup"><span data-stu-id="a1bff-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="a1bff-110">There is an n:1 relationship between general ledger accounts and cost types.</span><span class="sxs-lookup"><span data-stu-id="a1bff-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="a1bff-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="a1bff-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="a1bff-112">The following table describes the details in the relationship.</span><span class="sxs-lookup"><span data-stu-id="a1bff-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="a1bff-113">Relationship</span><span class="sxs-lookup"><span data-stu-id="a1bff-113">Relationship</span></span>|<span data-ttu-id="a1bff-114">**G/L Account Range**</span><span class="sxs-lookup"><span data-stu-id="a1bff-114">**G/L Account Range**</span></span>|<span data-ttu-id="a1bff-115">**Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="a1bff-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="a1bff-116">One general ledger account for each cost type</span><span class="sxs-lookup"><span data-stu-id="a1bff-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="a1bff-117">One general ledger account</span><span class="sxs-lookup"><span data-stu-id="a1bff-117">One general ledger account</span></span>|<span data-ttu-id="a1bff-118">One cost type</span><span class="sxs-lookup"><span data-stu-id="a1bff-118">One cost type</span></span>|  
|<span data-ttu-id="a1bff-119">Several general ledger accounts for one cost type</span><span class="sxs-lookup"><span data-stu-id="a1bff-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="a1bff-120">General ledger account range, for example, 7110..7193 for each general ledger account</span><span class="sxs-lookup"><span data-stu-id="a1bff-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="a1bff-121">For each general ledger account in the range, there is only one cost type</span><span class="sxs-lookup"><span data-stu-id="a1bff-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="a1bff-122">Cost types without corresponding general ledger accounts</span><span class="sxs-lookup"><span data-stu-id="a1bff-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="a1bff-123">General ledger accounts whose entries will not be transferred</span><span class="sxs-lookup"><span data-stu-id="a1bff-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="a1bff-124">Cost Types Without a Relationship to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="a1bff-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="a1bff-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span><span class="sxs-lookup"><span data-stu-id="a1bff-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="a1bff-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span><span class="sxs-lookup"><span data-stu-id="a1bff-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="a1bff-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span><span class="sxs-lookup"><span data-stu-id="a1bff-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="a1bff-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="a1bff-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a1bff-129">See Also</span><span class="sxs-lookup"><span data-stu-id="a1bff-129">See Also</span></span>  
[<span data-ttu-id="a1bff-130">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="a1bff-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="a1bff-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="a1bff-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="a1bff-132">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="a1bff-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="a1bff-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a1bff-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

