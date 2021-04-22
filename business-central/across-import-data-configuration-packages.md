---
title: Use Excel to import data into Business Central
description: Use the default configuration package to add customer data in Excel and import the data back into Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 984186e8bb08cc9e99ab91dbc08f0e85c58e0804
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777955"
---
# <a name="importing-business-data-from-other-finance-systems"></a><span data-ttu-id="26b4f-103">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="26b4f-103">Importing Business Data from Other Finance Systems</span></span>

<span data-ttu-id="26b4f-104">When you sign up for [!INCLUDE[prod_short](includes/prod_short.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[prod_short](includes/prod_short.md)] company.</span><span class="sxs-lookup"><span data-stu-id="26b4f-104">When you sign up for [!INCLUDE[prod_short](includes/prod_short.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[prod_short](includes/prod_short.md)] company.</span></span> <span data-ttu-id="26b4f-105">Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.</span><span class="sxs-lookup"><span data-stu-id="26b4f-105">Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.</span></span>  

<span data-ttu-id="26b4f-106">From the Role Centre, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats.</span><span class="sxs-lookup"><span data-stu-id="26b4f-106">From the Role Center, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats.</span></span> <span data-ttu-id="26b4f-107">The type of files you can upload depends on the extensions that are available.</span><span class="sxs-lookup"><span data-stu-id="26b4f-107">The type of files you can upload depends on the extensions that are available.</span></span> <span data-ttu-id="26b4f-108">For example, you can migrate data from QuickBooks because [!INCLUDE[prod_short](includes/prod_short.md)] includes an extension that handles the conversion from QuickBooks.</span><span class="sxs-lookup"><span data-stu-id="26b4f-108">For example, you can migrate data from QuickBooks because [!INCLUDE[prod_short](includes/prod_short.md)] includes an extension that handles the conversion from QuickBooks.</span></span> <span data-ttu-id="26b4f-109">If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.</span><span class="sxs-lookup"><span data-stu-id="26b4f-109">If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.</span></span>  

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="26b4f-110">includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.</span><span class="sxs-lookup"><span data-stu-id="26b4f-110">includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.</span></span>

<span data-ttu-id="26b4f-111">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="26b4f-111">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="26b4f-112">On the **Configuration Packages** page, you can work with the package to import and validate the data before you apply the package.</span><span class="sxs-lookup"><span data-stu-id="26b4f-112">On the **Configuration Packages** page, you can work with the package to import and validate the data before you apply the package.</span></span>  

> [!TIP]  
> <span data-ttu-id="26b4f-113">We recommend that you use data migration wizards to import data from Dynamics GP, Dynamics NAV, or QuickBooks.</span><span class="sxs-lookup"><span data-stu-id="26b4f-113">We recommend that you use data migration wizards to import data from Dynamics GP, Dynamics NAV, or QuickBooks.</span></span> <span data-ttu-id="26b4f-114">For more information, see [Migrating On-Premises Data to Business Central Online](/dynamics365/business-central/dev-itpro/administration/migrate-data) in the administration content, or [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md).</span><span class="sxs-lookup"><span data-stu-id="26b4f-114">For more information, see [Migrating On-Premises Data to Business Central Online](/dynamics365/business-central/dev-itpro/administration/migrate-data) in the administration content, or [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md).</span></span>

> [!NOTE]  
> <span data-ttu-id="26b4f-115">For larger implementation work, you can use RapidStart Services for [!INCLUDE[prod_short](includes/prod_short.md)], which is an extensive toolkit for setting up new solutions based on customers' business requirements and setup data.</span><span class="sxs-lookup"><span data-stu-id="26b4f-115">For larger implementation work, you can use RapidStart Services for [!INCLUDE[prod_short](includes/prod_short.md)], which is an extensive toolkit for setting up new solutions based on customers' business requirements and setup data.</span></span> <span data-ttu-id="26b4f-116">RapidStart Services also offers functionality for import of business data.</span><span class="sxs-lookup"><span data-stu-id="26b4f-116">RapidStart Services also offers functionality for import of business data.</span></span> <span data-ttu-id="26b4f-117">For more information, see [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).</span><span class="sxs-lookup"><span data-stu-id="26b4f-117">For more information, see [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).</span></span>

<span data-ttu-id="26b4f-118">To import item pictures, you can use a dedicated function on the **Inventory Setup** page.</span><span class="sxs-lookup"><span data-stu-id="26b4f-118">To import item pictures, you can use a dedicated function on the **Inventory Setup** page.</span></span> <span data-ttu-id="26b4f-119">For more information, see [Import Multiple Item Pictures](inventory-how-import-item-pictures.md).</span><span class="sxs-lookup"><span data-stu-id="26b4f-119">For more information, see [Import Multiple Item Pictures](inventory-how-import-item-pictures.md).</span></span>

## <a name="importing-data-from-configuration-packages"></a><span data-ttu-id="26b4f-120">Importing Data from Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="26b4f-120">Importing Data from Configuration Packages</span></span>
[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="26b4f-121">includes a configuration package that you can export to Excel and set up your data there.</span><span class="sxs-lookup"><span data-stu-id="26b4f-121">includes a configuration package that you can export to Excel and set up your data there.</span></span> <span data-ttu-id="26b4f-122">Then, you can import the data from Excel again.</span><span class="sxs-lookup"><span data-stu-id="26b4f-122">Then, you can import the data from Excel again.</span></span> <span data-ttu-id="26b4f-123">The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.</span><span class="sxs-lookup"><span data-stu-id="26b4f-123">The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="26b4f-124">Working with configuration packages is advanced functionality, and we recommend that you contact your administrator.</span><span class="sxs-lookup"><span data-stu-id="26b4f-124">Working with configuration packages is advanced functionality, and we recommend that you contact your administrator.</span></span> <span data-ttu-id="26b4f-125">For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="26b4f-125">For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).</span></span>

## <a name="working-with-data-in-excel"></a><span data-ttu-id="26b4f-126">Working with Data in Excel</span><span class="sxs-lookup"><span data-stu-id="26b4f-126">Working with Data in Excel</span></span>
<span data-ttu-id="26b4f-127">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span><span class="sxs-lookup"><span data-stu-id="26b4f-127">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span></span> <span data-ttu-id="26b4f-128">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span><span class="sxs-lookup"><span data-stu-id="26b4f-128">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span></span> <span data-ttu-id="26b4f-129">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span><span class="sxs-lookup"><span data-stu-id="26b4f-129">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span></span> <span data-ttu-id="26b4f-130">For example, add a blank worksheet and copy the legacy data to it.</span><span class="sxs-lookup"><span data-stu-id="26b4f-130">For example, add a blank worksheet and copy the legacy data to it.</span></span> <span data-ttu-id="26b4f-131">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span><span class="sxs-lookup"><span data-stu-id="26b4f-131">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span></span> <span data-ttu-id="26b4f-132">After you have mapped all of the data, copy the range of data onto the table worksheet.</span><span class="sxs-lookup"><span data-stu-id="26b4f-132">After you have mapped all of the data, copy the range of data onto the table worksheet.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="26b4f-133">Do not change the columns in the worksheets.</span><span class="sxs-lookup"><span data-stu-id="26b4f-133">Do not change the columns in the worksheets.</span></span> <span data-ttu-id="26b4f-134">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="26b4f-134">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="26b4f-135">Fields of type Blob cannot be exported/imported using Excel.</span><span class="sxs-lookup"><span data-stu-id="26b4f-135">Fields of type Blob cannot be exported/imported using Excel.</span></span>

## <a name="tables-in-the-default-configuration-package"></a><span data-ttu-id="26b4f-136">Tables in the Default Configuration Package</span><span class="sxs-lookup"><span data-stu-id="26b4f-136">Tables in the Default Configuration Package</span></span>
<span data-ttu-id="26b4f-137">The default configuration package supports the following tables:</span><span class="sxs-lookup"><span data-stu-id="26b4f-137">The default configuration package supports the following tables:</span></span>

-   <span data-ttu-id="26b4f-138">Payment Terms</span><span class="sxs-lookup"><span data-stu-id="26b4f-138">Payment Terms</span></span>
-   <span data-ttu-id="26b4f-139">Customer Price Group</span><span class="sxs-lookup"><span data-stu-id="26b4f-139">Customer Price Group</span></span>
-   <span data-ttu-id="26b4f-140">Shipment Method</span><span class="sxs-lookup"><span data-stu-id="26b4f-140">Shipment Method</span></span>
-   <span data-ttu-id="26b4f-141">Salesperson/Purchaser</span><span class="sxs-lookup"><span data-stu-id="26b4f-141">Salesperson/Purchaser</span></span>
-   <span data-ttu-id="26b4f-142">Location</span><span class="sxs-lookup"><span data-stu-id="26b4f-142">Location</span></span>
-   <span data-ttu-id="26b4f-143">GL Account</span><span class="sxs-lookup"><span data-stu-id="26b4f-143">GL Account</span></span>
-   <span data-ttu-id="26b4f-144">Customer</span><span class="sxs-lookup"><span data-stu-id="26b4f-144">Customer</span></span>
-   <span data-ttu-id="26b4f-145">Vendor</span><span class="sxs-lookup"><span data-stu-id="26b4f-145">Vendor</span></span>
-   <span data-ttu-id="26b4f-146">Item</span><span class="sxs-lookup"><span data-stu-id="26b4f-146">Item</span></span>
-   <span data-ttu-id="26b4f-147">Sales Header</span><span class="sxs-lookup"><span data-stu-id="26b4f-147">Sales Header</span></span>
-   <span data-ttu-id="26b4f-148">Sales Line</span><span class="sxs-lookup"><span data-stu-id="26b4f-148">Sales Line</span></span>
-   <span data-ttu-id="26b4f-149">Purchase Header</span><span class="sxs-lookup"><span data-stu-id="26b4f-149">Purchase Header</span></span>
-   <span data-ttu-id="26b4f-150">Purchase Line</span><span class="sxs-lookup"><span data-stu-id="26b4f-150">Purchase Line</span></span>
-   <span data-ttu-id="26b4f-151">Gen.</span><span class="sxs-lookup"><span data-stu-id="26b4f-151">Gen.</span></span> <span data-ttu-id="26b4f-152">Journal Line</span><span class="sxs-lookup"><span data-stu-id="26b4f-152">Journal Line</span></span>
-   <span data-ttu-id="26b4f-153">Item Journal Line</span><span class="sxs-lookup"><span data-stu-id="26b4f-153">Item Journal Line</span></span>
-   <span data-ttu-id="26b4f-154">Customer Posting Group</span><span class="sxs-lookup"><span data-stu-id="26b4f-154">Customer Posting Group</span></span>
-   <span data-ttu-id="26b4f-155">Vendor Posting Group</span><span class="sxs-lookup"><span data-stu-id="26b4f-155">Vendor Posting Group</span></span>
-   <span data-ttu-id="26b4f-156">Inventory Posting Group</span><span class="sxs-lookup"><span data-stu-id="26b4f-156">Inventory Posting Group</span></span>
-   <span data-ttu-id="26b4f-157">Unit of Measure</span><span class="sxs-lookup"><span data-stu-id="26b4f-157">Unit of Measure</span></span>
-   <span data-ttu-id="26b4f-158">Gen.</span><span class="sxs-lookup"><span data-stu-id="26b4f-158">Gen.</span></span> <span data-ttu-id="26b4f-159">Business Posting Group</span><span class="sxs-lookup"><span data-stu-id="26b4f-159">Business Posting Group</span></span>
-   <span data-ttu-id="26b4f-160">Gen.</span><span class="sxs-lookup"><span data-stu-id="26b4f-160">Gen.</span></span> <span data-ttu-id="26b4f-161">Product Posting Group</span><span class="sxs-lookup"><span data-stu-id="26b4f-161">Product Posting Group</span></span>
-   <span data-ttu-id="26b4f-162">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="26b4f-162">General Posting Setup</span></span>
-   <span data-ttu-id="26b4f-163">Territory</span><span class="sxs-lookup"><span data-stu-id="26b4f-163">Territory</span></span>
-   <span data-ttu-id="26b4f-164">Item Category</span><span class="sxs-lookup"><span data-stu-id="26b4f-164">Item Category</span></span>
-   <span data-ttu-id="26b4f-165">Sales Price</span><span class="sxs-lookup"><span data-stu-id="26b4f-165">Sales Price</span></span>
-   <span data-ttu-id="26b4f-166">Purchase Price</span><span class="sxs-lookup"><span data-stu-id="26b4f-166">Purchase Price</span></span>

## <a name="see-also"></a><span data-ttu-id="26b4f-167">See Also</span><span class="sxs-lookup"><span data-stu-id="26b4f-167">See Also</span></span>
[<span data-ttu-id="26b4f-168">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="26b4f-168">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="26b4f-169">Migrating On-Premises Data to Business Central Online</span><span class="sxs-lookup"><span data-stu-id="26b4f-169">Migrating On-Premises Data to Business Central Online</span></span>](/dynamics365/business-central/dev-itpro/administration/migrate-data)  
[<span data-ttu-id="26b4f-170">QuickBooks Data Migration</span><span class="sxs-lookup"><span data-stu-id="26b4f-170">QuickBooks Data Migration</span></span>](ui-extensions-quickbooks-data-migration.md)  
[<span data-ttu-id="26b4f-171">Import Multiple Item Pictures</span><span class="sxs-lookup"><span data-stu-id="26b4f-171">Import Multiple Item Pictures</span></span>](inventory-how-import-item-pictures.md)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]