---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Business Central.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: c8eba304746125e9262ebfff95cfd2379eec08c8
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-CA
ms.lasthandoff: 10/01/2019
ms.locfileid: "2311341"
---
# <a name="the-c5-data-migration-extension"></a><span data-ttu-id="aa881-103">The C5 Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="aa881-103">The C5 Data Migration Extension</span></span>
<span data-ttu-id="aa881-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="aa881-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="aa881-105">You can also migrate historical entries for general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="aa881-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="aa881-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span><span class="sxs-lookup"><span data-stu-id="aa881-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="aa881-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span><span class="sxs-lookup"><span data-stu-id="aa881-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="aa881-108">What Data is Migrated?</span><span class="sxs-lookup"><span data-stu-id="aa881-108">What Data is Migrated?</span></span>
<span data-ttu-id="aa881-109">The following data is migrated for each entity:</span><span class="sxs-lookup"><span data-stu-id="aa881-109">The following data is migrated for each entity:</span></span>

<span data-ttu-id="aa881-110">**Customers**</span><span class="sxs-lookup"><span data-stu-id="aa881-110">**Customers**</span></span>
* <span data-ttu-id="aa881-111">Contacts</span><span class="sxs-lookup"><span data-stu-id="aa881-111">Contacts</span></span>  
* <span data-ttu-id="aa881-112">Location</span><span class="sxs-lookup"><span data-stu-id="aa881-112">Location</span></span>
* <span data-ttu-id="aa881-113">Country</span><span class="sxs-lookup"><span data-stu-id="aa881-113">Country</span></span>
* <span data-ttu-id="aa881-114">Customer dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="aa881-114">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="aa881-115">Shipment method</span><span class="sxs-lookup"><span data-stu-id="aa881-115">Shipment method</span></span>
* <span data-ttu-id="aa881-116">Sales Person</span><span class="sxs-lookup"><span data-stu-id="aa881-116">Sales Person</span></span>
* <span data-ttu-id="aa881-117">Payment terms</span><span class="sxs-lookup"><span data-stu-id="aa881-117">Payment terms</span></span>
* <span data-ttu-id="aa881-118">Payment method</span><span class="sxs-lookup"><span data-stu-id="aa881-118">Payment method</span></span>
* <span data-ttu-id="aa881-119">Customer price group</span><span class="sxs-lookup"><span data-stu-id="aa881-119">Customer price group</span></span>
* <span data-ttu-id="aa881-120">Customer invoice discount</span><span class="sxs-lookup"><span data-stu-id="aa881-120">Customer invoice discount</span></span>

<span data-ttu-id="aa881-121">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="aa881-121">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="aa881-122">Customer posting setup</span><span class="sxs-lookup"><span data-stu-id="aa881-122">Customer posting setup</span></span>
* <span data-ttu-id="aa881-123">General journal batch</span><span class="sxs-lookup"><span data-stu-id="aa881-123">General journal batch</span></span>
* <span data-ttu-id="aa881-124">Open transactions (customer ledger entries)</span><span class="sxs-lookup"><span data-stu-id="aa881-124">Open transactions (customer ledger entries)</span></span>

<span data-ttu-id="aa881-125">**Vendors**</span><span class="sxs-lookup"><span data-stu-id="aa881-125">**Vendors**</span></span>
* <span data-ttu-id="aa881-126">Contacts</span><span class="sxs-lookup"><span data-stu-id="aa881-126">Contacts</span></span>
* <span data-ttu-id="aa881-127">Location</span><span class="sxs-lookup"><span data-stu-id="aa881-127">Location</span></span>
* <span data-ttu-id="aa881-128">Country</span><span class="sxs-lookup"><span data-stu-id="aa881-128">Country</span></span>
* <span data-ttu-id="aa881-129">Vendor dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="aa881-129">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="aa881-130">Invoice discount</span><span class="sxs-lookup"><span data-stu-id="aa881-130">Invoice discount</span></span>
* <span data-ttu-id="aa881-131">Shipment method</span><span class="sxs-lookup"><span data-stu-id="aa881-131">Shipment method</span></span>
* <span data-ttu-id="aa881-132">Purchaser</span><span class="sxs-lookup"><span data-stu-id="aa881-132">Purchaser</span></span>
* <span data-ttu-id="aa881-133">Payment terms</span><span class="sxs-lookup"><span data-stu-id="aa881-133">Payment terms</span></span>
* <span data-ttu-id="aa881-134">Payment method</span><span class="sxs-lookup"><span data-stu-id="aa881-134">Payment method</span></span>
* <span data-ttu-id="aa881-135">Vendor invoice discount</span><span class="sxs-lookup"><span data-stu-id="aa881-135">Vendor invoice discount</span></span>

