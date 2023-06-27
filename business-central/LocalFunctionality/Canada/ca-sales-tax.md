---
title: 'Reporting Sales Tax [CA]'
description: 'Learn about how sales tax is set up, and how tax groups, tax areas (provinces/territories, counties, cities, and localities), tax jurisdictions, and tax details work in Canada.'
author: edupont04
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 10/12/2021
ms.author: edupont
---
# <a name="reporting-sales-tax-in-canada"></a>Reporting Sales Tax in Canada

[!INCLUDE [sales-tax](../includes/CAMXUS/sales-tax-setup.md)]

If you set up new tax areas and tax jurisdictions, you must make sure that you fill in the fields correctly. In Canada, the federal government and provinces can charge sales tax. Companies collect and remit sales tax to these government authorities for products sold to end users. Sales tax can also be charged to existing sales tax. For example, tax can be calculated on a sales invoice amount that already includes the tax from other jurisdictions.  

In Canada, tax amounts must be detailed in documents for each tax jurisdiction. Up to four jurisdictions can be displayed in a document, and jurisdictions that have the same print order are combined when they are printed.  

## <a name="tax-details"></a>Tax Details

The **Tax Details** page shows different combinations of sales tax jurisdictions and sales tax groups to establish sales tax rates. For each tax jurisdiction, we recommend that you set up one tax group for normal sales tax, another tax group for items or services that are not taxed, and an additional tax group for every type of item or service that is handled with a different sales tax rate in that jurisdiction. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]  

<!--COMMENTING OUT DUE TO ISSUE #535: In Canada, when you sell to a customer at a location where you do not have a *situs*—or a legal location in that state—you do not collect sales tax. For locations in which you do not have a situs, ensure that both the **Tax Below Minimum** and **Tax Above Maximum** fields are 0.00.  -->

## <a name="see-also"></a>See Also

[Canada Local Functionality](canada-local-functionality.md)  
[Finance](../../finance.md)  
[Setting Up Finance](../../finance-setup-finance.md)  
[Sales Tax and Goods and Services Tax in Canada](sales-tax-goods-services.md)  
[Set Up Sales Tax - Watch a Video](https://www.youtube.com/watch?v=qMs4BoSytN8&index=13&list=PLcakwueIHoT8K1m148oMqo7amR2a7Bz-8)  
[Work with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
