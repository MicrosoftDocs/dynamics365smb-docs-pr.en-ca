---
title: How to Manage Customer Credit Information | Microsoft Docs
description: In Finance and Operations, Business edition, you can add comments to customer credit information. You can also hold and block customers with bad credit before shipping or invoicing occurs.
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: b15c44ae471e7398985517a9cf596b15ff5efcc2
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---
# <a name="manage-customer-credit-information"></a>Manage Customer Credit Information
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can add comments to customer credit information. You can also hold and block customers with bad credit before shipping or invoicing occurs.  

## <a name="to-add-comments-to-customer-credit-information"></a>To add comments to customer credit information  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Credit Management**, and then choose the related link.  
2.  In the **Customer List - Credit Mgmt.** window, select a customer, and then choose the **Comments** action.  
3.  In the **Comment Sheet** window, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Date**|The date of the comment.|  
    |**Comment**|The comment about the customer. You can enter a maximum of 80 alphanumeric characters.|  

4.  Choose the **OK** button.  

## <a name="to-prevent-an-order-from-shipping-or-invoicing"></a>To prevent an order from shipping or invoicing  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.  
2.  Select the customer, and the choose the **Ledger Entries** action.  
3.  In the **On Hold** field, enter the initials of the customer.  
4.  Choose the **OK** button.  

    > [!NOTE]  
    >  You must have the proper security clearance to add or remove holds on individual sales orders using the **On Hold** field.  

## <a name="to-block-a-sales-order-for-a-customer"></a>To block a sales order for a customer  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.  
2.  Select a customer, and then choose the **Edit** action.  
3.  On the **General** FastTab, in the **Blocked** field, select one of the following options:  

    -   **<Blank>** – Transaction is allowed for this customer.  
    -   **Ship** – New orders and new shipments cannot be created for this customer. Existing shipments not yet invoiced can be invoiced.  
    -   **Invoice** – New orders, new shipments, and new invoices cannot be created for this customer. Existing shipments not yet invoiced cannot be invoiced.  
    -   **All** – No transaction is allowed for this customer, including payments.  
4.  Choose the **OK** button.  

## <a name="see-also"></a>See Also  
[Canada Local Functionality](canada-local-functionality.md)  
[Finance](../../finance.md)  
[Setting Up Finance](../../finance.md)