<span data-ttu-id="aa881-136">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="aa881-136">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="aa881-137">Vendor posting setup</span><span class="sxs-lookup"><span data-stu-id="aa881-137">Vendor posting setup</span></span>
* <span data-ttu-id="aa881-138">General journal batch</span><span class="sxs-lookup"><span data-stu-id="aa881-138">General journal batch</span></span>
* <span data-ttu-id="aa881-139">Open transactions (vendor ledger entries)</span><span class="sxs-lookup"><span data-stu-id="aa881-139">Open transactions (vendor ledger entries)</span></span>

<span data-ttu-id="aa881-140">**Items**</span><span class="sxs-lookup"><span data-stu-id="aa881-140">**Items**</span></span>
* <span data-ttu-id="aa881-141">Location</span><span class="sxs-lookup"><span data-stu-id="aa881-141">Location</span></span>
* <span data-ttu-id="aa881-142">Country</span><span class="sxs-lookup"><span data-stu-id="aa881-142">Country</span></span>
* <span data-ttu-id="aa881-143">Item dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="aa881-143">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="aa881-144">Sales line discounts</span><span class="sxs-lookup"><span data-stu-id="aa881-144">Sales line discounts</span></span>
* <span data-ttu-id="aa881-145">Customer discount groups</span><span class="sxs-lookup"><span data-stu-id="aa881-145">Customer discount groups</span></span>
* <span data-ttu-id="aa881-146">Item discount groups</span><span class="sxs-lookup"><span data-stu-id="aa881-146">Item discount groups</span></span>
* <span data-ttu-id="aa881-147">Sales price</span><span class="sxs-lookup"><span data-stu-id="aa881-147">Sales price</span></span>
* <span data-ttu-id="aa881-148">Tariff number</span><span class="sxs-lookup"><span data-stu-id="aa881-148">Tariff number</span></span>
* <span data-ttu-id="aa881-149">Units of measure</span><span class="sxs-lookup"><span data-stu-id="aa881-149">Units of measure</span></span>
* <span data-ttu-id="aa881-150">Item tracking code</span><span class="sxs-lookup"><span data-stu-id="aa881-150">Item tracking code</span></span>
* <span data-ttu-id="aa881-151">Customer price group</span><span class="sxs-lookup"><span data-stu-id="aa881-151">Customer price group</span></span>
* <span data-ttu-id="aa881-152">Assembly BOMs</span><span class="sxs-lookup"><span data-stu-id="aa881-152">Assembly BOMs</span></span>

<span data-ttu-id="aa881-153">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="aa881-153">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="aa881-154">Inventory posting setup</span><span class="sxs-lookup"><span data-stu-id="aa881-154">Inventory posting setup</span></span>
* <span data-ttu-id="aa881-155">General posting setup</span><span class="sxs-lookup"><span data-stu-id="aa881-155">General posting setup</span></span>
* <span data-ttu-id="aa881-156">Item journal batch</span><span class="sxs-lookup"><span data-stu-id="aa881-156">Item journal batch</span></span>
* <span data-ttu-id="aa881-157">Open transactions (item ledger entries)</span><span class="sxs-lookup"><span data-stu-id="aa881-157">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="aa881-158">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span><span class="sxs-lookup"><span data-stu-id="aa881-158">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="aa881-159">Other exchange rates are not migrated.</span><span class="sxs-lookup"><span data-stu-id="aa881-159">Other exchange rates are not migrated.</span></span>

