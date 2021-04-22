---
title: Create a Job Sales Invoice to Invoice a Job| Microsoft Docs
description: Describes how to invoice customers for job expenses as a project progresses.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f9290bda4437ea43edcaa19d7759f2fdee24e8c4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775072"
---
# <a name="invoice-jobs"></a><span data-ttu-id="ea94c-103">Invoice Jobs</span><span class="sxs-lookup"><span data-stu-id="ea94c-103">Invoice Jobs</span></span>
<span data-ttu-id="ea94c-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span><span class="sxs-lookup"><span data-stu-id="ea94c-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="ea94c-105">As the job progresses, these transactions get posted to the job journal.</span><span class="sxs-lookup"><span data-stu-id="ea94c-105">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="ea94c-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span><span class="sxs-lookup"><span data-stu-id="ea94c-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

> [!NOTE]
> <span data-ttu-id="ea94c-107">You can also purchase external resources unrelated to a job, for example, to invoice a vendor for work delivered.</span><span class="sxs-lookup"><span data-stu-id="ea94c-107">You can also purchase external resources unrelated to a job, for example, to invoice a vendor for work delivered.</span></span> <span data-ttu-id="ea94c-108">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="ea94c-108">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

<span data-ttu-id="ea94c-109">You can invoice the whole job from the **Job Task Lines** page or only invoice selected billable lines from the **Planning Lines** page.</span><span class="sxs-lookup"><span data-stu-id="ea94c-109">You can invoice the whole job from the **Job Task Lines** page or only invoice selected billable lines from the **Planning Lines** page.</span></span> <span data-ttu-id="ea94c-110">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span><span class="sxs-lookup"><span data-stu-id="ea94c-110">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

> [!NOTE]  
> <span data-ttu-id="ea94c-111">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span><span class="sxs-lookup"><span data-stu-id="ea94c-111">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="ea94c-112">For more information, see [Manage Project Supplies](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="ea94c-112">For more information, see [Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-multiple-job-sales-invoices"></a><span data-ttu-id="ea94c-113">To create multiple job sales invoices</span><span class="sxs-lookup"><span data-stu-id="ea94c-113">To create multiple job sales invoices</span></span>
<span data-ttu-id="ea94c-114">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span><span class="sxs-lookup"><span data-stu-id="ea94c-114">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="ea94c-115">The following procedure shows how to use a batch job to invoice multiple jobs.</span><span class="sxs-lookup"><span data-stu-id="ea94c-115">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="ea94c-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea94c-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ea94c-117">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea94c-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="ea94c-118">Set filters if you want to limit the jobs that the batch job will process.</span><span class="sxs-lookup"><span data-stu-id="ea94c-118">Set filters if you want to limit the jobs that the batch job will process.</span></span>
4. <span data-ttu-id="ea94c-119">Choose the **OK** button to create the invoices.</span><span class="sxs-lookup"><span data-stu-id="ea94c-119">Choose the **OK** button to create the invoices.</span></span>  

<span data-ttu-id="ea94c-120">You can review and post created invoices in the **Sales Invoices** window.</span><span class="sxs-lookup"><span data-stu-id="ea94c-120">You can review and post created invoices in the **Sales Invoices** window.</span></span>

> [!NOTE]
> <span data-ttu-id="ea94c-121">Alternatively, invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-121">Alternatively, invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> 

## <a name="to-create-and-post-job-sales-invoice-from-job-planning-lines"></a><span data-ttu-id="ea94c-122">To create and post job sales invoice from job planning lines</span><span class="sxs-lookup"><span data-stu-id="ea94c-122">To create and post job sales invoice from job planning lines</span></span>
<span data-ttu-id="ea94c-123">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span><span class="sxs-lookup"><span data-stu-id="ea94c-123">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="ea94c-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea94c-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea94c-125">Open a relevant job.</span><span class="sxs-lookup"><span data-stu-id="ea94c-125">Open a relevant job.</span></span>
3. <span data-ttu-id="ea94c-126">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-126">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="ea94c-127">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span><span class="sxs-lookup"><span data-stu-id="ea94c-127">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="ea94c-128">Choose the **Create Sales Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-128">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="ea94c-129">On the **Job Create Sales Invoice** page, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span><span class="sxs-lookup"><span data-stu-id="ea94c-129">On the **Job Create Sales Invoice** page, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="ea94c-130">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="ea94c-130">Choose the **OK** button.</span></span>  
8. <span data-ttu-id="ea94c-131">On the **Job Planning Lines** page, choose the **Sales Invoices/Credit Memos** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-131">On the **Job Planning Lines** page, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="ea94c-132">The **Sales Invoice** page opens, showing the quantity that you have transferred to the invoice.</span><span class="sxs-lookup"><span data-stu-id="ea94c-132">The **Sales Invoice** page opens, showing the quantity that you have transferred to the invoice.</span></span>
9. <span data-ttu-id="ea94c-133">Make any additional changes, and then choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-133">Make any additional changes, and then choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ea94c-134">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span><span class="sxs-lookup"><span data-stu-id="ea94c-134">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="ea94c-135">To calculate and post job completion entries</span><span class="sxs-lookup"><span data-stu-id="ea94c-135">To calculate and post job completion entries</span></span>
<span data-ttu-id="ea94c-136">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span><span class="sxs-lookup"><span data-stu-id="ea94c-136">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="ea94c-137">Then, you must reverse any WIP that has been posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="ea94c-137">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="ea94c-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea94c-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ea94c-139">Select an open job, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-139">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="ea94c-140">In the **Status** field, select **Completed**.</span><span class="sxs-lookup"><span data-stu-id="ea94c-140">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="ea94c-141">Follow the assistance steps to calculate and post WIP.</span><span class="sxs-lookup"><span data-stu-id="ea94c-141">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="ea94c-142">Alternatively, follows steps 5 and 6 to do so manually.</span><span class="sxs-lookup"><span data-stu-id="ea94c-142">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="ea94c-143">Choose the **Calculate WIP** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-143">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="ea94c-144">On the **Job Calculate WIP** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea94c-144">On the **Job Calculate WIP** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="ea94c-145">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span><span class="sxs-lookup"><span data-stu-id="ea94c-145">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  
7. <span data-ttu-id="ea94c-146">Choose the **Job Post WIP to G/L** action.</span><span class="sxs-lookup"><span data-stu-id="ea94c-146">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="ea94c-147">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ea94c-147">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="ea94c-148">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span><span class="sxs-lookup"><span data-stu-id="ea94c-148">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="ea94c-149">See Also</span><span class="sxs-lookup"><span data-stu-id="ea94c-149">See Also</span></span>
[<span data-ttu-id="ea94c-150">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="ea94c-150">Managing Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="ea94c-151">Finance</span><span class="sxs-lookup"><span data-stu-id="ea94c-151">Finance</span></span>](finance.md)  
<span data-ttu-id="ea94c-152">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="ea94c-152">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="ea94c-153">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="ea94c-153">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="ea94c-154">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ea94c-154">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]