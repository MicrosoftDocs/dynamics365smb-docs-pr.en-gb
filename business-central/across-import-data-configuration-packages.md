---
title: Use Excel to import data into Financials| Microsoft Docs
description: Use the default configuration package to add customer data in Excel and import the data back into Business Central .
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 05/17/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ad1b888d475c0523c5a905e804a3f89ab4531b28
ms.openlocfilehash: 379cfd2731bba2df6f5e31d2b8de2d72e2064ebb
ms.contentlocale: en-gb
ms.lasthandoff: 05/17/2018

---
# <a name="importing-business-data-from-other-finance-systems"></a><span data-ttu-id="f0af9-103">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="f0af9-103">Importing Business Data from Other Finance Systems</span></span>
<span data-ttu-id="f0af9-104">When you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="f0af9-104">When you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="f0af9-105">Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.</span><span class="sxs-lookup"><span data-stu-id="f0af9-105">Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.</span></span>  

<span data-ttu-id="f0af9-106">From the Role Centre, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats.</span><span class="sxs-lookup"><span data-stu-id="f0af9-106">From the Role Center, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats.</span></span> <span data-ttu-id="f0af9-107">The type of files you can upload depends on the extensions that are available.</span><span class="sxs-lookup"><span data-stu-id="f0af9-107">The type of files you can upload depends on the extensions that are available.</span></span> <span data-ttu-id="f0af9-108">For example, you can migrate data from QuickBooks because [!INCLUDE[d365fin](includes/d365fin_md.md)] includes an extension that handles the conversion from QuickBooks.</span><span class="sxs-lookup"><span data-stu-id="f0af9-108">For example, you can migrate data from QuickBooks because [!INCLUDE[d365fin](includes/d365fin_md.md)] includes an extension that handles the conversion from QuickBooks.</span></span> <span data-ttu-id="f0af9-109">If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.</span><span class="sxs-lookup"><span data-stu-id="f0af9-109">If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f0af9-110"> includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.</span><span class="sxs-lookup"><span data-stu-id="f0af9-110"> includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.</span></span>

<span data-ttu-id="f0af9-111">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f0af9-111">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="f0af9-112">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span><span class="sxs-lookup"><span data-stu-id="f0af9-112">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span></span>  

> [!TIP]  
> <span data-ttu-id="f0af9-113">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span><span class="sxs-lookup"><span data-stu-id="f0af9-113">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span></span> <span data-ttu-id="f0af9-114">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span><span class="sxs-lookup"><span data-stu-id="f0af9-114">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span></span>

> [!NOTE]  
> <span data-ttu-id="f0af9-115">For larger implementation work, you can use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], which is an extensive toolkit for setting up new solutions based on customers' business requirements and setup data.</span><span class="sxs-lookup"><span data-stu-id="f0af9-115">For larger implementation work, you can use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], which is an extensive toolkit for setting up new solutions based on customers' business requirements and setup data.</span></span> <span data-ttu-id="f0af9-116">RapidStart Services also offers functionality for import of business data.</span><span class="sxs-lookup"><span data-stu-id="f0af9-116">RapidStart Services also offers functionality for import of business data.</span></span> <span data-ttu-id="f0af9-117">For more information, see [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).</span><span class="sxs-lookup"><span data-stu-id="f0af9-117">For more information, see [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).</span></span>

## <a name="importing-data-from-configuration-packages"></a><span data-ttu-id="f0af9-118">Importing Data from Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="f0af9-118">Importing Data from Configuration Packages</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="f0af9-119"> includes a configuration package that you can export to Excel and set up your data there.</span><span class="sxs-lookup"><span data-stu-id="f0af9-119"> includes a configuration package that you can export to Excel and set up your data there.</span></span> <span data-ttu-id="f0af9-120">Then, you can import the data from Excel again.</span><span class="sxs-lookup"><span data-stu-id="f0af9-120">Then, you can import the data from Excel again.</span></span> <span data-ttu-id="f0af9-121">The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.</span><span class="sxs-lookup"><span data-stu-id="f0af9-121">The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="f0af9-122">Working with configuration packages is advanced functionality, and we recommend that you contact your administrator.</span><span class="sxs-lookup"><span data-stu-id="f0af9-122">Working with configuration packages is advanced functionality, and we recommend that you contact your administrator.</span></span> <span data-ttu-id="f0af9-123">For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="f0af9-123">For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).</span></span>

## <a name="working-with-data-in-excel"></a><span data-ttu-id="f0af9-124">Working with Data in Excel</span><span class="sxs-lookup"><span data-stu-id="f0af9-124">Working with Data in Excel</span></span>
<span data-ttu-id="f0af9-125">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span><span class="sxs-lookup"><span data-stu-id="f0af9-125">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span></span> <span data-ttu-id="f0af9-126">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span><span class="sxs-lookup"><span data-stu-id="f0af9-126">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span></span> <span data-ttu-id="f0af9-127">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span><span class="sxs-lookup"><span data-stu-id="f0af9-127">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span></span> <span data-ttu-id="f0af9-128">For example, add a blank worksheet and copy the legacy data to it.</span><span class="sxs-lookup"><span data-stu-id="f0af9-128">For example, add a blank worksheet and copy the legacy data to it.</span></span> <span data-ttu-id="f0af9-129">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span><span class="sxs-lookup"><span data-stu-id="f0af9-129">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span></span> <span data-ttu-id="f0af9-130">After you have mapped all of the data, copy the range of data onto the table worksheet.</span><span class="sxs-lookup"><span data-stu-id="f0af9-130">After you have mapped all of the data, copy the range of data onto the table worksheet.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="f0af9-131">Do not change the columns in the worksheets.</span><span class="sxs-lookup"><span data-stu-id="f0af9-131">Do not change the columns in the worksheets.</span></span> <span data-ttu-id="f0af9-132">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f0af9-132">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="tables-in-the-default-configuration-package"></a><span data-ttu-id="f0af9-133">Tables in the Default Configuration Package</span><span class="sxs-lookup"><span data-stu-id="f0af9-133">Tables in the Default Configuration Package</span></span>
<span data-ttu-id="f0af9-134">The default configuration package supports the following tables:</span><span class="sxs-lookup"><span data-stu-id="f0af9-134">The default configuration package supports the following tables:</span></span>

