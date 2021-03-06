---
title: Set Up a VAT Statement | Microsoft Docs
description: Set Up a VAT Statement
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: VAT, posting, tax, value-added tax
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 8a7373a22cff16a32fe92bf2f2d9064d2f12e950
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775460"
---
# <a name="set-up-a-vat-statement"></a>Set Up a VAT Statement

## <a name="setting-up-vat-statement-templates-and-vat-statement-names"></a>Setting up Tax Statement Templates and Tax Statement Names
Tax authorities can, and do, change their requirements for posting Tax. Tax Statement templates and tax statement names can help you prepare for upcoming changes and make a smooth transition to the new requirements. You can use VAT statement templates to setup different Reports when choosing to print the statement. Each VAT Statement Template can have multiple VAT Statement names which in turn define the calculations, and you can create a new VAT statement Name when requirements change. For example, one name might calculate VAT for this year based on the current requirements, and another might calculate VAT based on requirements for next year. Names are also a way to keep a history of VAT statement formats, for example, so that you can look back to see how you calculated VAT in previous years.

## <a name="to-define-a-vat-statements"></a>To define a tax statement
Tax statements let you calculate your Tax settlement amount for a certain period, for example, a quarter.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Tax Statements**, and then choose the related link.  
2. Choose the **Name** field, and then choose **New** on the **Tax Statement Names** page.
3. Fill in the required fields. Usually you want to have a setting for each VAT Bus. Posting Group / VAT Prod. Posting Group combination. For Row numbers it does make sense to use equvalent numbers or codes as in your official VAT Statement [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] 


> [!Tip]
> You can filter the information that the statement will include, depending on what you choose in the **Type** field. **Account Totalling** is useful when you want the tax from a specific account.
**Tax Entry Totalling** gets Tax from the accounts assigned to the selections in the **Gen. Posting Type**, **Tax Bus. Posting Group**, and/or the **Tax Prod. Posting Group** fields. **Row Totalling** lets you enter a value or quick filter criteria in the **Row Totalling** field. For more information, see [Searching, filtering, and Sorting Data](ui-enter-criteria-filters.md). **Description** is often used to add a note to the statement. For example, you could use it as a heading when you've used row totalling.

## <a name="to-preview-the-vat-statement"></a>To preview the tax statement
After you define a Tax statement, you can preview it to make sure it meets your needs.
> [!Tip]
> It is best practice to have one section in the VAT Statement using **Type** **VAT Entry Totalling** and another section below using **Type** **Account Totalling** to reconcile the amounts based on the **VAT Entry** table compared to the amount on the **G/L Accounts**. You can also use the **G/L - VAT Reconciliation** Report for this purpose.

1. Choose **Preview**.
2. Enter a date filter to limit the statement to a specific period. For more information about how to customize the page to show the date filter, see [Searching, filtering, and Sorting Data](ui-enter-criteria-filters.md).
3. You can select various options to specify the type of Tax entries to include in the statement.
4. On the lines where the **Type** field contains **Tax Entry Totalling** you can see a list of Tax entries by choosing the amount in the **Column Amount** field.
5. You can use personalization to show more fields in the lines. For example the Unrealized Base Amount and Unrealized VAT Amount, if you are using unrealized VAT.

## <a name="see-also"></a>See Also  
[Set Up Value-Added Tax](finance-setup-vat.md)  
[Setting Up Unrealized Value Added Tax](finance-setup-unrealized-vat.md)      
[Report Tax to a Tax Authority](finance-how-report-vat.md)  
[Work with Tax on Sales and Purchases](finance-work-with-vat.md)  
[Local functionality in Business Central](about-localization.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]