---
title: Set Up GST/HST
description: 'Make sure that you correctly calculate, post, and report on GST/HST for sales and purchases. We recommend that you use the assisted setup guide to set up GST/HST.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'VAT, posting, tax, value-added tax'
ms.search.form: '10, 118, 391, 470, 471, 472, 575, 734, 747, 748, 1877,'
ms.date: 01/31/2023
ms.author: bholtorf
---

# <a name="set-up-calculations-and-posting-methods-for-value-added-tax" />Set Up Calculations and Posting Methods for GST/HST

Consumers and businesses pay GST/HST when they purchase goods or services. The amount of GST/HST to pay can vary, depending on several factors. In [!INCLUDE[prod_short](includes/prod_short.md)], you set up GST/HST to specify the rates used to calculate tax amounts based on the following parameters:

* Who you sell to  
* Who you buy from  
* What you sell  
* What you buy  

You can set up GST/HST calculations manually, but that can be tricky and time-consuming. That's because it's very easy to use different GST/HST rates by mistake and create inaccurate GST/HST-related reports. To make GST/HST set up easier, we recommend you use the assisted **GST/HST Setup** guide provided in the product. 

However, if you want to set up the GST/HST calculations yourself, or just want to learn about each step, this article contains descriptions of each step:  

[!INCLUDE [finance-vat](includes/finance-vat.md)]

## <a name="set-up-vat-using-the-assisted-setup-guide-recommended" />Set up GST/HST using the assisted setup guide (recommended)

> [!NOTE]
> You can use the **GST/HST Setup** guide only if you have created a *My Company* and have not yet posted transactions that include GST/HST.

To start the assisted setup guide, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon and enter **Assisted Setup**. 
2. Choose **Set up GST/HST** and complete the steps.
3. When you have completed the assisted setup, visit the **GST/HST Posting Setup** page to check if you need to fill in more fields according to the local requirements in your version of [!INCLUDE [prod_short](includes/prod_short.md)]. Learn more at [Local functionality in Business Central](about-localization.md).  

### <a name="check-the-vat-posting-setup" />Check the GST/HST posting setup

To support your fast start, [!INCLUDE [prod_short](includes/prod_short.md)] notifies you of missing general ledger (G/L) accounts in posting groups or posting setups, such as on the **GST/HST Posting Setup** page. You can turn this type of notification on or off using the *G/L Account is missing in posting group or setup* notification in the **My Notifications** page. Just go to the **My settings** page, and then choose the *Change when I receive notifications.* link.  

If you choose such a notification, [!INCLUDE [prod_short](includes/prod_short.md)] automatically creates those posting setups based on the posting groups in the document or journal you're currently working on.  

At this point, you can just fill in the missing G/L accounts. But, later, when you further refine the setup, you might realize this initial setup is wrong. And [!INCLUDE [prod_short](includes/prod_short.md)] does not allow the deletion of a GST/HST posting setup and general posting setup when entries have been created based on such configurations. So starting in 2022 release wave 1, you can use the **Blocked** field on the **GST/HST Posting Setup** page to prevent users from mistakenly using a setup that is no longer relevant for new postings.

## <a name="set-up-a-default-vat-date-for-documents-and-journals" />Set up a default GST/HST date for documents and journals

GST/HST reporting in [!INCLUDE [prod_short](includes/prod_short.md)] is based on the **GST/HST Date** to include GST/HST entries on GST/HST reports in a GST/HST period. The GST/HST date can be changed on all documents and journals, but you must specify a default value for GST/HST date.

> [!NOTE]
> After posting the document or journal, the **GST/HST Date** will appear on **GST/HST Entries** and **G/L Entries** as well as on the posted document if exists.

To set up a default value for a GST/HST date, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon and enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **Default GST/HST Date** field, choose either **Posting Date** or **Document Date**.
3. Close the page.  

> [!NOTE]
> By default, the **Default GST/HST Date** is the **Posting Date**.

### <a name="enabling-or-disabling-the-vat-date-feature" />Enabling or disabling the GST/HST Date feature

Some countries require that businesses use a specific GST/HST date, but other countries don't. Some countries also require businesses to change the GST/HST date in specific situations after they have posted documents, but other countries don't allow changes to GST/HST dates. To allow for different contexts, you can choose whether you want to use this functionality and, if so, to what degree.

To set up the level of GST/HST date usage, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon and enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **GST/HST Date Usage** field, specify the degree to which you want to use the GST/HST date feature. You can choose one of the following options:

