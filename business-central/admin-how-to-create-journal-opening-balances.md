---
title: How to Create Journal Opening Balances | Microsoft Docs
description: Business Central includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company. You can easily transfer this data with journals postings.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/14/2020
ms.author: edupont
ms.openlocfilehash: 9984d61e97ff6c04733bd10818deb1d6cf57a66c
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3783633"
---
# <a name="create-journal-opening-balances"></a><span data-ttu-id="90496-104">Create Journal Opening Balances</span><span class="sxs-lookup"><span data-stu-id="90496-104">Create Journal Opening Balances</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="90496-105">includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company.</span><span class="sxs-lookup"><span data-stu-id="90496-105">includes several batch jobs that are provided to help in the transfer of legacy account balances to a newly configured company.</span></span> <span data-ttu-id="90496-106">You can easily transfer this data with the customer journal, the vendor journal, the item journal, or the G/L journal.</span><span class="sxs-lookup"><span data-stu-id="90496-106">You can easily transfer this data with the customer journal, the vendor journal, the item journal, or the G/L journal.</span></span>

<span data-ttu-id="90496-107">The first step is to create a configuration package that includes the setup tables for those journals.</span><span class="sxs-lookup"><span data-stu-id="90496-107">The first step is to create a configuration package that includes the setup tables for those journals.</span></span> <span data-ttu-id="90496-108">The following procedure assumes that this step is completed.</span><span class="sxs-lookup"><span data-stu-id="90496-108">The following procedure assumes that this step is completed.</span></span> <span data-ttu-id="90496-109">For more information, see [Set Up Company Configuration](admin-set-up-company-configuration.md).</span><span class="sxs-lookup"><span data-stu-id="90496-109">For more information, see [Set Up Company Configuration](admin-set-up-company-configuration.md).</span></span> <span data-ttu-id="90496-110">This procedure describes the subsequent steps, which include applying the package that is provided by a partner.</span><span class="sxs-lookup"><span data-stu-id="90496-110">This procedure describes the subsequent steps, which include applying the package that is provided by a partner.</span></span>  

<span data-ttu-id="90496-111">Before you start, make sure that you are using the Administration Role Centre page because it provides the correct context for your configuration work.</span><span class="sxs-lookup"><span data-stu-id="90496-111">Before you start, make sure that you are using the Administration Role Center page because it provides the correct context for your configuration work.</span></span> <span data-ttu-id="90496-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="90496-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>

## <a name="to-apply-the-entries-in-a-journal-to-a-new-company"></a><span data-ttu-id="90496-113">To apply the entries in a journal to a new company</span><span class="sxs-lookup"><span data-stu-id="90496-113">To apply the entries in a journal to a new company</span></span>

1. <span data-ttu-id="90496-114">Configure a new company and apply a configuration package to it.</span><span class="sxs-lookup"><span data-stu-id="90496-114">Configure a new company and apply a configuration package to it.</span></span> <span data-ttu-id="90496-115">For more information, see [Configure a Company with the RapidStart Wizard](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).</span><span class="sxs-lookup"><span data-stu-id="90496-115">For more information, see [Configure a Company with the RapidStart Wizard](admin-how-to-configure-a-company-with-the-rapidstart-wizard.md).</span></span>  

    <span data-ttu-id="90496-116">The new company does not contain information about journal opening balances.</span><span class="sxs-lookup"><span data-stu-id="90496-116">The new company does not contain information about journal opening balances.</span></span>  

