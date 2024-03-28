---
title: Set Up a GST/HST Statement
description: This topic tells you how to set Up a GST/HST Statement Template and GST/HST Statement Names to meet changing tax authority requirements.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'VAT, posting, tax, value-added tax'
ms.search.form: '317, 318, 320, 474'
ms.date: 06/16/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Set Up GST/HST Statement Templates and GST/HST Statement Names

Tax authorities can, and do, change their requirements for posting GST/HST. GST/HST Statement templates and GST/HST statement names can help you prepare for upcoming changes and make a smooth transition to the new requirements. You can use GST/HST statement templates to setup different Reports when choosing to print the statement. Each GST/HST Statement Template can have multiple GST/HST Statement names which in turn define the calculations, and you can create a new GST/HST statement name when requirements change. For example, one name might calculate GST/HST for this year based on the current requirements, and another might calculate GST/HST based on requirements for next year. Names are also a way to keep a history of GST/HST statement formats, for example, so that you can look back to see how you calculated GST/HST in previous years.

## To define a GST/HST statement

GST/HST statements let you calculate your GST/HST settlement amount for a certain period, for example, a quarter.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **GST/HST Statements**, and then choose the related link.  
2. Choose the **Name** field, and then choose **New** on the **GST/HST Statement Names** page.
3. Fill in the required fields. Usually you want to have a setting for each GST/HST Bus. Posting Group / GST/HST Prod. Posting Group combination. For Row numbers it does make sense to use equvalent numbers or codes as in your official GST/HST Statement [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

> [!Tip]
> You can filter the information that the statement will include, depending on what you choose in the **Type** field. **Account Totalling** is useful when you want the GST/HST from a specific account.
**GST/HST Entry Totalling** gets GST/HST from the accounts assigned to the selections in the **Gen. Posting Type**, **GST/HST Bus. Posting Group**, and/or the **GST/HST Prod. Posting Group** fields. **Row Totalling** lets you enter a value or quick filter criteria in the **Row Totalling** field. For more information, see [Searching, filtering, and Sorting Data](ui-enter-criteria-filters.md). **Description** is often used to add a note to the statement. For example, you could use it as a heading when you've used row totalling.

## To preview the GST/HST statement

After you define a GST/HST statement, you can preview it to make sure it meets your needs.
> [!Tip]
> It is best practice to have one section in the GST/HST Statement using **Type** **GST/HST Entry Totalling** and another section below using **Type** **Account Totalling** to reconcile the amounts based on the **GST/HST Entry** table compared to the amount on the **G/L Accounts**. You can also use the **G/L - GST/HST Reconciliation** Report for this purpose.

1. Choose **Preview**.
2. Enter a date filter to limit the statement to a specific period. For more information about how to customize the page to show the date filter, see [Searching, filtering, and Sorting Data](ui-enter-criteria-filters.md).
3. You can select various options to specify the type of GST/HST entries to include in the statement.
4. On the lines where the **Type** field contains **GST/HST Entry Totalling** you can see a list of GST/HST entries by choosing the amount in the **Column Amount** field.
5. You can use personalization to show more fields in the lines. For example the Unrealized Base Amount and Unrealized GST/HST Amount, if you are using unrealized GST/HST.

## See also 

[Set Up GST/HST](finance-setup-vat.md)  
[Setting Up Unrealized GST/HST](finance-setup-unrealized-vat.md)  
[Report GST/HST to a Tax Authority](finance-how-report-vat.md)  
[Work with GST/HST on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
