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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: c14ee9ecb06487aa08324fa10660c5094d1daa0b
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-unrealized-sales-tax-and-sales-payment-discounts"></a><span data-ttu-id="cc597-105">How to: Set Up Unrealized Sales Tax and Sales Payment Discounts</span><span class="sxs-lookup"><span data-stu-id="cc597-105">How to: Set Up Unrealized Sales Tax and Sales Payment Discounts</span></span>
<span data-ttu-id="cc597-106">You can use the **General Ledger Setup** window to set up unrealized sales tax.</span><span class="sxs-lookup"><span data-stu-id="cc597-106">You can use the **General Ledger Setup** window to set up unrealized sales tax.</span></span> <span data-ttu-id="cc597-107">You can also set up maximum correction tax amounts so that you can limit the tax correction amounts that are entered for sales and purchases.</span><span class="sxs-lookup"><span data-stu-id="cc597-107">You can also set up maximum correction tax amounts so that you can limit the tax correction amounts that are entered for sales and purchases.</span></span> <span data-ttu-id="cc597-108">This allows you to overwrite the calculated tax when there are rounding differences between what is calculated on the purchase order, and what is calculated on the purchase invoice from the vendor.</span><span class="sxs-lookup"><span data-stu-id="cc597-108">This allows you to overwrite the calculated tax when there are rounding differences between what is calculated on the purchase order, and what is calculated on the purchase invoice from the vendor.</span></span>  

## <a name="to-set-up-unrealized-sales-tax"></a><span data-ttu-id="cc597-109">To set up unrealized sales tax</span><span class="sxs-lookup"><span data-stu-id="cc597-109">To set up unrealized sales tax</span></span>  
1.  <span data-ttu-id="cc597-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc597-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cc597-111">In the **General Ledger Setup** window, on the **General** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="cc597-111">In the **General Ledger Setup** window, on the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cc597-112">Field</span><span class="sxs-lookup"><span data-stu-id="cc597-112">Field</span></span>|<span data-ttu-id="cc597-113">Description</span><span class="sxs-lookup"><span data-stu-id="cc597-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cc597-114">**Pmt. Disc. Excl. Tax**</span><span class="sxs-lookup"><span data-stu-id="cc597-114">**Pmt. Disc. Excl. Tax**</span></span>|<span data-ttu-id="cc597-115">Select to calculate the payment discount on amounts excluding sales tax.</span><span class="sxs-lookup"><span data-stu-id="cc597-115">Select to calculate the payment discount on amounts excluding sales tax.</span></span>|  
    |<span data-ttu-id="cc597-116">**Adjust for Payment Disc.**</span><span class="sxs-lookup"><span data-stu-id="cc597-116">**Adjust for Payment Disc.**</span></span>|<span data-ttu-id="cc597-117">Select to recalculate the tax amounts when you post payments that trigger payment discounts.</span><span class="sxs-lookup"><span data-stu-id="cc597-117">Select to recalculate the tax amounts when you post payments that trigger payment discounts.</span></span><br /><br /> <span data-ttu-id="cc597-118">This field is used in the context of Tax, not sales tax.</span><span class="sxs-lookup"><span data-stu-id="cc597-118">This field is used in the context of VAT, not sales tax.</span></span>|  
    |<span data-ttu-id="cc597-119">**Unrealized Tax**</span><span class="sxs-lookup"><span data-stu-id="cc597-119">**Unrealized VAT**</span></span>|<span data-ttu-id="cc597-120">Select if any of your sales tax jurisdictions allow you to pay your sales tax after you have been paid.</span><span class="sxs-lookup"><span data-stu-id="cc597-120">Select if any of your sales tax jurisdictions allow you to pay your sales tax after you have been paid.</span></span> <span data-ttu-id="cc597-121">If you do not select this check box this function will be blocked for all sales tax jurisdictions.</span><span class="sxs-lookup"><span data-stu-id="cc597-121">If you do not select this check box this function will be blocked for all sales tax jurisdictions.</span></span>|  
3.  <span data-ttu-id="cc597-122">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc597-122">Choose the **OK** button.</span></span>  

