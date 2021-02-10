---
title: Using the C5 Data Migration Extension | Microsoft Docs
description: Use this extension to migrate customers, vendors, items, and general ledger accounts from Microsoft Dynamics C5 2012 to Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 0f257b81f1e36e86e40e67ca8ba07169ec22d938
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4747600"
---
# <a name="the-c5-data-migration-extension"></a><span data-ttu-id="8fa46-103">The C5 Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="8fa46-103">The C5 Data Migration Extension</span></span>

<span data-ttu-id="8fa46-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamics C5 2012 to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="8fa46-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamics C5 2012 to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="8fa46-105">You can also migrate historical entries for general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="8fa46-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="8fa46-106">The company in [!INCLUDE[prod_short](includes/prod_short.md)] must not contain any data.</span><span class="sxs-lookup"><span data-stu-id="8fa46-106">The company in [!INCLUDE[prod_short](includes/prod_short.md)] must not contain any data.</span></span> <span data-ttu-id="8fa46-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span><span class="sxs-lookup"><span data-stu-id="8fa46-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="8fa46-108">What Data is Migrated?</span><span class="sxs-lookup"><span data-stu-id="8fa46-108">What Data is Migrated?</span></span>
<span data-ttu-id="8fa46-109">The following data is migrated for each entity:</span><span class="sxs-lookup"><span data-stu-id="8fa46-109">The following data is migrated for each entity:</span></span>

### <a name="customers"></a><span data-ttu-id="8fa46-110">Customers</span><span class="sxs-lookup"><span data-stu-id="8fa46-110">Customers</span></span>

* <span data-ttu-id="8fa46-111">Contacts</span><span class="sxs-lookup"><span data-stu-id="8fa46-111">Contacts</span></span>  
* <span data-ttu-id="8fa46-112">Location</span><span class="sxs-lookup"><span data-stu-id="8fa46-112">Location</span></span>
* <span data-ttu-id="8fa46-113">Country</span><span class="sxs-lookup"><span data-stu-id="8fa46-113">Country</span></span>
* <span data-ttu-id="8fa46-114">Customer dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="8fa46-114">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="8fa46-115">Shipment method</span><span class="sxs-lookup"><span data-stu-id="8fa46-115">Shipment method</span></span>
* <span data-ttu-id="8fa46-116">Sales Person</span><span class="sxs-lookup"><span data-stu-id="8fa46-116">Sales Person</span></span>
* <span data-ttu-id="8fa46-117">Payment terms</span><span class="sxs-lookup"><span data-stu-id="8fa46-117">Payment terms</span></span>
* <span data-ttu-id="8fa46-118">Payment method</span><span class="sxs-lookup"><span data-stu-id="8fa46-118">Payment method</span></span>
* <span data-ttu-id="8fa46-119">Customer price group</span><span class="sxs-lookup"><span data-stu-id="8fa46-119">Customer price group</span></span>
* <span data-ttu-id="8fa46-120">Customer invoice discount</span><span class="sxs-lookup"><span data-stu-id="8fa46-120">Customer invoice discount</span></span>

<span data-ttu-id="8fa46-121">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="8fa46-121">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="8fa46-122">Customer posting setup</span><span class="sxs-lookup"><span data-stu-id="8fa46-122">Customer posting setup</span></span>
* <span data-ttu-id="8fa46-123">General journal batch</span><span class="sxs-lookup"><span data-stu-id="8fa46-123">General journal batch</span></span>
* <span data-ttu-id="8fa46-124">Open transactions (customer ledger entries)</span><span class="sxs-lookup"><span data-stu-id="8fa46-124">Open transactions (customer ledger entries)</span></span>

### <a name="vendors"></a><span data-ttu-id="8fa46-125">Vendors</span><span class="sxs-lookup"><span data-stu-id="8fa46-125">Vendors</span></span>

