---
title: Design Details - Accounts in the General Ledger | Microsoft Docs
description: To reconcile inventory and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger.
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: a9d313a4fee3dedf74cc2f0c635516397e26d8ef
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-accounts-in-the-general-ledger"></a><span data-ttu-id="7076b-103">Design Details: Accounts in the General Ledger</span><span class="sxs-lookup"><span data-stu-id="7076b-103">Design Details: Accounts in the General Ledger</span></span>
<span data-ttu-id="7076b-104">To reconcile inventory and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="7076b-104">To reconcile inventory and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger.</span></span> <span data-ttu-id="7076b-105">For more information, see [Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="7076b-105">For more information, see [Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md).</span></span>  

## <a name="from-the-inventory-ledger"></a><span data-ttu-id="7076b-106">From the Inventory Ledger</span><span class="sxs-lookup"><span data-stu-id="7076b-106">From the Inventory Ledger</span></span>  
<span data-ttu-id="7076b-107">The following table shows the relationship between different types of inventory value entries and the accounts and balancing accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="7076b-107">The following table shows the relationship between different types of inventory value entries and the accounts and balancing accounts in the general ledger.</span></span>  

|<span data-ttu-id="7076b-108">**Item Ledger Entry Type**</span><span class="sxs-lookup"><span data-stu-id="7076b-108">**Item Ledger Entry Type**</span></span>|<span data-ttu-id="7076b-109">**Value Entry Ttype**</span><span class="sxs-lookup"><span data-stu-id="7076b-109">**Value Entry Ttype**</span></span>|<span data-ttu-id="7076b-110">**Variance Type**</span><span class="sxs-lookup"><span data-stu-id="7076b-110">**Variance Type**</span></span>|<span data-ttu-id="7076b-111">**Expected Cost**</span><span class="sxs-lookup"><span data-stu-id="7076b-111">**Expected Cost**</span></span>|<span data-ttu-id="7076b-112">**Account**</span><span class="sxs-lookup"><span data-stu-id="7076b-112">**Account**</span></span>|<span data-ttu-id="7076b-113">**Balancing Account**</span><span class="sxs-lookup"><span data-stu-id="7076b-113">**Balancing Account**</span></span>|  
|--------------------------------|--------------------------|-----------------------|-----------------------|-----------------|---------------------------|  
|<span data-ttu-id="7076b-114">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-114">Purchase</span></span>|<span data-ttu-id="7076b-115">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-115">Direct Cost</span></span>||<span data-ttu-id="7076b-116">Yes</span><span class="sxs-lookup"><span data-stu-id="7076b-116">Yes</span></span>|<span data-ttu-id="7076b-117">Inventory  (Interim)</span><span class="sxs-lookup"><span data-stu-id="7076b-117">Inventory  (Interim)</span></span>|<span data-ttu-id="7076b-118">Invt. Accrual Acc. (Interim)</span><span class="sxs-lookup"><span data-stu-id="7076b-118">Invt. Accrual Acc. (Interim)</span></span>|  
|<span data-ttu-id="7076b-119">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-119">Purchase</span></span>|<span data-ttu-id="7076b-120">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-120">Direct Cost</span></span>||<span data-ttu-id="7076b-121">No</span><span class="sxs-lookup"><span data-stu-id="7076b-121">No</span></span>|<span data-ttu-id="7076b-122">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-122">Inventory</span></span>|<span data-ttu-id="7076b-123">Direct Cost Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-123">Direct Cost Applied</span></span>|  
|<span data-ttu-id="7076b-124">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-124">Purchase</span></span>|<span data-ttu-id="7076b-125">Indirect Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-125">Indirect Cost</span></span>||<span data-ttu-id="7076b-126">No</span><span class="sxs-lookup"><span data-stu-id="7076b-126">No</span></span>|<span data-ttu-id="7076b-127">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-127">Inventory</span></span>|<span data-ttu-id="7076b-128">Overhead Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-128">Overhead Applied</span></span>|  
|<span data-ttu-id="7076b-129">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-129">Purchase</span></span>|<span data-ttu-id="7076b-130">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-130">Variance</span></span>|<span data-ttu-id="7076b-131">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-131">Purchase</span></span>|<span data-ttu-id="7076b-132">No</span><span class="sxs-lookup"><span data-stu-id="7076b-132">No</span></span>|<span data-ttu-id="7076b-133">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-133">Inventory</span></span>|<span data-ttu-id="7076b-134">Purchase Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-134">Purchase Variance</span></span>|  
|<span data-ttu-id="7076b-135">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-135">Purchase</span></span>|<span data-ttu-id="7076b-136">Revaluation</span><span class="sxs-lookup"><span data-stu-id="7076b-136">Revaluation</span></span>||<span data-ttu-id="7076b-137">No</span><span class="sxs-lookup"><span data-stu-id="7076b-137">No</span></span>|<span data-ttu-id="7076b-138">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-138">Inventory</span></span>|<span data-ttu-id="7076b-139">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-139">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-140">Purchase</span><span class="sxs-lookup"><span data-stu-id="7076b-140">Purchase</span></span>|<span data-ttu-id="7076b-141">Rounding</span><span class="sxs-lookup"><span data-stu-id="7076b-141">Rounding</span></span>||<span data-ttu-id="7076b-142">No</span><span class="sxs-lookup"><span data-stu-id="7076b-142">No</span></span>|<span data-ttu-id="7076b-143">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-143">Inventory</span></span>|<span data-ttu-id="7076b-144">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-144">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-145">Sale</span><span class="sxs-lookup"><span data-stu-id="7076b-145">Sale</span></span>|<span data-ttu-id="7076b-146">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-146">Direct Cost</span></span>||<span data-ttu-id="7076b-147">Yes</span><span class="sxs-lookup"><span data-stu-id="7076b-147">Yes</span></span>|<span data-ttu-id="7076b-148">Inventory  (Interim)</span><span class="sxs-lookup"><span data-stu-id="7076b-148">Inventory  (Interim)</span></span>|<span data-ttu-id="7076b-149">COGS (Interim)</span><span class="sxs-lookup"><span data-stu-id="7076b-149">COGS (Interim)</span></span>|  
|<span data-ttu-id="7076b-150">Sale</span><span class="sxs-lookup"><span data-stu-id="7076b-150">Sale</span></span>|<span data-ttu-id="7076b-151">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-151">Direct Cost</span></span>||<span data-ttu-id="7076b-152">No</span><span class="sxs-lookup"><span data-stu-id="7076b-152">No</span></span>|<span data-ttu-id="7076b-153">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-153">Inventory</span></span>|<span data-ttu-id="7076b-154">COGS</span><span class="sxs-lookup"><span data-stu-id="7076b-154">COGS</span></span>|  
|<span data-ttu-id="7076b-155">Sale</span><span class="sxs-lookup"><span data-stu-id="7076b-155">Sale</span></span>|<span data-ttu-id="7076b-156">Revaluation</span><span class="sxs-lookup"><span data-stu-id="7076b-156">Revaluation</span></span>||<span data-ttu-id="7076b-157">No</span><span class="sxs-lookup"><span data-stu-id="7076b-157">No</span></span>|<span data-ttu-id="7076b-158">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-158">Inventory</span></span>|<span data-ttu-id="7076b-159">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-159">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-160">Sale</span><span class="sxs-lookup"><span data-stu-id="7076b-160">Sale</span></span>|<span data-ttu-id="7076b-161">Rounding</span><span class="sxs-lookup"><span data-stu-id="7076b-161">Rounding</span></span>||<span data-ttu-id="7076b-162">No</span><span class="sxs-lookup"><span data-stu-id="7076b-162">No</span></span>|<span data-ttu-id="7076b-163">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-163">Inventory</span></span>|<span data-ttu-id="7076b-164">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-164">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-165">Positive Adjmt.,Negative Adjmt., Transfer</span><span class="sxs-lookup"><span data-stu-id="7076b-165">Positive Adjmt.,Negative Adjmt., Transfer</span></span>|<span data-ttu-id="7076b-166">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-166">Direct Cost</span></span>||<span data-ttu-id="7076b-167">No</span><span class="sxs-lookup"><span data-stu-id="7076b-167">No</span></span>|<span data-ttu-id="7076b-168">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-168">Inventory</span></span>|<span data-ttu-id="7076b-169">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-169">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-170">Positive Adjmt.,Negative Adjmt., Transfer</span><span class="sxs-lookup"><span data-stu-id="7076b-170">Positive Adjmt.,Negative Adjmt., Transfer</span></span>|<span data-ttu-id="7076b-171">Revaluation</span><span class="sxs-lookup"><span data-stu-id="7076b-171">Revaluation</span></span>||<span data-ttu-id="7076b-172">No</span><span class="sxs-lookup"><span data-stu-id="7076b-172">No</span></span>|<span data-ttu-id="7076b-173">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-173">Inventory</span></span>|<span data-ttu-id="7076b-174">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-174">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-175">Positive Adjmt.,Negative Adjmt., Transfer</span><span class="sxs-lookup"><span data-stu-id="7076b-175">Positive Adjmt.,Negative Adjmt., Transfer</span></span>|<span data-ttu-id="7076b-176">Rounding</span><span class="sxs-lookup"><span data-stu-id="7076b-176">Rounding</span></span>||<span data-ttu-id="7076b-177">No</span><span class="sxs-lookup"><span data-stu-id="7076b-177">No</span></span>|<span data-ttu-id="7076b-178">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-178">Inventory</span></span>|<span data-ttu-id="7076b-179">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-179">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-180">(Production) Consumption</span><span class="sxs-lookup"><span data-stu-id="7076b-180">(Production) Consumption</span></span>|<span data-ttu-id="7076b-181">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-181">Direct Cost</span></span>||<span data-ttu-id="7076b-182">No</span><span class="sxs-lookup"><span data-stu-id="7076b-182">No</span></span>|<span data-ttu-id="7076b-183">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-183">Inventory</span></span>|<span data-ttu-id="7076b-184">WIP</span><span class="sxs-lookup"><span data-stu-id="7076b-184">WIP</span></span>|  
|<span data-ttu-id="7076b-185">(Production) Consumption</span><span class="sxs-lookup"><span data-stu-id="7076b-185">(Production) Consumption</span></span>|<span data-ttu-id="7076b-186">Revaluation</span><span class="sxs-lookup"><span data-stu-id="7076b-186">Revaluation</span></span>||<span data-ttu-id="7076b-187">No</span><span class="sxs-lookup"><span data-stu-id="7076b-187">No</span></span>|<span data-ttu-id="7076b-188">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-188">Inventory</span></span>|<span data-ttu-id="7076b-189">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-189">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-190">(Production) Consumption</span><span class="sxs-lookup"><span data-stu-id="7076b-190">(Production) Consumption</span></span>|<span data-ttu-id="7076b-191">Rounding</span><span class="sxs-lookup"><span data-stu-id="7076b-191">Rounding</span></span>||<span data-ttu-id="7076b-192">No</span><span class="sxs-lookup"><span data-stu-id="7076b-192">No</span></span>|<span data-ttu-id="7076b-193">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-193">Inventory</span></span>|<span data-ttu-id="7076b-194">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-194">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-195">Assembly Consumption</span><span class="sxs-lookup"><span data-stu-id="7076b-195">Assembly Consumption</span></span>|<span data-ttu-id="7076b-196">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-196">Direct Cost</span></span>||<span data-ttu-id="7076b-197">No</span><span class="sxs-lookup"><span data-stu-id="7076b-197">No</span></span>|<span data-ttu-id="7076b-198">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-198">Inventory</span></span>|<span data-ttu-id="7076b-199">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-199">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-200">Assembly Consumption</span><span class="sxs-lookup"><span data-stu-id="7076b-200">Assembly Consumption</span></span>|<span data-ttu-id="7076b-201">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-201">Direct Cost</span></span>||<span data-ttu-id="7076b-202">No</span><span class="sxs-lookup"><span data-stu-id="7076b-202">No</span></span>|<span data-ttu-id="7076b-203">Direct Cost Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-203">Direct Cost Applied</span></span>|<span data-ttu-id="7076b-204">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-204">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-205">Assembly Consumption</span><span class="sxs-lookup"><span data-stu-id="7076b-205">Assembly Consumption</span></span>|<span data-ttu-id="7076b-206">Indirect Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-206">Indirect Cost</span></span>||<span data-ttu-id="7076b-207">No</span><span class="sxs-lookup"><span data-stu-id="7076b-207">No</span></span>|<span data-ttu-id="7076b-208">Overhead Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-208">Overhead Applied</span></span>|<span data-ttu-id="7076b-209">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-209">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-210">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-210">(Production) Output</span></span>|<span data-ttu-id="7076b-211">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-211">Direct Cost</span></span>||<span data-ttu-id="7076b-212">Yes</span><span class="sxs-lookup"><span data-stu-id="7076b-212">Yes</span></span>|<span data-ttu-id="7076b-213">Inventory  (Interim)</span><span class="sxs-lookup"><span data-stu-id="7076b-213">Inventory  (Interim)</span></span>|<span data-ttu-id="7076b-214">WIP</span><span class="sxs-lookup"><span data-stu-id="7076b-214">WIP</span></span>|  
|<span data-ttu-id="7076b-215">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-215">(Production) Output</span></span>|<span data-ttu-id="7076b-216">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-216">Direct Cost</span></span>||<span data-ttu-id="7076b-217">No</span><span class="sxs-lookup"><span data-stu-id="7076b-217">No</span></span>|<span data-ttu-id="7076b-218">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-218">Inventory</span></span>|<span data-ttu-id="7076b-219">WIP</span><span class="sxs-lookup"><span data-stu-id="7076b-219">WIP</span></span>|  
|<span data-ttu-id="7076b-220">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-220">(Production) Output</span></span>|<span data-ttu-id="7076b-221">Indirect Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-221">Indirect Cost</span></span>||<span data-ttu-id="7076b-222">No</span><span class="sxs-lookup"><span data-stu-id="7076b-222">No</span></span>|<span data-ttu-id="7076b-223">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-223">Inventory</span></span>|<span data-ttu-id="7076b-224">Overhead Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-224">Overhead Applied</span></span>|  
|<span data-ttu-id="7076b-225">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-225">(Production) Output</span></span>|<span data-ttu-id="7076b-226">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-226">Variance</span></span>|<span data-ttu-id="7076b-227">Material</span><span class="sxs-lookup"><span data-stu-id="7076b-227">Material</span></span>|<span data-ttu-id="7076b-228">No</span><span class="sxs-lookup"><span data-stu-id="7076b-228">No</span></span>|<span data-ttu-id="7076b-229">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-229">Inventory</span></span>|<span data-ttu-id="7076b-230">Material Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-230">Material Variance</span></span>|  
|<span data-ttu-id="7076b-231">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-231">(Production) Output</span></span>|<span data-ttu-id="7076b-232">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-232">Variance</span></span>|<span data-ttu-id="7076b-233">Capacity</span><span class="sxs-lookup"><span data-stu-id="7076b-233">Capacity</span></span>|<span data-ttu-id="7076b-234">No</span><span class="sxs-lookup"><span data-stu-id="7076b-234">No</span></span>|<span data-ttu-id="7076b-235">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-235">Inventory</span></span>|<span data-ttu-id="7076b-236">Capacity Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-236">Capacity Variance</span></span>|  
|<span data-ttu-id="7076b-237">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-237">(Production) Output</span></span>|<span data-ttu-id="7076b-238">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-238">Variance</span></span>|<span data-ttu-id="7076b-239">Subcontracted</span><span class="sxs-lookup"><span data-stu-id="7076b-239">Subcontracted</span></span>|<span data-ttu-id="7076b-240">No</span><span class="sxs-lookup"><span data-stu-id="7076b-240">No</span></span>|<span data-ttu-id="7076b-241">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-241">Inventory</span></span>|<span data-ttu-id="7076b-242">Subcontracted Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-242">Subcontracted Variance</span></span>|  
|<span data-ttu-id="7076b-243">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-243">(Production) Output</span></span>|<span data-ttu-id="7076b-244">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-244">Variance</span></span>|<span data-ttu-id="7076b-245">Capacity Overhead</span><span class="sxs-lookup"><span data-stu-id="7076b-245">Capacity Overhead</span></span>|<span data-ttu-id="7076b-246">No</span><span class="sxs-lookup"><span data-stu-id="7076b-246">No</span></span>|<span data-ttu-id="7076b-247">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-247">Inventory</span></span>|<span data-ttu-id="7076b-248">Cap. Overhead Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-248">Cap. Overhead Variance</span></span>|  
|<span data-ttu-id="7076b-249">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-249">(Production) Output</span></span>|<span data-ttu-id="7076b-250">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-250">Variance</span></span>|<span data-ttu-id="7076b-251">Manufacturing Overhead</span><span class="sxs-lookup"><span data-stu-id="7076b-251">Manufacturing Overhead</span></span>|<span data-ttu-id="7076b-252">No</span><span class="sxs-lookup"><span data-stu-id="7076b-252">No</span></span>|<span data-ttu-id="7076b-253">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-253">Inventory</span></span>|<span data-ttu-id="7076b-254">Mfg. Overhead Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-254">Mfg. Overhead Variance</span></span>|  
|<span data-ttu-id="7076b-255">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-255">(Production) Output</span></span>|<span data-ttu-id="7076b-256">Revaluation</span><span class="sxs-lookup"><span data-stu-id="7076b-256">Revaluation</span></span>||<span data-ttu-id="7076b-257">No</span><span class="sxs-lookup"><span data-stu-id="7076b-257">No</span></span>|<span data-ttu-id="7076b-258">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-258">Inventory</span></span>|<span data-ttu-id="7076b-259">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-259">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-260">(Production) Output</span><span class="sxs-lookup"><span data-stu-id="7076b-260">(Production) Output</span></span>|<span data-ttu-id="7076b-261">Rounding</span><span class="sxs-lookup"><span data-stu-id="7076b-261">Rounding</span></span>||<span data-ttu-id="7076b-262">No</span><span class="sxs-lookup"><span data-stu-id="7076b-262">No</span></span>|<span data-ttu-id="7076b-263">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-263">Inventory</span></span>|<span data-ttu-id="7076b-264">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-264">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-265">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-265">Assembly Output</span></span>|<span data-ttu-id="7076b-266">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-266">Direct Cost</span></span>||<span data-ttu-id="7076b-267">No</span><span class="sxs-lookup"><span data-stu-id="7076b-267">No</span></span>|<span data-ttu-id="7076b-268">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-268">Inventory</span></span>|<span data-ttu-id="7076b-269">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-269">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-270">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-270">Assembly Output</span></span>|<span data-ttu-id="7076b-271">Revaluation</span><span class="sxs-lookup"><span data-stu-id="7076b-271">Revaluation</span></span>||<span data-ttu-id="7076b-272">No</span><span class="sxs-lookup"><span data-stu-id="7076b-272">No</span></span>|<span data-ttu-id="7076b-273">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-273">Inventory</span></span>|<span data-ttu-id="7076b-274">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-274">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-275">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-275">Assembly Output</span></span>|<span data-ttu-id="7076b-276">Indirect Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-276">Indirect Cost</span></span>||<span data-ttu-id="7076b-277">No</span><span class="sxs-lookup"><span data-stu-id="7076b-277">No</span></span>|<span data-ttu-id="7076b-278">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-278">Inventory</span></span>|<span data-ttu-id="7076b-279">Overhead Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-279">Overhead Applied</span></span>|  
|<span data-ttu-id="7076b-280">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-280">Assembly Output</span></span>|<span data-ttu-id="7076b-281">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-281">Variance</span></span>|<span data-ttu-id="7076b-282">Material</span><span class="sxs-lookup"><span data-stu-id="7076b-282">Material</span></span>|<span data-ttu-id="7076b-283">No</span><span class="sxs-lookup"><span data-stu-id="7076b-283">No</span></span>|<span data-ttu-id="7076b-284">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-284">Inventory</span></span>|<span data-ttu-id="7076b-285">Material Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-285">Material Variance</span></span>|  
|<span data-ttu-id="7076b-286">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-286">Assembly Output</span></span>|<span data-ttu-id="7076b-287">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-287">Variance</span></span>|<span data-ttu-id="7076b-288">Capacity</span><span class="sxs-lookup"><span data-stu-id="7076b-288">Capacity</span></span>|<span data-ttu-id="7076b-289">No</span><span class="sxs-lookup"><span data-stu-id="7076b-289">No</span></span>|<span data-ttu-id="7076b-290">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-290">Inventory</span></span>|<span data-ttu-id="7076b-291">Capacity Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-291">Capacity Variance</span></span>|  
|<span data-ttu-id="7076b-292">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-292">Assembly Output</span></span>|<span data-ttu-id="7076b-293">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-293">Variance</span></span>|<span data-ttu-id="7076b-294">Capacity Overhead</span><span class="sxs-lookup"><span data-stu-id="7076b-294">Capacity Overhead</span></span>|<span data-ttu-id="7076b-295">No</span><span class="sxs-lookup"><span data-stu-id="7076b-295">No</span></span>|<span data-ttu-id="7076b-296">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-296">Inventory</span></span>|<span data-ttu-id="7076b-297">Cap. Overhead Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-297">Cap. Overhead Variance</span></span>|  
|<span data-ttu-id="7076b-298">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-298">Assembly Output</span></span>|<span data-ttu-id="7076b-299">Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-299">Variance</span></span>|<span data-ttu-id="7076b-300">Manufacturing Overhead</span><span class="sxs-lookup"><span data-stu-id="7076b-300">Manufacturing Overhead</span></span>|<span data-ttu-id="7076b-301">No</span><span class="sxs-lookup"><span data-stu-id="7076b-301">No</span></span>|<span data-ttu-id="7076b-302">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-302">Inventory</span></span>|<span data-ttu-id="7076b-303">Mfg. Overhead Variance</span><span class="sxs-lookup"><span data-stu-id="7076b-303">Mfg. Overhead Variance</span></span>|  
|<span data-ttu-id="7076b-304">Assembly Output</span><span class="sxs-lookup"><span data-stu-id="7076b-304">Assembly Output</span></span>|<span data-ttu-id="7076b-305">Rounding</span><span class="sxs-lookup"><span data-stu-id="7076b-305">Rounding</span></span>||<span data-ttu-id="7076b-306">No</span><span class="sxs-lookup"><span data-stu-id="7076b-306">No</span></span>|<span data-ttu-id="7076b-307">Qty. on Hand</span><span class="sxs-lookup"><span data-stu-id="7076b-307">Inventory</span></span>|<span data-ttu-id="7076b-308">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-308">Inventory Adjmt.</span></span>|  

## <a name="from-the-capacity-ledger"></a><span data-ttu-id="7076b-309">From the Capacity Ledger</span><span class="sxs-lookup"><span data-stu-id="7076b-309">From the Capacity Ledger</span></span>  
 <span data-ttu-id="7076b-310">The following table shows the relationship between different types of capacity value entries and the accounts and balancing accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="7076b-310">The following table shows the relationship between different types of capacity value entries and the accounts and balancing accounts in the general ledger.</span></span> <span data-ttu-id="7076b-311">Capacity ledger entries represent labour time consumed in assembly or production work.</span><span class="sxs-lookup"><span data-stu-id="7076b-311">Capacity ledger entries represent labor time consumed in assembly or production work.</span></span>  

|<span data-ttu-id="7076b-312">**Work Type**</span><span class="sxs-lookup"><span data-stu-id="7076b-312">**Work Type**</span></span>|<span data-ttu-id="7076b-313">**Capacity Ledger Entry Type**</span><span class="sxs-lookup"><span data-stu-id="7076b-313">**Capacity Ledger Entry Type**</span></span>|<span data-ttu-id="7076b-314">**Value Entry Type**</span><span class="sxs-lookup"><span data-stu-id="7076b-314">**Value Entry Type**</span></span>|<span data-ttu-id="7076b-315">**Account**</span><span class="sxs-lookup"><span data-stu-id="7076b-315">**Account**</span></span>|<span data-ttu-id="7076b-316">**Balancing Account**</span><span class="sxs-lookup"><span data-stu-id="7076b-316">**Balancing Account**</span></span>|  
|-------------------|------------------------------------|--------------------------|-----------------|---------------------------|  
|<span data-ttu-id="7076b-317">Assembly</span><span class="sxs-lookup"><span data-stu-id="7076b-317">Assembly</span></span>|<span data-ttu-id="7076b-318">Resource</span><span class="sxs-lookup"><span data-stu-id="7076b-318">Resource</span></span>|<span data-ttu-id="7076b-319">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-319">Direct Cost</span></span>|<span data-ttu-id="7076b-320">Direct Cost Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-320">Direct Cost Applied</span></span>|<span data-ttu-id="7076b-321">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-321">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-322">Assembly</span><span class="sxs-lookup"><span data-stu-id="7076b-322">Assembly</span></span>|<span data-ttu-id="7076b-323">Resource</span><span class="sxs-lookup"><span data-stu-id="7076b-323">Resource</span></span>|<span data-ttu-id="7076b-324">Indirect Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-324">Indirect Cost</span></span>|<span data-ttu-id="7076b-325">Overhead Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-325">Overhead Applied</span></span>|<span data-ttu-id="7076b-326">Inventory Adjmt.</span><span class="sxs-lookup"><span data-stu-id="7076b-326">Inventory Adjmt.</span></span>|  
|<span data-ttu-id="7076b-327">Production</span><span class="sxs-lookup"><span data-stu-id="7076b-327">Production</span></span>|<span data-ttu-id="7076b-328">Machine Centre/Work Centre</span><span class="sxs-lookup"><span data-stu-id="7076b-328">Machine Center/Work Center</span></span>|<span data-ttu-id="7076b-329">Direct Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-329">Direct Cost</span></span>|<span data-ttu-id="7076b-330">WIP Account</span><span class="sxs-lookup"><span data-stu-id="7076b-330">WIP Account</span></span>|<span data-ttu-id="7076b-331">Direct Cost Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-331">Direct Cost Applied</span></span>|  
|<span data-ttu-id="7076b-332">Production</span><span class="sxs-lookup"><span data-stu-id="7076b-332">Production</span></span>|<span data-ttu-id="7076b-333">Machine Centre/Work Centre</span><span class="sxs-lookup"><span data-stu-id="7076b-333">Machine Center/Work Center</span></span>|<span data-ttu-id="7076b-334">Indirect Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-334">Indirect Cost</span></span>|<span data-ttu-id="7076b-335">WIP Account</span><span class="sxs-lookup"><span data-stu-id="7076b-335">WIP Account</span></span>|<span data-ttu-id="7076b-336">Overhead Applied</span><span class="sxs-lookup"><span data-stu-id="7076b-336">Overhead Applied</span></span>|  

## <a name="assembly-costs-are-always-actual"></a><span data-ttu-id="7076b-337">Assembly Costs are Always Actual</span><span class="sxs-lookup"><span data-stu-id="7076b-337">Assembly Costs are Always Actual</span></span>  
 <span data-ttu-id="7076b-338">As shown in the table above, assembly postings are not represented in interim accounts.</span><span class="sxs-lookup"><span data-stu-id="7076b-338">As shown in the table above, assembly postings are not represented in interim accounts.</span></span> <span data-ttu-id="7076b-339">This is because the concept of work in process (WIP) does not apply in assembly output posting, unlike in production output posting.</span><span class="sxs-lookup"><span data-stu-id="7076b-339">This is because the concept of work in process (WIP) does not apply in assembly output posting, unlike in production output posting.</span></span> <span data-ttu-id="7076b-340">Assembly costs are only posted as actual cost, never as expected cost.</span><span class="sxs-lookup"><span data-stu-id="7076b-340">Assembly costs are only posted as actual cost, never as expected cost.</span></span>  

 <span data-ttu-id="7076b-341">For more information, see [Design Details: Assembly Order Posting](design-details-assembly-order-posting.md).</span><span class="sxs-lookup"><span data-stu-id="7076b-341">For more information, see [Design Details: Assembly Order Posting](design-details-assembly-order-posting.md).</span></span>  

## <a name="calculating-the-amount-to-post-to-the-general-ledger"></a><span data-ttu-id="7076b-342">Calculating the Amount to Post to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="7076b-342">Calculating the Amount to Post to the General Ledger</span></span>  
 <span data-ttu-id="7076b-343">The following fields in the **Value Entry** table are used to calculate the expected cost amount that is posted to the general ledger:</span><span class="sxs-lookup"><span data-stu-id="7076b-343">The following fields in the **Value Entry** table are used to calculate the expected cost amount that is posted to the general ledger:</span></span>  

-   <span data-ttu-id="7076b-344">Cost Amount (Actual)</span><span class="sxs-lookup"><span data-stu-id="7076b-344">Cost Amount (Actual)</span></span>  
-   <span data-ttu-id="7076b-345">Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="7076b-345">Cost Posted to G/L</span></span>  
-   <span data-ttu-id="7076b-346">Cost Amount (Expected)</span><span class="sxs-lookup"><span data-stu-id="7076b-346">Cost Amount (Expected)</span></span>  
-   <span data-ttu-id="7076b-347">Expected Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="7076b-347">Expected Cost Posted to G/L</span></span>  

<span data-ttu-id="7076b-348">The following table shows how the amounts to post to the general ledger are calculated for the two different cost types.</span><span class="sxs-lookup"><span data-stu-id="7076b-348">The following table shows how the amounts to post to the general ledger are calculated for the two different cost types.</span></span>  

|<span data-ttu-id="7076b-349">Cost Type</span><span class="sxs-lookup"><span data-stu-id="7076b-349">Cost Type</span></span>|<span data-ttu-id="7076b-350">Calculation</span><span class="sxs-lookup"><span data-stu-id="7076b-350">Calculation</span></span>|  
|---------------|-----------------|  
|<span data-ttu-id="7076b-351">Actual Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-351">Actual Cost</span></span>|<span data-ttu-id="7076b-352">Cost Amount (Actual) – Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="7076b-352">Cost Amount (Actual) – Cost Posted to G/L</span></span>|  
|<span data-ttu-id="7076b-353">Expected Cost</span><span class="sxs-lookup"><span data-stu-id="7076b-353">Expected Cost</span></span>|<span data-ttu-id="7076b-354">Cost Amount (Expected) –  Expected Cost Posted to G/L</span><span class="sxs-lookup"><span data-stu-id="7076b-354">Cost Amount (Expected) –  Expected Cost Posted to G/L</span></span>|  

## <a name="see-also"></a><span data-ttu-id="7076b-355">See Also</span><span class="sxs-lookup"><span data-stu-id="7076b-355">See Also</span></span>  
 <span data-ttu-id="7076b-356">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="7076b-356">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="7076b-357">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span><span class="sxs-lookup"><span data-stu-id="7076b-357">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span></span>  
 [<span data-ttu-id="7076b-358">Design Details: Expected Cost Posting</span><span class="sxs-lookup"><span data-stu-id="7076b-358">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
 [<span data-ttu-id="7076b-359">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="7076b-359">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
 [<span data-ttu-id="7076b-360">Finance</span><span class="sxs-lookup"><span data-stu-id="7076b-360">Finance</span></span>](finance.md)  
 <span data-ttu-id="7076b-361">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7076b-361">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
