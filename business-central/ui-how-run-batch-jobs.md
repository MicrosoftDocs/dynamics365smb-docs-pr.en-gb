---
title: Create and Run a Batch Job | Microsoft Docs
description: You run batch jobs to process data and update information, for example, to do periodic accounting activities, or to do calculations.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 10/01/2020
ms.author: solsen
ms.openlocfilehash: 7c9d67168308491daef838e91c5a1b84645b222a
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920429"
---
# <a name="run-batch-jobs-and-xmlports"></a><span data-ttu-id="b9dc3-103">Run Batch Jobs and XMLports</span><span class="sxs-lookup"><span data-stu-id="b9dc3-103">Run Batch Jobs and XMLports</span></span>
<span data-ttu-id="b9dc3-104">A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-104">A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job.</span></span> <span data-ttu-id="b9dc3-105">There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-105">There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year.</span></span> <span data-ttu-id="b9dc3-106">Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-106">Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.</span></span>

<span data-ttu-id="b9dc3-107">A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-107">A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.</span></span>

<span data-ttu-id="b9dc3-108">You can schedule when a batch job runs.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-108">You can schedule when a batch job runs.</span></span> <span data-ttu-id="b9dc3-109">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="b9dc3-109">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

## <a name="to-run-a-batch-job"></a><span data-ttu-id="b9dc3-110">To run a batch job</span><span class="sxs-lookup"><span data-stu-id="b9dc3-110">To run a batch job</span></span>
1. <span data-ttu-id="b9dc3-111">To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-111">To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.</span></span>
2. <span data-ttu-id="b9dc3-112">If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-112">If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.</span></span>
3. <span data-ttu-id="b9dc3-113">The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-113">The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job.</span></span> <span data-ttu-id="b9dc3-114">You can enter criteria in the suggested filters or add more filters.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-114">You can enter criteria in the suggested filters or add more filters.</span></span>
4. <span data-ttu-id="b9dc3-115">Choose the **OK** button to start the batch job.</span><span class="sxs-lookup"><span data-stu-id="b9dc3-115">Choose the **OK** button to start the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="b9dc3-116">See Also</span><span class="sxs-lookup"><span data-stu-id="b9dc3-116">See Also</span></span>
[<span data-ttu-id="b9dc3-117">Sorting, Searching, and Filtering Lists</span><span class="sxs-lookup"><span data-stu-id="b9dc3-117">Sorting, Searching, and Filtering Lists</span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="b9dc3-118">Use Job Queues to Schedule Tasks</span><span class="sxs-lookup"><span data-stu-id="b9dc3-118">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)  
<span data-ttu-id="b9dc3-119">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b9dc3-119">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
