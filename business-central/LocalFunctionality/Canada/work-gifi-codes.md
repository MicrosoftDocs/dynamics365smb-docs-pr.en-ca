---
title: GIFI Codes in Canada | Microsoft Docs
Description: In Canada, you can set up General Index of Financial Information (GIFI) codes and assign them to posting accounts
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0c4a29b19292047757247a057bd3502958510f05
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 02/15/2021
ms.locfileid: "5379733"
---
# <a name="work-with-gifi-codes"></a><span data-ttu-id="da914-103">Work With GIFI Codes</span><span class="sxs-lookup"><span data-stu-id="da914-103">Work With GIFI Codes</span></span>
<span data-ttu-id="da914-104">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span><span class="sxs-lookup"><span data-stu-id="da914-104">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span></span> <span data-ttu-id="da914-105">Fiscal information is classified using codes.</span><span class="sxs-lookup"><span data-stu-id="da914-105">Fiscal information is classified using codes.</span></span> <span data-ttu-id="da914-106">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span><span class="sxs-lookup"><span data-stu-id="da914-106">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span></span> <span data-ttu-id="da914-107">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span><span class="sxs-lookup"><span data-stu-id="da914-107">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span></span> <span data-ttu-id="da914-108">For more information, see the [Canada Revenue Agency website](https://www.cra-arc.gc.ca/).</span><span class="sxs-lookup"><span data-stu-id="da914-108">For more information, see the [Canada Revenue Agency website](https://www.cra-arc.gc.ca/).</span></span>

<span data-ttu-id="da914-109">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span><span class="sxs-lookup"><span data-stu-id="da914-109">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span></span> <span data-ttu-id="da914-110">It is a best practice to assign GIFI codes only to posting accounts, so that all totalling is done by your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="da914-110">It is a best practice to assign GIFI codes only to posting accounts, so that all totaling is done by your tax preparation software.</span></span>

<span data-ttu-id="da914-111">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span><span class="sxs-lookup"><span data-stu-id="da914-111">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span></span> <span data-ttu-id="da914-112">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span><span class="sxs-lookup"><span data-stu-id="da914-112">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span></span>

<span data-ttu-id="da914-113">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="da914-113">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span></span>

## <a name="to-set-up-gifi-codes"></a><span data-ttu-id="da914-114">To set up GIFI codes</span><span class="sxs-lookup"><span data-stu-id="da914-114">To set up GIFI codes</span></span>
<span data-ttu-id="da914-115">In [!INCLUDE[prod_short](../../includes/prod_short.md)], you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span><span class="sxs-lookup"><span data-stu-id="da914-115">In [!INCLUDE[prod_short](../../includes/prod_short.md)], you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span></span>

1. <span data-ttu-id="da914-116">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GIFI Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="da914-116">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GIFI Codes**, and then choose the related link.</span></span>
2. <span data-ttu-id="da914-117">On the **GIFI Codes** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="da914-117">On the **GIFI Codes** page, choose the **New** action.</span></span>
3. <span data-ttu-id="da914-118">Set up GIFI codes by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="da914-118">Set up GIFI codes by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]

## <a name="to-associate-gifi-codes-with-gl-accounts"></a><span data-ttu-id="da914-119">To associate GIFI codes with G/L accounts</span><span class="sxs-lookup"><span data-stu-id="da914-119">To associate GIFI codes with G/L accounts</span></span>
<span data-ttu-id="da914-120">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="da914-120">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span></span>

1. <span data-ttu-id="da914-121">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="da914-121">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="da914-122">Select a relevant general ledger account, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="da914-122">Select a relevant general ledger account, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="da914-123">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span><span class="sxs-lookup"><span data-stu-id="da914-123">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span></span>

## <a name="to-view-account-balances-using-the-gifi-code-report"></a><span data-ttu-id="da914-124">To view account balances using the GIFI code report</span><span class="sxs-lookup"><span data-stu-id="da914-124">To view account balances using the GIFI code report</span></span>
<span data-ttu-id="da914-125">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span><span class="sxs-lookup"><span data-stu-id="da914-125">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span></span>

1. <span data-ttu-id="da914-126">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="da914-126">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span></span>
2. <span data-ttu-id="da914-127">Specify what to include in the report by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="da914-127">Specify what to include in the report by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="da914-128">Choose the **Print** or the **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="da914-128">Choose the **Print** or the **Preview** button.</span></span>

## <a name="to-export-balance-information-using-gifi-codes"></a><span data-ttu-id="da914-129">To export balance information using GIFI codes</span><span class="sxs-lookup"><span data-stu-id="da914-129">To export balance information using GIFI codes</span></span>
<span data-ttu-id="da914-130">You can export balance information using GIFI codes and save the exported file in Excel.</span><span class="sxs-lookup"><span data-stu-id="da914-130">You can export balance information using GIFI codes and save the exported file in Excel.</span></span> <span data-ttu-id="da914-131">You can modify, save, or delete the file.</span><span class="sxs-lookup"><span data-stu-id="da914-131">You can modify, save, or delete the file.</span></span> <span data-ttu-id="da914-132">You can use the file to transfer information to your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="da914-132">You can use the file to transfer information to your tax preparation software.</span></span>

1. <span data-ttu-id="da914-133">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="da914-133">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span></span>
2. <span data-ttu-id="da914-134">Specify what to export to Excel by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="da914-134">Specify what to export to Excel by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="da914-135">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="da914-135">Choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="da914-136">The Excel file has the following characteristics:</span><span class="sxs-lookup"><span data-stu-id="da914-136">The Excel file has the following characteristics:</span></span>

* <span data-ttu-id="da914-137">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="da914-137">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span></span>
* <span data-ttu-id="da914-138">Negative numbers are represented as positive number in brackets.</span><span class="sxs-lookup"><span data-stu-id="da914-138">Negative numbers are represented as positive number in brackets.</span></span> <span data-ttu-id="da914-139">Accordingly, -123 is represented as (123).</span><span class="sxs-lookup"><span data-stu-id="da914-139">Accordingly, -123 is represented as (123).</span></span>

## <a name="see-also"></a><span data-ttu-id="da914-140">See Also</span><span class="sxs-lookup"><span data-stu-id="da914-140">See Also</span></span>
[<span data-ttu-id="da914-141">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="da914-141">Canada Local Functionality</span></span>](canada-local-functionality.md)  
<span data-ttu-id="da914-142">[Finance](../../finance.md) </span><span class="sxs-lookup"><span data-stu-id="da914-142">[Finance](../../finance.md) </span></span>  
[<span data-ttu-id="da914-143">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="da914-143">Setting Up Finance</span></span>](../../finance.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]