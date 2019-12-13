---
title: How to Create Custom Company Configuration Packages | Microsoft Docs
description: As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers. You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 99fad48961dc201a25af061cf982a1c65d9446bd
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878872"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="79b23-104">Create Custom Company Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="79b23-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="79b23-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span><span class="sxs-lookup"><span data-stu-id="79b23-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="79b23-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span><span class="sxs-lookup"><span data-stu-id="79b23-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="79b23-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span><span class="sxs-lookup"><span data-stu-id="79b23-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="79b23-108">That lets you apply and set up new areas in a company as you need them</span><span class="sxs-lookup"><span data-stu-id="79b23-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="79b23-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span><span class="sxs-lookup"><span data-stu-id="79b23-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="79b23-110">Fixed Asset Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="79b23-111">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="79b23-112">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-112">Inventory Setup</span></span>  
-   <span data-ttu-id="79b23-113">Manufacturing Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="79b23-114">Purchases and Payables Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="79b23-115">Marketing Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-115">Marketing Setup</span></span>  
-   <span data-ttu-id="79b23-116">Service Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-116">Service Setup</span></span>  
-   <span data-ttu-id="79b23-117">Sales and Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="79b23-118">Warehouse Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="79b23-119">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-119">General Posting Setup</span></span>  
-   <span data-ttu-id="79b23-120">VAT Posting Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="79b23-121">Inventory Posting Setup</span><span class="sxs-lookup"><span data-stu-id="79b23-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="79b23-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="79b23-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="79b23-123">To create a custom company configuration package</span><span class="sxs-lookup"><span data-stu-id="79b23-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="79b23-124">Create a new company.</span><span class="sxs-lookup"><span data-stu-id="79b23-124">Create a new company.</span></span> <span data-ttu-id="79b23-125">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="79b23-125">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span></span>  
3.  <span data-ttu-id="79b23-126">Set up the new company in the way you need.</span><span class="sxs-lookup"><span data-stu-id="79b23-126">Set up the new company in the way you need.</span></span> <span data-ttu-id="79b23-127">Fill in all required setup tables.</span><span class="sxs-lookup"><span data-stu-id="79b23-127">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="79b23-128">Open the new company.</span><span class="sxs-lookup"><span data-stu-id="79b23-128">Open the new company.</span></span>
5. <span data-ttu-id="79b23-129">Open the **Configuration Worksheet** page.</span><span class="sxs-lookup"><span data-stu-id="79b23-129">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="79b23-130">Add the tables that you want to transfer to another company to the worksheet.</span><span class="sxs-lookup"><span data-stu-id="79b23-130">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="79b23-131">Assign the worksheet lines to the package.</span><span class="sxs-lookup"><span data-stu-id="79b23-131">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="79b23-132">Create a questionnaire for the most frequently used setup tables.</span><span class="sxs-lookup"><span data-stu-id="79b23-132">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="79b23-133">Create configuration templates to make it easier to create master data, such as customers or items.</span><span class="sxs-lookup"><span data-stu-id="79b23-133">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="79b23-134">Export your package as a .rapidstart file.</span><span class="sxs-lookup"><span data-stu-id="79b23-134">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="79b23-135">See Also</span><span class="sxs-lookup"><span data-stu-id="79b23-135">See Also</span></span>  
[<span data-ttu-id="79b23-136">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="79b23-136">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="79b23-137">Administration</span><span class="sxs-lookup"><span data-stu-id="79b23-137">Administration</span></span>](admin-setup-and-administration.md)