## <a name="to-set-up-unrealized-tax-for-jurisdictions"></a><span data-ttu-id="cc597-123">To set up unrealized tax for jurisdictions</span><span class="sxs-lookup"><span data-stu-id="cc597-123">To set up unrealized tax for jurisdictions</span></span>  
1.  <span data-ttu-id="cc597-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Jurisdictions**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc597-124">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Jurisdictions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cc597-125">In the **Tax Jurisdictions** window, choose the **Edit List** action.</span><span class="sxs-lookup"><span data-stu-id="cc597-125">In the **Tax Jurisdictions** window, choose the **Edit List** action.</span></span>  
3.  <span data-ttu-id="cc597-126">Fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="cc597-126">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cc597-127">Field</span><span class="sxs-lookup"><span data-stu-id="cc597-127">Field</span></span>|<span data-ttu-id="cc597-128">Description</span><span class="sxs-lookup"><span data-stu-id="cc597-128">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cc597-129">**Unrealized Tax Type**</span><span class="sxs-lookup"><span data-stu-id="cc597-129">**Unrealized Tax Type**</span></span>|<span data-ttu-id="cc597-130"><Blank> – The unrealized tax feature is not used for this tax jurisdiction.</span><span class="sxs-lookup"><span data-stu-id="cc597-130"><Blank> – The unrealized tax feature is not used for this tax jurisdiction.</span></span><br /><br /> <span data-ttu-id="cc597-131">–or–</span><span class="sxs-lookup"><span data-stu-id="cc597-131">–or–</span></span><br /><br /> <span data-ttu-id="cc597-132">**Percentage** – Each payment covers both tax amounts and invoice amounts in proportion to the remaining invoice amount.</span><span class="sxs-lookup"><span data-stu-id="cc597-132">**Percentage** – Each payment covers both tax amounts and invoice amounts in proportion to the remaining invoice amount.</span></span> <span data-ttu-id="cc597-133">The paid tax amount is transferred from the unrealized tax account to the tax account.</span><span class="sxs-lookup"><span data-stu-id="cc597-133">The paid tax amount is transferred from the unrealized tax account to the tax account.</span></span><br /><br /> <span data-ttu-id="cc597-134">–or–</span><span class="sxs-lookup"><span data-stu-id="cc597-134">–or–</span></span><br /><br /> <span data-ttu-id="cc597-135">**First** – Payments cover the tax first, and then the invoice amount.</span><span class="sxs-lookup"><span data-stu-id="cc597-135">**First** – Payments cover the tax first, and then the invoice amount.</span></span><br /><br /> <span data-ttu-id="cc597-136">–or–</span><span class="sxs-lookup"><span data-stu-id="cc597-136">–or–</span></span><br /><br /> <span data-ttu-id="cc597-137">**Last** – Payments cover the invoice amount first, and then the tax amount.</span><span class="sxs-lookup"><span data-stu-id="cc597-137">**Last** – Payments cover the invoice amount first, and then the tax amount.</span></span> <span data-ttu-id="cc597-138">In this case, nothing will be transferred from the unrealized tax account to the tax account until the total invoice amount—exclusive of tax—has been paid.</span><span class="sxs-lookup"><span data-stu-id="cc597-138">In this case, nothing will be transferred from the unrealized tax account to the tax account until the total invoice amount—exclusive of tax—has been paid.</span></span><br /><br /> <span data-ttu-id="cc597-139">–or–</span><span class="sxs-lookup"><span data-stu-id="cc597-139">–or–</span></span><br /><br /> <span data-ttu-id="cc597-140">**First (Fully Paid)** – Payments cover the tax first, but nothing is transferred to the tax account until the full tax amount has been paid.</span><span class="sxs-lookup"><span data-stu-id="cc597-140">**First (Fully Paid)** – Payments cover the tax first, but nothing is transferred to the tax account until the full tax amount has been paid.</span></span><br /><br /> <span data-ttu-id="cc597-141">–or–</span><span class="sxs-lookup"><span data-stu-id="cc597-141">–or–</span></span><br /><br /> <span data-ttu-id="cc597-142">**Last (Fully Paid)** – Payments cover the invoice amount first, but nothing is transferred to the tax account until the full tax amount has been paid.</span><span class="sxs-lookup"><span data-stu-id="cc597-142">**Last (Fully Paid)** – Payments cover the invoice amount first, but nothing is transferred to the tax account until the full tax amount has been paid.</span></span> <span data-ttu-id="cc597-143">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="cc597-143">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="cc597-144">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="cc597-144">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |<span data-ttu-id="cc597-145">**Unreal. Tax Acc (Sales)**</span><span class="sxs-lookup"><span data-stu-id="cc597-145">**Unreal. Tax Acc (Sales)**</span></span>|<span data-ttu-id="cc597-146">The general ledger account that you want to use to post calculated unrealized tax on sales transactions.</span><span class="sxs-lookup"><span data-stu-id="cc597-146">The general ledger account that you want to use to post calculated unrealized tax on sales transactions.</span></span> <span data-ttu-id="cc597-147">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="cc597-147">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="cc597-148">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="cc597-148">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |<span data-ttu-id="cc597-149">**Unreal. Tax Acc (Purchases)**</span><span class="sxs-lookup"><span data-stu-id="cc597-149">**Unreal. Tax Acc (Purchases)**</span></span>|<span data-ttu-id="cc597-150">The general ledger account that you want to use to post calculated unrealized tax on purchase transactions.</span><span class="sxs-lookup"><span data-stu-id="cc597-150">The general ledger account that you want to use to post calculated unrealized tax on purchase transactions.</span></span> <span data-ttu-id="cc597-151">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="cc597-151">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="cc597-152">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="cc597-152">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |<span data-ttu-id="cc597-153">**Unreal. Rev. Charge (Purch.)**</span><span class="sxs-lookup"><span data-stu-id="cc597-153">**Unreal. Rev. Charge (Purch.)**</span></span>|<span data-ttu-id="cc597-154">The general ledger account that you want to use for posting calculated unrealized reverse-charge tax on purchase transactions.</span><span class="sxs-lookup"><span data-stu-id="cc597-154">The general ledger account that you want to use for posting calculated unrealized reverse-charge tax on purchase transactions.</span></span> <span data-ttu-id="cc597-155">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="cc597-155">**Important:**  This field is available in the **Tax Jurisdiction** window, but it is not shown by default.</span></span> <span data-ttu-id="cc597-156">To select the field, you must first add the column that shows this field.</span><span class="sxs-lookup"><span data-stu-id="cc597-156">To select the field, you must first add the column that shows this field.</span></span> [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
4.  <span data-ttu-id="cc597-157">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc597-157">Choose the **OK** button.</span></span>  

## <a name="to-set-up-adjustments-for-payment-discounts-in-a-tax-posting-group"></a><span data-ttu-id="cc597-158">To set up adjustments for payment discounts in a tax posting group</span><span class="sxs-lookup"><span data-stu-id="cc597-158">To set up adjustments for payment discounts in a tax posting group</span></span>  
1.  <span data-ttu-id="cc597-159">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Posting Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc597-159">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Posting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cc597-160">Choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="cc597-160">Choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="cc597-161">In the **Tax Posting Setup Card** window, select the **Adjust for Payment Discount** check box.</span><span class="sxs-lookup"><span data-stu-id="cc597-161">In the **Tax Posting Setup Card** window, select the **Adjust for Payment Discount** check box.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="cc597-162">This field is available in the **Tax Posting Setup** window, but it is not shown by default.</span><span class="sxs-lookup"><span data-stu-id="cc597-162">This field is available in the **VAT Posting Setup** window, but it is not shown by default.</span></span>
4.  <span data-ttu-id="cc597-163">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc597-163">Choose the **OK** button.</span></span>  

## <a name="to-set-up-maximum-tax-correction-amounts"></a><span data-ttu-id="cc597-164">To set up maximum tax correction amounts</span><span class="sxs-lookup"><span data-stu-id="cc597-164">To set up maximum tax correction amounts</span></span>  
1.  <span data-ttu-id="cc597-165">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc597-165">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cc597-166">In the **Sales Receivables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span><span class="sxs-lookup"><span data-stu-id="cc597-166">In the **Sales Receivables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span></span>  
3.  <span data-ttu-id="cc597-167">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc597-167">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="cc597-168">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc597-168">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
5.  <span data-ttu-id="cc597-169">In the **Purchases & Payables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span><span class="sxs-lookup"><span data-stu-id="cc597-169">In the **Purchases & Payables Setup** window, on the **General** FastTab, select the **Allow Tax Difference** check box.</span></span>  
6.  <span data-ttu-id="cc597-170">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc597-170">Choose the **OK** button.</span></span>  
7.  <span data-ttu-id="cc597-171">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc597-171">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
8.  <span data-ttu-id="cc597-172">In the **General Ledger Setup** window, in the **Max. Tax Difference Allowed** field, enter the maximum tax correction amount that is allowed for the local currency.</span><span class="sxs-lookup"><span data-stu-id="cc597-172">In the **General Ledger Setup** window, in the **Max. Tax Difference Allowed** field, enter the maximum tax correction amount that is allowed for the local currency.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="cc597-173">In this field, if you enter CAD 5, you may correct tax amounts by up to five dollars.</span><span class="sxs-lookup"><span data-stu-id="cc597-173">In this field, if you enter USD 5, you may correct tax amounts by up to five dollars.</span></span> <span data-ttu-id="cc597-174">To use the tax difference function, an amount must be entered in the **Max. Tax Difference Allowed** field.</span><span class="sxs-lookup"><span data-stu-id="cc597-174">To use the tax difference function, an amount must be entered in the **Max. Tax Difference Allowed** field.</span></span>  
9. <span data-ttu-id="cc597-175">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc597-175">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cc597-176">See Also</span><span class="sxs-lookup"><span data-stu-id="cc597-176">See Also</span></span>  
[<span data-ttu-id="cc597-177">Canada Local Functionality</span><span class="sxs-lookup"><span data-stu-id="cc597-177">Canada Local Functionality</span></span>](canada-local-functionality.md)  
[<span data-ttu-id="cc597-178">Reporting Sales Tax in Canada</span><span class="sxs-lookup"><span data-stu-id="cc597-178">Reporting Sales Tax in Canada</span></span>](ca-sales-tax.md)  
[<span data-ttu-id="cc597-179">Finance</span><span class="sxs-lookup"><span data-stu-id="cc597-179">Finance</span></span>](../../finance.md)  
[<span data-ttu-id="cc597-180">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="cc597-180">Setting Up Finance</span></span>](../../finance.md)
