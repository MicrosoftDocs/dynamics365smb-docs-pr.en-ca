---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Financials.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 11/21/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: d3b8d3d01ce75da59c1cce873077955776963ce9
ms.contentlocale: en-ca
ms.lasthandoff: 03/22/2018

---

# <a name="the-c5-data-migration-extension-for-finance-and-operations-business-edition"></a><span data-ttu-id="e80b7-103">The C5 Data Migration Extension for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="e80b7-103">The C5 Data Migration Extension for Finance and Operations, Business edition</span></span>
<span data-ttu-id="e80b7-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e80b7-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e80b7-105">You can also migrate historical entries for general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="e80b7-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="e80b7-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span><span class="sxs-lookup"><span data-stu-id="e80b7-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="e80b7-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span><span class="sxs-lookup"><span data-stu-id="e80b7-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

##<a name="what-data-is-migrated"></a><span data-ttu-id="e80b7-108">What Data is Migrated?</span><span class="sxs-lookup"><span data-stu-id="e80b7-108">What Data is Migrated?</span></span>
<span data-ttu-id="e80b7-109">The following data is migrated for each entity:</span><span class="sxs-lookup"><span data-stu-id="e80b7-109">The following data is migrated for each entity:</span></span>

<span data-ttu-id="e80b7-110">**Customers**</span><span class="sxs-lookup"><span data-stu-id="e80b7-110">**Customers**</span></span>
* <span data-ttu-id="e80b7-111">Location</span><span class="sxs-lookup"><span data-stu-id="e80b7-111">Location</span></span>
* <span data-ttu-id="e80b7-112">Country</span><span class="sxs-lookup"><span data-stu-id="e80b7-112">Country</span></span>
* <span data-ttu-id="e80b7-113">Customer dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="e80b7-113">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="e80b7-114">Shipment method</span><span class="sxs-lookup"><span data-stu-id="e80b7-114">Shipment method</span></span>
* <span data-ttu-id="e80b7-115">Sales Person</span><span class="sxs-lookup"><span data-stu-id="e80b7-115">Sales Person</span></span>
* <span data-ttu-id="e80b7-116">Payment terms</span><span class="sxs-lookup"><span data-stu-id="e80b7-116">Payment terms</span></span>
* <span data-ttu-id="e80b7-117">Payment method</span><span class="sxs-lookup"><span data-stu-id="e80b7-117">Payment method</span></span>
* <span data-ttu-id="e80b7-118">Customer price group</span><span class="sxs-lookup"><span data-stu-id="e80b7-118">Customer price group</span></span>
* <span data-ttu-id="e80b7-119">Customer invoice discount</span><span class="sxs-lookup"><span data-stu-id="e80b7-119">Customer invoice discount</span></span>

<span data-ttu-id="e80b7-120">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="e80b7-120">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="e80b7-121">Customer posting setup</span><span class="sxs-lookup"><span data-stu-id="e80b7-121">Customer posting setup</span></span>
* <span data-ttu-id="e80b7-122">General journal batch</span><span class="sxs-lookup"><span data-stu-id="e80b7-122">General journal batch</span></span>
* <span data-ttu-id="e80b7-123">Open transactions (customer ledger entries)</span><span class="sxs-lookup"><span data-stu-id="e80b7-123">Open transactions (customer ledger entries)</span></span>

<span data-ttu-id="e80b7-124">**Vendors**</span><span class="sxs-lookup"><span data-stu-id="e80b7-124">**Vendors**</span></span>
* <span data-ttu-id="e80b7-125">Location</span><span class="sxs-lookup"><span data-stu-id="e80b7-125">Location</span></span>
* <span data-ttu-id="e80b7-126">Country</span><span class="sxs-lookup"><span data-stu-id="e80b7-126">Country</span></span>
* <span data-ttu-id="e80b7-127">Vendor dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="e80b7-127">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="e80b7-128">Invoice discount</span><span class="sxs-lookup"><span data-stu-id="e80b7-128">Invoice discount</span></span>
* <span data-ttu-id="e80b7-129">Shipment method</span><span class="sxs-lookup"><span data-stu-id="e80b7-129">Shipment method</span></span>
* <span data-ttu-id="e80b7-130">Purchaser</span><span class="sxs-lookup"><span data-stu-id="e80b7-130">Purchaser</span></span>
* <span data-ttu-id="e80b7-131">Payment terms</span><span class="sxs-lookup"><span data-stu-id="e80b7-131">Payment terms</span></span>
* <span data-ttu-id="e80b7-132">Payment method</span><span class="sxs-lookup"><span data-stu-id="e80b7-132">Payment method</span></span>
* <span data-ttu-id="e80b7-133">Vendor invoice discount</span><span class="sxs-lookup"><span data-stu-id="e80b7-133">Vendor invoice discount</span></span>

