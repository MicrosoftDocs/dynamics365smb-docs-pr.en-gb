---
title: How to Create a New Company | Microsoft Docs
description: To use RapidStart Services tables and pages are created, but there is no data in them.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7583837e515a4fd5fb415fe1b482512e7edf6b5a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754012"
---
# <a name="create-a-new-company"></a><span data-ttu-id="9ff54-103">Create a New Company</span><span class="sxs-lookup"><span data-stu-id="9ff54-103">Create a New Company</span></span>
<span data-ttu-id="9ff54-104">To use RapidStart Services for [!INCLUDE[prod_short](includes/prod_short.md)], you first create a new company for which you want to perform a customer implementation.</span><span class="sxs-lookup"><span data-stu-id="9ff54-104">To use RapidStart Services for [!INCLUDE[prod_short](includes/prod_short.md)], you first create a new company for which you want to perform a customer implementation.</span></span> <span data-ttu-id="9ff54-105">When you create a new company, the standard [!INCLUDE[prod_short](includes/prod_short.md)] tables and pages are created, but there is no data in them.</span><span class="sxs-lookup"><span data-stu-id="9ff54-105">When you create a new company, the standard [!INCLUDE[prod_short](includes/prod_short.md)] tables and pages are created, but there is no data in them.</span></span>

<span data-ttu-id="9ff54-106">In addition, you can apply specific setup data to your company after you initialise it.</span><span class="sxs-lookup"><span data-stu-id="9ff54-106">In addition, you can apply specific setup data to your company after you initialize it.</span></span> <span data-ttu-id="9ff54-107">The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.</span><span class="sxs-lookup"><span data-stu-id="9ff54-107">The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.</span></span>  

<span data-ttu-id="9ff54-108">Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company.</span><span class="sxs-lookup"><span data-stu-id="9ff54-108">Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company.</span></span> <span data-ttu-id="9ff54-109">Use the following procedures to use the example configuration package with a new company.</span><span class="sxs-lookup"><span data-stu-id="9ff54-109">Use the following procedures to use the example configuration package with a new company.</span></span>  

## <a name="to-use-the-sample-basicconfig-configuration-package"></a><span data-ttu-id="9ff54-110">To use the sample BASICCONFIG configuration package</span><span class="sxs-lookup"><span data-stu-id="9ff54-110">To use the sample BASICCONFIG configuration package</span></span>  
1. <span data-ttu-id="9ff54-111">Open the CRONUS International Ltd. company.</span><span class="sxs-lookup"><span data-stu-id="9ff54-111">Open the CRONUS International Ltd. company.</span></span> <span data-ttu-id="9ff54-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="9ff54-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>
2. <span data-ttu-id="9ff54-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9ff54-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span></span>  
3. <span data-ttu-id="9ff54-114">Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.</span><span class="sxs-lookup"><span data-stu-id="9ff54-114">Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.</span></span>  

<span data-ttu-id="9ff54-115">Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.</span><span class="sxs-lookup"><span data-stu-id="9ff54-115">Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.</span></span>  

## <a name="to-create-a-new-company"></a><span data-ttu-id="9ff54-116">To create a new company</span><span class="sxs-lookup"><span data-stu-id="9ff54-116">To create a new company</span></span>  
1. <span data-ttu-id="9ff54-117">Create a new company.</span><span class="sxs-lookup"><span data-stu-id="9ff54-117">Create a new company.</span></span> <span data-ttu-id="9ff54-118">For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="9ff54-118">For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).</span></span>
2. <span data-ttu-id="9ff54-119">From the RapidStart Services Implementer Role Centre, you can now import the configuration package that you exported from the CRONUS International Ltd. company.</span><span class="sxs-lookup"><span data-stu-id="9ff54-119">From the RapidStart Services Implementer Role Center, you can now import the configuration package that you exported from the CRONUS International Ltd. company.</span></span>

