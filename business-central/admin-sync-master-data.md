---
title: Manage Master Data Synchronization
description: Learn how manage master data synchronization.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bnielse
ms.service: dynamics-365-business-central
ms.topic: conceptual
ms.date: 01/25/2023
ms.custom: bap-template
ms.search.form: '7230, 7233, 5338, 7236, 672, 7234'
---
# Manage Master Data Synchronization

After you set up master data synchronization and synchronize for the first time, records in the selected tables are coupled and a recurring job queue entry is created for each table. The job queue entries automatically synchronize data in the subsidiary companies when someone makes a change in the source company. Otherwise, you don't need to do anything.

> [!NOTE]
> By default, the job queue entries are scheduled run every minute, and you can't change the schedule.

However, sometimes things go wrong, and there might be situations that you need to manage or investigate. For example, if people change the same record in both the source company and a subsidiary, synchronization will fail so that you can specify the change that's correct. Or, the source company might install an extension that changes the schema of one of the tables your synchronizing by adding a field or two. If you want to synchronize the new fields in the subsidiaries, you'll need to install the same extensions and update the table schemas in their setup.

This article describes the tools you can use to keep synchronization running smoothly.

## Investigate the status of synchronization

There are two actions on the **Synchronization Tables** page that can help you monitor your synchronization:

* **Integration Synchronization Jobs**
* **Job Queue Entries**

The following table describes the actions.

|Page  |Description  |
|---------|---------|
|**Integration Synchronization Jobs**     | Open the **Integration Synchronization Jobs** page to investigate what happened each time a job queue entry ran. To dig deeper into the details about new records that were added, or explore why a record failed to synchronize, choose the numbers in the **Inserted** or **Failed** columns. You can also use this page to clean up older records that you might not need. To learn more about cleaning up, go to [Clean up old entries](#clean-up-old-entries).        |
|**Job Queue Entries**     | Access details about the job queue entry that synchronize data for a selected table. For example, use this page to manage the status of the job queue entry,    To learn more about job queue entries, go to [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).     |

> [!NOTE]
> If you find an error on the **Integration Synchronization Jobs** page that you can't resolve yourself, if you contact your partner or Microsoft for support, it's helpful to provide the error message and callstack information.

## Synchronize modified records

If you change a setting for a table or field in a subsidiary, you must update the synchronization. For example, if you decide to select the **Overwrite Local Change** checkbox on a field to allow data from the source company to overwrite local changes. To update the synchronization, use the **Synchronize Modified Records** action on the **Synchronization Tables** page.

## Update table schemas

If the source company changes a table, for example, by adding a field that you want to synchronize, subsidiaries must update their field mappings. On the **Synchronization Fields** page, use the **Update Fields** action. 

## Enable or disable couplings between records

To start or stop coupling on specific records on a table, on the **Synchronization Fields** page, choose the fields, and then use either the **Enable** or **Disable** actions. 

> [!TIP]
> A fast way to enable or disable multiple fields at the same time is to select them in the list, and then use either the **Enable** or **Disable** actions.

## Adding extensions

If the source company installs a new extension, the subsidiary must also install it if they want to synchronize data for it. The subsidiary can use the **Update Fields** action On the **Synchronization Fields** page to add the tables from the extension to the list.

> [!NOTE]
> Some tables get data from related tables. If you add an extension that doesn't include related tables, the fields on those tables won't be available. Verify that you've added all related tables.

## Clean up old entries

Over time, the number of entries in the synchronization log will become large, so you might want to do a little housekeeping to remove unneeded entries. To make it easier to clean up old entries, the **Integration Synchronization Jobs** page offers the following actions:

* **Delete Entries Older Than 7 Days**
* **Delete All Entries**

<!--
## Recreate a deleted job queue entry

If the recurring job queue entry is deleted for a table, you can quickly recreate it. On the **Synchronization Tables** page, choose the **Use Default Synchronization Setup** action.
-->

## See Also

[Get ready to synchronize master data](admin-set-up-data-sync.md)