| Type | Description |
|--------------------|-----------------------------------------|
| **Use full GST/HST Date functionality** | Everything related to **GST/HST Date** works by default, giving you the maximum **GST/HST Date** functionality. You can set up the date, change it in documents, report based on it, and modify the date after posting as long as the period isn't closed or protected with allowed dates for posting. |
| **Use but do not allow modifications** | Everything related to **GST/HST Date** works by default with one exception. You can't modify the **GST/HST Date** in **GST/HST Entries**. |
| **Not using GST/HST Date functionality** | [!INCLUDE [prod_short](includes/prod_short.md)] will hide and make the **GST/HST Date** fields not available on documents, journals, and entries. The **Default GST/HST Date** will be configured as the **Posting Date**. |

3. Close the page.

> [!IMPORTANT]
> Even if you choose the **Not using GST/HST Date functionality** option, [!INCLUDE [prod_short](includes/prod_short.md)] will use the **GST/HST Date** in the background. Because the **Default GST/HST Date** is configured as the **Posting Date**, and you can't change it in this case, you'll get the same experience as without this feature. **GST/HST Date** fields will be removed from all pages, but this field will still exist in tables and reports will work based on it.

### <a name="limiting-periods-for-posting-and-changing-the-vat-date" />Limiting periods for posting and changing the GST/HST date

You can prevent people from posting or changing GST/HST entries in specific date ranges. You set the restriction using using two settings:

* Based on closed **GST/HST Return Period**
* Based on the **Allow Posting From** and **Allow Posting To** fields.

#### <a name="to-limit-posting-based-on-vat-return-period" />To limit posting based on GST/HST return period

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **Control GST/HST Period** field, specify the degree of GST/HST Return Period control. The following table describes the options.

| Type | Description |
|--------------------|-----------------------------------------|
| **Block posting within closed and warn for released period** | Prevent people from posting a document or journal, or changing GST/HST entries, that have a GST/HST date within a closed **GST/HST Return Period**. [!INCLUDE [prod_short](includes/prod_short.md)] will also show a warning if your **GST/HST Return Period** is open, but the status of **GST/HST Return** is **Released** or **Submitted**. |
| **Block posting within closed period** | Prevent people from posting a document or journal, or changing GST/HST entries, that have a GST/HST date within the closed **GST/HST Return Period**. |
| **Warn when posting in closed period** | Show a warning, but don't block posting, if you want to post a document or journal that has a GST/HST date within a closed **GST/HST Return Period**. |
| **Disabled** | Take no action based on a closed **GST/HST Return Period**. |

#### <a name="to-limit-posting-based-on-allow-fromto-period" />To limit posting based on Allow from/to period

You can set up limitation on the company or specific user levels.

To limit all postings for the whole company:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, in the **Allow Posting From** field, specify the GST/HST date from which you allow posting. Posting a document or journal with a GST/HST date before this date isn't allowed.  
3. On the **General** FastTab, in the **Allow Posting To** field, specify the GST/HST date until which you allow posting. Posting a document or journal with a GST/HST date after this date isn't allowed.

To limit postings for the specific user:

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.  
2. In the **User ID** field, specify the user you want to allow to post in specific period.  
3. In the **Allow Posting From** field, specify the GST/HST date from which you allow posting. Posting a document or journal with a GST/HST date before this date isn't allowed.
4. In the **Allow Posting To** field, specify the GST/HST date until which you allow posting. Posting a document or journal with a GST/HST date after this date isn't allowed.

## <a name="set-up-vat-registration-numbers-for-your-country-or-region" />Set up GST/HST registration numbers for your country or region

To help ensure people enter valid GST/HST registration numbers, you can define formats for the GST/HST registration numbers that are used in the countries or regions in which you do business. [!INCLUDE[prod_short](includes/prod_short.md)] will display an error message if someone makes a mistake or uses a format that is incorrect for the country or region.

To set up GST/HST registration numbers, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 2.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**.
2. Choose the country or region, and then choose the **GST/HST Reg. No. Formats** action.
3. In the **Formats** field, define the format by entering one or more of the following characters:  

* **#** Requires a single-digit number.  
* **@** Requires a letter. This format is not case-sensitive.  
* **?** Allows any character.  

    > [!TIP]
    > You can use other characters as long as they are always present in the country or region format. So, if you need to include a period or a hyphen between sets of numbers, you can define the format as ##.####.### or @@-###-###.  

## <a name="set-up-vat-business-posting-groups" />Set up GST/HST business posting groups

GST/HST business posting groups should represent the markets in which you do business with customers and vendors, and define how to calculate and post GST/HST in each market. Examples of GST/HST business posting groups are **Domestic** and **European Union (EU)**.  

