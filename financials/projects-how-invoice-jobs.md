---
title: Create a Job Sales Invoice to Invoice a Job| Microsoft Docs
description: Describes how to invoice customers for job expenses as a project progresses.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9367dc5875b687b95076efffb3b0df2019332651
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-invoice-jobs"></a><span data-ttu-id="ab20d-103">How to: Invoice Jobs</span><span class="sxs-lookup"><span data-stu-id="ab20d-103">How to: Invoice Jobs</span></span>
<span data-ttu-id="ab20d-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span><span class="sxs-lookup"><span data-stu-id="ab20d-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="ab20d-105">As the job progresses, these transactions get posted to the job journal.</span><span class="sxs-lookup"><span data-stu-id="ab20d-105">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="ab20d-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span><span class="sxs-lookup"><span data-stu-id="ab20d-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

<span data-ttu-id="ab20d-107">You can invoice the whole job from the **Job Task Lines** window or only invoice selected billable lines from the **Planning Lines** window.</span><span class="sxs-lookup"><span data-stu-id="ab20d-107">You can invoice the whole job from the **Job Task Lines** window or only invoice selected billable lines from the **Planning Lines** window.</span></span> <span data-ttu-id="ab20d-108">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span><span class="sxs-lookup"><span data-stu-id="ab20d-108">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ab20d-109">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span><span class="sxs-lookup"><span data-stu-id="ab20d-109">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="ab20d-110">For more information, see [How to: Manage Project Supplies](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="ab20d-110">For more information, see [How to: Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-and-post-a-job-sales-invoice"></a><span data-ttu-id="ab20d-111">To create and post a job sales invoice</span><span class="sxs-lookup"><span data-stu-id="ab20d-111">To create and post a job sales invoice</span></span>
<span data-ttu-id="ab20d-112">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span><span class="sxs-lookup"><span data-stu-id="ab20d-112">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="ab20d-113">From the **Jobs** window, you can invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-113">From the **Jobs** window, you can invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> <span data-ttu-id="ab20d-114">The following procedure shows how to use a batch job to invoice multiple jobs.</span><span class="sxs-lookup"><span data-stu-id="ab20d-114">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="ab20d-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab20d-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ab20d-116">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ab20d-116">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="ab20d-117">Set filters if you want to limit the jobs that the batch job will process.</span><span class="sxs-lookup"><span data-stu-id="ab20d-117">Set filters if you want to limit the jobs that the batch job will process.</span></span>
4. <span data-ttu-id="ab20d-118">Choose the **OK** button to create the invoices.</span><span class="sxs-lookup"><span data-stu-id="ab20d-118">Choose the **OK** button to create the invoices.</span></span>  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a><span data-ttu-id="ab20d-119">To create multiple job sales invoices from job planning lines</span><span class="sxs-lookup"><span data-stu-id="ab20d-119">To create multiple job sales invoices from job planning lines</span></span>
<span data-ttu-id="ab20d-120">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span><span class="sxs-lookup"><span data-stu-id="ab20d-120">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="ab20d-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab20d-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="ab20d-122">Open a relevant job.</span><span class="sxs-lookup"><span data-stu-id="ab20d-122">Open a relevant job.</span></span>
3. <span data-ttu-id="ab20d-123">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-123">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="ab20d-124">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span><span class="sxs-lookup"><span data-stu-id="ab20d-124">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="ab20d-125">Choose the **Create Sales Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-125">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="ab20d-126">In the **Job Create Sales Invoice** window, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span><span class="sxs-lookup"><span data-stu-id="ab20d-126">In the **Job Create Sales Invoice** window, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="ab20d-127">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="ab20d-127">Choose the **OK** button.</span></span>  

    <span data-ttu-id="ab20d-128">On the job planning line, in the **Qty. Transferred to Invoice** field, you can see the quantity.</span><span class="sxs-lookup"><span data-stu-id="ab20d-128">On the job planning line, in the **Qty. Transferred to Invoice** field, you can see the quantity.</span></span>
8. <span data-ttu-id="ab20d-129">In the **Job Planning Lines** window, choose the **Sales Invoices/Credit Memos** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-129">In the **Job Planning Lines** window, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="ab20d-130">The **Sales Invoice** window opens, showing the quantity that you have transferred to the invoice.</span><span class="sxs-lookup"><span data-stu-id="ab20d-130">The **Sales Invoice** window opens, showing the quantity that you have transferred to the invoice.</span></span>  
9. <span data-ttu-id="ab20d-131">Make any additional changes, and then choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-131">Make any additional changes, and then choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ab20d-132">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span><span class="sxs-lookup"><span data-stu-id="ab20d-132">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="ab20d-133">To calculate and post job completion entries</span><span class="sxs-lookup"><span data-stu-id="ab20d-133">To calculate and post job completion entries</span></span>
<span data-ttu-id="ab20d-134">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span><span class="sxs-lookup"><span data-stu-id="ab20d-134">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="ab20d-135">Then, you must reverse any WIP that has been posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="ab20d-135">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="ab20d-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab20d-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ab20d-137">Select an open job, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-137">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="ab20d-138">In the **Status** field, select **Completed**.</span><span class="sxs-lookup"><span data-stu-id="ab20d-138">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="ab20d-139">Follow the assistance steps to calculate and post WIP.</span><span class="sxs-lookup"><span data-stu-id="ab20d-139">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="ab20d-140">Alternatively, follows steps 5 and 6 to do so manually.</span><span class="sxs-lookup"><span data-stu-id="ab20d-140">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="ab20d-141">Choose the **Calculate WIP** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-141">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="ab20d-142">In the **Job Calculate WIP** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ab20d-142">In the **Job Calculate WIP** window, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="ab20d-143">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span><span class="sxs-lookup"><span data-stu-id="ab20d-143">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  
7. <span data-ttu-id="ab20d-144">Choose the **Job Post WIP to G/L** action.</span><span class="sxs-lookup"><span data-stu-id="ab20d-144">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="ab20d-145">In the **Job Post WIP to G/L** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ab20d-145">In the **Job Post WIP to G/L** window, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="ab20d-146">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span><span class="sxs-lookup"><span data-stu-id="ab20d-146">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="ab20d-147">See Also</span><span class="sxs-lookup"><span data-stu-id="ab20d-147">See Also</span></span>
[<span data-ttu-id="ab20d-148">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="ab20d-148">Managing Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="ab20d-149">Finance</span><span class="sxs-lookup"><span data-stu-id="ab20d-149">Finance</span></span>](finance.md)  
<span data-ttu-id="ab20d-150">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="ab20d-150">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="ab20d-151">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="ab20d-151">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="ab20d-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ab20d-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

