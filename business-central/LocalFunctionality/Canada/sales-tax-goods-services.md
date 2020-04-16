---
title: Sales Tax in Canada| Microsoft Docs
description: Learn about local sales tax and goods and services tax in Canada.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales tax, local
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 5783e0b116287823b9118a12050ceebbb14cad3c
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180828"
---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a>Reporting Sales Tax and Goods/Services Tax in Canada
In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only. However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province. When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records. Therefore, the tax area code selected here should be one where only the PST is included, not the GST.  

## <a name="submitting-the-gsthst-file"></a>Submitting the GST/HST File
The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities. This file includes goods and services tax (GST) and harmonized sales tax (HST). The file is created in a .tax file format, which can be transferred online.  

## <a name="see-also"></a>See Also
[Canada Local Functionality](canada-local-functionality.md)  
[Finance](../../finance.md)  
[Setting Up Finance](../../finance-setup-finance.md)  
[Reporting Sales Tax in Canada](ca-sales-tax.md)  
[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)