Use codes that are easy to remember and describe the business posting group, such as **EU**, **Non-EU**, or **Domestic**. Each code must be unique, meaning you can set up as many codes as you need, but you cannot have the same code more than once in a table.

To set up a GST/HST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Business Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

You can set up default GST/HST business posting groups by linking them to general business posting groups. [!INCLUDE[prod_short](includes/prod_short.md)] automatically assigns the GST/HST business posting group when you assign the business posting group to a customer, vendor, or general ledger account.

## <a name="set-up-vat-product-posting-groups" />Set up GST/HST product posting groups

GST/HST product posting groups represent the items and resources you buy or sell, and determine how to calculate and post GST/HST according to the type of item or resource.

It is a good idea to use codes that are easy to remember and describe the rate, such as **NO-GST/HST** or **Zero**, **GST/HST10** or **Reduced** for 10 percent GST/HST, and **GST/HST25** or **Standard** for 25 percent.

To set up a GST/HST business posting group, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 4.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST product Posting Groups**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="combine-vat-posting-groups-in-vat-posting-setups" />Combine GST/HST posting groups in GST/HST posting setups

[!INCLUDE[prod_short](includes/prod_short.md)] calculates GST/HST amounts on sales and purchases based on GST/HST posting setups, which are combinations of GST/HST business and product posting groups. For each combination, you can specify the GST/HST percent, GST/HST calculation type, and general ledger accounts for posting GST/HST for sales, purchases, and reverse charges. You can also specify whether to recalculate GST/HST when a payment discount is applied or received.  

Set up as many combinations as you need. If you want to group GST/HST posting setup combinations with similar attributes, you can define a **GST/HST Identifier** for each group, and assign the identifier to the group members.

To combine GST/HST posting setups, follow these steps:

