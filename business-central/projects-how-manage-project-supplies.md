---
title: Purchase Items or Services for a Job and Manage Supplies| Microsoft Docs
description: Describes how to manage the supply and purchase of material and services to jobs.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 78a11b0c20f8ef6c1c190f38cc5dcfcee918c8e2
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3191242"
---
# <a name="manage-job-supplies"></a><span data-ttu-id="375f2-103">Manage Job Supplies</span><span class="sxs-lookup"><span data-stu-id="375f2-103">Manage Job Supplies</span></span>
<span data-ttu-id="375f2-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span><span class="sxs-lookup"><span data-stu-id="375f2-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="375f2-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="375f2-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="375f2-106">For example, a service job on a computer requires a new disk.</span><span class="sxs-lookup"><span data-stu-id="375f2-106">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="375f2-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span><span class="sxs-lookup"><span data-stu-id="375f2-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="375f2-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed on the **Job G/L Journal** page.</span><span class="sxs-lookup"><span data-stu-id="375f2-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed on the **Job G/L Journal** page.</span></span> <span data-ttu-id="375f2-109">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="375f2-109">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="375f2-110">To purchase items or services for a job</span><span class="sxs-lookup"><span data-stu-id="375f2-110">To purchase items or services for a job</span></span>
<span data-ttu-id="375f2-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span><span class="sxs-lookup"><span data-stu-id="375f2-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="375f2-112">The same steps apply when using a purchase order.</span><span class="sxs-lookup"><span data-stu-id="375f2-112">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="375f2-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="375f2-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="375f2-114">Choose the **New** action and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="375f2-114">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="375f2-115">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="375f2-115">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="375f2-116">In the **Job No.** and **Job Task No.** fields, select the information of the job that you want to purchase items or services for.</span><span class="sxs-lookup"><span data-stu-id="375f2-116">In the **Job No.** and **Job Task No.** fields, select the information of the job that you want to purchase items or services for.</span></span> <span data-ttu-id="375f2-117">Use the **Choose Columns** function if the field is not visible.</span><span class="sxs-lookup"><span data-stu-id="375f2-117">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="375f2-118">For more information, see [Personalise Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="375f2-118">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

    <span data-ttu-id="375f2-119">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span><span class="sxs-lookup"><span data-stu-id="375f2-119">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="375f2-120">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span><span class="sxs-lookup"><span data-stu-id="375f2-120">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="375f2-121">For more information, see [Invoice Jobs](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="375f2-121">For more information, see [Invoice Jobs](projects-how-invoice-jobs.md).</span></span>
4. <span data-ttu-id="375f2-122">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="375f2-122">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="375f2-123">To view the value of purchases for a job</span><span class="sxs-lookup"><span data-stu-id="375f2-123">To view the value of purchases for a job</span></span>
1. <span data-ttu-id="375f2-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="375f2-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="375f2-125">Open a relevant job card.</span><span class="sxs-lookup"><span data-stu-id="375f2-125">Open a relevant job card.</span></span>

    <span data-ttu-id="375f2-126">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span><span class="sxs-lookup"><span data-stu-id="375f2-126">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="375f2-127">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span><span class="sxs-lookup"><span data-stu-id="375f2-127">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  
3. <span data-ttu-id="375f2-128">Choose either of the fields to open the **Purchase Lines** page where you can review information about the related purchase document lines, including which items or services have been received.</span><span class="sxs-lookup"><span data-stu-id="375f2-128">Choose either of the fields to open the **Purchase Lines** page where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="375f2-129">To post a job-related expense</span><span class="sxs-lookup"><span data-stu-id="375f2-129">To post a job-related expense</span></span>
<span data-ttu-id="375f2-130">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** page to post them directly to the relevant job account.</span><span class="sxs-lookup"><span data-stu-id="375f2-130">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** page to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="375f2-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="375f2-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="375f2-132">Create a new line and enter information about the expense, including information in the **Job No.** and **Job Task No** fields.</span><span class="sxs-lookup"><span data-stu-id="375f2-132">Create a new line and enter information about the expense, including information in the **Job No.** and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="375f2-133">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="375f2-133">When the journal is complete, choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="375f2-134">See Also</span><span class="sxs-lookup"><span data-stu-id="375f2-134">See Also</span></span>
[<span data-ttu-id="375f2-135">Project Management</span><span class="sxs-lookup"><span data-stu-id="375f2-135">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="375f2-136">Finance</span><span class="sxs-lookup"><span data-stu-id="375f2-136">Finance</span></span>](finance.md)  
<span data-ttu-id="375f2-137">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="375f2-137">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="375f2-138">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="375f2-138">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="375f2-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="375f2-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
