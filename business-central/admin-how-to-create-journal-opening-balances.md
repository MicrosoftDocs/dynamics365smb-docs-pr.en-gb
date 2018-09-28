---
title: How to Create Journal Opening Balances | Microsoft Docs
description: Business Central includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company. You can easily transfer this data with journals postings.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 612eb9cfa5c6cd45bf154f4813efa3b349f44841
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="create-journal-opening-balances"></a><span data-ttu-id="60cb7-104">Create Journal Opening Balances</span><span class="sxs-lookup"><span data-stu-id="60cb7-104">Create Journal Opening Balances</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="60cb7-105">includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company.</span><span class="sxs-lookup"><span data-stu-id="60cb7-105"> includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company.</span></span> <span data-ttu-id="60cb7-106">You can easily transfer this data with the customer journal, the vendor journal, the item journal, or the G/L journal.</span><span class="sxs-lookup"><span data-stu-id="60cb7-106">You can easily transfer this data with the customer journal, the vendor journal, the item journal, or the G/L journal.</span></span>

<span data-ttu-id="60cb7-107">The first step is to create a configuration package that includes the setup tables for those journals.</span><span class="sxs-lookup"><span data-stu-id="60cb7-107">The first step is to create a configuration package that includes the setup tables for those journals.</span></span> <span data-ttu-id="60cb7-108">The following procedure assumes that this step is completed.</span><span class="sxs-lookup"><span data-stu-id="60cb7-108">The following procedure assumes that this step is completed.</span></span> <span data-ttu-id="60cb7-109">For more information, see [Set Up Company Configuration](admin-set-up-company-configuration.md).</span><span class="sxs-lookup"><span data-stu-id="60cb7-109">For more information, see [Set Up Company Configuration](admin-set-up-company-configuration.md).</span></span> <span data-ttu-id="60cb7-110">This procedure describes the subsequent steps, which include applying the package that is provided by a partner.</span><span class="sxs-lookup"><span data-stu-id="60cb7-110">This procedure describes the subsequent steps, which include applying the package that is provided by a partner.</span></span>  

<span data-ttu-id="60cb7-111">Before you start, make sure that you are on the RapidStart Services Implementer Role Centre page as it provides the correct context for your configuration work.</span><span class="sxs-lookup"><span data-stu-id="60cb7-111">Before you start, make sure that you are on the RapidStart Services Implementer Role Center page as it provides the correct context for your configuration work.</span></span> <span data-ttu-id="60cb7-112">For more information, see [Changing Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="60cb7-112">For more information, see [Changing Basic Settings](ui-change-basic-settings.md).</span></span>

## <a name="to-apply-the-entries-in-a-journal-to-a-new-company"></a><span data-ttu-id="60cb7-113">To apply the entries in a journal to a new company</span><span class="sxs-lookup"><span data-stu-id="60cb7-113">To apply the entries in a journal to a new company</span></span>  
1. <span data-ttu-id="60cb7-114">Configure a new company and apply a configuration package to it.</span><span class="sxs-lookup"><span data-stu-id="60cb7-114">Configure a new company and apply a configuration package to it.</span></span> <span data-ttu-id="60cb7-115">For more information, see [Configure a Company with the RapidStart Wizard](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).</span><span class="sxs-lookup"><span data-stu-id="60cb7-115">For more information, see [Configure a Company with the RapidStart Wizard](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).</span></span>  

    <span data-ttu-id="60cb7-116">The new company does not contain information about journal opening balances.</span><span class="sxs-lookup"><span data-stu-id="60cb7-116">The new company does not contain information about journal opening balances.</span></span>  

2. <span data-ttu-id="60cb7-117">Open the configuration worksheet and import existing data about customers, items, vendors, and the general ledger.</span><span class="sxs-lookup"><span data-stu-id="60cb7-117">Open the configuration worksheet and import existing data about customers, items, vendors, and the general ledger.</span></span> <span data-ttu-id="60cb7-118">For more information, see [Migrate Customer Data](admin-migrate-customer-data.md).</span><span class="sxs-lookup"><span data-stu-id="60cb7-118">For more information, see [Migrate Customer Data](admin-migrate-customer-data.md).</span></span>  
3. <span data-ttu-id="60cb7-119">Choose, for example, the **Create G/L Journal Lines** action.</span><span class="sxs-lookup"><span data-stu-id="60cb7-119">Choose, for example, the **Create G/L Journal Lines** action.</span></span>  
4. <span data-ttu-id="60cb7-120">Fill in the **Options** FastTab as appropriate, and set filters as needed.</span><span class="sxs-lookup"><span data-stu-id="60cb7-120">Fill in the **Options** FastTab as appropriate, and set filters as needed.</span></span> <span data-ttu-id="60cb7-121">For example, in the **Journal Template** field, enter a name.</span><span class="sxs-lookup"><span data-stu-id="60cb7-121">For example, in the **Journal Template** field, enter a name.</span></span>  
5. <span data-ttu-id="60cb7-122">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="60cb7-122">Choose the **OK** button.</span></span> <span data-ttu-id="60cb7-123">The records are now in the journal, but the amounts are empty.</span><span class="sxs-lookup"><span data-stu-id="60cb7-123">The records are now in the journal, but the amounts are empty.</span></span>  
6. <span data-ttu-id="60cb7-124">Export the journal table to Excel and manually enter the posting and balancing account information from the legacy data.</span><span class="sxs-lookup"><span data-stu-id="60cb7-124">Export the journal table to Excel and manually enter the posting and balancing account information from the legacy data.</span></span>
7. <span data-ttu-id="60cb7-125">Import and apply the table information into the new company.</span><span class="sxs-lookup"><span data-stu-id="60cb7-125">Import and apply the table information into the new company.</span></span> <span data-ttu-id="60cb7-126">The journal lines are ready for posting.</span><span class="sxs-lookup"><span data-stu-id="60cb7-126">The journal lines are ready for posting.</span></span>  
8. <span data-ttu-id="60cb7-127">In the configuration worksheet, select the journal line table, and then choose the **Database Data** action.</span><span class="sxs-lookup"><span data-stu-id="60cb7-127">In the configuration worksheet, select the journal line table, and then choose the **Database Data** action.</span></span>  
9. <span data-ttu-id="60cb7-128">Review the information, and then choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="60cb7-128">Review the information, and then choose the **Post** action.</span></span>  
10. <span data-ttu-id="60cb7-129">Repeat the steps to import and post any other opening balances.</span><span class="sxs-lookup"><span data-stu-id="60cb7-129">Repeat the steps to import and post any other opening balances.</span></span>  

## <a name="see-also"></a><span data-ttu-id="60cb7-130">See Also</span><span class="sxs-lookup"><span data-stu-id="60cb7-130">See Also</span></span>  
[<span data-ttu-id="60cb7-131">Apply Configurations to New Companies</span><span class="sxs-lookup"><span data-stu-id="60cb7-131">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="60cb7-132">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="60cb7-132">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="60cb7-133">Administration</span><span class="sxs-lookup"><span data-stu-id="60cb7-133">Administration</span></span>](admin-setup-and-administration.md)

