---
title: GIFI Codes in Canada | Microsoft Docs
Description: In Canada, you can set up General Index of Financial Information (GIFI) codes and assign them to posting accounts
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 08/11/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9203d6baea1d2780759e526143c445a0e7c6fad7
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-gifi-codes"></a><span data-ttu-id="12890-103">How to: Work With GIFI Codes</span><span class="sxs-lookup"><span data-stu-id="12890-103">How to: Work With GIFI Codes</span></span>
<span data-ttu-id="12890-104">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span><span class="sxs-lookup"><span data-stu-id="12890-104">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span></span> <span data-ttu-id="12890-105">Fiscal information is classified using codes.</span><span class="sxs-lookup"><span data-stu-id="12890-105">Fiscal information is classified using codes.</span></span> <span data-ttu-id="12890-106">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span><span class="sxs-lookup"><span data-stu-id="12890-106">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span></span> <span data-ttu-id="12890-107">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span><span class="sxs-lookup"><span data-stu-id="12890-107">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span></span> <span data-ttu-id="12890-108">For more information, see the [Canada Revenue Agency website](http://www.cra-arc.gc.ca/).</span><span class="sxs-lookup"><span data-stu-id="12890-108">For more information, see the [Canada Revenue Agency website](http://www.cra-arc.gc.ca/).</span></span>

<span data-ttu-id="12890-109">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span><span class="sxs-lookup"><span data-stu-id="12890-109">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span></span> <span data-ttu-id="12890-110">It is a best practice to assign GIFI codes only to posting accounts, so that all totalling is done by your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="12890-110">It is a best practice to assign GIFI codes only to posting accounts, so that all totaling is done by your tax preparation software.</span></span>

<span data-ttu-id="12890-111">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span><span class="sxs-lookup"><span data-stu-id="12890-111">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span></span> <span data-ttu-id="12890-112">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span><span class="sxs-lookup"><span data-stu-id="12890-112">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span></span>

<span data-ttu-id="12890-113">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="12890-113">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span></span>

## <a name="to-set-up-gifi-codes"></a><span data-ttu-id="12890-114">To set up GIFI codes</span><span class="sxs-lookup"><span data-stu-id="12890-114">To set up GIFI codes</span></span>
<span data-ttu-id="12890-115">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span><span class="sxs-lookup"><span data-stu-id="12890-115">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span></span>

1. <span data-ttu-id="12890-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **GIFI Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="12890-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **GIFI Codes**, and then choose the related link.</span></span>
2. <span data-ttu-id="12890-117">In the **GIFI Codes** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="12890-117">In the **GIFI Codes** window, choose the **New** action.</span></span>
3. <span data-ttu-id="12890-118">Set up GIFI codes by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="12890-118">Set up GIFI codes by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]

## <a name="to-associate-gifi-codes-with-gl-accounts"></a><span data-ttu-id="12890-119">To associate GIFI codes with G/L accounts</span><span class="sxs-lookup"><span data-stu-id="12890-119">To associate GIFI codes with G/L accounts</span></span>
<span data-ttu-id="12890-120">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="12890-120">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span></span>

1. <span data-ttu-id="12890-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="12890-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="12890-122">Select a relevant general ledger account, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="12890-122">Select a relevant general ledger account, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="12890-123">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span><span class="sxs-lookup"><span data-stu-id="12890-123">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span></span>

## <a name="to-view-account-balances-using-the-gifi-code-report"></a><span data-ttu-id="12890-124">To view account balances using the GIFI code report</span><span class="sxs-lookup"><span data-stu-id="12890-124">To view account balances using the GIFI code report</span></span>
<span data-ttu-id="12890-125">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span><span class="sxs-lookup"><span data-stu-id="12890-125">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span></span>

1. <span data-ttu-id="12890-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="12890-126">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span></span>
2. <span data-ttu-id="12890-127">Specify what to include in the report by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="12890-127">Specify what to include in the report by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="12890-128">Choose the **Print** or the **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="12890-128">Choose the **Print** or the **Preview** button.</span></span>

## <a name="to-export-balance-information-using-gifi-codes"></a><span data-ttu-id="12890-129">To export balance information using GIFI codes</span><span class="sxs-lookup"><span data-stu-id="12890-129">To export balance information using GIFI codes</span></span>
<span data-ttu-id="12890-130">You can export balance information using GIFI codes and save the exported file in Excel.</span><span class="sxs-lookup"><span data-stu-id="12890-130">You can export balance information using GIFI codes and save the exported file in Excel.</span></span> <span data-ttu-id="12890-131">You can modify, save, or delete the file.</span><span class="sxs-lookup"><span data-stu-id="12890-131">You can modify, save, or delete the file.</span></span> <span data-ttu-id="12890-132">You can use the file to transfer information to your tax preparation software.</span><span class="sxs-lookup"><span data-stu-id="12890-132">You can use the file to transfer information to your tax preparation software.</span></span>

1. <span data-ttu-id="12890-133">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="12890-133">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span></span>
2. <span data-ttu-id="12890-134">Specify what to export to Excel by filling the fields.</span><span class="sxs-lookup"><span data-stu-id="12890-134">Specify what to export to Excel by filling the fields.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="12890-135">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="12890-135">Choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="12890-136">The Excel file has the following characteristics:</span><span class="sxs-lookup"><span data-stu-id="12890-136">The Excel file has the following characteristics:</span></span>

* <span data-ttu-id="12890-137">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="12890-137">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span></span>
* <span data-ttu-id="12890-138">Negative numbers are represented as positive number in brackets.</span><span class="sxs-lookup"><span data-stu-id="12890-138">Negative numbers are represented as positive number in brackets.</span></span> <span data-ttu-id="12890-139">Accordingly, -123 is represented as (123).</span><span class="sxs-lookup"><span data-stu-id="12890-139">Accordingly, -123 is represented as (123).</span></span>

## <a name="see-also"></a><span data-ttu-id="12890-140">See Also</span><span class="sxs-lookup"><span data-stu-id="12890-140">See Also</span></span>
[<span data-ttu-id="12890-141">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="12890-141">Canada Local Functionality</span></span>](canada-local-functionality.md)  
<span data-ttu-id="12890-142">[Finance](../../finance.md) </span><span class="sxs-lookup"><span data-stu-id="12890-142">[Finance](../../finance.md) </span></span>  
[<span data-ttu-id="12890-143">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="12890-143">Setting Up Finance</span></span>](../../finance.md)

