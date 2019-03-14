---
title: How to Set Up Unrealized Sales Tax and Sales Payment Discounts | Microsoft Docs
description: You can use the **General Ledger Setup** window to set up unrealized sales tax. You can also set up maximum correction tax amounts so that you can limit the tax correction amounts that are entered for sales and purchases. This allows you to overwrite the calculated tax when there are rounding differences between what is calculated on the purchase order, and what is calculated on the purchase invoice from the vendor.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: ac7bbcc95818646cdf8e3cb354bbce7673a5e43c
ms.contentlocale: en-ca
ms.lasthandoff: 04/16/2018

---
# <a name="set-up-unrealized-sales-tax-and-sales-payment-discounts"></a><span data-ttu-id="952ee-105">Set Up Unrealized Sales Tax and Sales Payment Discounts</span><span class="sxs-lookup"><span data-stu-id="952ee-105">Set Up Unrealized Sales Tax and Sales Payment Discounts</span></span>
<span data-ttu-id="952ee-106">You can use the **General Ledger Setup** window to set up unrealized sales tax.</span><span class="sxs-lookup"><span data-stu-id="952ee-106">You can use the **General Ledger Setup** window to set up unrealized sales tax.</span></span> <span data-ttu-id="952ee-107">You can also set up maximum correction tax amounts so that you can limit the tax correction amounts that are entered for sales and purchases.</span><span class="sxs-lookup"><span data-stu-id="952ee-107">You can also set up maximum correction tax amounts so that you can limit the tax correction amounts that are entered for sales and purchases.</span></span> <span data-ttu-id="952ee-108">This allows you to overwrite the calculated tax when there are rounding differences between what is calculated on the purchase order, and what is calculated on the purchase invoice from the vendor.</span><span class="sxs-lookup"><span data-stu-id="952ee-108">This allows you to overwrite the calculated tax when there are rounding differences between what is calculated on the purchase order, and what is calculated on the purchase invoice from the vendor.</span></span>  

## <a name="to-set-up-unrealized-sales-tax"></a><span data-ttu-id="952ee-109">To set up unrealized sales tax</span><span class="sxs-lookup"><span data-stu-id="952ee-109">To set up unrealized sales tax</span></span>  
1.  <span data-ttu-id="952ee-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="952ee-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="952ee-111">In the **General Ledger Setup** window, on the **General** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="952ee-111">In the **General Ledger Setup** window, on the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="952ee-112">Field</span><span class="sxs-lookup"><span data-stu-id="952ee-112">Field</span></span>|<span data-ttu-id="952ee-113">Description</span><span class="sxs-lookup"><span data-stu-id="952ee-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="952ee-114">**Pmt. Disc. Excl. Tax**</span><span class="sxs-lookup"><span data-stu-id="952ee-114">**Pmt. Disc. Excl. Tax**</span></span>|<span data-ttu-id="952ee-115">Select to calculate the payment discount on amounts excluding sales tax.</span><span class="sxs-lookup"><span data-stu-id="952ee-115">Select to calculate the payment discount on amounts excluding sales tax.</span></span>|  
    |<span data-ttu-id="952ee-116">**Adjust for Payment Disc.**</span><span class="sxs-lookup"><span data-stu-id="952ee-116">**Adjust for Payment Disc.**</span></span>|<span data-ttu-id="952ee-117">Select to recalculate the tax amounts when you post payments that trigger payment discounts.</span><span class="sxs-lookup"><span data-stu-id="952ee-117">Select to recalculate the tax amounts when you post payments that trigger payment discounts.</span></span><br /><br /> <span data-ttu-id="952ee-118">This field is used in the context of Tax, not sales tax.</span><span class="sxs-lookup"><span data-stu-id="952ee-118">This field is used in the context of VAT, not sales tax.</span></span>|  
    |<span data-ttu-id="952ee-119">**Unrealized Tax**</span><span class="sxs-lookup"><span data-stu-id="952ee-119">**Unrealized VAT**</span></span>|<span data-ttu-id="952ee-120">Select if any of your sales tax jurisdictions allow you to pay your sales tax after you have been paid.</span><span class="sxs-lookup"><span data-stu-id="952ee-120">Select if any of your sales tax jurisdictions allow you to pay your sales tax after you have been paid.</span></span> <span data-ttu-id="952ee-121">If you do not select this check box this function will be blocked for all sales tax jurisdictions.</span><span class="sxs-lookup"><span data-stu-id="952ee-121">If you do not select this check box this function will be blocked for all sales tax jurisdictions.</span></span>|  
3.  <span data-ttu-id="952ee-122">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="952ee-122">Choose the **OK** button.</span></span>  

