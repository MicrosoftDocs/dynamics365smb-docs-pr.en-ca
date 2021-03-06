---
title: Sales Tax in Canada| Microsoft Docs
description: Learn about local sales tax and goods and services tax in Canada.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales tax, local
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 5f40e98cb54aaefe9fd105baaffd48d6373f179e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771021"
---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a>Reporting Sales Tax and Goods/Services Tax in Canada
In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only. However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province. When a Provincial Tax Area Code is selected, [!INCLUDE[prod_short](../../includes/prod_short.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records. Therefore, the tax area code selected here should be one where only the PST is included, not the GST.  

## <a name="submitting-the-gsthst-file"></a>Submitting the GST/HST File
The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities. This file includes goods and services tax (GST) and harmonized sales tax (HST). The file is created in a .tax file format, which can be transferred online.  

## <a name="see-also"></a>See Also
[Canada Local Functionality](canada-local-functionality.md)  
[Finance](../../finance.md)  
[Setting Up Finance](../../finance-setup-finance.md)  
[Reporting Sales Tax in Canada](ca-sales-tax.md)  
[Working with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]