<span data-ttu-id="9ff54-120">After you create a new company, some tables are automatically filled in, even if no company template is applied.</span><span class="sxs-lookup"><span data-stu-id="9ff54-120">After you create a new company, some tables are automatically filled in, even if no company template is applied.</span></span> <span data-ttu-id="9ff54-121">For example, you can review the standard codes for posting and batch transactions on the **Source Code** page.</span><span class="sxs-lookup"><span data-stu-id="9ff54-121">For example, you can review the standard codes for posting and batch transactions on the **Source Code** page.</span></span> <span data-ttu-id="9ff54-122">If you provide a local version of [!INCLUDE[prod_short](includes/prod_short.md)], you should review this table and consider any local language issues.</span><span class="sxs-lookup"><span data-stu-id="9ff54-122">If you provide a local version of [!INCLUDE[prod_short](includes/prod_short.md)], you should review this table and consider any local language issues.</span></span>

## <a name="about-data-tables"></a><span data-ttu-id="9ff54-123">About Data Tables</span><span class="sxs-lookup"><span data-stu-id="9ff54-123">About Data Tables</span></span>
[!INCLUDE[prod_short](includes/prod_short.md)]<span data-ttu-id="9ff54-124">, data tables come in two basic types: Master and Setup.</span><span class="sxs-lookup"><span data-stu-id="9ff54-124">, data tables come in two basic types: Master and Setup.</span></span> <span data-ttu-id="9ff54-125">When you are setting up a company configuration, you can use these types to focus your configuration strategy.</span><span class="sxs-lookup"><span data-stu-id="9ff54-125">When you are setting up a company configuration, you can use these types to focus your configuration strategy.</span></span>  

### <a name="master-data-tables"></a><span data-ttu-id="9ff54-126">Master Data Tables</span><span class="sxs-lookup"><span data-stu-id="9ff54-126">Master Data Tables</span></span>  
<span data-ttu-id="9ff54-127">The following table lists some of the master data tables.</span><span class="sxs-lookup"><span data-stu-id="9ff54-127">The following table lists some of the master data tables.</span></span> <span data-ttu-id="9ff54-128">When you initialise a new company, these tables are empty.</span><span class="sxs-lookup"><span data-stu-id="9ff54-128">When you initialize a new company, these tables are empty.</span></span>  

|<span data-ttu-id="9ff54-129">Table No.</span><span class="sxs-lookup"><span data-stu-id="9ff54-129">Table No.</span></span>|<span data-ttu-id="9ff54-130">Table Name</span><span class="sxs-lookup"><span data-stu-id="9ff54-130">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="9ff54-131">15</span><span class="sxs-lookup"><span data-stu-id="9ff54-131">15</span></span>|<span data-ttu-id="9ff54-132">G/L Account</span><span class="sxs-lookup"><span data-stu-id="9ff54-132">G/L Account</span></span>|  
|<span data-ttu-id="9ff54-133">18</span><span class="sxs-lookup"><span data-stu-id="9ff54-133">18</span></span>|<span data-ttu-id="9ff54-134">Customer</span><span class="sxs-lookup"><span data-stu-id="9ff54-134">Customer</span></span>|  
|<span data-ttu-id="9ff54-135">23</span><span class="sxs-lookup"><span data-stu-id="9ff54-135">23</span></span>|<span data-ttu-id="9ff54-136">Vendor</span><span class="sxs-lookup"><span data-stu-id="9ff54-136">Vendor</span></span>|  
|<span data-ttu-id="9ff54-137">27</span><span class="sxs-lookup"><span data-stu-id="9ff54-137">27</span></span>|<span data-ttu-id="9ff54-138">Item</span><span class="sxs-lookup"><span data-stu-id="9ff54-138">Item</span></span>|  
|<span data-ttu-id="9ff54-139">5050</span><span class="sxs-lookup"><span data-stu-id="9ff54-139">5050</span></span>|<span data-ttu-id="9ff54-140">Contact</span><span class="sxs-lookup"><span data-stu-id="9ff54-140">Contact</span></span>|  

### <a name="setup-data-tables"></a><span data-ttu-id="9ff54-141">Setup Data Tables</span><span class="sxs-lookup"><span data-stu-id="9ff54-141">Setup Data Tables</span></span>  
<span data-ttu-id="9ff54-142">The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire.</span><span class="sxs-lookup"><span data-stu-id="9ff54-142">The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire.</span></span> <span data-ttu-id="9ff54-143">These tables contain baseline information when the company is created.</span><span class="sxs-lookup"><span data-stu-id="9ff54-143">These tables contain baseline information when the company is created.</span></span>  

