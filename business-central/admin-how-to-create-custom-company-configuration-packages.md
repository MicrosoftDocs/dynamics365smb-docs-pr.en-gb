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
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 511281b5f4d8c7437324ed123a5a5a62bd4cc51d
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3783665"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="fb5bc-104">Create Custom Company Configuration Packages</span><span class="sxs-lookup"><span data-stu-id="fb5bc-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="fb5bc-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="fb5bc-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="fb5bc-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="fb5bc-108">That lets you apply and set up new areas in a company as you need them</span><span class="sxs-lookup"><span data-stu-id="fb5bc-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="fb5bc-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span><span class="sxs-lookup"><span data-stu-id="fb5bc-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="fb5bc-110">Fixed Asset Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="fb5bc-111">General Ledger Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="fb5bc-112">Inventory Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-112">Inventory Setup</span></span>  
-   <span data-ttu-id="fb5bc-113">Manufacturing Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="fb5bc-114">Purchases and Payables Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="fb5bc-115">Marketing Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-115">Marketing Setup</span></span>  
-   <span data-ttu-id="fb5bc-116">Service Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-116">Service Setup</span></span>  
-   <span data-ttu-id="fb5bc-117">Sales and Receivables Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="fb5bc-118">Warehouse Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="fb5bc-119">General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-119">General Posting Setup</span></span>  
-   <span data-ttu-id="fb5bc-120">VAT Posting Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="fb5bc-121">Inventory Posting Setup</span><span class="sxs-lookup"><span data-stu-id="fb5bc-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="fb5bc-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="fb5bc-123">Use caution if you choose tables or fields that have the same temporal name but are differentiated by special characters, such as %, &, <, >, (, and ).</span><span class="sxs-lookup"><span data-stu-id="fb5bc-123">Use caution if you choose tables or fields that have the same temporal name but are differentiated by special characters, such as %, &, <, >, (, and ).</span></span> <span data-ttu-id="fb5bc-124">For example, table "XYZ" might contain the "Field 1" and "Field 1%" fields.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-124">For example, table "XYZ" might contain the "Field 1" and "Field 1%" fields.</span></span>
>
> <span data-ttu-id="fb5bc-125">The XML processor accepts only some special characters, and will remove those it does not.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-125">The XML processor accepts only some special characters, and will remove those it does not.</span></span> <span data-ttu-id="fb5bc-126">If removing a special character, such as the % sign in "Field 1%," results in two or more tables or fields with the same name an error will occur when you export or import a configuration package.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-126">If removing a special character, such as the % sign in "Field 1%," results in two or more tables or fields with the same name an error will occur when you export or import a configuration package.</span></span>

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="fb5bc-127">To create a custom company configuration package</span><span class="sxs-lookup"><span data-stu-id="fb5bc-127">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="fb5bc-128">Create a new company.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-128">Create a new company.</span></span> <span data-ttu-id="fb5bc-129">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="fb5bc-129">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span></span>  
3.  <span data-ttu-id="fb5bc-130">Set up the new company in the way you need.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-130">Set up the new company in the way you need.</span></span> <span data-ttu-id="fb5bc-131">Fill in all required setup tables.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-131">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="fb5bc-132">Open the new company.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-132">Open the new company.</span></span>
5. <span data-ttu-id="fb5bc-133">Open the **Configuration Worksheet** page.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-133">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="fb5bc-134">Add the tables that you want to transfer to another company to the worksheet.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-134">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="fb5bc-135">Assign the worksheet lines to the package.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-135">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="fb5bc-136">Create a questionnaire for the most frequently used setup tables.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-136">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="fb5bc-137">Create configuration templates to make it easier to create master data, such as customers or items.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-137">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="fb5bc-138">Export your package as a .rapidstart file.</span><span class="sxs-lookup"><span data-stu-id="fb5bc-138">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fb5bc-139">See Also</span><span class="sxs-lookup"><span data-stu-id="fb5bc-139">See Also</span></span>  
[<span data-ttu-id="fb5bc-140">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="fb5bc-140">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="fb5bc-141">Administration</span><span class="sxs-lookup"><span data-stu-id="fb5bc-141">Administration</span></span>](admin-setup-and-administration.md)
