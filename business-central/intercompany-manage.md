---
title: Managing intercompany transactions
description: With the Intercompany functionality, you can simplify business processes and transactions between companies within the same organization.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: IC, group, consolidation, affiliate, subsidiary
ms.date: 06/02/2021
ms.author: edupont
ms.openlocfilehash: 0a69507b32f8782fe876458adb590529bfd64b20
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184433"
---
# <a name="managing-intercompany-transactions"></a>Managing Intercompany Transactions

Your organization may consist of several companies, but might not have the equivalent number of accounting and administrative teams. The Intercompany functionality lets you do business with your subsidiary and internal partner organizations in the same way as you engage with your external vendors and customers. You enter intercompany transaction information only once in the appropriate documents. You can use the functionality you are already familiar with, such as receivables and payables management. Mapping facilities for the chart of accounts and dimensions help ensure that information appears in the right places.  

There are four main benefits to the Intercompany functionality:  

- Increased productivity as a result of time saved and simplified transactions  
- Minimized error potential with one-time entry of information and system-wide, automated updates  
- Complete audit trail and full visibility into business activities and transaction histories  
- Efficient, cost-effective transactions with affiliate and subsidiary companies  

You are in full control of all transaction documents. For example, you can reject a document sent to you and, in this way, Reverse Journal Postings and Undo Receipts/Shipments that were incorrect. Or, when making a purchase from a partner or subsidiary company, you can update the purchase order as long as the selling company has not shipped any goods.  

When you enter a transaction, you do not need to specify the accounts for an individual set of books, but simply give the identification of the partner company. The Intercompany functionality creates general journal lines that result in the balancing of the books of both companies involved in a transaction. In receivables and payables, you assign an intercompany partner code to any customer or vendor. From that moment on, all orders and invoices generated pertaining to transactions with these companies will produce corresponding documents in the partner company, resulting in correct balancing of the accounts.  

After you set up business partners as customers and vendors in the system, and assign them intercompany partner codes, it is possible to exchange intercompany purchase and sales documents, including items and item charges. [!INCLUDE [prod_short](includes/prod_short.md)] supports intercompany transactions between multiple databases, for example, in different countries/regions, as well as multiple currencies, different charts of accounts, different dimensions, and different item numbering.  

> [!NOTE]
> Not all types of data can be exchanged between companies in this way. Purchase invoices are not submitted to business partners through intercompany processes. But sales invoices that are submitted through intercompany processes will be created as purchase invoices in the receiving company.

Consolidating financial data may especially be relevant for intercompany processes. For more information, see [Consolidating Financial Data from Multiple Companies](finance-consolidated-company-reporting.md).

The following table describes a sequence of tasks, with links to the articles that describe them.

|To |See|
|---|---|
|Create your intercompany vendors and customers as so-called intercompany partners, and set up an intercompany chart of accounts.|[Set Up Intercompany](intercompany-how-setup.md)|
|Use intercompany documents or journals to post transactions with your intercompany partners.|[Work with Intercompany Documents and Journals](intercompany-how-work-documents-journals.md)|
|Organize and process incoming and outgoing transactions that you exchange with your intercompany partners.|[Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md)|
|Use intercompany postings to distribute costs between partner companies.|[Allocate Costs to Intercompany Partners](intercompany-allocate-costs.md)|

## <a name="see-also"></a>See Also

[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Working with General Journals](ui-work-general-journals.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]