<span data-ttu-id="e80b7-134">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="e80b7-134">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="e80b7-135">Vendor posting setup</span><span class="sxs-lookup"><span data-stu-id="e80b7-135">Vendor posting setup</span></span>
* <span data-ttu-id="e80b7-136">General journal batch</span><span class="sxs-lookup"><span data-stu-id="e80b7-136">General journal batch</span></span>
* <span data-ttu-id="e80b7-137">Open transactions (vendor ledger entries)</span><span class="sxs-lookup"><span data-stu-id="e80b7-137">Open transactions (vendor ledger entries)</span></span>

<span data-ttu-id="e80b7-138">**Items**</span><span class="sxs-lookup"><span data-stu-id="e80b7-138">**Items**</span></span>
* <span data-ttu-id="e80b7-139">Location</span><span class="sxs-lookup"><span data-stu-id="e80b7-139">Location</span></span>
* <span data-ttu-id="e80b7-140">Country</span><span class="sxs-lookup"><span data-stu-id="e80b7-140">Country</span></span>
* <span data-ttu-id="e80b7-141">Item dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="e80b7-141">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="e80b7-142">Sales line discounts</span><span class="sxs-lookup"><span data-stu-id="e80b7-142">Sales line discounts</span></span>
* <span data-ttu-id="e80b7-143">Customer discount groups</span><span class="sxs-lookup"><span data-stu-id="e80b7-143">Customer discount groups</span></span>
* <span data-ttu-id="e80b7-144">Item discount groups</span><span class="sxs-lookup"><span data-stu-id="e80b7-144">Item discount groups</span></span>
* <span data-ttu-id="e80b7-145">Sales price</span><span class="sxs-lookup"><span data-stu-id="e80b7-145">Sales price</span></span>
* <span data-ttu-id="e80b7-146">Tariff number</span><span class="sxs-lookup"><span data-stu-id="e80b7-146">Tariff number</span></span>
* <span data-ttu-id="e80b7-147">Units of measure</span><span class="sxs-lookup"><span data-stu-id="e80b7-147">Units of measure</span></span>
* <span data-ttu-id="e80b7-148">Item tracking code</span><span class="sxs-lookup"><span data-stu-id="e80b7-148">Item tracking code</span></span>
* <span data-ttu-id="e80b7-149">Customer price group</span><span class="sxs-lookup"><span data-stu-id="e80b7-149">Customer price group</span></span>