1. Choose the ![Lightbulb that opens the Tell Me feature 5.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

## <a name="assign-vat-posting-groups-by-default-to-multiple-entities" />Assign GST/HST posting groups by default to multiple entities

If you want to apply the same GST/HST posting groups to multiple entities, you can set up [!INCLUDE[prod_short](includes/prod_short.md)] to do so by default. There are a couple of ways to do this:

* You can assign GST/HST business posting groups to general business posting groups, or customer or vendor templates
* You can assign GST/HST product posting groups on general product posting groups  

The GST/HST business or product posting group is assigned when you choose a business or product posting group for a customer, vendor, item, or resource.

## <a name="assign-vat-posting-groups-to-accounts-customers-vendors-items-and-resources" />Assign GST/HST posting groups to accounts, customers, vendors, items, and resources

The following sections describe how to assign GST/HST posting groups to individual entities.

### <a name="to-assign-vat-posting-groups-to-individual-general-ledger-accounts" />To assign GST/HST posting groups to individual general ledger accounts

1. Choose the ![Lightbulb that opens the Tell Me feature 6.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.  
2. Open the **G/L Account** card for the account.  
3. On the **Posting** FastTab, in the **Gen. Posting Type** field, choose either **Sale** or **Purchase**.  
4. Choose the GST/HST posting groups to use for the sales or purchase account.  

### <a name="to-assign-vat-business-posting-groups-to-customers-and-vendors" />To assign GST/HST business posting groups to customers and vendors

1. Choose the ![Lightbulb that opens the Tell Me feature 7.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Vendor**, and then choose the related link.  
2. On the **Customer** or **Vendor** card, expand the **Invoicing** FastTab.  
3. Choose the GST/HST business posting group.  

### <a name="to-assign-vat-product-posting-groups-to-individual-items-and-resources" />To assign GST/HST product posting groups to individual items and resources

1. Choose the ![Lightbulb that opens the Tell Me feature 8.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item** or **Resource**, and then choose the related link.  
2. Do one of the following:  

    * On the **Item** card, expand the **Price & Posting** FastTab, and then choose **Show more** to display the **GST/HST Product Posting Group** field.  
    * On the **Resource** card, expand the **Invoicing** FastTab.  
3. Choose the GST/HST product posting group.  

## <a name="set-up-clauses-to-explain-vat-exemption-or-non-standard-vat-rates" />Set up clauses to explain GST/HST exemption or non-standard GST/HST rates

You set up a GST/HST clause to describe information about the type of GST/HST that is being applied. The information may be required by government regulations. After you set up a GST/HST clause, and associate it with a GST/HST posting setup, the GST/HST clause is displayed on printed sales documents that use the GST/HST posting setup group.

If needed, you can also specify how to translate GST/HST clauses to other languages. Then, when you create and print a sales document that contains a GST/HST identifier, the document will include the translated GST/HST clause. The language code specified on the customer card determines the language.

When non-standard GST/HST rates are used in different types of documents, such as invoices or credit memos, companies are usually required to include an exemption text (GST/HST clause) stating why a reduced GST/HST or zero GST/HST rate has been calculated. You can define different GST/HST clauses to be included on business documents per the type of document, such as invoice or credit memo. You do this on the **GST/HST Clauses by Document Type** page.

You can modify or delete a GST/HST clause, and your modifications will be reflected in a generated report. However, [!INCLUDE[prod_short](includes/prod_short.md)] does not keep a history of the change. On the report, the GST/HST clause descriptions are printed and displayed for all lines in the report alongside the GST/HST amount and the GST/HST base amount. If a GST/HST clause has not been defined for any lines on the sales document, then the whole section is omitted when the report is printed.

### <a name="to-set-up-vat-clauses" />To set up GST/HST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 9.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Clauses**, and then choose the related link.  
2. On the **GST/HST Clauses** page, create a new line.  
3. In the **Code** field, enter an identifier for the clause. You use this code to assign the clause to GST/HST posting groups.  
4. In the **Description** field, enter the GST/HST exemption text that you want to display on documents that can include GST/HST. In the **Description 2** field, enter more text, if needed. The text will be displayed on new document lines.
5. Choose the **Description by document type** action.
6. On the **GST/HST Clauses by Document Type** page, fill in the fields to set up which GST/HST exemption text to display for which document type.  
7. Optional: To assign the GST/HST clause to a GST/HST posting setup right away, choose **Setup**, and then choose the clause. If you want to wait, you can assign the clause later on the **GST/HST Posting Setup** page.  
8. Optional: To specify how to translate the GST/HST clause, choose the **Translations** action.

### <a name="to-assign-a-vat-clause-to-a-vat-posting-setup" />To assign a GST/HST clause to a GST/HST posting setup

1. Choose the ![Lightbulb that opens the Tell Me feature 10.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then choose the related link.  
2. In the **GST/HST Clause** column, choose the clause to use for each GST/HST posting setup it applies to.  

### <a name="to-specify-translations-for-vat-clauses" />To specify translations for GST/HST clauses

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Clauses**, and then choose the related link.  
2. Choose the **Translations** action.  
3. In the **Language Code** field, choose the language you are translating to.  
4. In the **Description** and **Description 2** fields, enter the translations of the descriptions. This text displays in the translated GST/HST report documents.  

### <a name="to-specify-extended-text-for-vat-clauses" />To specify extended text for GST/HST clauses

> [!NOTE]  
> If your country or region requires longer text for the GST/HST clauses than the default version supports, you can specify the longer text for the GST/HST clauses as *extended text* so that it prints on the sales and purchase reports.  

1. Choose the ![Lightbulb that opens the Tell Me feature 11.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Clauses**, and then choose the related link.  
2. Choose the **Extended Text** action.  
3. Choose the **New** action.  
4. Fill in the **Language Code** and **Description** fields.  
5. Optionally, select the **All Language Codes** field, or specify the relevant language in the **Language Code** field if you use language codes.  
6. Fill in the **Starting Date** and **Ending Date** fields if you want to limit the dates on which the extended text is used.  
7. In the **Text** lines, write the extended text for your GST/HST clauses.  
8. Select the relevant fields for the document types where you want the extended text printed.  
9. Close the page.  

## <a name="create-a-vat-posting-setup-to-handle-import-vat" />Create a GST/HST posting setup to handle Import GST/HST

You use the *Import GST/HST* feature when you need to post a document where the entire amount is GST/HST. You will use this if you receive an invoice from the tax authorities for GST/HST for imported goods.  

To set up codes for import GST/HST, follow these steps:  

1. Choose the ![Lightbulb that opens the Tell Me feature 12.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST product Posting Groups**, and then choose the related link.  
2. On the GST/HST product Posting Groups page, set up a new GST/HST product posting group for import GST/HST.  
3. Choose the ![Lightbulb that opens the Tell Me feature 13.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Posting Setup**, and then choose the related link.  
4. On the GST/HST Posting Setup page, create a new line, or use an existing GST/HST business posting groups in combination with the new GST/HST product posting group for import GST/HST.  
5. In the **GST/HST Calculation Type** field, choose **Full GST/HST**.  
6. In the **Purchase GST/HST Account** field, enter the general ledger account to use for posting import GST/HST. All other accounts are optional.  

## <a name="use-reverse-charge-vat-for-trade-between-eu-countries-or-regions" />Use reverse charge GST/HST for trade between EU countries or regions

Some companies must use reverse charge VAT when trading with other companies. For example, this rule applies to purchases from EU countries/regions and sales to EU countries/regions.  

> [!NOTE]  
> This rule applies when trading with companies that are registered as GST/HST liable in another EU country/region. If you do business directly with consumers in other EU countries/regions, then you should contact your tax authority for applicable VAT rules.  

> [!TIP]  
> You can verify that a company is registered as VAT liable in another EU country by using the EU VAT Registration Number Validation service. The service is available for free in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Verify VAT registration numbers](finance-how-validate-vat-registration-number.md).

### <a name="sales-to-eu-countries-or-regions" />Sales to EU countries or regions

VAT is not calculated on sales to VAT-liable companies in other EU countries/regions. You must report the value of these sales to EU countries/regions separately on your VAT statement.  

To correctly calculate VAT on sales to EU countries/regions, you should:  

* Set up a line for sales with the same information for purchases. If you have already set up lines on the **VAT Posting Setup** page for purchases from EU countries/regions, then you can also use these lines for sales.  
* Assign the VAT business posting groups in the **VAT Bus. Posting Group** field on the **Invoicing** FastTab of the customer card of each EU customer. You should also enter the customer's VAT registration number in the **VAT Registration No.** field on the **Foreign Trade** FastTab.  

When you post a sale to a customer in another EU country/region, the VAT amount is calculated, and a VAT entry is created by using the information about the reverse charge VAT and the VAT base, which is the amount that is used to calculate the VAT amount. No entries are posted to the tax accounts in the general ledger.

If you want to use combination of GST/HST business posting group and GST/HST product posting group for reporting as services in the periodic GST/HST reports, mark the **EU Service** field.

> [!NOTE]  
> The **EU Service** field is only applicable for GST/HST reports. The field isn't related to the **Service Declaration** or **Intrastat for Services** features.

## <a name="vat-rounding-for-documents" />GST/HST rounding for documents

Amounts in documents that are not yet posted are rounded and displayed to correspond with the final rounding of amounts that are actually posted. GST/HST is calculated for a complete document, which means that GST/HST is calculated based on the sum of all lines with the same GST/HST identifier in the document.  

## <a name="set-up-vat-reporting" />Set up GST/HST reporting

You must set up information about how the tax authorities in your country or region require you to submit GST/HST reports. The following steps illustrate the most commonly used information. However, your country or region may require other steps. For more information, see the relevant article in the *Local functionality* section in the panel to the left.

[!INCLUDE [vat-report-setup](includes/vat-report-setup.md)]

## <a name="see-related-microsoft-trainingtrainingpathsprocess-vat-dynamics-365-business-central" />See related [Microsoft training](/training/paths/process-vat-dynamics-365-business-central/)

## <a name="see-also" />See also

[Set Up GST/HST Statement Templates and GST/HST Statement Names](finance-how-setup-vat-statement.md)  
[Set Up Unrealized GST/HST](finance-setup-unrealized-vat.md)  
[Report GST/HST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST/HST on Sales and Purchases](finance-work-with-vat.md)  
[Work with the GST/HST Rate Change Tool](finance-how-use-vat-rate-change-tool.md)  
[Verify VAT identification numbers](finance-how-validate-vat-registration-number.md)  
[Local functionality in Business Central](about-localization.md)  
[VAT Reporting in the German version](LocalFunctionality/Germany/vat-reporting.md)  
[Belgian VAT](LocalFunctionality/Belgium/belgian-vat.md)  
[Italian VAT](LocalFunctionality/Italy/italian-vat.md)  
[Set Up Electronic VAT and ICP Declarations in the Dutch Version](LocalFunctionality/Netherlands/how-to-set-up-electronic-vat-and-icp-declarations.md)  
[VAT Reports in the Spanish Version](LocalFunctionality/Spain/vat-reports.md)  
[Set Up Goods and Services Tax Posting in the Australian Version](LocalFunctionality/Australia/how-to-set-up-goods-and-service-tax-posting.md)  
[VAT in the Czech Version](LocalFunctionality/Czech/finance-vat.md)  
[VAT Reporting in the Norwegian Version](LocalFunctionality/Norway/norwegian-vat-reporting.md)  
[Reporting Goods/Services Tax and Harmonized Sales Tax in Canada](LocalFunctionality/Canada/sales-tax-goods-services.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