<span data-ttu-id="aa881-160">**Chart of Accounts**</span><span class="sxs-lookup"><span data-stu-id="aa881-160">**Chart of Accounts**</span></span>  
* <span data-ttu-id="aa881-161">Standard dimensions: Department, Cost Centre, Purpose</span><span class="sxs-lookup"><span data-stu-id="aa881-161">Standard dimensions: Department, Cost Center, Purpose</span></span>  
* <span data-ttu-id="aa881-162">Historical G/L transactions</span><span class="sxs-lookup"><span data-stu-id="aa881-162">Historical G/L transactions</span></span>  

> [!Note]
> <span data-ttu-id="aa881-163">Historical G/L transactions are treated a little differently.</span><span class="sxs-lookup"><span data-stu-id="aa881-163">Historical G/L transactions are treated a little differently.</span></span> <span data-ttu-id="aa881-164">When you migrate data you set a **Current Period** parameter.</span><span class="sxs-lookup"><span data-stu-id="aa881-164">When you migrate data you set a **Current Period** parameter.</span></span> <span data-ttu-id="aa881-165">This parameter specifies how to process G/L transactions.</span><span class="sxs-lookup"><span data-stu-id="aa881-165">This parameter specifies how to process G/L transactions.</span></span> <span data-ttu-id="aa881-166">Transactions after this date are migrated individually.</span><span class="sxs-lookup"><span data-stu-id="aa881-166">Transactions after this date are migrated individually.</span></span> <span data-ttu-id="aa881-167">Transactions before this date are aggregated per account and migrated as a single amount.</span><span class="sxs-lookup"><span data-stu-id="aa881-167">Transactions before this date are aggregated per account and migrated as a single amount.</span></span> <span data-ttu-id="aa881-168">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span><span class="sxs-lookup"><span data-stu-id="aa881-168">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span></span> <span data-ttu-id="aa881-169">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span><span class="sxs-lookup"><span data-stu-id="aa881-169">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span></span> <span data-ttu-id="aa881-170">All trascations after this date will be migrated individually.</span><span class="sxs-lookup"><span data-stu-id="aa881-170">All trascations after this date will be migrated individually.</span></span>