* <span data-ttu-id="8fa46-126">Contacts</span><span class="sxs-lookup"><span data-stu-id="8fa46-126">Contacts</span></span>
* <span data-ttu-id="8fa46-127">Location</span><span class="sxs-lookup"><span data-stu-id="8fa46-127">Location</span></span>
* <span data-ttu-id="8fa46-128">Country</span><span class="sxs-lookup"><span data-stu-id="8fa46-128">Country</span></span>
* <span data-ttu-id="8fa46-129">Vendor dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="8fa46-129">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="8fa46-130">Invoice discount</span><span class="sxs-lookup"><span data-stu-id="8fa46-130">Invoice discount</span></span>
* <span data-ttu-id="8fa46-131">Shipment method</span><span class="sxs-lookup"><span data-stu-id="8fa46-131">Shipment method</span></span>
* <span data-ttu-id="8fa46-132">Purchaser</span><span class="sxs-lookup"><span data-stu-id="8fa46-132">Purchaser</span></span>
* <span data-ttu-id="8fa46-133">Payment terms</span><span class="sxs-lookup"><span data-stu-id="8fa46-133">Payment terms</span></span>
* <span data-ttu-id="8fa46-134">Payment method</span><span class="sxs-lookup"><span data-stu-id="8fa46-134">Payment method</span></span>
* <span data-ttu-id="8fa46-135">Vendor invoice discount</span><span class="sxs-lookup"><span data-stu-id="8fa46-135">Vendor invoice discount</span></span>

<span data-ttu-id="8fa46-136">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="8fa46-136">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="8fa46-137">Vendor posting setup</span><span class="sxs-lookup"><span data-stu-id="8fa46-137">Vendor posting setup</span></span>
* <span data-ttu-id="8fa46-138">General journal batch</span><span class="sxs-lookup"><span data-stu-id="8fa46-138">General journal batch</span></span>
* <span data-ttu-id="8fa46-139">Open transactions (vendor ledger entries)</span><span class="sxs-lookup"><span data-stu-id="8fa46-139">Open transactions (vendor ledger entries)</span></span>

### <a name="items"></a><span data-ttu-id="8fa46-140">Items</span><span class="sxs-lookup"><span data-stu-id="8fa46-140">Items</span></span>

* <span data-ttu-id="8fa46-141">Location</span><span class="sxs-lookup"><span data-stu-id="8fa46-141">Location</span></span>
* <span data-ttu-id="8fa46-142">Country</span><span class="sxs-lookup"><span data-stu-id="8fa46-142">Country</span></span>
* <span data-ttu-id="8fa46-143">Item dimensions (department, centre, purpose)</span><span class="sxs-lookup"><span data-stu-id="8fa46-143">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="8fa46-144">Sales line discounts</span><span class="sxs-lookup"><span data-stu-id="8fa46-144">Sales line discounts</span></span>
* <span data-ttu-id="8fa46-145">Customer discount groups</span><span class="sxs-lookup"><span data-stu-id="8fa46-145">Customer discount groups</span></span>
* <span data-ttu-id="8fa46-146">Item discount groups</span><span class="sxs-lookup"><span data-stu-id="8fa46-146">Item discount groups</span></span>
* <span data-ttu-id="8fa46-147">Sales price</span><span class="sxs-lookup"><span data-stu-id="8fa46-147">Sales price</span></span>
* <span data-ttu-id="8fa46-148">Commodity Code</span><span class="sxs-lookup"><span data-stu-id="8fa46-148">Tariff number</span></span>
* <span data-ttu-id="8fa46-149">Units of measure</span><span class="sxs-lookup"><span data-stu-id="8fa46-149">Units of measure</span></span>
* <span data-ttu-id="8fa46-150">Item tracking code</span><span class="sxs-lookup"><span data-stu-id="8fa46-150">Item tracking code</span></span>
* <span data-ttu-id="8fa46-151">Customer price group</span><span class="sxs-lookup"><span data-stu-id="8fa46-151">Customer price group</span></span>
* <span data-ttu-id="8fa46-152">Assembly BOMs</span><span class="sxs-lookup"><span data-stu-id="8fa46-152">Assembly BOMs</span></span>

<span data-ttu-id="8fa46-153">If you migrate accounts, the following data is also migrated:</span><span class="sxs-lookup"><span data-stu-id="8fa46-153">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="8fa46-154">Inventory posting setup</span><span class="sxs-lookup"><span data-stu-id="8fa46-154">Inventory posting setup</span></span>
* <span data-ttu-id="8fa46-155">General posting setup</span><span class="sxs-lookup"><span data-stu-id="8fa46-155">General posting setup</span></span>
* <span data-ttu-id="8fa46-156">Item journal batch</span><span class="sxs-lookup"><span data-stu-id="8fa46-156">Item journal batch</span></span>
* <span data-ttu-id="8fa46-157">Open transactions (item ledger entries)</span><span class="sxs-lookup"><span data-stu-id="8fa46-157">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="8fa46-158">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span><span class="sxs-lookup"><span data-stu-id="8fa46-158">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="8fa46-159">Other exchange rates are not migrated.</span><span class="sxs-lookup"><span data-stu-id="8fa46-159">Other exchange rates are not migrated.</span></span>

