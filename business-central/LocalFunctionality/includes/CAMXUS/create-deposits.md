---
author: edupont04
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 75205f4c9fd94cd499b1f1c017a8bfc396465ae7
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 02/15/2022
ms.locfileid: "8146016"
---
You can make deposits to maintain a transaction record that contains information that can be applied to outstanding invoices and credit memos.  

The **Deposit** page specifies bank deposit information. The information includes the bank account number, total deposit amount, deposit lines, posting date, document date, department code, currency code, and deposit notes. You can use the page to create new deposits, post deposits, print deposits, view deposit comments, or view a report that shows the deposit amount to be reconciled.

The **Deposit** report displays customer and vendor deposits with the original deposit amount, the amount of the deposit that remains open, and the amount applied. The report also shows the total posted deposit amount to be reconciled.

Deposit lines contain information about the individual deposited items, such as cheques from customers. This information includes the document date and number, account type and number, and amount. The total of the amounts on the lines must add up to the total amount of the deposit entered on the deposit header.

After you have filled in the deposit information and the associated deposit lines, you must post it in order to update the bank ledger, general ledger, customer ledger, and any other relevant ledgers. Posted deposits are stored for future reference and can be viewed on the **Posted Deposits** page.

## <a name="to-create-a-deposit"></a>To create a deposit  
1.  Choose the ![Lightbulb that opens the Tell Me feature.](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Deposits**, and then choose the related link.  
2.  Choose the **New** action.  
3.  On the **General** FastTab, fill in the required fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**No.**|The unique identification number for the deposit.|  
    |**Bank Account No.**|The bank account number for the deposit.|  
    |**Total Deposit Amount**|The total deposit amount posted to the bank ledger.<br /><br /> You can post this deposit only if the sum of the deposit lines is equal to the value in this field.|  
    |**Posting Date**|The posting date for the deposit.|  
    |**Document Date**|The deposit document date.|  
4.  On the **Lines** FastTab, fill in the required fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Account Type**|The account type.|  
    |**Account No.**|The unique identification account number that is associated with the selected account type, to which the entry will be posted.|  
    |**Description**|The journal line entry description.|  
    |**Document Date**|The journal line entry document date.|  
    |**Document Type**|The journal line entry document type.|  
    |**Document No.**|The journal line entry document number.|  
    |**Credit Amount**|The total credit amount on the journal line.|  

5.  Optionally, choose the **Dimensions** action, and then add relevant dimensions on the **Dimension Set Entries** page.  
6. Choose the **Post** action.  

    > [!NOTE]  
    >  You can post a deposit only if the amount displayed in the **Total Deposit Lines** field is equal to the amount in the **Total Deposit Amount** field.  

Next, you can use the **Deposit Test** and **Deposit** reports to reconcile your posted deposits with outstanding invoices and credit memos.  
