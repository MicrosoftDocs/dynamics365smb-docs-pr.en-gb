---
title: How to Create Custom Company Configuration Packages | Microsoft Docs
description: As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers. You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 0f87e3708802898d1b86dfaae31b37cdee37ff74
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1244637"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="09a0f-104">Create Custom Company Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="09a0f-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="09a0f-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span><span class="sxs-lookup"><span data-stu-id="09a0f-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="09a0f-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span><span class="sxs-lookup"><span data-stu-id="09a0f-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="09a0f-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span><span class="sxs-lookup"><span data-stu-id="09a0f-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="09a0f-108">That lets you apply and set up new areas in a company as you need them</span><span class="sxs-lookup"><span data-stu-id="09a0f-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="09a0f-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span><span class="sxs-lookup"><span data-stu-id="09a0f-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="09a0f-110">Fixed Asset Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="09a0f-111">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="09a0f-112">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-112">Inventory Setup</span></span>  
-   <span data-ttu-id="09a0f-113">Manufacturing Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="09a0f-114">Purchases and Payables Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="09a0f-115">Marketing Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-115">Marketing Setup</span></span>  
-   <span data-ttu-id="09a0f-116">Service Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-116">Service Setup</span></span>  
-   <span data-ttu-id="09a0f-117">Sales and Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="09a0f-118">Warehouse Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="09a0f-119">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-119">General Posting Setup</span></span>  
-   <span data-ttu-id="09a0f-120">VAT Posting Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="09a0f-121">Inventory Posting Setup</span><span class="sxs-lookup"><span data-stu-id="09a0f-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="09a0f-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="09a0f-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="09a0f-123">To create a custom company configuration package</span><span class="sxs-lookup"><span data-stu-id="09a0f-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="09a0f-124">Create a new company.</span><span class="sxs-lookup"><span data-stu-id="09a0f-124">Create a new company.</span></span> <span data-ttu-id="09a0f-125">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="09a0f-125">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span></span>  
3.  <span data-ttu-id="09a0f-126">Set up the new company in the way you need.</span><span class="sxs-lookup"><span data-stu-id="09a0f-126">Set up the new company in the way you need.</span></span> <span data-ttu-id="09a0f-127">Fill in all required setup tables.</span><span class="sxs-lookup"><span data-stu-id="09a0f-127">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="09a0f-128">Open the new company.</span><span class="sxs-lookup"><span data-stu-id="09a0f-128">Open the new company.</span></span>
5. <span data-ttu-id="09a0f-129">Open the **Configuration Worksheet** page.</span><span class="sxs-lookup"><span data-stu-id="09a0f-129">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="09a0f-130">Add the tables that you want to transfer to another company to the worksheet.</span><span class="sxs-lookup"><span data-stu-id="09a0f-130">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="09a0f-131">Assign the worksheet lines to the package.</span><span class="sxs-lookup"><span data-stu-id="09a0f-131">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="09a0f-132">Create a questionnaire for the most frequently used setup tables.</span><span class="sxs-lookup"><span data-stu-id="09a0f-132">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="09a0f-133">Create configuration templates to make it easier to create master data, such as customers or items.</span><span class="sxs-lookup"><span data-stu-id="09a0f-133">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="09a0f-134">Export your package as a .rapidstart file.</span><span class="sxs-lookup"><span data-stu-id="09a0f-134">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="09a0f-135">See Also</span><span class="sxs-lookup"><span data-stu-id="09a0f-135">See Also</span></span>  
[<span data-ttu-id="09a0f-136">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="09a0f-136">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="09a0f-137">Administration</span><span class="sxs-lookup"><span data-stu-id="09a0f-137">Administration</span></span>](admin-setup-and-administration.md)
