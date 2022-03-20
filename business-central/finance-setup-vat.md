---
title: Set Up GST/HST
description: Make sure that you correctly calculate, post, and report on GST/HST for sales and purchases. We recommend that you use the assisted setup guide to set up GST/HST.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.search.form: 10, 1877, 470, 471, 472
ms.date: 01/31/2022
ms.author: bholtorf
ms.openlocfilehash: 80264ff085ab9d88a2d6a32d8f0f1189b3622832
ms.sourcegitcommit: 5a02f8527faecdffcc54f9c5c70cefe8c4b3b3f4
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/04/2022
ms.locfileid: "8383680"
---
# <a name="set-up-calculations-and-posting-methods-for-value-added-tax"></a>Set Up Calculations and Posting Methods for GST/HST

Consumers and businesses pay GST/HST when they purchase goods or services. The amount of GST/HST to pay can vary, depending on several factors. In [!INCLUDE[prod_short](includes/prod_short.md)], you set up GST/HST to specify the rates to use to calculate tax amounts based on the following parameters:

* Who you sell to  
* Who you buy from  
* What you sell  
* What you buy  

You can set up GST/HST calculations manually, but that can be tricky and time consuming. To make it easy, we provide an assisted setup guide named **GST/HST Setup** that will help you with the steps. We recommend that you use the assisted setup guide to set up GST/HST.

> [!NOTE]  
> You can use the guide only if you have created a My Company, and have not posted transactions that include GST/HST. Otherwise, it would be very easy to use different GST/HST rates by mistake, and make GST/HST-related reports inaccurate.  

If you want to set up GST/HST calculations yourself, or just want to learn about each step, this topic contains descriptions of each step.  

[!INCLUDE [finance-vat](includes/finance-vat.md)]

## <a name="use-the-vat-setup-assisted-setup-guide-to-set-up-vat-recommended"></a>Use the GST/HST Setup assisted setup guide to set up GST/HST (recommended)

We recommend that you use the GST/HST Setup assisted setup guide to set up GST/HST in [!INCLUDE[prod_short](includes/prod_short.md)].

To start the assisted setup guide, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**.  
2. Choose **Set up GST/HST** and complete the steps.
3. When you have completed the assisted setup, visit the **GST/HST Posting Setup** page and check if you have to fill in more fields according to the local requirements in your version of [!INCLUDE [prod_short](includes/prod_short.md)]. For more information, see [Local functionality in Business Central](about-localization.md)  

## <a name="set-up-vat-registration-numbers-for-your-country-or-region"></a>Set up GST/HST registration numbers for your country or region

To help ensure that people enter valid GST/HST registration numbers, you can define formats for the GST/HST registration numbers that are used in the countries or regions in which you do business. [!INCLUDE[prod_short](includes/prod_short.md)] will display an error message when someone makes a mistake or uses a format that is incorrect for the country or region.

To set up GST/HST registration numbers, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 2.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**.
2. Choose the country or region, and then choose the **GST/HST Reg. No. Formats** action.
3. In the **Formats** field, define the format by entering one or more of the following characters:  

* **#** Requires a single-digit number.  
* **@** Requires a letter. This format is not case-sensitive.  
* **?** Allows any character.  

    > [!Tip]
    > You can use other characters as long as they are always present in the country or region format. For example, if you need to include a period or a hyphen between sets of numbers, you can define the format as ##.####.### or @@-###-###.  

## <a name="set-up-vat-business-posting-groups"></a>Set up GST/HST business posting groups

GST/HST business posting groups should represent the markets in which you do business with customers and vendors, and define how to calculate and post GST/HST in each market. Examples of GST/HST business posting groups are **Domestic** and **European Union (EU)**.  

Use codes that are easy to remember and describe the business posting group, such as **EU**, **Non-EU**, or **Domestic**. The code must be unique. You can set up as many codes as you need, but you cannot have the same code more than once in a table.

To set up a GST/HST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Business Posting Group**, and then choose the related link.  
2. Fill in the fields as necessary.

You set up default GST/HST business posting groups by linking them to general business posting groups. [!INCLUDE[prod_short](includes/prod_short.md)] automatically assigns the GST/HST business posting group when you assign the business posting group to a customer, vendor, or general ledger account.

## <a name="set-up-vat-product-posting-groups"></a>Set up GST/HST product posting groups

GST/HST product posting groups represent the items and resources you buy or sell, and determine how to calculate and post GST/HST according to the type of item or resource that is being bought or sold.  
It is a good idea to use codes that are easy to remember and describe the rate, such as **NO-GST/HST** or **Zero**, **GST/HST10** or **Reduced** for 10% GST/HST, and **GST/HST25** or **Standard** for 25%.

To set up a GST/HST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 4.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST product Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="combine-vat-posting-groups-in-vat-posting-setups"></a>Combine GST/HST posting groups in GST/HST posting setups

