---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: 50b4b331f00bdcdf030bac2332ffb5dafdfd2de6
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116033"
---
On sales documents and journals, you can specify a document number that refers to the customer's numbering system. <!--You can enter a maximum of ten characters, both numbers and letters.--> Use this field to record the number that the customer assigned to the order, invoice, or credit memo. You can then use the number later if, for some reason, you need to search for the posted entry using this number.  

The **Ext. Doc. No. Mandatory** field on the **Sales & Receivables Setup** page specifies whether it is mandatory to enter an external document number in the **External Document No.** field on a sales header and the **External Document No.** field on a general journal line.

If you select this field, it will not be possible to post an invoice or a general journal line without an external document number.

The external document number is included in posted documents where you can search by the relevant number. You can also search using the external document number when navigating on customer ledger entries.

A different way to handle external document numbers is to use the **Your Reference** field. If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields. But the field is not available on journal lines.