-   <span data-ttu-id="f0af9-135">Payment Terms</span><span class="sxs-lookup"><span data-stu-id="f0af9-135">Payment Terms</span></span>
-   <span data-ttu-id="f0af9-136">Customer Price Group</span><span class="sxs-lookup"><span data-stu-id="f0af9-136">Customer Price Group</span></span>
-   <span data-ttu-id="f0af9-137">Shipment Method</span><span class="sxs-lookup"><span data-stu-id="f0af9-137">Shipment Method</span></span>
-   <span data-ttu-id="f0af9-138">Salesperson/Purchaser</span><span class="sxs-lookup"><span data-stu-id="f0af9-138">Salesperson/Purchaser</span></span>
-   <span data-ttu-id="f0af9-139">Location</span><span class="sxs-lookup"><span data-stu-id="f0af9-139">Location</span></span>
-   <span data-ttu-id="f0af9-140">GL Account</span><span class="sxs-lookup"><span data-stu-id="f0af9-140">GL Account</span></span>
-   <span data-ttu-id="f0af9-141">Customer</span><span class="sxs-lookup"><span data-stu-id="f0af9-141">Customer</span></span>
-   <span data-ttu-id="f0af9-142">Vendor</span><span class="sxs-lookup"><span data-stu-id="f0af9-142">Vendor</span></span>
-   <span data-ttu-id="f0af9-143">Item</span><span class="sxs-lookup"><span data-stu-id="f0af9-143">Item</span></span>
-   <span data-ttu-id="f0af9-144">Sales Header</span><span class="sxs-lookup"><span data-stu-id="f0af9-144">Sales Header</span></span>
-   <span data-ttu-id="f0af9-145">Sales Line</span><span class="sxs-lookup"><span data-stu-id="f0af9-145">Sales Line</span></span>
-   <span data-ttu-id="f0af9-146">Purchase Header</span><span class="sxs-lookup"><span data-stu-id="f0af9-146">Purchase Header</span></span>
-   <span data-ttu-id="f0af9-147">Purchase Line</span><span class="sxs-lookup"><span data-stu-id="f0af9-147">Purchase Line</span></span>
-   <span data-ttu-id="f0af9-148">Gen. Journal Line</span><span class="sxs-lookup"><span data-stu-id="f0af9-148">Gen. Journal Line</span></span>
-   <span data-ttu-id="f0af9-149">Item Journal Line</span><span class="sxs-lookup"><span data-stu-id="f0af9-149">Item Journal Line</span></span>
-   <span data-ttu-id="f0af9-150">Customer Posting Group</span><span class="sxs-lookup"><span data-stu-id="f0af9-150">Customer Posting Group</span></span>
-   <span data-ttu-id="f0af9-151">Vendor Posting Group</span><span class="sxs-lookup"><span data-stu-id="f0af9-151">Vendor Posting Group</span></span>
-   <span data-ttu-id="f0af9-152">Inventory Posting Group</span><span class="sxs-lookup"><span data-stu-id="f0af9-152">Inventory Posting Group</span></span>
-   <span data-ttu-id="f0af9-153">Unit of Measure</span><span class="sxs-lookup"><span data-stu-id="f0af9-153">Unit of Measure</span></span>
-   <span data-ttu-id="f0af9-154">Gen. Business Posting Group</span><span class="sxs-lookup"><span data-stu-id="f0af9-154">Gen. Business Posting Group</span></span>
-   <span data-ttu-id="f0af9-155">Gen. Product Posting Group</span><span class="sxs-lookup"><span data-stu-id="f0af9-155">Gen. Product Posting Group</span></span>
-   <span data-ttu-id="f0af9-156">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="f0af9-156">General Posting Setup</span></span>
-   <span data-ttu-id="f0af9-157">Territory</span><span class="sxs-lookup"><span data-stu-id="f0af9-157">Territory</span></span>
-   <span data-ttu-id="f0af9-158">Item Category</span><span class="sxs-lookup"><span data-stu-id="f0af9-158">Item Category</span></span>
-   <span data-ttu-id="f0af9-159">Sales Price</span><span class="sxs-lookup"><span data-stu-id="f0af9-159">Sales Price</span></span>
-   <span data-ttu-id="f0af9-160">Purchase Price</span><span class="sxs-lookup"><span data-stu-id="f0af9-160">Purchase Price</span></span>

## <a name="see-also"></a><span data-ttu-id="f0af9-161">See Also</span><span class="sxs-lookup"><span data-stu-id="f0af9-161">See Also</span></span>
[<span data-ttu-id="f0af9-162">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="f0af9-162">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="f0af9-163">QuickBooks Data Migration</span><span class="sxs-lookup"><span data-stu-id="f0af9-163">QuickBooks Data Migration</span></span>](ui-extensions-quickbooks-data-migration.md)  
[<span data-ttu-id="f0af9-164">Dynamics GP Data Migration</span><span class="sxs-lookup"><span data-stu-id="f0af9-164">Dynamics GP Data Migration</span></span>](ui-extensions-dynamicsgp-data-migration.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]