[!INCLUDE[prod_short](includes/prod_short.md)] calculates GST/HST amounts on sales and purchases based on GST/HST posting setups, which are combinations of GST/HST business and product posting groups. For each combination, you can specify the GST/HST percent, GST/HST calculation type, and general ledger accounts for posting GST/HST for sales, purchases, and reverse charges. You can also specify whether to recalculate GST/HST when a payment discount is applied or received.  

Set up as many combinations as you need. If you want to group GST/HST posting setup combinations with similar attributes, you can define a **GST/HST Identifier** for each group, and assign the identifier to the group members.

To combine GST/HST posting setups, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 5.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then choose the related link.
2. Fill in the fields as necessary.

## <a name="assign-vat-posting-groups-by-default-to-multiple-entities"></a>Assign GST/HST posting groups by default to multiple entities

If you want to apply the same GST/HST posting groups to multiple entities, you can set up [!INCLUDE[prod_short](includes/prod_short.md)] to do so by default. There are a couple of ways to do this:

* You can assign GST/HST business posting groups to general business posting groups, or customer or vendor templates
* You can assign GST/HST product posting groups on general product posting groups  

The GST/HST business or product posting group is assigned when you choose a business or product posting group for a customer, vendor, item, or resource.

## <a name="assign-vat-posting-groups-to-accounts-customers-vendors-items-and-resources"></a>Assign GST/HST posting groups to accounts, customers, vendors, items, and resources

The following sections describe how to assign GST/HST posting groups to individual entities.

### <a name="to-assign-vat-posting-groups-to-individual-general-ledger-accounts"></a>To assign GST/HST posting groups to individual general ledger accounts