### <a name="chart-of-accounts"></a><span data-ttu-id="8fa46-160">Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="8fa46-160">Chart of Accounts</span></span>

* <span data-ttu-id="8fa46-161">Standard dimensions: Department, Cost Centre, Purpose</span><span class="sxs-lookup"><span data-stu-id="8fa46-161">Standard dimensions: Department, Cost Center, Purpose</span></span>  
* <span data-ttu-id="8fa46-162">Historical G/L transactions</span><span class="sxs-lookup"><span data-stu-id="8fa46-162">Historical G/L transactions</span></span>  

> [!Note]
> <span data-ttu-id="8fa46-163">Historical G/L transactions are treated a little differently.</span><span class="sxs-lookup"><span data-stu-id="8fa46-163">Historical G/L transactions are treated a little differently.</span></span> <span data-ttu-id="8fa46-164">When you migrate data you set a **Current Period** parameter.</span><span class="sxs-lookup"><span data-stu-id="8fa46-164">When you migrate data you set a **Current Period** parameter.</span></span> <span data-ttu-id="8fa46-165">This parameter specifies how to process G/L transactions.</span><span class="sxs-lookup"><span data-stu-id="8fa46-165">This parameter specifies how to process G/L transactions.</span></span> <span data-ttu-id="8fa46-166">Transactions after this date are migrated individually.</span><span class="sxs-lookup"><span data-stu-id="8fa46-166">Transactions after this date are migrated individually.</span></span> <span data-ttu-id="8fa46-167">Transactions before this date are aggregated per account and migrated as a single amount.</span><span class="sxs-lookup"><span data-stu-id="8fa46-167">Transactions before this date are aggregated per account and migrated as a single amount.</span></span> <span data-ttu-id="8fa46-168">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span><span class="sxs-lookup"><span data-stu-id="8fa46-168">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span></span> <span data-ttu-id="8fa46-169">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span><span class="sxs-lookup"><span data-stu-id="8fa46-169">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span></span> <span data-ttu-id="8fa46-170">All transactions after this date will be migrated individually.</span><span class="sxs-lookup"><span data-stu-id="8fa46-170">All transactions after this date will be migrated individually.</span></span>

## <a name="file-size-requirements"></a><span data-ttu-id="8fa46-171">File Size Requirements</span><span class="sxs-lookup"><span data-stu-id="8fa46-171">File Size Requirements</span></span>

<span data-ttu-id="8fa46-172">The largest file size you can upload to [!INCLUDE[prod_short](includes/prod_short.md)] is 150 MB.</span><span class="sxs-lookup"><span data-stu-id="8fa46-172">The largest file size you can upload to [!INCLUDE[prod_short](includes/prod_short.md)] is 150 MB.</span></span> <span data-ttu-id="8fa46-173">If the file you export from C5 is larger than that, consider migrating data in multiple files.</span><span class="sxs-lookup"><span data-stu-id="8fa46-173">If the file you export from C5 is larger than that, consider migrating data in multiple files.</span></span> <span data-ttu-id="8fa46-174">For example, export one or two types of entities from C5, such as customers and vendors, to a file, and then export items to another file, and so on.</span><span class="sxs-lookup"><span data-stu-id="8fa46-174">For example, export one or two types of entities from C5, such as customers and vendors, to a file, and then export items to another file, and so on.</span></span> <span data-ttu-id="8fa46-175">You can import files individually in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="8fa46-175">You can import files individually in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="8fa46-176">To migrate data</span><span class="sxs-lookup"><span data-stu-id="8fa46-176">To migrate data</span></span>

<span data-ttu-id="8fa46-177">There are just a few steps to export data from C5, and import it in [!INCLUDE[prod_short](includes/prod_short.md)]:</span><span class="sxs-lookup"><span data-stu-id="8fa46-177">There are just a few steps to export data from C5, and import it in [!INCLUDE[prod_short](includes/prod_short.md)]:</span></span>  

