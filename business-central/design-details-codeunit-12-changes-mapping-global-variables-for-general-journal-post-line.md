---
title: Design Details - Codeunit 12 Changes in Mapping Global Variables for General Journal Post Line | Microsoft Docs
description: The following changes have been implemented in this release of Business Central.
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
ms.openlocfilehash: 9cb19558c8c441eac188504e798ca36d86b599d5
ms.contentlocale: en-ca
ms.lasthandoff: 09/28/2018

---
# <a name="codeunit-12-changes-mapping-global-variables-for-general-journal-post-line"></a><span data-ttu-id="ca080-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="ca080-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>
<span data-ttu-id="ca080-104">The following changes have been implemented in this release of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ca080-104">The following changes have been implemented in this release of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

|<span data-ttu-id="ca080-105">**Microsoft Dynamics NAV 2009 R2**</span><span class="sxs-lookup"><span data-stu-id="ca080-105">**Microsoft Dynamics NAV 2009 R2**</span></span>|<span data-ttu-id="ca080-106">**Microsoft Dynamics NAV 2013 R2**</span><span class="sxs-lookup"><span data-stu-id="ca080-106">**Microsoft Dynamics NAV 2013 R2**</span></span>|<span data-ttu-id="ca080-107">**Comment**</span><span class="sxs-lookup"><span data-stu-id="ca080-107">**Comment**</span></span>|  
|----------------------------------------|----------------------------------------|-----------------|  
|<span data-ttu-id="ca080-108">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="ca080-108">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="ca080-109">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="ca080-109">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="ca080-110">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-110">Unchanged</span></span>|  
|<span data-ttu-id="ca080-111">SalesSetup@1010 : Record 311;</span><span class="sxs-lookup"><span data-stu-id="ca080-111">SalesSetup@1010 : Record 311;</span></span>||<span data-ttu-id="ca080-112">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-112">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-113">PurchSetup@1011 : Record 312;</span><span class="sxs-lookup"><span data-stu-id="ca080-113">PurchSetup@1011 : Record 312;</span></span>||<span data-ttu-id="ca080-114">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-114">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-115">AccountingPeriod@1012 : Record 50;</span><span class="sxs-lookup"><span data-stu-id="ca080-115">AccountingPeriod@1012 : Record 50;</span></span>||<span data-ttu-id="ca080-116">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-116">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-117">GLAcc@1013 : Record 15;</span><span class="sxs-lookup"><span data-stu-id="ca080-117">GLAcc@1013 : Record 15;</span></span>||<span data-ttu-id="ca080-118">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-118">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-119">GLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-119">GLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="ca080-120">GlobalGLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-120">GlobalGLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="ca080-121">Renamed</span><span class="sxs-lookup"><span data-stu-id="ca080-121">Renamed</span></span>|  
|<span data-ttu-id="ca080-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="ca080-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="ca080-124">Renamed</span><span class="sxs-lookup"><span data-stu-id="ca080-124">Renamed</span></span>|  
|<span data-ttu-id="ca080-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="ca080-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="ca080-127">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-127">Unchanged</span></span>|  
|<span data-ttu-id="ca080-128">OrigGLEntry@1017 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-128">OrigGLEntry@1017 : Record 17;</span></span>||<span data-ttu-id="ca080-129">Deleted</span><span class="sxs-lookup"><span data-stu-id="ca080-129">Deleted</span></span>|  
|<span data-ttu-id="ca080-130">VATPostingSetup@1019 : Record 325;</span><span class="sxs-lookup"><span data-stu-id="ca080-130">VATPostingSetup@1019 : Record 325;</span></span>||<span data-ttu-id="ca080-131">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-131">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-132">Cust@1020 : Record 18;</span><span class="sxs-lookup"><span data-stu-id="ca080-132">Cust@1020 : Record 18;</span></span>||<span data-ttu-id="ca080-133">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-133">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-134">Vend@1021 : Record 23;</span><span class="sxs-lookup"><span data-stu-id="ca080-134">Vend@1021 : Record 23;</span></span>||<span data-ttu-id="ca080-135">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-135">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-136">GenJnlLine@1022 : Record 81;</span><span class="sxs-lookup"><span data-stu-id="ca080-136">GenJnlLine@1022 : Record 81;</span></span>||<span data-ttu-id="ca080-137">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-137">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-138">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="ca080-138">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="ca080-139">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="ca080-139">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="ca080-140">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-140">Unchanged</span></span>|  
|<span data-ttu-id="ca080-141">CustPostingGr@1030 : Record 92;</span><span class="sxs-lookup"><span data-stu-id="ca080-141">CustPostingGr@1030 : Record 92;</span></span>||<span data-ttu-id="ca080-142">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-142">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-143">VendPostingGr@1031 : Record 93;</span><span class="sxs-lookup"><span data-stu-id="ca080-143">VendPostingGr@1031 : Record 93;</span></span>||<span data-ttu-id="ca080-144">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-144">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-145">Currency@1032 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="ca080-145">Currency@1032 : Record 4;</span></span>||<span data-ttu-id="ca080-146">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-146">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-147">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="ca080-147">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="ca080-148">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="ca080-148">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="ca080-149">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-149">Unchanged</span></span>|  
|<span data-ttu-id="ca080-150">ApplnCurrency@1034 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="ca080-150">ApplnCurrency@1034 : Record 4;</span></span>||<span data-ttu-id="ca080-151">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-151">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-152">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="ca080-152">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="ca080-153">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="ca080-153">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="ca080-154">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-154">Unchanged</span></span>|  
|<span data-ttu-id="ca080-155">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="ca080-155">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="ca080-156">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="ca080-156">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="ca080-157">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-157">Unchanged</span></span>|  
|<span data-ttu-id="ca080-158">BankAcc@1039 : Record 270;</span><span class="sxs-lookup"><span data-stu-id="ca080-158">BankAcc@1039 : Record 270;</span></span>||<span data-ttu-id="ca080-159">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-159">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-160">BankAccLedgEntry@1040 : Record 271;</span><span class="sxs-lookup"><span data-stu-id="ca080-160">BankAccLedgEntry@1040 : Record 271;</span></span>||<span data-ttu-id="ca080-161">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-161">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-162">CheckLedgEntry@1041 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="ca080-162">CheckLedgEntry@1041 : Record 272;</span></span>||<span data-ttu-id="ca080-163">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-163">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-164">CheckLedgEntry2@1042 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="ca080-164">CheckLedgEntry2@1042 : Record 272;</span></span>||<span data-ttu-id="ca080-165">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-165">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-166">BankAccPostingGr@1043 : Record 277;</span><span class="sxs-lookup"><span data-stu-id="ca080-166">BankAccPostingGr@1043 : Record 277;</span></span>||<span data-ttu-id="ca080-167">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-167">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-168">GenJnlTemplate@1044 : Record 80;</span><span class="sxs-lookup"><span data-stu-id="ca080-168">GenJnlTemplate@1044 : Record 80;</span></span>||<span data-ttu-id="ca080-169">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-169">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-170">TaxJurisdiction@1045 : Record 320;</span><span class="sxs-lookup"><span data-stu-id="ca080-170">TaxJurisdiction@1045 : Record 320;</span></span>||<span data-ttu-id="ca080-171">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-171">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-172">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="ca080-172">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="ca080-173">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="ca080-173">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="ca080-174">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-174">Unchanged</span></span>|  
|<span data-ttu-id="ca080-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span><span class="sxs-lookup"><span data-stu-id="ca080-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span></span>||<span data-ttu-id="ca080-176">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-176">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-177">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="ca080-177">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="ca080-178">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="ca080-178">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="ca080-179">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-179">Unchanged</span></span>|  
|<span data-ttu-id="ca080-180">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="ca080-180">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="ca080-181">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="ca080-181">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="ca080-182">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-182">Unchanged</span></span>|  
|<span data-ttu-id="ca080-183">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="ca080-183">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="ca080-184">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="ca080-184">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="ca080-185">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-185">Unchanged</span></span>|  
|<span data-ttu-id="ca080-186">TempVATEntry@1088 : TEMPORARY Record 254;</span><span class="sxs-lookup"><span data-stu-id="ca080-186">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="ca080-187">TempVATEntry@1088 : TEMPORARY Record 254;</span><span class="sxs-lookup"><span data-stu-id="ca080-187">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="ca080-188">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-188">Unchanged</span></span>|  
|<span data-ttu-id="ca080-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="ca080-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span></span>||<span data-ttu-id="ca080-190">Moved to Codeunit17</span><span class="sxs-lookup"><span data-stu-id="ca080-190">Moved to Codeunit17</span></span>|  
|<span data-ttu-id="ca080-191">CostAccSetup@1092 : Record 1108;</span><span class="sxs-lookup"><span data-stu-id="ca080-191">CostAccSetup@1092 : Record 1108;</span></span>||<span data-ttu-id="ca080-192">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-192">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-193">GenJnlCheckLine@1048 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="ca080-193">GenJnlCheckLine@1048 : Codeunit 11;</span></span>|<span data-ttu-id="ca080-194">GenJnlCheckLine@1001 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="ca080-194">GenJnlCheckLine@1001 : Codeunit 11;</span></span>|<span data-ttu-id="ca080-195">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-195">Unchanged</span></span>|  
|<span data-ttu-id="ca080-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span><span class="sxs-lookup"><span data-stu-id="ca080-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span></span>||<span data-ttu-id="ca080-197">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-197">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-198">FAJnlPostLine@1050 : Codeunit 5632;</span><span class="sxs-lookup"><span data-stu-id="ca080-198">FAJnlPostLine@1050 : Codeunit 5632;</span></span>||<span data-ttu-id="ca080-199">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-199">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-200">SalesTaxCalculate@1051 : Codeunit 398;</span><span class="sxs-lookup"><span data-stu-id="ca080-200">SalesTaxCalculate@1051 : Codeunit 398;</span></span>||<span data-ttu-id="ca080-201">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-201">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-202">GenJnlApply@1052 : Codeunit 225;</span><span class="sxs-lookup"><span data-stu-id="ca080-202">GenJnlApply@1052 : Codeunit 225;</span></span>||<span data-ttu-id="ca080-203">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-203">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-204">DimMgt@1053 : Codeunit 408;</span><span class="sxs-lookup"><span data-stu-id="ca080-204">DimMgt@1053 : Codeunit 408;</span></span>||<span data-ttu-id="ca080-205">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-205">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-206">JobPostLine@1028 : Codeunit 1001;</span><span class="sxs-lookup"><span data-stu-id="ca080-206">JobPostLine@1028 : Codeunit 1001;</span></span>||<span data-ttu-id="ca080-207">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-207">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span><span class="sxs-lookup"><span data-stu-id="ca080-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span></span>||<span data-ttu-id="ca080-209">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-209">Changed to Local</span></span>|  
||<span data-ttu-id="ca080-210">PaymentToleranceMgt@1002 : Codeunit 426;</span><span class="sxs-lookup"><span data-stu-id="ca080-210">PaymentToleranceMgt@1002 : Codeunit 426;</span></span>|<span data-ttu-id="ca080-211">Added</span><span class="sxs-lookup"><span data-stu-id="ca080-211">Added</span></span>|  
||<span data-ttu-id="ca080-212">AddCurrencyCode@1117 : Code[10];</span><span class="sxs-lookup"><span data-stu-id="ca080-212">AddCurrencyCode@1117 : Code[10];</span></span>|<span data-ttu-id="ca080-213">Added</span><span class="sxs-lookup"><span data-stu-id="ca080-213">Added</span></span>|  
|<span data-ttu-id="ca080-214">FiscalYearStartDate@1054 : Date;</span><span class="sxs-lookup"><span data-stu-id="ca080-214">FiscalYearStartDate@1054 : Date;</span></span>|<span data-ttu-id="ca080-215">FiscalYearStartDate@1011 : Date;</span><span class="sxs-lookup"><span data-stu-id="ca080-215">FiscalYearStartDate@1011 : Date;</span></span>|<span data-ttu-id="ca080-216">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-216">Unchanged</span></span>|  
|<span data-ttu-id="ca080-217">NextEntryNo@1055 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-217">NextEntryNo@1055 : Integer;</span></span>|<span data-ttu-id="ca080-218">NextEntryNo@1022 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-218">NextEntryNo@1022 : Integer;</span></span>|<span data-ttu-id="ca080-219">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-219">Unchanged</span></span>|  
|<span data-ttu-id="ca080-220">BalanceCheckAmount@1056 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-220">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="ca080-221">BalanceCheckAmount@1056 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-221">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="ca080-222">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-222">Unchanged</span></span>|  
|<span data-ttu-id="ca080-223">BalanceCheckAmount2@1057 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-223">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="ca080-224">BalanceCheckAmount2@1057 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-224">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="ca080-225">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-225">Unchanged</span></span>|  
|<span data-ttu-id="ca080-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="ca080-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="ca080-228">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-228">Unchanged</span></span>|  
|<span data-ttu-id="ca080-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="ca080-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="ca080-231">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-231">Unchanged</span></span>|  
|<span data-ttu-id="ca080-232">CurrentBalance@1060 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-232">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="ca080-233">CurrentBalance@1060 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-233">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="ca080-234">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-234">Unchanged</span></span>|  
|<span data-ttu-id="ca080-235">SalesTaxBaseAmount@1061 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-235">SalesTaxBaseAmount@1061 : Decimal;</span></span>||<span data-ttu-id="ca080-236">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-236">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-237">TotalAddCurrAmount@1062 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-237">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="ca080-238">TotalAddCurrAmount@1062 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-238">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="ca080-239">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-239">Unchanged</span></span>|  
|<span data-ttu-id="ca080-240">TotalAmount@1063 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-240">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="ca080-241">TotalAmount@1063 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-241">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="ca080-242">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-242">Unchanged</span></span>|  
|<span data-ttu-id="ca080-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="ca080-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="ca080-245">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-245">Unchanged</span></span>|  
|<span data-ttu-id="ca080-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="ca080-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="ca080-248">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-248">Unchanged</span></span>|  
|<span data-ttu-id="ca080-249">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-249">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="ca080-250">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-250">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="ca080-251">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-251">Unchanged</span></span>|  
|<span data-ttu-id="ca080-252">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-252">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="ca080-253">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-253">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="ca080-254">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-254">Unchanged</span></span>|  
|<span data-ttu-id="ca080-255">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-255">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="ca080-256">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-256">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="ca080-257">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-257">Unchanged</span></span>|  
|<span data-ttu-id="ca080-258">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-258">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="ca080-259">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-259">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="ca080-260">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-260">Unchanged</span></span>|  
|<span data-ttu-id="ca080-261">InsertedTempGLEntryVAT@1068 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-261">InsertedTempGLEntryVAT@1068 : Integer;</span></span>|<span data-ttu-id="ca080-262">InsertedTempGLEntryVAT@1027 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-262">InsertedTempGLEntryVAT@1027 : Integer;</span></span>|<span data-ttu-id="ca080-263">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-263">Unchanged</span></span>|  
|<span data-ttu-id="ca080-264">LastDocNo@1069 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="ca080-264">LastDocNo@1069 : Code[20];</span></span>|<span data-ttu-id="ca080-265">LastDocNo@1023 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="ca080-265">LastDocNo@1023 : Code[20];</span></span>|<span data-ttu-id="ca080-266">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-266">Unchanged</span></span>|  
|<span data-ttu-id="ca080-267">LastLineNo@1070 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-267">LastLineNo@1070 : Integer;</span></span>||<span data-ttu-id="ca080-268">Deleted</span><span class="sxs-lookup"><span data-stu-id="ca080-268">Deleted</span></span>|  
|<span data-ttu-id="ca080-269">LastDate@1071 : Date;</span><span class="sxs-lookup"><span data-stu-id="ca080-269">LastDate@1071 : Date;</span></span>|<span data-ttu-id="ca080-270">LastDate@1021 : Date;</span><span class="sxs-lookup"><span data-stu-id="ca080-270">LastDate@1021 : Date;</span></span>|<span data-ttu-id="ca080-271">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-271">Unchanged</span></span>|  
|<span data-ttu-id="ca080-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span><span class="sxs-lookup"><span data-stu-id="ca080-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="ca080-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span><span class="sxs-lookup"><span data-stu-id="ca080-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="ca080-274">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-274">Unchanged</span></span>|  
|<span data-ttu-id="ca080-275">NextCheckEntryNo@1073 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-275">NextCheckEntryNo@1073 : Integer;</span></span>|<span data-ttu-id="ca080-276">NextCheckEntryNo@1028 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-276">NextCheckEntryNo@1028 : Integer;</span></span>|<span data-ttu-id="ca080-277">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-277">Unchanged</span></span>|  
|<span data-ttu-id="ca080-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span></span>|<span data-ttu-id="ca080-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span></span>|<span data-ttu-id="ca080-280">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-280">Unchanged</span></span>|  
|<span data-ttu-id="ca080-281">CurrencyDate@1076 : Date;</span><span class="sxs-lookup"><span data-stu-id="ca080-281">CurrencyDate@1076 : Date;</span></span>|<span data-ttu-id="ca080-282">CurrencyDate@1020 : Date;</span><span class="sxs-lookup"><span data-stu-id="ca080-282">CurrencyDate@1020 : Date;</span></span>|<span data-ttu-id="ca080-283">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-283">Unchanged</span></span>|  
|<span data-ttu-id="ca080-284">CurrencyFactor@1077 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-284">CurrencyFactor@1077 : Decimal;</span></span>|<span data-ttu-id="ca080-285">CurrencyFactor@1019 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-285">CurrencyFactor@1019 : Decimal;</span></span>|<span data-ttu-id="ca080-286">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-286">Unchanged</span></span>|  
|<span data-ttu-id="ca080-287">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-287">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="ca080-288">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-288">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="ca080-289">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-289">Unchanged</span></span>|  
|<span data-ttu-id="ca080-290">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-290">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="ca080-291">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-291">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="ca080-292">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-292">Unchanged</span></span>|  
|<span data-ttu-id="ca080-293">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-293">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="ca080-294">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-294">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="ca080-295">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-295">Unchanged</span></span>|  
|<span data-ttu-id="ca080-296">AllApplied@1081 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-296">AllApplied@1081 : Boolean;</span></span>||<span data-ttu-id="ca080-297">Changed to Local</span><span class="sxs-lookup"><span data-stu-id="ca080-297">Changed to Local</span></span>|  
|<span data-ttu-id="ca080-298">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-298">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="ca080-299">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-299">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="ca080-300">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-300">Unchanged</span></span>|  
|<span data-ttu-id="ca080-301">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-301">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="ca080-302">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-302">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="ca080-303">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-303">Unchanged</span></span>|  
|<span data-ttu-id="ca080-304">Prepayment@1037 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-304">Prepayment@1037 : Boolean;</span></span>||<span data-ttu-id="ca080-305">Deleted</span><span class="sxs-lookup"><span data-stu-id="ca080-305">Deleted</span></span>|  
|<span data-ttu-id="ca080-306">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-306">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="ca080-307">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-307">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="ca080-308">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-308">Unchanged</span></span>|  
|<span data-ttu-id="ca080-309">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-309">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="ca080-310">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-310">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="ca080-311">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-311">Unchanged</span></span>|  
|<span data-ttu-id="ca080-312">GLEntryNo@1090 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-312">GLEntryNo@1090 : Integer;</span></span>|<span data-ttu-id="ca080-313">GLEntryNo@1026 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-313">GLEntryNo@1026 : Integer;</span></span>|<span data-ttu-id="ca080-314">Unchanged</span><span class="sxs-lookup"><span data-stu-id="ca080-314">Unchanged</span></span>|  
||<span data-ttu-id="ca080-315">GLSetupRead@1015 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="ca080-315">GLSetupRead@1015 : Boolean;</span></span>|<span data-ttu-id="ca080-316">Added</span><span class="sxs-lookup"><span data-stu-id="ca080-316">Added</span></span>|  
||<span data-ttu-id="ca080-317">AmountRoundingPrecision@1012 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="ca080-317">AmountRoundingPrecision@1012 : Decimal;</span></span>|<span data-ttu-id="ca080-318">Added</span><span class="sxs-lookup"><span data-stu-id="ca080-318">Added</span></span>|  
||<span data-ttu-id="ca080-319">CrCardTransactionEntryNo@1013 : Integer;</span><span class="sxs-lookup"><span data-stu-id="ca080-319">CrCardTransactionEntryNo@1013 : Integer;</span></span>|<span data-ttu-id="ca080-320">Added</span><span class="sxs-lookup"><span data-stu-id="ca080-320">Added</span></span>|  

## <a name="see-also"></a><span data-ttu-id="ca080-321">See Also</span><span class="sxs-lookup"><span data-stu-id="ca080-321">See Also</span></span>  
 [<span data-ttu-id="ca080-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="ca080-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)
