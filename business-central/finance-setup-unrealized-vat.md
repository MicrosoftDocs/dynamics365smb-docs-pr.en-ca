---
title: Set Up Unrealized GST/HST
description: 'If you''re using cash-based accounting, you can specify how to handle unrealized GST/HST for sales and purchases.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'cash, VAT, unrealized, cash-based'
ms.search.form: '118, 472, 473'
ms.date: 04/01/2021
ms.author: bholtorf
---

# <a name="set-up-unrealized-vat-for-cash-based-accounting" />Set Up Unrealized GST/HST for Cash-Based Accounting

If you are using cash-based accounting methods, you can set up [!INCLUDE[prod_short](includes/prod_short.md)] to handle unrealized GST/HST.

## <a name="to-use-general-ledger-accounts-for-unrealized-vat" />To use general ledger accounts for unrealized GST/HST

You can choose to have GST/HST amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in GST/HST statements when the actual payment of the invoice is posted. Before you can do this, you must complete the [GST/HST posting setup](finance-setup-vat.md).

To use accounts for unrealized GST/HST, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, and enter **General Ledger Setup**.
2. On the **General Ledger Setup** page, select the **Unrealized GST/HST** check box.
3. Choose the **Search for Page or Report** icon ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do"), and enter **GST/HST Posting Setup**.
4. On the **GST/HST Posting Setup** page, choose the GST/HST posting group, and then choose the **Edit** action.
5. In the **Unrealized GST/HST Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding GST/HST) and the GST/HST amount itself, and how to transfer GST/HST amounts from the unrealized GST/HST account to the realized account. The following table describes the options.

| Option | Description |
| --- | --- |
| Blank | Choose this option if you don't want to use the unrealized GST/HST feature. |
| Percentage | Payments covers both GST/HST and the invoice amount in proportion to the payment's percentage of the remaining invoice amount. The paid GST/HST amount is transferred from the unrealized GST/HST account to the realized GST/HST account. |
| First | Payments cover GST/HST first and then invoice amounts. In this case, the amount transferred from the unrealized GST/HST account to the GST/HST account will equal the amount of the payment until the total GST/HST has been paid. |
| Last | Payments cover the invoice amount first and then GST/HST. In this case, no amount will be transferred from the unrealized GST/HST account to the GST/HST account until the total amount of the invoice, excluding GST/HST, has been paid. |
| First (Fully Paid) | Payments will cover GST/HST first (like the _First_ option), but no amount will be transferred to the GST/HST account until the full amount of GST/HST has been paid. |
| Last (Fully Paid) | Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the GST/HST account until the full amount of GST/HST has been paid. |

6. In the **Sales GST/HST Unreal. Account** field, choose the account for unrealized sales GST/HST.

    > [!NOTE]  
    > The GST/HST amount will be posted to this account, and stay there until the customer payment is posted. The amount is then transferred to the account for sales GST/HST.
7. In the **Purch. GST/HST Unreal. Account** field, enter the general ledger account for unrealized purchase GST/HST.

> [!NOTE]  
> The GST/HST amount will be posted to this account, and stay there until the customer payment is posted. The amount is then transferred to the account for purchase GST/HST.

## <a name="see-also" />See Also
[Set Up Calculations and Posting Methods for GST/HST](finance-setup-vat.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