1. <span data-ttu-id="8fa46-178">In C5, use the **Export Database** feature to export the data.</span><span class="sxs-lookup"><span data-stu-id="8fa46-178">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="8fa46-179">Then send the export folder to a compressed (zipped) folder.</span><span class="sxs-lookup"><span data-stu-id="8fa46-179">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="8fa46-180">In [!INCLUDE[prod_short](includes/prod_short.md)], choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Migration**, and then choose **Data Migration**.</span><span class="sxs-lookup"><span data-stu-id="8fa46-180">In [!INCLUDE[prod_short](includes/prod_short.md)], choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="8fa46-181">Complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="8fa46-181">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="8fa46-182">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span><span class="sxs-lookup"><span data-stu-id="8fa46-182">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="8fa46-183">Viewing the Status of the Migration</span><span class="sxs-lookup"><span data-stu-id="8fa46-183">Viewing the Status of the Migration</span></span>

<span data-ttu-id="8fa46-184">Use the **Data Migration Overview** page to monitor the success of the migration.</span><span class="sxs-lookup"><span data-stu-id="8fa46-184">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="8fa46-185">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span><span class="sxs-lookup"><span data-stu-id="8fa46-185">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="8fa46-186">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span><span class="sxs-lookup"><span data-stu-id="8fa46-186">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="8fa46-187">For more information, see the next section in this topic.</span><span class="sxs-lookup"><span data-stu-id="8fa46-187">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="8fa46-188">While you are waiting for the results of the migration, you must refresh the page to display the results.</span><span class="sxs-lookup"><span data-stu-id="8fa46-188">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="how-to-avoid-double-posting"></a><span data-ttu-id="8fa46-189">How to Avoid Double-Posting</span><span class="sxs-lookup"><span data-stu-id="8fa46-189">How to Avoid Double-Posting</span></span>

<span data-ttu-id="8fa46-190">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span><span class="sxs-lookup"><span data-stu-id="8fa46-190">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span></span>  

* <span data-ttu-id="8fa46-191">For vendors, we use the A/P account from the vendor posting group.</span><span class="sxs-lookup"><span data-stu-id="8fa46-191">For vendors, we use the A/P account from the vendor posting group.</span></span>  
* <span data-ttu-id="8fa46-192">For customers, we use the A/R account from the customer posting group.</span><span class="sxs-lookup"><span data-stu-id="8fa46-192">For customers, we use the A/R account from the customer posting group.</span></span>  
* <span data-ttu-id="8fa46-193">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span><span class="sxs-lookup"><span data-stu-id="8fa46-193">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span></span>  

## <a name="correcting-errors"></a><span data-ttu-id="8fa46-194">Correcting Errors</span><span class="sxs-lookup"><span data-stu-id="8fa46-194">Correcting Errors</span></span>

<span data-ttu-id="8fa46-195">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span><span class="sxs-lookup"><span data-stu-id="8fa46-195">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="8fa46-196">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span><span class="sxs-lookup"><span data-stu-id="8fa46-196">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="8fa46-197">The number in the **Error Count** field for the entity.</span><span class="sxs-lookup"><span data-stu-id="8fa46-197">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="8fa46-198">The entity, and then the **Show Errors** action.</span><span class="sxs-lookup"><span data-stu-id="8fa46-198">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="8fa46-199">On the **Data Migration Errors** page, to fix an error you can choose an error message, and then choose **Edit Record** to view the migrated data for the entity.</span><span class="sxs-lookup"><span data-stu-id="8fa46-199">On the **Data Migration Errors** page, to fix an error you can choose an error message, and then choose **Edit Record** to view the migrated data for the entity.</span></span> <span data-ttu-id="8fa46-200">If you have several errors to fix, you can choose **Bulk-Fix Errors** to edit the entities in a list.</span><span class="sxs-lookup"><span data-stu-id="8fa46-200">If you have several errors to fix, you can choose **Bulk-Fix Errors** to edit the entities in a list.</span></span> <span data-ttu-id="8fa46-201">You still need to open individual records if the error was caused by a related entry though.</span><span class="sxs-lookup"><span data-stu-id="8fa46-201">You still need to open individual records if the error was caused by a related entry though.</span></span> <span data-ttu-id="8fa46-202">For example, a vendor will not be migrated if an email address one of their contacts has an invalid format.</span><span class="sxs-lookup"><span data-stu-id="8fa46-202">For example, a vendor will not be migrated if an email address one of their contacts has an invalid format.</span></span>