## <a name="to-set-up-unrealized-tax-for-jurisdictions"></a><span data-ttu-id="952ee-123">To set up unrealized tax for jurisdictions</span><span class="sxs-lookup"><span data-stu-id="952ee-123">To set up unrealized tax for jurisdictions</span></span>  
1. <span data-ttu-id="952ee-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Jurisdictions**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="952ee-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Jurisdictions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="952ee-125">In the **Tax Jurisdictions** window, choose the **Edit List** action.</span><span class="sxs-lookup"><span data-stu-id="952ee-125">In the **Tax Jurisdictions** window, choose the **Edit List** action.</span></span>  
3. <span data-ttu-id="952ee-126">Fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="952ee-126">Fill in the fields as described in the following table.</span></span>  


   |              <span data-ttu-id="952ee-127">Field</span><span class="sxs-lookup"><span data-stu-id="952ee-127">Field</span></span>               |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      <span data-ttu-id="952ee-128">Description</span><span class="sxs-lookup"><span data-stu-id="952ee-128">Description</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
   |----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |     <span data-ttu-id="952ee-129">**Unrealized Tax Type**</span><span class="sxs-lookup"><span data-stu-id="952ee-129">**Unrealized Tax Type**</span></span>      | <span data-ttu-id="952ee-130"><Blank> – The unrealized tax feature is not used for this tax jurisdiction.</span><span class="sxs-lookup"><span data-stu-id="952ee-130"><Blank> – The unrealized tax feature is not used for this tax jurisdiction.</span></span><br /><br /> <span data-ttu-id="952ee-131">–or–</span><span class="sxs-lookup"><span data-stu-id="952ee-131">–or–</span></span><br /><br /> <span data-ttu-id="952ee-132">**Percentage** – Each payment covers both tax amounts and invoice amounts in proportion to the remaining invoice amount.</span><span class="sxs-lookup"><span data-stu-id="952ee-132">**Percentage** – Each payment covers both tax amounts and invoice amounts in proportion to the remaining invoice amount.</span></span> <span data-ttu-id="952ee-133">The paid tax amount is transferred from the unrealized tax account to the tax account.</span><span class="sxs-lookup"><span data-stu-id="952ee-133">The paid tax amount is transferred from the unrealized tax account to the tax account.</span></span><br /><br /> <span data-ttu-id="952ee-134">–or–</span><span class="sxs-lookup"><span data-stu-id="952ee-134">–or–</span></span><br /><br /> <span data-ttu-id="952ee-135">**First** – Payments cover the tax first, and then the invoice amount.</span><span class="sxs-lookup"><span data-stu-id="952ee-135">**First** – Payments cover the tax first, and then the invoice amount.</span></span><br /><br /> <span data-ttu-id="952ee-136">–or–</span><span class="sxs-lookup"><span data-stu-id="952ee-136">–or–</span></span><br /><br /> <span data-ttu-id="952ee-137">**Last** – Payments cover the invoice amount first, and then the tax amount.</span><span class="sxs-lookup"><span data-stu-id="952ee-137">**Last** – Payments cover the invoice amount first, and then the tax amount.</span></span> <span data-ttu-id="952ee-138">In this case, nothing will be transferred from the unrealized tax account to the tax account until the total invoice amount—exclusive of tax—has been paid.</span><span class="sxs-lookup"><span data-stu-id="952ee-138">In this case, nothing will be transferred from the unrealized tax account to the tax account until the total invoice amount—exclusive of tax—has been paid.</span></span><br /><br /> <span data-ttu-id="952ee-139">–or–</span><span class="sxs-lookup"><span data-stu-id="952ee-139">–or–</span></span><br /><br /> <span data-ttu-id="952ee-140">**First (Fully Paid)** – Payments cover the tax first, but nothing is transferred to the tax account until the full tax amount has been paid.</span><span class="sxs-lookup"><span data-stu-id="952ee-140">**First (Fully Paid)** – Payments cover the tax first, but nothing is transferred to the tax account until the full tax amount has been paid.</span></span><br /><br /> <span data-ttu-id="952ee-141">–or–</span><span class="sxs-lookup"><span data-stu-id="952ee-141">–or–</span></span><br /><br /> <span data-ttu-id="952ee-142">**Last (Fully Paid)** – Payments cover the invoice amount first, but nothing is transferred to the tax account until the full tax amount has been paid.</span><span class="sxs-lookup"><span data-stu-id="952ee-142">**Last (Fully Paid)** – Payments cover the invoice amount first, but nothing is transferred to the tax account until the full tax amount has been paid.</span></span> <span data-ttu-id="952ee-143">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="952ee-143">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="952ee-144">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="952ee-144">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE [bp_customize](../../includes/bp_customize_md.md)] |
   |   <span data-ttu-id="952ee-145">**Unreal. Tax Acc (Sales)**</span><span class="sxs-lookup"><span data-stu-id="952ee-145">**Unreal. Tax Acc (Sales)**</span></span>    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                              <span data-ttu-id="952ee-146">The general ledger account that you want to use to post calculated unrealized tax on sales transactions.</span><span class="sxs-lookup"><span data-stu-id="952ee-146">The general ledger account that you want to use to post calculated unrealized tax on sales transactions.</span></span> <span data-ttu-id="952ee-147">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="952ee-147">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="952ee-148">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="952ee-148">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE [bp_customize](../../includes/bp_customize_md.md)]                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
   | <span data-ttu-id="952ee-149">**Unreal. Tax Acc (Purchases)**</span><span class="sxs-lookup"><span data-stu-id="952ee-149">**Unreal. Tax Acc (Purchases)**</span></span>  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                            <span data-ttu-id="952ee-150">The general ledger account that you want to use to post calculated unrealized tax on purchase transactions.</span><span class="sxs-lookup"><span data-stu-id="952ee-150">The general ledger account that you want to use to post calculated unrealized tax on purchase transactions.</span></span> <span data-ttu-id="952ee-151">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="952ee-151">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="952ee-152">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="952ee-152">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE [bp_customize](../../includes/bp_customize_md.md)]                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
   | <span data-ttu-id="952ee-153">**Unreal. Rev. Charge (Purch.)**</span><span class="sxs-lookup"><span data-stu-id="952ee-153">**Unreal. Rev. Charge (Purch.)**</span></span> |                                                                                                                                                                                                                                                                                                                                                                                                                                                                   <span data-ttu-id="952ee-154">The general ledger account that you want to use for posting calculated unrealized reverse-charge tax on purchase transactions.</span><span class="sxs-lookup"><span data-stu-id="952ee-154">The general ledger account that you want to use for posting calculated unrealized reverse-charge tax on purchase transactions.</span></span> <span data-ttu-id="952ee-155">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="952ee-155">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="952ee-156">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="952ee-156">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE [bp_customize](../../includes/bp_customize_md.md)]                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |


4. <span data-ttu-id="952ee-157">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="952ee-157">Choose the **OK** button.</span></span>  

## <a name="to-set-up-adjustments-for-payment-discounts-in-a-tax-posting-group"></a><span data-ttu-id="952ee-158">To set up adjustments for payment discounts in a tax posting group</span><span class="sxs-lookup"><span data-stu-id="952ee-158">To set up adjustments for payment discounts in a tax posting group</span></span>  
1.  <span data-ttu-id="952ee-159">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Posting Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="952ee-159">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Posting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="952ee-160">Choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="952ee-160">Choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="952ee-161">In the **Tax Posting Setup Card** window, select the **Adjust for Payment Discount** check box.</span><span class="sxs-lookup"><span data-stu-id="952ee-161">In the **Tax Posting Setup Card** window, select the **Adjust for Payment Discount** check box.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="952ee-162">This field is available in the **Tax Posting Setup** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="952ee-162">This field is available in the **VAT Posting Setup** window, but it is not shown by default.</span></span>
4.  <span data-ttu-id="952ee-163">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="952ee-163">Choose the **OK** button.</span></span>  

## <a name="to-set-up-maximum-tax-correction-amounts"></a><span data-ttu-id="952ee-164">To set up maximum tax correction amounts</span><span class="sxs-lookup"><span data-stu-id="952ee-164">To set up maximum tax correction amounts</span></span>  
1.  <span data-ttu-id="952ee-165">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="952ee-165">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="952ee-166">In the **Sales Receivables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span><span class="sxs-lookup"><span data-stu-id="952ee-166">In the **Sales Receivables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span></span>  
3.  <span data-ttu-id="952ee-167">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="952ee-167">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="952ee-168">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="952ee-168">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
5.  <span data-ttu-id="952ee-169">In the **Purchases & Payables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span><span class="sxs-lookup"><span data-stu-id="952ee-169">In the **Purchases & Payables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span></span>  
6.  <span data-ttu-id="952ee-170">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="952ee-170">Choose the **OK** button.</span></span>  
7.  <span data-ttu-id="952ee-171">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="952ee-171">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
8.  <span data-ttu-id="952ee-172">In the **General Ledger Setup** window, in the **Max. Tax Difference Allowed** field, enter the maximum tax correction amount that is allowed for the local currency.</span><span class="sxs-lookup"><span data-stu-id="952ee-172">In the **General Ledger Setup** window, in the **Max. Tax Difference Allowed** field, enter the maximum tax correction amount that is allowed for the local currency.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="952ee-173">In this field, if you enter CAD 5, you may correct tax amounts by up to five dollars.</span><span class="sxs-lookup"><span data-stu-id="952ee-173">In this field, if you enter USD 5, you may correct tax amounts by up to five dollars.</span></span> <span data-ttu-id="952ee-174">To use the tax difference function, an amount must be entered in the **Max. Tax Difference Allowed** field.</span><span class="sxs-lookup"><span data-stu-id="952ee-174">To use the tax difference function, an amount must be entered in the **Max. Tax Difference Allowed** field.</span></span>  
9. <span data-ttu-id="952ee-175">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="952ee-175">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="952ee-176">See Also</span><span class="sxs-lookup"><span data-stu-id="952ee-176">See Also</span></span>  
[<span data-ttu-id="952ee-177">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="952ee-177">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="952ee-178">Reporting Sales Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="952ee-178">Reporting Sales Tax in Canada</span></span>](ca-sales-tax.md)  
[<span data-ttu-id="952ee-179">Finance</span><span class="sxs-lookup"><span data-stu-id="952ee-179">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="952ee-180">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="952ee-180">Setting Up Finance</span></span>](../../finance.md)
