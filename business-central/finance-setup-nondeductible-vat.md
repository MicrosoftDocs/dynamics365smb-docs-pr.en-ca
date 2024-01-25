---
title: Set up non-deductible GST/HST
description: This article explains how to configure non-deductible GST/HST in Microsoft Dynamics 365 Business Central.
author: altotovi
ms.author: altotovi
ms.reviewer: null
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.search.keywords: 'VAT, non-deductible, setup'
ms.search.form: '187, 472, 473'
ms.date: 04/26/2023
ms.custom: bap-template
---

# Set up non-deductible GST/HST

Non-deductible GST/HST is the GST/HST that's payable by a purchaser but that isn't deductible from the purchaser's own GST/HST liability. Companies can usually recover GST/HST on the purchase of goods and services that are related to their business activities. However, in some situations, a business incurs GST/HST that isn't deductible. These situations are typically related to the local regulations and can differ among countries/regions. However, the model of using non-deductible or partially deductible GST/HST is similar. You can use proportional GST/HST to calculate GST/HST when there's deductible and non-deductible GST/HST.

In general, GST/HST can't be deducted for some purchases because of the following factors:

- **The type of goods or services that are purchased** – GST/HST is fully or partially non-deductible by a provision of the law about goods such as cars, mobile phones, and food that's purchased at restaurants.
- **Partially deductible pro-rated GST/HST** – GST/HST is pro-rated according to the ratio between the sales operations that GST/HST is owed for and all operations that have been performed. GST/HST that exceeds this ratio can't be deducted.

Because it can be difficult to know where and how an item is used, you must contact the local tax authorities in your country/region to determine whether a specified percentage of the VAT is deductible based on historical data. 

> [!IMPORTANT]
> This global feature is available in all countries with enabled VAT **except for Belgium, Italy, and Norway**. These localizations already have existing local feature and will be upgraded in the future. Don't run this feature in these countries because the upgrade procedure doesn't exist.

## Use non-deductible GST/HST

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Setup**, and then select the related link.
2. Select the **Enable Non-Deductible GST/HST** checkbox.

    > [!IMPORTANT]
    > After you enable non-deductible GST/HST, you can't turn it off, because the feature might include changes to data and might initiate an upgrade of some database tables. Microsoft strongly recommends that you first enable and test this feature in the sandbox environment before you enable it in the production environment.

3. Configure how the system will treat non-deductible GST/HST values.

    1. In the **Use For Item Cost** field, specify whether the non-deductible GST/HST must be added to the item cost when you purchase items. Otherwise, the non-deductible GST/HST won't have an influence on the item cost, and the full amount will be recorded only at the general ledger level.
    2. Select the **Use For Fixed Asset Cost** checkbox to add the non-deductible GST/HST to the fixed asset cost when you purchase new fixed assets. Otherwise, the non-deductible GST/HST won't have an influence on the fixed asset cost, and the full amount will be recorded only at the general ledger level.
    3. Select the **Use For Job Cost** checkbox to specify that the non-deductible GST/HST must be added to the job cost when you purchase items for the job. Otherwise, the non-deductible GST/HST won't have an influence on the job cost, and the full amount will be recorded only at the general ledger level.
    4. Select the **Show Non-Ded. GST/HST In Lines** checkbox to specify that the non-deductible GST/HST must be shown on document line pages for easier manipulation of GST/HST amounts.

## Use the non-deductible GST/HST percentage

1. Select the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then select the related link.
2. On the **GST/HST Posting Setup** page, set the fields as described in the following table.

    | Field | Description |
    |-------|-------------|
    | Allow Non-Deductible Tax | Specify whether the non-deductible GST/HST is considered for the current combination of a GST/HST business posting group and a GST/HST product posting group. |
    | Non-Deductible Tax % | Specify the percentage of the transaction amount that GST/HST isn't applied to. |
    | Non-Deductible Purchase Tax Account | Specify the account that's associated with the GST/HST amount that isn't deducted because of the type of goods or services that are purchased. |

    > [!NOTE]
    > To have general ledger (G/L) entries that use the dedicated account instead of the sales/purchase account, you can either leave the **Non-Deductible Purchase GST/HST Account** field blank or set the **G/L Account** field.

3. Select **OK**.

> [!NOTE]
> You can't use unrealized GST/HST together with non-deductible GST/HST.
>
> Don't use the same **GST/HST identifier** value for both normal GST/HST where the **Non-Deductible GST/HST %** field is set to **0** (zero) and normal GST/HST where the **Non-Deductible GST/HST %** field is set to a non-zero value. Otherwise, the total non-deductible GST/HST amount will be incorrectly calculated.

## See also 

[Financial Management](finance.md)  
[Design details: Non-deductible GST/HST](design-details-nondeductible-vat.md)  
[Use non-deductible GST/HST](finance-how-use-non-deductible-vat.md)  
[Set Up Calculations and Posting Methods for GST/HST](finance-setup-vat.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
