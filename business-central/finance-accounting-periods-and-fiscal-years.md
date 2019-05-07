---
title: Working with Accounting Periods and Fiscal Years | Microsoft Docs
description: Learn how to work with accounting periods to define when your company reports financial performance.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 50df903e664f98f038a82c646dd3bd9c2f5ef479
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "936631"
---
# <a name="working-with-accounting-periods-and-fiscal-years"></a><span data-ttu-id="0aa62-103">Working with Accounting Periods and Fiscal Years</span><span class="sxs-lookup"><span data-stu-id="0aa62-103">Working with Accounting Periods and Fiscal Years</span></span>
<span data-ttu-id="0aa62-104">Accounting periods, which are also known as reporting periods, are periods of time for which a company or organisation reports financial performance, for example, by generating their income statement or balance sheet.</span><span class="sxs-lookup"><span data-stu-id="0aa62-104">Accounting periods, which are also known as reporting periods, are periods of time for which a company or organization reports financial performance, for example, by generating their income statement or balance sheet.</span></span> <span data-ttu-id="0aa62-105">Typically, accounting periods refer to the company's fiscal year, which can contain several accounting periods, such as months or quarters.</span><span class="sxs-lookup"><span data-stu-id="0aa62-105">Typically, accounting periods refer to the company's fiscal year, which can contain several accounting periods, such as months or quarters.</span></span>

<span data-ttu-id="0aa62-106">For many companies the fiscal year does not align with the calendar year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-106">For many companies the fiscal year does not align with the calendar year.</span></span> <span data-ttu-id="0aa62-107">For example, the fiscal year might end on June 30th rather than December 31st.</span><span class="sxs-lookup"><span data-stu-id="0aa62-107">For example, the fiscal year might end on June 30th rather than December 31st.</span></span> <span data-ttu-id="0aa62-108">For newly created companies, the fiscal might actually be longer than 12 months.</span><span class="sxs-lookup"><span data-stu-id="0aa62-108">For newly created companies, the fiscal might actually be longer than 12 months.</span></span> 

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="0aa62-109">only requires accounting periods only if you want to close an income statement, or run data compression tasks.</span><span class="sxs-lookup"><span data-stu-id="0aa62-109">only requires accounting periods only if you want to close an income statement, or run data compression tasks.</span></span> 

<span data-ttu-id="0aa62-110">You can use accounting periods in reporting.</span><span class="sxs-lookup"><span data-stu-id="0aa62-110">You can use accounting periods in reporting.</span></span> <span data-ttu-id="0aa62-111">For example, when you are reviewing posted entries on the **Balance/Budget** page where the reporting interval can be specified.</span><span class="sxs-lookup"><span data-stu-id="0aa62-111">For example, when you are reviewing posted entries on the **Balance/Budget** page where the reporting interval can be specified.</span></span> <span data-ttu-id="0aa62-112">One of the options you may specify to report by accounting period.</span><span class="sxs-lookup"><span data-stu-id="0aa62-112">One of the options you may specify to report by accounting period.</span></span> <span data-ttu-id="0aa62-113">You can also build an account schedule that compares results for different accounting periods.</span><span class="sxs-lookup"><span data-stu-id="0aa62-113">You can also build an account schedule that compares results for different accounting periods.</span></span>

## <a name="creating-a-new-fiscal-year"></a><span data-ttu-id="0aa62-114">Creating a new fiscal year</span><span class="sxs-lookup"><span data-stu-id="0aa62-114">Creating a new fiscal year</span></span>
<span data-ttu-id="0aa62-115">You can create accounting periods in bulk, by using eh **Create Fiscal Year** batch job, or manually.</span><span class="sxs-lookup"><span data-stu-id="0aa62-115">You can create accounting periods in bulk, by using eh **Create Fiscal Year** batch job, or manually.</span></span>

### <a name="how-to-create-accounting-periods-in-bulk"></a><span data-ttu-id="0aa62-116">How to create accounting periods in-bulk</span><span class="sxs-lookup"><span data-stu-id="0aa62-116">How to create accounting periods in-bulk</span></span>
<span data-ttu-id="0aa62-117">Use the **Create Fiscal Year** batch job to divide a fiscal year into periods of equal length.</span><span class="sxs-lookup"><span data-stu-id="0aa62-117">Use the **Create Fiscal Year** batch job to divide a fiscal year into periods of equal length.</span></span>  

1. <span data-ttu-id="0aa62-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0aa62-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0aa62-119">Choose the **Create Year** action.</span><span class="sxs-lookup"><span data-stu-id="0aa62-119">Choose the **Create Year** action.</span></span>  <!--What about the Scheduling option? Should we mention that? There's also the Report Output Type field...-->
3. <span data-ttu-id="0aa62-120">In the **Starting Date** field, enter the date on which the fiscal year starts.</span><span class="sxs-lookup"><span data-stu-id="0aa62-120">In the **Starting Date** field, enter the date on which the fiscal year starts.</span></span>  
4. <span data-ttu-id="0aa62-121">In the **No. of Periods** field, enter the number of accounting periods to divide the fiscal year into.</span><span class="sxs-lookup"><span data-stu-id="0aa62-121">In the **No. of Periods** field, enter the number of accounting periods to divide the fiscal year into.</span></span> <span data-ttu-id="0aa62-122">There can be up to 365 periods in a year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-122">There can be up to 365 periods in a year.</span></span>  
5. <span data-ttu-id="0aa62-123">In the **Period Length** field, enter a duration for each period.</span><span class="sxs-lookup"><span data-stu-id="0aa62-123">In the **Period Length** field, enter a duration for each period.</span></span> <span data-ttu-id="0aa62-124">For example, 1M for one month, 1Q for one quarter, and 1Y for one year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-124">For example, 1M for one month, 1Q for one quarter, and 1Y for one year.</span></span>  
6. <span data-ttu-id="0aa62-125">Choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="0aa62-125">Choose **OK**.</span></span>  

