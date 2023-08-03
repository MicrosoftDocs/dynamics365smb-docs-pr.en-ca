---
title: Design details - Non-deductible GST/HST
description: 'This article provides information about non-deductible GST/HST that''s payable by a purchaser, but that isn''t deductible from the purchaser''s own GST/HST liability.'
author: altotovi
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 07/04/2023
ms.author: altotovi
---

# <a name="design-details-non-deductible-vat"></a>Design details: Non-deductible GST/HST

Non-deductible GST/HST is the GST/HST that's payable by a purchaser, but that isn't deductible from the purchaser's own GST/HST liability. Because it can be difficult to know where and how an item is used, you must contact the local tax authorities in your country or region to determine whether a specified percentage of the GST/HST is deductible. Even when you know that a specific percentage of the GST/HST isn't deductible, there are different models for handling non-deductible amounts as they are related to **items** and **fixed assets**.

## <a name="prerequisites-for-using-non-deductible-vat"></a>Prerequisites for using non-deductible GST/HST

To use and post non-deductible GST/HST, follow these steps.

1. On the **GST/HST Setup** page, select **Enable Non-Deductible GST/HST** to enable the feature.
2. On the **GST/HST Posting Setup** page, select which GST/HST posting groups can use non-deductible GST/HST.

## <a name="examples"></a>Examples

For the following examples, non-deductible GST/HST is enabled, and the following setup is completed:

- The **GST/HST Product Posting Group** field is set to **NDGST/HST**.
- On the **GST/HST Posting Setup** page:

    - **NDGST/HST** is set as the GST/HST product posting group, and **DOMESTIC** is set as the GST/HST business posting group.
    - The **GST/HST Identifier** value must be unique.
    - The **GST/HST %** field is set to **25**.
    - The **Allow Non-deductible GST/HST** field is set to **Allow**.
    - The **Non-deductible GST/HST %** field is set to **100**.
    - The **GST/HST Calculation Type** field is set to **Normal GST/HST**.
    - Only the sales GST/HST account and purchase GST/HST account are configured.

All the examples use items and fixed assets where the GST/HST product posting group is **NDGST/HST**.

### <a name="items"></a>Items

A new item has **NDGST/HST** set as the GST/HST product posting group. In the purchase document, **Quantity** = **1** and **Direct Unit Cost Excl. GST/HST** = **1,000.00**.

Regardless of the option that's used, the results in the GST/HST entry are the same.

| Document Type | Type | Base | Amount | Non-Deductible Tax Base | Non-deductible GST/HST Amount |
|---|---|---|---|---|---|
| Invoice | Purchase | 0.00 | 0.00 | 1,000.00 | 250.00 |

The details are shown in the value entries.

> [!NOTE]
> You can enable the **Use for Item Cost** field on the **GST/HST Setup** page.

#### <a name="use-for-item-cost-isnt-enabled"></a>Use for Item Cost isn't enabled

| Item Ledger Entry Type | Entry Type | Cost Amount (Actual) | Item Ledger Entry Quantity |
|---|---|---|---|
| Purchase | Direct Cost | 1,000.00 | 1 |

#### <a name="use-for-item-cost-is-enabled"></a>Use for Item Cost is enabled

| Item Ledger Entry Type | Entry Type | Cost Amount (Actual) | Item Ledger Entry Quantity |
|---|---|---|---|
| Purchase | Direct Cost | 1,250.00 | 1 |

### <a name="fixed-assets"></a>Fixed assets

A new fixed asset has the acquisition cost account set to use **NDGST/HST** as the GST/HST product posting group. In the purchase document, **Quantity** = **1** and **Direct Unit Cost Excl. GST/HST** = **1,000.00**.

Regardless of the option that's used, the results in the GST/HST entry are the same.

| Document Type | Type | Base | Amount | Non-Deductible Tax Base | Non-deductible GST/HST Amount |
|---|---|---|---|---|---|
| Invoice | Purchase | 0.00 | 0.00 | 1,000.00 | 250.00 |

The details are shown in the fixed asset ledger entries.

> [!NOTE]
> You can enable the **Use for Fixed Asset Cost** field on the **GST/HST Setup** page.

#### <a name="use-for-fixed-asset-cost-isnt-enabled"></a>Use for Fixed Asset Cost isn't enabled

| Document Type | FA Posting Type | Amount | Tax Amount |
|---|---|---|---|
| Invoice | Acquisition Cost | 1,000.00 | 250.00 |

#### <a name="use-for-fixed-asset-cost-is-enabled"></a>Use for Fixed Asset Cost is enabled

| Document Type | FA Posting Type | Amount | Tax Amount |
|---|---|---|---|
| Invoice | Acquisition Cost | 1,000.00 | 250.00 |
| Invoice | Acquisition Cost | 250.00 | 0.00 |

## <a name="see-also"></a>See also

[Set up non-deductible GST/HST](finance-setup-nondeductible-vat.md)  
[Finance](finance.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
