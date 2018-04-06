---
title: Overview of Tasks to Allocate Costs and Income | Microsoft Docs
description: Outlines the tasks to allocate an entry in a general journal to several different accounts when you post the journal.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 3f2a1f762f9380f3cd272e78c4c2f269e9960f38
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="allocate-costs-and-income"></a><span data-ttu-id="5b621-103">Allocate Costs and Income</span><span class="sxs-lookup"><span data-stu-id="5b621-103">Allocate Costs and Income</span></span>
<span data-ttu-id="5b621-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span><span class="sxs-lookup"><span data-stu-id="5b621-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="5b621-105">The allocation can be made by three different methods:</span><span class="sxs-lookup"><span data-stu-id="5b621-105">The allocation can be made by three different methods:</span></span>

* <span data-ttu-id="5b621-106">Quantity</span><span class="sxs-lookup"><span data-stu-id="5b621-106">Quantity</span></span>
* <span data-ttu-id="5b621-107">Percentage (%)</span><span class="sxs-lookup"><span data-stu-id="5b621-107">Percentage (%)</span></span>
* <span data-ttu-id="5b621-108">Amount</span><span class="sxs-lookup"><span data-stu-id="5b621-108">Amount</span></span>

<span data-ttu-id="5b621-109">The allocation features can be used with recurring general journals and in fixed assets journals.</span><span class="sxs-lookup"><span data-stu-id="5b621-109">The allocation features can be used with recurring general journals and in fixed assets journals.</span></span>
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

<span data-ttu-id="5b621-110">The following procedures describe how to prepare to allocate costs in a recurring general journal by defining allocation keys.</span><span class="sxs-lookup"><span data-stu-id="5b621-110">The following procedures describe how to prepare to allocate costs in a recurring general journal by defining allocation keys.</span></span> <span data-ttu-id="5b621-111">When allocation keys are defined, you complete and post the journal like any other recurring general journal.</span><span class="sxs-lookup"><span data-stu-id="5b621-111">When allocation keys are defined, you complete and post the journal like any other recurring general journal.</span></span> <span data-ttu-id="5b621-112">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="5b621-112">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="5b621-113">To set up allocation keys</span><span class="sxs-lookup"><span data-stu-id="5b621-113">To set up allocation keys</span></span>
<span data-ttu-id="5b621-114">You can allocate an entry in a recurring general journal to several different accounts when you post the journal.</span><span class="sxs-lookup"><span data-stu-id="5b621-114">You can allocate an entry in a recurring general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="5b621-115">The allocation can be made by quantity, percentage, or amount.</span><span class="sxs-lookup"><span data-stu-id="5b621-115">The allocation can be made by quantity, percentage, or amount.</span></span>
1. <span data-ttu-id="5b621-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5b621-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="5b621-117">Choose the **Batch Name** field to open the **General Journal Batches** window.</span><span class="sxs-lookup"><span data-stu-id="5b621-117">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="5b621-118">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span><span class="sxs-lookup"><span data-stu-id="5b621-118">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
   * <span data-ttu-id="5b621-119">To create a new batch, choose the **New** action, and go to the next step.</span><span class="sxs-lookup"><span data-stu-id="5b621-119">To create a new batch, choose the **New** action, and go to the next step.</span></span>
   * <span data-ttu-id="5b621-120">To change the allocations of an existing journal, select the journal and go to step 7.</span><span class="sxs-lookup"><span data-stu-id="5b621-120">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="5b621-121">In the **Name** field, enter a name for the batch, such as CLEANING.</span><span class="sxs-lookup"><span data-stu-id="5b621-121">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="5b621-122">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span><span class="sxs-lookup"><span data-stu-id="5b621-122">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="5b621-123">When you are done, close the window.</span><span class="sxs-lookup"><span data-stu-id="5b621-123">When you are done, close the window.</span></span> <span data-ttu-id="5b621-124">A new, empty recurring journal opens.</span><span class="sxs-lookup"><span data-stu-id="5b621-124">A new, empty recurring journal opens.</span></span>
6. <span data-ttu-id="5b621-125">Fill in the fields on the line.</span><span class="sxs-lookup"><span data-stu-id="5b621-125">Fill in the fields on the line.</span></span>
7. <span data-ttu-id="5b621-126">Choose the **Allocations** action.</span><span class="sxs-lookup"><span data-stu-id="5b621-126">Choose the **Allocations** action.</span></span>
8. <span data-ttu-id="5b621-127">Add a line for each allocation.</span><span class="sxs-lookup"><span data-stu-id="5b621-127">Add a line for each allocation.</span></span> <span data-ttu-id="5b621-128">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="5b621-128">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="5b621-129">You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span><span class="sxs-lookup"><span data-stu-id="5b621-129">You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="5b621-130">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span><span class="sxs-lookup"><span data-stu-id="5b621-130">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="5b621-131">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span><span class="sxs-lookup"><span data-stu-id="5b621-131">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="5b621-132">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span><span class="sxs-lookup"><span data-stu-id="5b621-132">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="5b621-133">The **Allocated Amt. (GBP)** field is filled in and matches the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="5b621-133">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="5b621-134">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="5b621-134">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="5b621-135">To change an allocation key that has already been set up</span><span class="sxs-lookup"><span data-stu-id="5b621-135">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="5b621-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5b621-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="5b621-137">In the **Recurring General Journal** window, select the journal with the allocation.</span><span class="sxs-lookup"><span data-stu-id="5b621-137">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="5b621-138">Choose the line with the allocation, and then choose **Allocations** action.</span><span class="sxs-lookup"><span data-stu-id="5b621-138">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="5b621-139">Change the relevant fields, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="5b621-139">Change the relevant fields, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="5b621-140">See Also</span><span class="sxs-lookup"><span data-stu-id="5b621-140">See Also</span></span>
[<span data-ttu-id="5b621-141">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="5b621-141">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="5b621-142">[Working with General Journals](ui-work-general-journals.md)  </span><span class="sxs-lookup"><span data-stu-id="5b621-142">[Working with General Journals](ui-work-general-journals.md)  </span></span>  
<span data-ttu-id="5b621-143">[Posting Documents and Journals](ui-post-documents-journals.md)  </span><span class="sxs-lookup"><span data-stu-id="5b621-143">[Posting Documents and Journals](ui-post-documents-journals.md)  </span></span>  
<span data-ttu-id="5b621-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5b621-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

