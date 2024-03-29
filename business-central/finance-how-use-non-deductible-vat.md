---
title: Use non-deductible GST/HST
description: This article explains how to use and report non-deductible GST/HST.
author: altotovi
ms.author: altotovi
ms.reviewer: null
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.search.keywords: 'VAT, non-deductible, return, settlement'
ms.search.form: '50, 51, 52, 161, 187, 317, 403, 6640, 9401'
ms.date: 04/26/2023
ms.custom: bap-template
---

# <a name="use-non-deductible-vat"></a>Use non-deductible GST/HST

This article explains how to use and report non-deductible GST/HST.

## <a name="create-a-purchase-invoice-with-non-deductible-vat"></a>Create a purchase invoice with non-deductible GST/HST

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then select the related link.
2. Select **New** to create a purchase invoice, and enter the appropriate information on the invoice header.
3. In the **Lines** section, create a new line of any type, based on the GST/HST business posting group and the GST/HST product posting group where you configure non-deductible GST/HST.
4. In the **Quantity** and **Direct Unit Cost** fields, enter appropriate values.

    If you selected the **Show Non-Ded. GST/HST In Lines** checkbox on the **GST/HST Setup** page, the amounts in the **Non-Deductible GST/HST Base** and **Non-Deductible GST/HST Amount** fields are calculated based on the **Non-Deductible GST/HST %** field on the **GST/HST Posting Setup** page.

5. Post the invoice.

## <a name="create-a-purchase-order-with-non-deductible-vat"></a>Create a purchase order with non-deductible GST/HST

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders** and then select the related link.
2. Select **New** to create a purchase order, and enter the appropriate information on the document header.
3. In the **Lines** section, create a new line of any type, based on the GST/HST business posting group and the GST/HST product posting group where you configure non-deductible GST/HST.
4. In the **Quantity** and **Direct Unit Cost** fields, enter appropriate values.

    If you selected the **Show Non-Ded. GST/HST In Lines** checkbox on the **GST/HST Setup** page, the amounts in the **Non-Deductible GST/HST Base** and **Non-Deductible GST/HST Amount** fields are calculated based on the **Non-Deductible GST/HST %** field on the **GST/HST Posting Setup** page.

5. Post the purchase order.

## <a name="adjust-rounded-vat-amounts-before-document-posting"></a>Adjust rounded GST/HST amounts before document posting

If GST/HST amounts aren't rounded in the same way in your environment and in the external accounting system (the original invoice document), you can adjust the GST/HST amount before you post the document. To make this adjustment, follow these steps before you post the document.

1. On the Action Pane, select **Statistic**.
2. If you're working with a purchase invoice, follow these steps:

    1. On the **Lines** FastTab, select the GST/HST amount or non-deductible GST/HST amount.
    2. Set the values that you need from the original document, and then close the **Purchase Invoice Statistics** page.

3.  If you're working with the purchase order, follow these steps:

    1. On the **Invoicing** FastTab, select **No. of Tax Lines** to open the **GST/HST Amounts Lines** page.
    2. Select the GST/HST amount or non-deductible GST/HST amount that you want to correct.
    3. Enter the values that you need from the original document, close the **GST/HST Amount lines** page, and then close the **Purchase Order Statistics** page.

To use adjustments of GST/HST amounts, you must enable the adjustments. On the **General Ledger Setup** page, in the **Max. GST/HST Difference Allowed** field, enter the maximum allowed GST/HST amount for correction. Then, on the **Purchases & Payables Setup** page, select **Allow GST/HST Difference**.

You can adjust the values of the **GST/HST Amount** and **Non-Deductible GST/HST Amount** fields. The value of the **Deductible GST/HST Amount** field is the result of these two values. The amount that you enter in the **Non-Deductible GST/HST Amount** field can't be more than the amount that you enter in the **GST/HST Amount** field. The **Max. GST/HST Difference Allowed** field on the **General Ledger Setup** page works independently for deductible and non-deductible GST/HST amounts on statistic pages when you want to adjust GST/HST amounts.

> [!IMPORTANT]
> You can't use non-deductible GST/HST on the prepayment invoices.

## <a name="see-also"></a>See also

[Financial Management](finance.md)

[Set Up Calculations and Posting Methods for GST/HST](finance-setup-vat.md)  

[Set up Non-deductible GST/HST](finance-setup-nondeductible-vat.md)

[Design details about non-deductible GST/HST](design-details-nondeductible-vat.md)

[Report VAT to Tax Authorities](finance-how-report-vat.md)

[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
