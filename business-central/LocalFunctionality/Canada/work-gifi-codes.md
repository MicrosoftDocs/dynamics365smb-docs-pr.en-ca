---
title: GIFI Codes in Canada | Microsoft Docs
Description: In Canada, you can set up General Index of Financial Information (GIFI) codes and assign them to posting accounts
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 10/01/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 2ada7e3cb796b8907b6a7e79a2dbadb4741ddc86
ms.contentlocale: en-ca
ms.lasthandoff: 11/26/2018

---
# <a name="work-with-gifi-codes"></a><span data-ttu-id="a54d0-102">Work With GIFI Codes</span><span class="sxs-lookup"><span data-stu-id="a54d0-102">Work With GIFI Codes</span></span>
<span data-ttu-id="a54d0-103">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span><span class="sxs-lookup"><span data-stu-id="a54d0-103">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span></span> <span data-ttu-id="a54d0-104">Fiscal information is classified using codes.</span><span class="sxs-lookup"><span data-stu-id="a54d0-104">Fiscal information is classified using codes.</span></span> <span data-ttu-id="a54d0-105">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span><span class="sxs-lookup"><span data-stu-id="a54d0-105">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span></span> <span data-ttu-id="a54d0-106">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span><span class="sxs-lookup"><span data-stu-id="a54d0-106">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span></span> <span data-ttu-id="a54d0-107">For more information, see the [Canada Revenue Agency website](https://www.cra-arc.gc.ca/).</span><span class="sxs-lookup"><span data-stu-id="a54d0-107">For more information, see the [Canada Revenue Agency website](https://www.cra-arc.gc.ca/).</span></span>

<span data-ttu-id="a54d0-108">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span><span class="sxs-lookup"><span data-stu-id="a54d0-108">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span></span> <span data-ttu-id="a54d0-109">It is a best practice to assign GIFI codes only to posting accounts, so that all totalling is done by your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="a54d0-109">It is a best practice to assign GIFI codes only to posting accounts, so that all totaling is done by your tax preparation software.</span></span>

<span data-ttu-id="a54d0-110">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span><span class="sxs-lookup"><span data-stu-id="a54d0-110">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span></span> <span data-ttu-id="a54d0-111">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span><span class="sxs-lookup"><span data-stu-id="a54d0-111">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span></span>

<span data-ttu-id="a54d0-112">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="a54d0-112">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span></span>

## <a name="to-set-up-gifi-codes"></a><span data-ttu-id="a54d0-113">To set up GIFI codes</span><span class="sxs-lookup"><span data-stu-id="a54d0-113">To set up GIFI codes</span></span>
<span data-ttu-id="a54d0-114">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span><span class="sxs-lookup"><span data-stu-id="a54d0-114">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span></span>

1. <span data-ttu-id="a54d0-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **GIFI Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a54d0-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **GIFI Codes**, and then choose the related link.</span></span>
2. <span data-ttu-id="a54d0-116">On the **GIFI Codes** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="a54d0-116">On the **GIFI Codes** page, choose the **New** action.</span></span>
3. <span data-ttu-id="a54d0-117">Set up GIFI codes by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="a54d0-117">Set up GIFI codes by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]

## <a name="to-associate-gifi-codes-with-gl-accounts"></a><span data-ttu-id="a54d0-118">To associate GIFI codes with G/L accounts</span><span class="sxs-lookup"><span data-stu-id="a54d0-118">To associate GIFI codes with G/L accounts</span></span>
<span data-ttu-id="a54d0-119">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="a54d0-119">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span></span>

1. <span data-ttu-id="a54d0-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a54d0-120">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="a54d0-121">Select a relevant general ledger account, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="a54d0-121">Select a relevant general ledger account, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="a54d0-122">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span><span class="sxs-lookup"><span data-stu-id="a54d0-122">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span></span>

## <a name="to-view-account-balances-using-the-gifi-code-report"></a><span data-ttu-id="a54d0-123">To view account balances using the GIFI code report</span><span class="sxs-lookup"><span data-stu-id="a54d0-123">To view account balances using the GIFI code report</span></span>
<span data-ttu-id="a54d0-124">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span><span class="sxs-lookup"><span data-stu-id="a54d0-124">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span></span>

1. <span data-ttu-id="a54d0-125">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a54d0-125">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span></span>
2. <span data-ttu-id="a54d0-126">Specify what to include in the report by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="a54d0-126">Specify what to include in the report by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="a54d0-127">Choose the **Print** or the **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="a54d0-127">Choose the **Print** or the **Preview** button.</span></span>

## <a name="to-export-balance-information-using-gifi-codes"></a><span data-ttu-id="a54d0-128">To export balance information using GIFI codes</span><span class="sxs-lookup"><span data-stu-id="a54d0-128">To export balance information using GIFI codes</span></span>
<span data-ttu-id="a54d0-129">You can export balance information using GIFI codes and save the exported file in Excel.</span><span class="sxs-lookup"><span data-stu-id="a54d0-129">You can export balance information using GIFI codes and save the exported file in Excel.</span></span> <span data-ttu-id="a54d0-130">You can modify, save, or delete the file.</span><span class="sxs-lookup"><span data-stu-id="a54d0-130">You can modify, save, or delete the file.</span></span> <span data-ttu-id="a54d0-131">You can use the file to transfer information to your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="a54d0-131">You can use the file to transfer information to your tax preparation software.</span></span>

1. <span data-ttu-id="a54d0-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a54d0-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span></span>
2. <span data-ttu-id="a54d0-133">Specify what to export to Excel by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="a54d0-133">Specify what to export to Excel by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="a54d0-134">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a54d0-134">Choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="a54d0-135">The Excel file has the following characteristics:</span><span class="sxs-lookup"><span data-stu-id="a54d0-135">The Excel file has the following characteristics:</span></span>

* <span data-ttu-id="a54d0-136">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="a54d0-136">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span></span>
* <span data-ttu-id="a54d0-137">Negative numbers are represented as positive number in brackets.</span><span class="sxs-lookup"><span data-stu-id="a54d0-137">Negative numbers are represented as positive number in brackets.</span></span> <span data-ttu-id="a54d0-138">Accordingly, -123 is represented as (123).</span><span class="sxs-lookup"><span data-stu-id="a54d0-138">Accordingly, -123 is represented as (123).</span></span>

## <a name="see-also"></a><span data-ttu-id="a54d0-139">See Also</span><span class="sxs-lookup"><span data-stu-id="a54d0-139">See Also</span></span>
[<span data-ttu-id="a54d0-140">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="a54d0-140">Canada Local Functionality</span></span>](canada-local-functionality.md)  
<span data-ttu-id="a54d0-141">[Finance](../../finance.md) </span><span class="sxs-lookup"><span data-stu-id="a54d0-141">[Finance](../../finance.md) </span></span>  
[<span data-ttu-id="a54d0-142">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="a54d0-142">Setting Up Finance</span></span>](../../finance.md)

