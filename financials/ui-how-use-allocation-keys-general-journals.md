---
title: 'How to: Use Allocation Keys in General Journals | Microsoft Docs'
description: Learn how you can use allocation keys in journals.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost accounting
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: bbacf9b5634d51478dd4d54ac4b587ea9bfaaf99
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="d9099-103">How to: Use Allocation Keys in General Journals</span><span class="sxs-lookup"><span data-stu-id="d9099-103">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="d9099-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span><span class="sxs-lookup"><span data-stu-id="d9099-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="d9099-105">The allocation can be made by quantity, percentage, or amount.</span><span class="sxs-lookup"><span data-stu-id="d9099-105">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="d9099-106">To set up allocation keys</span><span class="sxs-lookup"><span data-stu-id="d9099-106">To set up allocation keys</span></span>
1. <span data-ttu-id="d9099-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d9099-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="d9099-108">Choose the **Batch Name** field to open the **General Journal Batches** window.</span><span class="sxs-lookup"><span data-stu-id="d9099-108">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="d9099-109">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span><span class="sxs-lookup"><span data-stu-id="d9099-109">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
   * <span data-ttu-id="d9099-110">To create a new batch, choose the **New** action, and go to the next step.</span><span class="sxs-lookup"><span data-stu-id="d9099-110">To create a new batch, choose the **New** action, and go to the next step.</span></span>
   * <span data-ttu-id="d9099-111">To change the allocations of an existing journal, select the journal and go to step 7.</span><span class="sxs-lookup"><span data-stu-id="d9099-111">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="d9099-112">In the **Name** field, enter a name for the batch, such as CLEANING.</span><span class="sxs-lookup"><span data-stu-id="d9099-112">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="d9099-113">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span><span class="sxs-lookup"><span data-stu-id="d9099-113">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="d9099-114">When you are done, close the window.</span><span class="sxs-lookup"><span data-stu-id="d9099-114">When you are done, close the window.</span></span> <span data-ttu-id="d9099-115">A new, empty recurring journal opens.</span><span class="sxs-lookup"><span data-stu-id="d9099-115">A new, empty recurring journal opens.</span></span>
6. <span data-ttu-id="d9099-116">Fill in the fields on the line.</span><span class="sxs-lookup"><span data-stu-id="d9099-116">Fill in the fields on the line.</span></span>
7. <span data-ttu-id="d9099-117">Choose the **Allocations** action.</span><span class="sxs-lookup"><span data-stu-id="d9099-117">Choose the **Allocations** action.</span></span>
8. <span data-ttu-id="d9099-118">Add a line for each allocation.</span><span class="sxs-lookup"><span data-stu-id="d9099-118">Add a line for each allocation.</span></span> <span data-ttu-id="d9099-119">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="d9099-119">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="d9099-120">You must also fill in the **Account No.**</span><span class="sxs-lookup"><span data-stu-id="d9099-120">You must also fill in the **Account No.**</span></span> <span data-ttu-id="d9099-121">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span><span class="sxs-lookup"><span data-stu-id="d9099-121">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="d9099-122">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span><span class="sxs-lookup"><span data-stu-id="d9099-122">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="d9099-123">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span><span class="sxs-lookup"><span data-stu-id="d9099-123">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="d9099-124">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span><span class="sxs-lookup"><span data-stu-id="d9099-124">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="d9099-125">The **Allocated Amt. (GBP)** field is filled in and matches the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="d9099-125">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="d9099-126">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="d9099-126">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="d9099-127">To change an allocation key that has already been set up</span><span class="sxs-lookup"><span data-stu-id="d9099-127">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="d9099-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d9099-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="d9099-129">In the **Recurring General Journal** window, select the journal with the allocation.</span><span class="sxs-lookup"><span data-stu-id="d9099-129">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="d9099-130">Choose the line with the allocation, and then choose **Allocations** action.</span><span class="sxs-lookup"><span data-stu-id="d9099-130">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="d9099-131">Change the relevant fields, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="d9099-131">Change the relevant fields, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="d9099-132">See Also</span><span class="sxs-lookup"><span data-stu-id="d9099-132">See Also</span></span>
[<span data-ttu-id="d9099-133">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="d9099-133">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="d9099-134">Posting Documents and Journals</span><span class="sxs-lookup"><span data-stu-id="d9099-134">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="d9099-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d9099-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