## <a name="file-size-requirements"></a><span data-ttu-id="aa881-171">File Size Requirements</span><span class="sxs-lookup"><span data-stu-id="aa881-171">File Size Requirements</span></span>
<span data-ttu-id="aa881-172">The largest file size you can upload to [!INCLUDE[d365fin](includes/d365fin_md.md)] is 150 MB.</span><span class="sxs-lookup"><span data-stu-id="aa881-172">The largest file size you can upload to [!INCLUDE[d365fin](includes/d365fin_md.md)] is 150 MB.</span></span> <span data-ttu-id="aa881-173">If the file you export from C5 is larger than that, consider migrating data in multiple files.</span><span class="sxs-lookup"><span data-stu-id="aa881-173">If the file you export from C5 is larger than that, consider migrating data in multiple files.</span></span> <span data-ttu-id="aa881-174">For example, export one or two types of entities from C5, such as customers and vendors, to a file, and then export items to another file, and so on.</span><span class="sxs-lookup"><span data-stu-id="aa881-174">For example, export one or two types of entities from C5, such as customers and vendors, to a file, and then export items to another file, and so on.</span></span> <span data-ttu-id="aa881-175">You can import files individually in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="aa881-175">You can import files individually in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="aa881-176">To migrate data</span><span class="sxs-lookup"><span data-stu-id="aa881-176">To migrate data</span></span>
<span data-ttu-id="aa881-177">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="aa881-177">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="aa881-178">In C5, use the **Export Database** feature to export the data.</span><span class="sxs-lookup"><span data-stu-id="aa881-178">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="aa881-179">Then send the export folder to a compressed (zipped) folder.</span><span class="sxs-lookup"><span data-stu-id="aa881-179">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="aa881-180">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Migration**, and then choose **Data Migration**.</span><span class="sxs-lookup"><span data-stu-id="aa881-180">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="aa881-181">Complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="aa881-181">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="aa881-182">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span><span class="sxs-lookup"><span data-stu-id="aa881-182">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="aa881-183">Viewing the Status of the Migration</span><span class="sxs-lookup"><span data-stu-id="aa881-183">Viewing the Status of the Migration</span></span>
<span data-ttu-id="aa881-184">Use the **Data Migration Overview** page to monitor the success of the migration.</span><span class="sxs-lookup"><span data-stu-id="aa881-184">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="aa881-185">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span><span class="sxs-lookup"><span data-stu-id="aa881-185">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="aa881-186">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span><span class="sxs-lookup"><span data-stu-id="aa881-186">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="aa881-187">For more information, see the next section in this topic.</span><span class="sxs-lookup"><span data-stu-id="aa881-187">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="aa881-188">While you are waiting for the results of the migration, you must refresh the page to display the results.</span><span class="sxs-lookup"><span data-stu-id="aa881-188">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="how-to-avoid-double-posting"></a><span data-ttu-id="aa881-189">How to Avoid Double-Posting</span><span class="sxs-lookup"><span data-stu-id="aa881-189">How to Avoid Double-Posting</span></span>
<span data-ttu-id="aa881-190">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span><span class="sxs-lookup"><span data-stu-id="aa881-190">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span></span>  

* <span data-ttu-id="aa881-191">For vendors, we use the A/P account from the vendor posting group.</span><span class="sxs-lookup"><span data-stu-id="aa881-191">For vendors, we use the A/P account from the vendor posting group.</span></span>  
* <span data-ttu-id="aa881-192">For customers, we use the A/R account from the customer posting group.</span><span class="sxs-lookup"><span data-stu-id="aa881-192">For customers, we use the A/R account from the customer posting group.</span></span>  
* <span data-ttu-id="aa881-193">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span><span class="sxs-lookup"><span data-stu-id="aa881-193">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span></span>  

## <a name="correcting-errors"></a><span data-ttu-id="aa881-194">Correcting Errors</span><span class="sxs-lookup"><span data-stu-id="aa881-194">Correcting Errors</span></span>
<span data-ttu-id="aa881-195">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span><span class="sxs-lookup"><span data-stu-id="aa881-195">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="aa881-196">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span><span class="sxs-lookup"><span data-stu-id="aa881-196">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="aa881-197">The number in the **Error Count** field for the entity.</span><span class="sxs-lookup"><span data-stu-id="aa881-197">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="aa881-198">The entity, and then the **Show Errors** action.</span><span class="sxs-lookup"><span data-stu-id="aa881-198">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="aa881-199">On the **Data Migration Errors** page, to fix an error you can choose an error message, and then choose **Edit Record** to view the migrated data for the entity.</span><span class="sxs-lookup"><span data-stu-id="aa881-199">On the **Data Migration Errors** page, to fix an error you can choose an error message, and then choose **Edit Record** to view the migrated data for the entity.</span></span> <span data-ttu-id="aa881-200">If you have several errors to fix, you can choose **Bulk-Fix Errors** to edit the entities in a list.</span><span class="sxs-lookup"><span data-stu-id="aa881-200">If you have several errors to fix, you can choose **Bulk-Fix Errors** to edit the entities in a list.</span></span> <span data-ttu-id="aa881-201">You still need to open individual records if the error was caused by a related entry though.</span><span class="sxs-lookup"><span data-stu-id="aa881-201">You still need to open individual records if the error was caused by a related entry though.</span></span> <span data-ttu-id="aa881-202">For example, a vendor will not be migrated if an email address one of their contacts has an invalid format.</span><span class="sxs-lookup"><span data-stu-id="aa881-202">For example, a vendor will not be migrated if an email address one of their contacts has an invalid format.</span></span>