2. <span data-ttu-id="90496-117">Open the configuration worksheet and import existing data about customers, items, vendors, and the general ledger.</span><span class="sxs-lookup"><span data-stu-id="90496-117">Open the configuration worksheet and import existing data about customers, items, vendors, and the general ledger.</span></span> <span data-ttu-id="90496-118">For more information, see [Migrate Customer Data](admin-migrate-customer-data.md).</span><span class="sxs-lookup"><span data-stu-id="90496-118">For more information, see [Migrate Customer Data](admin-migrate-customer-data.md).</span></span>  

    <span data-ttu-id="90496-119">Now you have master data in place.</span><span class="sxs-lookup"><span data-stu-id="90496-119">Now you have master data in place.</span></span> <span data-ttu-id="90496-120">Next, you add the opening balances.</span><span class="sxs-lookup"><span data-stu-id="90496-120">Next, you add the opening balances.</span></span> <span data-ttu-id="90496-121">The following steps describe how to create journal lines for G/L accounts, but the same apply to creating journal lines for customers, vendors, and items.</span><span class="sxs-lookup"><span data-stu-id="90496-121">The following steps describe how to create journal lines for G/L accounts, but the same apply to creating journal lines for customers, vendors, and items.</span></span>  
3. <span data-ttu-id="90496-122">Choose the **Create G/L Acct. Journal Lines** action.</span><span class="sxs-lookup"><span data-stu-id="90496-122">Choose the **Create G/L Acct. Journal Lines** action.</span></span>  
4. <span data-ttu-id="90496-123">Fill in the **Options** FastTab as appropriate, and set filters as needed.</span><span class="sxs-lookup"><span data-stu-id="90496-123">Fill in the **Options** FastTab as appropriate, and set filters as needed.</span></span> <span data-ttu-id="90496-124">For example, in the **Journal Template** field, enter a name.</span><span class="sxs-lookup"><span data-stu-id="90496-124">For example, in the **Journal Template** field, enter a name.</span></span>  
5. <span data-ttu-id="90496-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="90496-125">Choose the **OK** button.</span></span> <span data-ttu-id="90496-126">The records are now in the journal, but the amounts are empty.</span><span class="sxs-lookup"><span data-stu-id="90496-126">The records are now in the journal, but the amounts are empty.</span></span>  
6. <span data-ttu-id="90496-127">Export the journal table to Excel and manually enter the posting and balancing account information from the legacy data.</span><span class="sxs-lookup"><span data-stu-id="90496-127">Export the journal table to Excel and manually enter the posting and balancing account information from the legacy data.</span></span>
7. <span data-ttu-id="90496-128">Import and apply the table information into the new company.</span><span class="sxs-lookup"><span data-stu-id="90496-128">Import and apply the table information into the new company.</span></span> <span data-ttu-id="90496-129">The journal lines are ready for posting.</span><span class="sxs-lookup"><span data-stu-id="90496-129">The journal lines are ready for posting.</span></span>  
8. <span data-ttu-id="90496-130">In the configuration worksheet, select the journal line table, and then choose the **Database Data** action.</span><span class="sxs-lookup"><span data-stu-id="90496-130">In the configuration worksheet, select the journal line table, and then choose the **Database Data** action.</span></span>  
9. <span data-ttu-id="90496-131">Review the information, and then choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="90496-131">Review the information, and then choose the **Post** action.</span></span>  
10. <span data-ttu-id="90496-132">Repeat the steps to import and post any other opening balances.</span><span class="sxs-lookup"><span data-stu-id="90496-132">Repeat the steps to import and post any other opening balances.</span></span>  

> [!TIP]
> <span data-ttu-id="90496-133">You can use the same batch jobs to add opening balances whenever you register a new customer or vendor that you have done business with before but not registered in [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="90496-133">You can use the same batch jobs to add opening balances whenever you register a new customer or vendor that you have done business with before but not registered in [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="90496-134">Just search for the relevant task, and then choose the relevant link.</span><span class="sxs-lookup"><span data-stu-id="90496-134">Just search for the relevant task, and then choose the relevant link.</span></span>

## <a name="see-also"></a><span data-ttu-id="90496-135">See Also</span><span class="sxs-lookup"><span data-stu-id="90496-135">See Also</span></span>

[<span data-ttu-id="90496-136">Apply Configurations to New Companies</span><span class="sxs-lookup"><span data-stu-id="90496-136">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="90496-137">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="90496-137">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="90496-138">Administration</span><span class="sxs-lookup"><span data-stu-id="90496-138">Administration</span></span>](admin-setup-and-administration.md)  