<span data-ttu-id="e80b7-150">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="e80b7-150">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="e80b7-151">Inventory posting setup</span><span class="sxs-lookup"><span data-stu-id="e80b7-151">Inventory posting setup</span></span>
* <span data-ttu-id="e80b7-152">General posting setup</span><span class="sxs-lookup"><span data-stu-id="e80b7-152">General posting setup</span></span>
* <span data-ttu-id="e80b7-153">Item journal batch</span><span class="sxs-lookup"><span data-stu-id="e80b7-153">Item journal batch</span></span>
* <span data-ttu-id="e80b7-154">Open transactions (item ledger entries)</span><span class="sxs-lookup"><span data-stu-id="e80b7-154">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="e80b7-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span><span class="sxs-lookup"><span data-stu-id="e80b7-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="e80b7-156">Other exchange rates are not migrated.</span><span class="sxs-lookup"><span data-stu-id="e80b7-156">Other exchange rates are not migrated.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="e80b7-157">To migrate data</span><span class="sxs-lookup"><span data-stu-id="e80b7-157">To migrate data</span></span>
<span data-ttu-id="e80b7-158">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="e80b7-158">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="e80b7-159">In C5, use the **Export Database** feature to export the data.</span><span class="sxs-lookup"><span data-stu-id="e80b7-159">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="e80b7-160">Then send the export folder to a compressed (zipped) folder.</span><span class="sxs-lookup"><span data-stu-id="e80b7-160">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="e80b7-161">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span><span class="sxs-lookup"><span data-stu-id="e80b7-161">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="e80b7-162">Complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="e80b7-162">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="e80b7-163">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span><span class="sxs-lookup"><span data-stu-id="e80b7-163">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note]
> <span data-ttu-id="e80b7-164">Companies often add fields to customize C5 for their specific line of business.</span><span class="sxs-lookup"><span data-stu-id="e80b7-164">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="e80b7-165"> does not migrate data from custom fields.</span><span class="sxs-lookup"><span data-stu-id="e80b7-165"> does not migrate data from custom fields.</span></span> <span data-ttu-id="e80b7-166">Also, migration will fail if you have more than 10 custom fields.</span><span class="sxs-lookup"><span data-stu-id="e80b7-166">Also, migration will fail if you have more than 10 custom fields.</span></span>

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="e80b7-167">Viewing the Status of the Migration</span><span class="sxs-lookup"><span data-stu-id="e80b7-167">Viewing the Status of the Migration</span></span>
<span data-ttu-id="e80b7-168">Use the **Data Migration Overview** page to monitor the success of the migration.</span><span class="sxs-lookup"><span data-stu-id="e80b7-168">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="e80b7-169">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span><span class="sxs-lookup"><span data-stu-id="e80b7-169">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="e80b7-170">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span><span class="sxs-lookup"><span data-stu-id="e80b7-170">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="e80b7-171">For more information, see the next section in this topic.</span><span class="sxs-lookup"><span data-stu-id="e80b7-171">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="e80b7-172">While you are waiting for the results of the migration, you must refresh the page to display the results.</span><span class="sxs-lookup"><span data-stu-id="e80b7-172">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="correcting-errors"></a><span data-ttu-id="e80b7-173">Correcting Errors</span><span class="sxs-lookup"><span data-stu-id="e80b7-173">Correcting Errors</span></span>
<span data-ttu-id="e80b7-174">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span><span class="sxs-lookup"><span data-stu-id="e80b7-174">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="e80b7-175">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span><span class="sxs-lookup"><span data-stu-id="e80b7-175">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="e80b7-176">The number in the **Error Count** field for the entity.</span><span class="sxs-lookup"><span data-stu-id="e80b7-176">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="e80b7-177">The entity, and then the **Show Errors** action.</span><span class="sxs-lookup"><span data-stu-id="e80b7-177">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="e80b7-178">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span><span class="sxs-lookup"><span data-stu-id="e80b7-178">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="e80b7-179">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span><span class="sxs-lookup"><span data-stu-id="e80b7-179">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="e80b7-180">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span><span class="sxs-lookup"><span data-stu-id="e80b7-180">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="e80b7-181">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span><span class="sxs-lookup"><span data-stu-id="e80b7-181">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="e80b7-182">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span><span class="sxs-lookup"><span data-stu-id="e80b7-182">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="e80b7-183">If an item variant is created first, the reference to the original item can cause an error message.</span><span class="sxs-lookup"><span data-stu-id="e80b7-183">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="e80b7-184">Verifying Data After Migrating</span><span class="sxs-lookup"><span data-stu-id="e80b7-184">Verifying Data After Migrating</span></span>
<span data-ttu-id="e80b7-185">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e80b7-185">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="e80b7-186">Microsoft Dynamcis C5 2012</span><span class="sxs-lookup"><span data-stu-id="e80b7-186">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]|
|-----|-----|
|<span data-ttu-id="e80b7-187">Customer Entries</span><span class="sxs-lookup"><span data-stu-id="e80b7-187">Customer Entries</span></span>| <span data-ttu-id="e80b7-188">General Journals</span><span class="sxs-lookup"><span data-stu-id="e80b7-188">General Journals</span></span>|
|<span data-ttu-id="e80b7-189">Vendor Entries</span><span class="sxs-lookup"><span data-stu-id="e80b7-189">Vendor Entries</span></span>| <span data-ttu-id="e80b7-190">General Journals</span><span class="sxs-lookup"><span data-stu-id="e80b7-190">General Journals</span></span>|
|<span data-ttu-id="e80b7-191">Item Entries</span><span class="sxs-lookup"><span data-stu-id="e80b7-191">Item Entries</span></span>| <span data-ttu-id="e80b7-192">Item Journals</span><span class="sxs-lookup"><span data-stu-id="e80b7-192">Item Journals</span></span>|

<span data-ttu-id="e80b7-193">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span><span class="sxs-lookup"><span data-stu-id="e80b7-193">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span></span>

## <a name="stopping-data-migration"></a><span data-ttu-id="e80b7-194">Stopping Data Migration</span><span class="sxs-lookup"><span data-stu-id="e80b7-194">Stopping Data Migration</span></span>
<span data-ttu-id="e80b7-195">You can stop migrating data by choosing **Stop All Migrations**.</span><span class="sxs-lookup"><span data-stu-id="e80b7-195">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="e80b7-196">If you do, all pending migrations are also stopped.</span><span class="sxs-lookup"><span data-stu-id="e80b7-196">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="e80b7-197">See Also</span><span class="sxs-lookup"><span data-stu-id="e80b7-197">See Also</span></span>
<span data-ttu-id="e80b7-198">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e80b7-198">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="e80b7-199">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="e80b7-199">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  