### <a name="how-to-create-accounting-periods-manually"></a><span data-ttu-id="0aa62-126">How to create accounting periods manually</span><span class="sxs-lookup"><span data-stu-id="0aa62-126">How to create accounting periods manually</span></span>
<span data-ttu-id="0aa62-127">If the accounting periods in your fiscal year have different durations, like the 4-4-5 calendar used in retail, you can manually set it up.</span><span class="sxs-lookup"><span data-stu-id="0aa62-127">If the accounting periods in your fiscal year have different durations, like the 4-4-5 calendar used in retail, you can manually set it up.</span></span>  
  
1. <span data-ttu-id="0aa62-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0aa62-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0aa62-129">In the **Starting Date** field, enter the date on which the fiscal year starts.</span><span class="sxs-lookup"><span data-stu-id="0aa62-129">In the **Starting Date** field, enter the date on which the fiscal year starts.</span></span> <span data-ttu-id="0aa62-130">The **Name** field will show the name of the month.</span><span class="sxs-lookup"><span data-stu-id="0aa62-130">The **Name** field will show the name of the month.</span></span>  
3. <span data-ttu-id="0aa62-131">Choose the **New Fiscal Year** check box to indicate that this is the first period in the year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-131">Choose the **New Fiscal Year** check box to indicate that this is the first period in the year.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="0aa62-132">will use this period to determine which periods to close at year-end.</span><span class="sxs-lookup"><span data-stu-id="0aa62-132">will use this period to determine which periods to close at year-end.</span></span>
4. <span data-ttu-id="0aa62-133">Repeat steps 2 and 3 for each remaining period.</span><span class="sxs-lookup"><span data-stu-id="0aa62-133">Repeat steps 2 and 3 for each remaining period.</span></span>  

## <a name="closing-a-fiscal-year"></a><span data-ttu-id="0aa62-134">Closing a Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="0aa62-134">Closing a Fiscal Year</span></span>
<span data-ttu-id="0aa62-135">Closing the fiscal year is one of the tasks for closing the books.</span><span class="sxs-lookup"><span data-stu-id="0aa62-135">Closing the fiscal year is one of the tasks for closing the books.</span></span> <span data-ttu-id="0aa62-136">After you close a fiscal year, the **Closed** and **Date Locked** check boxes are selected for all periods in the year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-136">After you close a fiscal year, the **Closed** and **Date Locked** check boxes are selected for all periods in the year.</span></span> <span data-ttu-id="0aa62-137">You cannot reopen a year or clear the check boxes.</span><span class="sxs-lookup"><span data-stu-id="0aa62-137">You cannot reopen a year or clear the check boxes.</span></span>

> [!NOTE]  
>  <span data-ttu-id="0aa62-138">You must always have at least one open fiscal year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-138">You must always have at least one open fiscal year.</span></span> <span data-ttu-id="0aa62-139">When closing a year, ensure that a new year has been created.</span><span class="sxs-lookup"><span data-stu-id="0aa62-139">When closing a year, ensure that a new year has been created.</span></span> <span data-ttu-id="0aa62-140">Also, note that after you close one year, you cannot change the starting date of the following year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-140">Also, note that after you close one year, you cannot change the starting date of the following year.</span></span>

1. <span data-ttu-id="0aa62-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0aa62-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0aa62-142">Choose the **Close Year** action.</span><span class="sxs-lookup"><span data-stu-id="0aa62-142">Choose the **Close Year** action.</span></span>  

## <a name="posting-entries-to-a-closed-fiscal-year"></a><span data-ttu-id="0aa62-143">Posting Entries to a Closed Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="0aa62-143">Posting Entries to a Closed Fiscal Year</span></span>
<span data-ttu-id="0aa62-144">Although a fiscal year is closed, you can still post general ledger entries to it.</span><span class="sxs-lookup"><span data-stu-id="0aa62-144">Although a fiscal year is closed, you can still post general ledger entries to it.</span></span> <span data-ttu-id="0aa62-145">When you do, the entries are marked as posted to a closed fiscal year and the **Prior Year Entry** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="0aa62-145">When you do, the entries are marked as posted to a closed fiscal year and the **Prior Year Entry** check box is selected.</span></span> <span data-ttu-id="0aa62-146">By default, the check box is not displayed on the page, but you can add it.</span><span class="sxs-lookup"><span data-stu-id="0aa62-146">By default, the check box is not displayed on the page, but you can add it.</span></span> <span data-ttu-id="0aa62-147">The next steps are to close the income statement accounts and transfer the year's results to an account in the balance sheet.</span><span class="sxs-lookup"><span data-stu-id="0aa62-147">The next steps are to close the income statement accounts and transfer the year's results to an account in the balance sheet.</span></span> <span data-ttu-id="0aa62-148">Repeat these steps each time you post entries to a closed fiscal year.</span><span class="sxs-lookup"><span data-stu-id="0aa62-148">Repeat these steps each time you post entries to a closed fiscal year.</span></span>

## <a name="see-also"></a><span data-ttu-id="0aa62-149">See Also</span><span class="sxs-lookup"><span data-stu-id="0aa62-149">See Also</span></span>
[<span data-ttu-id="0aa62-150">Closing the Books</span><span class="sxs-lookup"><span data-stu-id="0aa62-150">Closing the Books</span></span>](year-close-books.md)  
[<span data-ttu-id="0aa62-151">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="0aa62-151">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="0aa62-152">How to Work with Account Schedules</span><span class="sxs-lookup"><span data-stu-id="0aa62-152">How to Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)  
  





