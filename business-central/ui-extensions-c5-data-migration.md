---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Business Central.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 04/09/208
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: fa6779ee8fb2bbb453014e32cb7f3cf8dcfa18da
ms.openlocfilehash: 698bde6949c6053501881d07135586810fc81bdd
ms.contentlocale: en-ca
ms.lasthandoff: 04/11/2018

---

# <a name="the-c5-data-migration-extension-for-business-central"></a>The C5 Data Migration Extension for Business Central
This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)]. You can also migrate historical entries for general ledger accounts.

> [!Note]
> The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data. Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.

## <a name="what-data-is-migrated"></a>What Data is Migrated?
The following data is migrated for each entity:

**Customers**
* Location
* Country
* Customer dimensions (department, centre, purpose)
* Shipment method
* Sales Person
* Payment terms
* Payment method
* Customer price group
* Customer invoice discount

If you migrate accounts, the following data is also migrated:

* Customer posting setup
* General journal batch
* Open transactions (customer ledger entries)

**Vendors**
* Location
* Country
* Vendor dimensions (department, centre, purpose)
* Invoice discount
* Shipment method
* Purchaser
* Payment terms
* Payment method
* Vendor invoice discount

If you migrate accounts, the following data is also migrated:

* Vendor posting setup
* General journal batch
* Open transactions (vendor ledger entries)

**Items**
* Location
* Country
* Item dimensions (department, centre, purpose)
* Sales line discounts
* Customer discount groups
* Item discount groups
* Sales price
* Tariff number
* Units of measure
* Item tracking code
* Customer price group

If you migrate accounts, the following data is also migrated:

* Inventory posting setup
* General posting setup
* Item journal batch
* Open transactions (item ledger entries)

> [!Note]
> If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated. Other exchange rates are not migrated.

**Chart of Accounts**  
* Standard dimensions: Department, Cost Centre, Purpose  
* Historical G/L transactions  

> [!Note]
> Historical G/L transactions are treated a little differently. When you migrate data you set a **Current Period** parameter. This parameter specifies how to process G/L transactions. Transactions after this date are migrated individually. Transactions before this date are aggregated per account and migrated as a single amount. For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field. For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account. All trascations after this date will be migrated individually.

## <a name="to-migrate-data"></a>To migrate data
There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:  

1. In C5, use the **Export Database** feature to export the data. Then send the export folder to a compressed (zipped) folder.  
2. In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.  
3. Complete the steps in the assisted setup guide. Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.  

> [!Note]
> Companies often add fields to customize C5 for their specific line of business. [!INCLUDE[d365fin](includes/d365fin_md.md)] does not migrate data from custom fields. Also, migration will fail if you have more than 10 custom fields.

## <a name="viewing-the-status-of-the-migration"></a>Viewing the Status of the Migration
Use the **Data Migration Overview** page to monitor the success of the migration. The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull. It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues. For more information, see the next section in this topic.  

> [!Note]
> While you are waiting for the results of the migration, you must refresh the page to display the results.

## <a name="how-to-avoid-double-posting"></a>How to Avoid Double-Posting
To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:  
  
* For vendors, we use the A/P account from the vendor posting group.  
* For customers, we use the A/R account from the customer posting group.  
* For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.  

## <a name="correcting-errors"></a>Correcting Errors
If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many. To view a list of the errors, you can open the **Data Migration Errors** page by choosing:  

* The number in the **Error Count** field for the entity.  
* The entity, and then the **Show Errors** action.  

On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity. After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.  

> [!Tip]
> If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate. Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.

> [!Note]
> If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it. If an item variant is created first, the reference to the original item can cause an error message.  

## <a name="verifying-data-after-migrating"></a>Verifying Data After Migrating
One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].

|Microsoft Dynamcis C5 2012 | [!INCLUDE[d365fin](includes/d365fin_md.md)]| Batch Job to Use |
|-----|-----|-----|
|Customer Entries| General Journals| CUSTMIGR |
|Vendor Entries| General Journals| VENDMIGR|
|Item Entries| Item Journals| ITEMMIGR |
|G/L Entries| General Journals| GLACMIGR |

## <a name="stopping-data-migration"></a>Stopping Data Migration
You can stop migrating data by choosing **Stop All Migrations**. If you do, all pending migrations are also stopped.

## <a name="see-also"></a>See Also
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  
[Getting Started](product-get-started.md) 