|<span data-ttu-id="9ff54-144">Table No.</span><span class="sxs-lookup"><span data-stu-id="9ff54-144">Table No.</span></span>|<span data-ttu-id="9ff54-145">Table Name</span><span class="sxs-lookup"><span data-stu-id="9ff54-145">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="9ff54-146">98</span><span class="sxs-lookup"><span data-stu-id="9ff54-146">98</span></span>|<span data-ttu-id="9ff54-147">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="9ff54-147">General Ledger Setup</span></span>|  
|<span data-ttu-id="9ff54-148">311</span><span class="sxs-lookup"><span data-stu-id="9ff54-148">311</span></span>|<span data-ttu-id="9ff54-149">Sales & Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="9ff54-149">Sales & Receivables Setup</span></span>|  
|<span data-ttu-id="9ff54-150">312</span><span class="sxs-lookup"><span data-stu-id="9ff54-150">312</span></span>|<span data-ttu-id="9ff54-151">Purchases & Payables Setup</span><span class="sxs-lookup"><span data-stu-id="9ff54-151">Purchases & Payables Setup</span></span>|  
|<span data-ttu-id="9ff54-152">313</span><span class="sxs-lookup"><span data-stu-id="9ff54-152">313</span></span>|<span data-ttu-id="9ff54-153">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="9ff54-153">Inventory Setup</span></span>|  

<span data-ttu-id="9ff54-154">In addition to setup data tables, [!INCLUDE[prod_short](includes/prod_short.md)] also has setup-type data tables that specify core information about the company and its business processes.</span><span class="sxs-lookup"><span data-stu-id="9ff54-154">In addition to setup data tables, [!INCLUDE[prod_short](includes/prod_short.md)] also has setup-type data tables that specify core information about the company and its business processes.</span></span> <span data-ttu-id="9ff54-155">The following table lists some of them.</span><span class="sxs-lookup"><span data-stu-id="9ff54-155">The following table lists some of them.</span></span>  

|<span data-ttu-id="9ff54-156">Table No.</span><span class="sxs-lookup"><span data-stu-id="9ff54-156">Table No.</span></span>|<span data-ttu-id="9ff54-157">Table Name</span><span class="sxs-lookup"><span data-stu-id="9ff54-157">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="9ff54-158">3</span><span class="sxs-lookup"><span data-stu-id="9ff54-158">3</span></span>|<span data-ttu-id="9ff54-159">Payment Terms</span><span class="sxs-lookup"><span data-stu-id="9ff54-159">Payment Terms</span></span>|  
|<span data-ttu-id="9ff54-160">4</span><span class="sxs-lookup"><span data-stu-id="9ff54-160">4</span></span>|<span data-ttu-id="9ff54-161">Currency</span><span class="sxs-lookup"><span data-stu-id="9ff54-161">Currency</span></span>|  
|<span data-ttu-id="9ff54-162">6</span><span class="sxs-lookup"><span data-stu-id="9ff54-162">6</span></span>|<span data-ttu-id="9ff54-163">Customer Price Groups</span><span class="sxs-lookup"><span data-stu-id="9ff54-163">Customer Price Groups</span></span>|  
|<span data-ttu-id="9ff54-164">5700</span><span class="sxs-lookup"><span data-stu-id="9ff54-164">5700</span></span>|<span data-ttu-id="9ff54-165">Stockkeeping Unit</span><span class="sxs-lookup"><span data-stu-id="9ff54-165">Stockkeeping Unit</span></span>|

  

## <a name="see-also"></a><span data-ttu-id="9ff54-166">See Also</span><span class="sxs-lookup"><span data-stu-id="9ff54-166">See Also</span></span>  
[<span data-ttu-id="9ff54-167">Apply Configurations to New Companies</span><span class="sxs-lookup"><span data-stu-id="9ff54-167">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="9ff54-168">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="9ff54-168">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="9ff54-169">Administration</span><span class="sxs-lookup"><span data-stu-id="9ff54-169">Administration</span></span>](admin-setup-and-administration.md)
