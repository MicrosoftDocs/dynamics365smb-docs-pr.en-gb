---
title: Purchase Items or Services for a Job and Manage Supplies| Microsoft Docs
description: Describes how to manage the supply and purchase of material and services to jobs.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 46cae53022ba5d65a370694c9818f52a7bf45525
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="419a7-103">How to: Manage Job Supplies</span><span class="sxs-lookup"><span data-stu-id="419a7-103">How to: Manage Job Supplies</span></span>
<span data-ttu-id="419a7-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span><span class="sxs-lookup"><span data-stu-id="419a7-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="419a7-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="419a7-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="419a7-106">For example, a service job on a computer requires a new disk.</span><span class="sxs-lookup"><span data-stu-id="419a7-106">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="419a7-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span><span class="sxs-lookup"><span data-stu-id="419a7-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="419a7-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span><span class="sxs-lookup"><span data-stu-id="419a7-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="419a7-109">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="419a7-109">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="419a7-110">To purchase items or services for a job</span><span class="sxs-lookup"><span data-stu-id="419a7-110">To purchase items or services for a job</span></span>
<span data-ttu-id="419a7-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span><span class="sxs-lookup"><span data-stu-id="419a7-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="419a7-112">The same steps apply when using a purchase order.</span><span class="sxs-lookup"><span data-stu-id="419a7-112">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="419a7-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="419a7-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="419a7-114">Choose the **New** action and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="419a7-114">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="419a7-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="419a7-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="419a7-116">In the **Job No.**</span><span class="sxs-lookup"><span data-stu-id="419a7-116">In the **Job No.**</span></span> <span data-ttu-id="419a7-117">and **Job Task No.**</span><span class="sxs-lookup"><span data-stu-id="419a7-117">and **Job Task No.**</span></span> <span data-ttu-id="419a7-118">fields, select the information of the job that you want to purchase items or services for.</span><span class="sxs-lookup"><span data-stu-id="419a7-118">fields, select the information of the job that you want to purchase items or services for.</span></span> <span data-ttu-id="419a7-119">Use the **Choose Columns** function if the field is not visible.</span><span class="sxs-lookup"><span data-stu-id="419a7-119">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="419a7-120">For more information, see [User Personalization](ui-user-personalization.md).</span><span class="sxs-lookup"><span data-stu-id="419a7-120">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

    <span data-ttu-id="419a7-121">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span><span class="sxs-lookup"><span data-stu-id="419a7-121">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="419a7-122">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span><span class="sxs-lookup"><span data-stu-id="419a7-122">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="419a7-123">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="419a7-123">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>
4. <span data-ttu-id="419a7-124">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="419a7-124">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="419a7-125">To view the value of purchases for a job</span><span class="sxs-lookup"><span data-stu-id="419a7-125">To view the value of purchases for a job</span></span>
1. <span data-ttu-id="419a7-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="419a7-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="419a7-127">Open a relevant job card.</span><span class="sxs-lookup"><span data-stu-id="419a7-127">Open a relevant job card.</span></span>

    <span data-ttu-id="419a7-128">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span><span class="sxs-lookup"><span data-stu-id="419a7-128">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="419a7-129">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span><span class="sxs-lookup"><span data-stu-id="419a7-129">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  
3. <span data-ttu-id="419a7-130">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span><span class="sxs-lookup"><span data-stu-id="419a7-130">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="419a7-131">To post a job-related expense</span><span class="sxs-lookup"><span data-stu-id="419a7-131">To post a job-related expense</span></span>
<span data-ttu-id="419a7-132">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span><span class="sxs-lookup"><span data-stu-id="419a7-132">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="419a7-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="419a7-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="419a7-134">Create a new line and enter information about the expense, including information in the **Job No.**</span><span class="sxs-lookup"><span data-stu-id="419a7-134">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="419a7-135">and **Job Task No** fields.</span><span class="sxs-lookup"><span data-stu-id="419a7-135">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="419a7-136">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="419a7-136">When the journal is complete, choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="419a7-137">See Also</span><span class="sxs-lookup"><span data-stu-id="419a7-137">See Also</span></span>
[<span data-ttu-id="419a7-138">Project Management</span><span class="sxs-lookup"><span data-stu-id="419a7-138">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="419a7-139">Finance</span><span class="sxs-lookup"><span data-stu-id="419a7-139">Finance</span></span>](finance.md)  
<span data-ttu-id="419a7-140">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="419a7-140">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="419a7-141">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="419a7-141">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="419a7-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="419a7-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