<span data-ttu-id="8fa46-203">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span><span class="sxs-lookup"><span data-stu-id="8fa46-203">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="8fa46-204">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span><span class="sxs-lookup"><span data-stu-id="8fa46-204">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="8fa46-205">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span><span class="sxs-lookup"><span data-stu-id="8fa46-205">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="8fa46-206">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span><span class="sxs-lookup"><span data-stu-id="8fa46-206">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="8fa46-207">If an item variant is created first, the reference to the original item can cause an error message.</span><span class="sxs-lookup"><span data-stu-id="8fa46-207">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="8fa46-208">Verifying Data After Migrating</span><span class="sxs-lookup"><span data-stu-id="8fa46-208">Verifying Data After Migrating</span></span>

<span data-ttu-id="8fa46-209">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="8fa46-209">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

|<span data-ttu-id="8fa46-210">Microsoft Dynamics C5 2012</span><span class="sxs-lookup"><span data-stu-id="8fa46-210">Microsoft Dynamics C5 2012</span></span> | <span data-ttu-id="8fa46-211">Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="8fa46-211">Dynamics 365 Business Central</span></span>| <span data-ttu-id="8fa46-212">Batch Job to Use</span><span class="sxs-lookup"><span data-stu-id="8fa46-212">Batch Job to Use</span></span> |
|---------------------------|------------------------------|------------------|
|<span data-ttu-id="8fa46-213">Customer Entries</span><span class="sxs-lookup"><span data-stu-id="8fa46-213">Customer Entries</span></span>| <span data-ttu-id="8fa46-214">General Journals</span><span class="sxs-lookup"><span data-stu-id="8fa46-214">General Journals</span></span>| <span data-ttu-id="8fa46-215">CUSTMIGR</span><span class="sxs-lookup"><span data-stu-id="8fa46-215">CUSTMIGR</span></span> |
|<span data-ttu-id="8fa46-216">Vendor Entries</span><span class="sxs-lookup"><span data-stu-id="8fa46-216">Vendor Entries</span></span>| <span data-ttu-id="8fa46-217">General Journals</span><span class="sxs-lookup"><span data-stu-id="8fa46-217">General Journals</span></span>| <span data-ttu-id="8fa46-218">VENDMIGR</span><span class="sxs-lookup"><span data-stu-id="8fa46-218">VENDMIGR</span></span>|
|<span data-ttu-id="8fa46-219">Item Entries</span><span class="sxs-lookup"><span data-stu-id="8fa46-219">Item Entries</span></span>| <span data-ttu-id="8fa46-220">Item Journals</span><span class="sxs-lookup"><span data-stu-id="8fa46-220">Item Journals</span></span>| <span data-ttu-id="8fa46-221">ITEMMIGR</span><span class="sxs-lookup"><span data-stu-id="8fa46-221">ITEMMIGR</span></span> |
|<span data-ttu-id="8fa46-222">G/L Entries</span><span class="sxs-lookup"><span data-stu-id="8fa46-222">G/L Entries</span></span>| <span data-ttu-id="8fa46-223">General Journals</span><span class="sxs-lookup"><span data-stu-id="8fa46-223">General Journals</span></span>| <span data-ttu-id="8fa46-224">GLACMIGR</span><span class="sxs-lookup"><span data-stu-id="8fa46-224">GLACMIGR</span></span> |

## <a name="stopping-data-migration"></a><span data-ttu-id="8fa46-225">Stopping Data Migration</span><span class="sxs-lookup"><span data-stu-id="8fa46-225">Stopping Data Migration</span></span>

<span data-ttu-id="8fa46-226">You can stop migrating data by choosing **Stop All Migrations**.</span><span class="sxs-lookup"><span data-stu-id="8fa46-226">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="8fa46-227">If you do, all pending migrations are also stopped.</span><span class="sxs-lookup"><span data-stu-id="8fa46-227">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="8fa46-228">See Also</span><span class="sxs-lookup"><span data-stu-id="8fa46-228">See Also</span></span>

<span data-ttu-id="8fa46-229">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="8fa46-229">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="8fa46-230">Getting Started</span><span class="sxs-lookup"><span data-stu-id="8fa46-230">Getting Started</span></span>](product-get-started.md)  
