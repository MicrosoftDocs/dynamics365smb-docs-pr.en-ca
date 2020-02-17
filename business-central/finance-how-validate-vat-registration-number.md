---
title: Validate a VAT Registration Number | Microsoft Docs
description: Validate a VAT Registration Number
author: andregu
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.date: 01/06/2020
ms.author: andregu
ms.openlocfilehash: f4d5023acba2e0cc5600b3f6675c3dcc325489d7
ms.sourcegitcommit: 877af26e3e4522ee234fbba606615e105ef3e90a
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 01/28/2020
ms.locfileid: "2992252"
---
# <a name="validate-a-vat-registration-number"></a>Validate a VAT Registration Number

## <a name="to-verify-vat-registration-numbers"></a>To verify VAT registration numbers
It is important that the GST/HST registration numbers you have for customers, vendors, and contacts are valid. For example, companies sometimes change their tax liability status, and in some countries tax authorities might ask you to provide reports, such as the EC Sales List report, that list the VAT registration numbers you use when you do business.

The European Commission provides the VIES Tax Number Validation service on its website, which is public and free. [!INCLUDE[d365fin](includes/d365fin_md.md)] can save you a step and let you use the VIES service to validate and track VAT numbers for customers, vendors, and contacts straight from the customer, vendor, and contact cards. The service in [!INCLUDE[d365fin](includes/d365fin_md.md)] is named **EU VAT Reg. No. Validation Service**. The service is available on the **Service Connections** page, and you can start using it right away. The service connection is free, and signup is not required.

In order to enable the **EU VAT Reg. No. Validation Service** open the entry in the **Service Connection** page. The **Service Endpoint** field should already be populated. If not, you can use the **Set Default Endpoint** action. Then set the **Enabled** field and you are good to go.

> [!Note]
> To enable the EU VAT Reg. No. Validation Service, you must have administrator permissions.

When you use our service connection, we record a history of VAT numbers and verifications for each customer, vendor, or contact, in the **VAT Registration Log**, so you can easily track them. The log is specific to each customer. For example, the log is useful for proving that you have verified that the current tax number is correct. When you verify a VAT number, the **Request Identifier** column in the log will reflect that you have taken action.

You can view the Tax Registration log on the Customer, Vendor, or Contact cards, on the **Invoicing** FastTab, by choosing the lookup button in the **GST/HST Registration No.** field.  

Our service can also save you time when you create a customer or vendor. If you know the customer's tax number, you can enter it in the **GST/HST Registration No.** field on the Customer or Vendor cards, and we will fill out the customer name for you. Some countries also provide company addresses in a structured format. In those countries, we fill in the address too.  

There are a couple of things to note about the VIES VAT Number Validation service:

* The service uses the http protocol, which means that data transferred through the service is not encrypted.  
* You may experience downtime for this service for which Microsoft is not responsible. The service is part of a broad EU network of national VAT registers.

## <a name="see-also"></a>See Also  
[Set Up Value-Added Tax](finance-setup-vat.md)  
[Setting Up Unrealized Value Added Tax](finance-setup-unrealized-vat.md)      
[Report Tax to a Tax Authority](finance-how-report-vat.md)  
[Work with Tax on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)