<span data-ttu-id="aa881-203">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span><span class="sxs-lookup"><span data-stu-id="aa881-203">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="aa881-204">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span><span class="sxs-lookup"><span data-stu-id="aa881-204">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="aa881-205">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span><span class="sxs-lookup"><span data-stu-id="aa881-205">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="aa881-206">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span><span class="sxs-lookup"><span data-stu-id="aa881-206">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="aa881-207">If an item variant is created first, the reference to the original item can cause an error message.</span><span class="sxs-lookup"><span data-stu-id="aa881-207">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="aa881-208">Verifying Data After Migrating</span><span class="sxs-lookup"><span data-stu-id="aa881-208">Verifying Data After Migrating</span></span>
<span data-ttu-id="aa881-209">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="aa881-209">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="aa881-210">Microsoft Dynamcis C5 2012</span><span class="sxs-lookup"><span data-stu-id="aa881-210">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]| <span data-ttu-id="aa881-211">Batch Job to Use</span><span class="sxs-lookup"><span data-stu-id="aa881-211">Batch Job to Use</span></span> |
|-----|-----|-----|
|<span data-ttu-id="aa881-212">Customer Entries</span><span class="sxs-lookup"><span data-stu-id="aa881-212">Customer Entries</span></span>| <span data-ttu-id="aa881-213">General Journals</span><span class="sxs-lookup"><span data-stu-id="aa881-213">General Journals</span></span>| <span data-ttu-id="aa881-214">CUSTMIGR</span><span class="sxs-lookup"><span data-stu-id="aa881-214">CUSTMIGR</span></span> |
|<span data-ttu-id="aa881-215">Vendor Entries</span><span class="sxs-lookup"><span data-stu-id="aa881-215">Vendor Entries</span></span>| <span data-ttu-id="aa881-216">General Journals</span><span class="sxs-lookup"><span data-stu-id="aa881-216">General Journals</span></span>| <span data-ttu-id="aa881-217">VENDMIGR</span><span class="sxs-lookup"><span data-stu-id="aa881-217">VENDMIGR</span></span>|
|<span data-ttu-id="aa881-218">Item Entries</span><span class="sxs-lookup"><span data-stu-id="aa881-218">Item Entries</span></span>| <span data-ttu-id="aa881-219">Item Journals</span><span class="sxs-lookup"><span data-stu-id="aa881-219">Item Journals</span></span>| <span data-ttu-id="aa881-220">ITEMMIGR</span><span class="sxs-lookup"><span data-stu-id="aa881-220">ITEMMIGR</span></span> |
|<span data-ttu-id="aa881-221">G/L Entries</span><span class="sxs-lookup"><span data-stu-id="aa881-221">G/L Entries</span></span>| <span data-ttu-id="aa881-222">General Journals</span><span class="sxs-lookup"><span data-stu-id="aa881-222">General Journals</span></span>| <span data-ttu-id="aa881-223">GLACMIGR</span><span class="sxs-lookup"><span data-stu-id="aa881-223">GLACMIGR</span></span> |

## <a name="stopping-data-migration"></a><span data-ttu-id="aa881-224">Stopping Data Migration</span><span class="sxs-lookup"><span data-stu-id="aa881-224">Stopping Data Migration</span></span>
<span data-ttu-id="aa881-225">You can stop migrating data by choosing **Stop All Migrations**.</span><span class="sxs-lookup"><span data-stu-id="aa881-225">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="aa881-226">If you do, all pending migrations are also stopped.</span><span class="sxs-lookup"><span data-stu-id="aa881-226">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="aa881-227">See Also</span><span class="sxs-lookup"><span data-stu-id="aa881-227">See Also</span></span>
<span data-ttu-id="aa881-228">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="aa881-228">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="aa881-229">Getting Started</span><span class="sxs-lookup"><span data-stu-id="aa881-229">Getting Started</span></span>](product-get-started.md)