1. Choose the ![Lightbulb that opens the Tell Me feature 6.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.  
2. Open the **G/L Account** card for the account.  
3. On the **Posting** FastTab, in the **Gen. Posting Type** field, choose either **Sale** or **Purchase**.  
4. Choose the GST/HST posting groups to use for the sales or purchase account.  

### <a name="to-assign-vat-business-posting-groups-to-customers-and-vendors"></a>To assign GST/HST business posting groups to customers and vendors

1. Choose the ![Lightbulb that opens the Tell Me feature 7.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.  
2. On the **Customer** or **Vendor** card, expand the **Invoicing** FastTab.  
3. Choose the GST/HST business posting group.  

### <a name="to-assign-vat-product-posting-groups-to-individual-items-and-resources"></a>To assign GST/HST product posting groups to individual items and resources

1. Choose the ![Lightbulb that opens the Tell Me feature 8.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item** or **Resource**, and then choose the related link.  
2. Do one of the following:  

    * On the **Item** card, expand the **Price & Posting** FastTab, and then choose **Show more** to display the **GST/HST Product Posting Group** field.  
    * On the **Resource** card, expand the **Invoicing** FastTab.  
3. Choose the GST/HST product posting group.  

## <a name="set-up-clauses-to-explain-vat-exemption-or-non-standard-vat-rates"></a>Set up clauses to explain GST/HST exemption or non-standard GST/HST rates

You set up a GST/HST clause to describe information about the type of GST/HST that is being applied. The information may be required by government regulation. After you set up a GST/HST clause, and associate it with a GST/HST posting setup, the GST/HST clause is displayed on printed sales documents that use the GST/HST posting setup group.

If needed, you can also specify how to translate GST/HST clauses to other languages. Then, when you create and print a sales document that contains a GST/HST identifier, the document will include the translated GST/HST clause. The language code specified on the customer card determines the language.

When non-standard GST/HST rates are used in different types of documents, such as invoices or credit memos, companies are usually required to include an exemption text (GST/HST clause) stating why a reduced GST/HST or zero GST/HST rate has been calculated. You can define different GST/HST clauses to be included on business documents per the type of document, such as invoice or credit memo. You do this on the **GST/HST Clauses by Doc. Type** page.

You can modify or delete a GST/HST clause, and your modifications will be reflected in a generated report. However, [!INCLUDE[prod_short](includes/prod_short.md)] does not keep a history of the change. On the report, the GST/HST clause descriptions are printed and displayed for all lines in the report alongside the GST/HST amount and the GST/HST base amount. If a GST/HST clause has not been defined for any lines on the sales document, then the whole section is omitted when the report is printed.

### <a name="to-set-up-vat-clauses"></a>To set up GST/HST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 9.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Clauses**, and then choose the related link.  
2. On the **GST/HST Clauses** page, create a new line.  
3. In the **Code** field, enter an identifier for the clause. You use this code to assign the clause to GST/HST posting groups.  
4. In the **Description** field, enter the GST/HST exemption text that you want to display on documents that can include GST/HST. In the **Description 2** field, enter more text, if needed. The text will be displayed on new document lines.
5. Choose the **Description by Document Type** action.
6. On the **GST/HST Clauses by Doc. Type** page, fill in the fields to set up which GST/HST exemption text to display for which document type.  
7. Optional: To assign the GST/HST clause to a GST/HST posting setup right away, choose **Setup**, and then choose the clause. If you want to wait, you can assign the clause later on the **GST/HST Posting Setup** page.  
8. Optional: To specify how to translate the GST/HST clause, choose the **Translations** action.

### <a name="to-assign-a-vat-clause-to-a-vat-posting-setup"></a>To assign a GST/HST clause to a GST/HST posting setup

1. Choose the ![Lightbulb that opens the Tell Me feature 10.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then choose the related link.  
2. In the **GST/HST Clause** column, choose the clause to use for each GST/HST posting setup it applies to.  

### <a name="to-specify-translations-for-vat-clauses"></a>To specify translations for GST/HST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Clauses**, and then choose the related link.  
2. Choose the **Translations** action.  
3. In the **Language Code** field, choose the language you are translating to.  
4. In the **Description** and **Description 2** fields, enter the translations of the descriptions. This text displays in the translated GST/HST report documents.  

## <a name="create-a-vat-posting-setup-to-handle-import-vat"></a>Create a GST/HST posting setup to handle Import GST/HST

You use the *Import GST/HST* feature when you need to post a document where the entire amount is GST/HST. You will use this if you receive an invoice from the tax authorities for GST/HST for imported goods.  

To set up codes for import GST/HST, follow these steps:  

1. Choose the ![Lightbulb that opens the Tell Me feature 12.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST product Posting Groups**, and then choose the related link.  
2. On the GST/HST product Posting Groups page, set up a new GST/HST product posting group for import GST/HST.  
3. Choose the ![Lightbulb that opens the Tell Me feature 13.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then choose the related link.  
4. On the GST/HST Posting Setup page, create a new line, or use an existing GST/HST business posting groups in combination with the new GST/HST product posting group for import GST/HST.  
5. In the **GST/HST Calculation Type** field, choose **Full GST/HST**.  
6. In the **Purchase GST/HST Account** field, enter the general ledger account to use for posting import GST/HST. All other accounts are optional.  

## <a name="use-reverse-charge-vat-for-trade-between-eu-countries-or-regions"></a>Use reverse charge GST/HST for trade between EU countries or regions

Some companies must use reverse charge VAT when trading with other companies. For example this rule applies to purchases from EU countries/regions and sales to EU countries/regions.  

> [!NOTE]  
> This rule applies when trading with companies that are registered as GST/HST liable in another EU country/region. If you do business directly with consumers in other EU countries/regions, then you should contact your tax authority for applicable VAT rules.  

> [!TIP]  
> You can verify that a company is registered as VAT liable in another EU country by using the EU VAT Registration Number Validation service. The service is available for free in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Verify VAT registration numbers](finance-how-validate-vat-registration-number.md).

### <a name="sales-to-eu-countries-or-regions"></a>Sales to EU countries or regions

VAT is not calculated on sales to VAT-liable companies in other EU countries/regions. You must report the value of these sales to EU countries/regions separately on your VAT statement.  

To correctly calculate VAT on sales to EU countries/regions, you should:  

* Set up a line for sales with the same information for purchases. If you have already set up lines on the VAT Posting Setup page for purchases from EU countries/regions, then you can also use these lines for sales.  
* Assign the VAT business posting groups in the **VAT Bus. Posting Group** field on the **Invoicing** FastTab of the customer card of each EU customer. You should also enter the customer's VAT registration number in the **VAT Registration No.** field on the **Foreign Trade** FastTab.  

When you post a sale to a customer in another EU country/region, the VAT amount is calculated, and a VAT entry is created by using the information about the reverse charge VAT and the VAT base, which is the amount that is used to calculate the VAT amount. No entries are posted to the VAT accounts in the general ledger.

## <a name="vat-rounding-for-documents"></a>GST/HST rounding for documents

Amounts in documents that are not yet posted are rounded and displayed to correspond with the final rounding of amounts that are actually posted. GST/HST is calculated for a complete document, which means that GST/HST is calculated based on the sum of all lines with the same GST/HST identifier in the document.  

## <a name="set-up-vat-reporting"></a>Set up GST/HST reporting

You must set up information about how the tax authorities in your country or region require you to submit GST/HST reports. The following steps illustrate the most commonly used information. However, your country or region may require additional steps. For more information, see the relevant article in the *Local functionality* section in the panel to the left.

[!INCLUDE [vat-report-setup](includes/vat-report-setup.md)]

## <a name="see-also"></a>See Also

[Setting up GST/HST Statement Templates and GST/HST Statement Names](finance-how-setup-vat-statement.md)  
[Setting Up Unrealized GST/HST](finance-setup-unrealized-vat.md)  
[Report GST/HST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST/HST on Sales and Purchases](finance-work-with-vat.md)  
[Work with the GST/HST Rate Change Tool](finance-how-use-vat-rate-change-tool.md)  
[Verify VAT identification numbers](finance-how-validate-vat-registration-number.md)  
[Local functionality in Business Central](about-localization.md)  

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/paths/process-vat-dynamics-365-business-central/)


[!INCLUDE[footer-include](includes/footer-banner.md)]
