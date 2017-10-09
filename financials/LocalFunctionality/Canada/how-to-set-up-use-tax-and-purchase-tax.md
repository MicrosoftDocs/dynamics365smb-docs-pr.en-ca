---
title: How to Set Up Use Tax and Purchase Tax | Microsoft Docs
description: Sales tax includes taxes that companies pay for using items
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 50a95ee803d4af5cbd0d2c375ac6411bec405a26
ms.contentlocale: en-ca
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-use-tax-and-purchase-tax"></a>How to: Set Up Use Tax and Purchase Tax
Sales tax includes taxes that companies pay for using items:  

- Use tax (United States) – Use tax is a United States sales tax that is paid on items that are purchased by a company and are used by that company instead of being sold to a customer. The company must pay sales tax for those items to the government, in the form of use tax.  
- Purchase tax (Canada) – Purchase tax is a Canadian sales tax that is paid by a company on items that are purchased from a vendor. When a company purchases items for use by the company itself, the vendor charges the appropriate sales tax for the items.  

## <a name="to-set-up-use-tax-for-a-purchase-order"></a>To set up use tax for a purchase order  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Orders**, and then choose the related link in **Order Processing**.  
2.  In the **Purchase Orders** window, on the **Home** tab, in the **New** group, choose **New**.  
3.  On the **Lines** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
4.  On the **Invoicing** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Tax Liable**|Select to set up tax liability. **Important:**  This field is available in the **Purchase Header** window, but it is not shown by default. To select the field, you must first add the column that shows this field. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |**Tax Area Code**|The tax area code of the vendor. **Important:**  This field is available in the **Purchase Header** window, but it is not shown by default. To select the field, you must first add the column that shows this field. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |**Tax Exemption No.**|The company's tax exemption number. You can enter a maximum of 30 alphanumeric characters. **Important:**  This field is available in the **Purchase Header** window, but it is not shown by default. To select the field, you must first add the column that shows this field. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |**Provincial Tax Area Code**|The tax code for the province. **Important:**  This field is available in the **Purchase Header** window, but it is not shown by default. To select the field, you must first add the column that shows this field. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
5.  Choose the **OK** button.  

## <a name="to-set-up-use-tax-details"></a>To set up use tax details  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Details**, and then choose the related link.  
2.  In the **Tax Details** window, choose the **New** action.  
3.  In the **New - Tax Details** window, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Tax Jurisdiction Code**|The tax jurisdiction code for the tax detail entry.|  
    |**Tax Group Code**|The tax group code for the tax detail entry.|  
    |**Tax Type**|**Sales and Use Tax** – To apply both sales tax and use tax to the tax detail entry.<br /><br /> –or–<br /><br /> **Excise Tax** – To apply excise tax to the tax detail entry.<br /><br /> –or–<br /><br /> **Sales Tax Only** – To apply only sales tax to the tax detail entry.<br /><br /> –or–<br /><br /> **Use Tax Only** – To apply only use tax to the tax detail entry.|  
4.  Choose the **OK** button.  

## <a name="to-set-up-purchase-tax-for-a-company"></a>To set up purchase tax for a company  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information** , and then choose the related link.  
2.  In the **Company Information** window, on the **Tax** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Tax Area Code**|The company's tax area code. The tax area code is used in conjunction with a tax group code field and the **Tax Liable** field to find the necessary information for calculating sales tax.|  
    |**Tax Exemption No.**|The company's tax exemption number. You can enter a maximum of 30 alphanumeric characters.|  
    |**Provincial Tax Area Code**|The tax code for the province.|  
3.  Choose the **OK** button.  

## <a name="to-set-up-purchase-tax-for-a-location"></a>To set up purchase tax for a location  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.  
2.  In the **Locations** window, select the required location, and then choose the **Edit** action.  
3.  On the **General** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Do Not Use For Tax Calculation**|Select to specify whether the tax information included on this location record is to be used for sales tax calculations on purchase documents.|  
    |**Tax Area Code**|The tax area code for the location. The tax area code is used in conjunction with a tax group code field and the **Tax Liable** field to find the necessary information for calculating sales tax.|  
    |**Tax Exemption No.**|The company's tax exemption number. You can enter a maximum of 30 alphanumeric characters.|  
    |**Provincial Tax Area Code**|The tax code for the province.|  
4.  Choose the **OK** button.  

## <a name="to-set-up-purchase-tax-for-non-recoverable-tax"></a>To set up purchase tax for non-recoverable tax  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Tax Details**, and then choose the related link.  
2.  In the **Tax Details** window, choose the **New** action.  
3.  Select the **Expense/Capitalize** check box.  

    > [!NOTE]  
    >  This check box must be selected if the tax paid is not recoverable.  
4.  Choose the **OK** button.  

## <a name="see-also"></a>See Also  
[Canada Local Functionality](canada-local-functionality.md)  
[Reporting Sales Tax in Canada](ca-sales-tax.md)  
[Finance](../../finance.md)  
[Setting Up Finance](../../finance.md)  

