---
title: Create and Run a Batch Job | Microsoft Docs
description: You run batch jobs to process data and update information, for example, to do periodic accounting activities, or to do calculations.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process
ms.date: 04/01/2021
ms.author: solsen
ms.openlocfilehash: 05b65f5b001259fff25d0f59dfc6267d9ee00c7f
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5782260"
---
# <a name="run-batch-jobs-and-xmlports"></a><span data-ttu-id="4761b-103">Run Batch Jobs and XMLports</span><span class="sxs-lookup"><span data-stu-id="4761b-103">Run Batch Jobs and XMLports</span></span>
<span data-ttu-id="4761b-104">A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job.</span><span class="sxs-lookup"><span data-stu-id="4761b-104">A batch job is a routine that processes data in batches, for example the **Adjust Exchange Rates** batch job.</span></span> <span data-ttu-id="4761b-105">There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year.</span><span class="sxs-lookup"><span data-stu-id="4761b-105">There are batch jobs that perform periodic accounting activities, such as closing the income statement at the end of a fiscal year.</span></span> <span data-ttu-id="4761b-106">Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.</span><span class="sxs-lookup"><span data-stu-id="4761b-106">Many batch jobs do calculation work, such as calculation of finance charges, exchange rate adjustment, and calculation of unit prices.</span></span>

<span data-ttu-id="4761b-107">A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.</span><span class="sxs-lookup"><span data-stu-id="4761b-107">A batch job is like a report, except the batch job uses the result of its work to update information directly, instead of printing the results.</span></span>

<span data-ttu-id="4761b-108">You can schedule when a batch job runs.</span><span class="sxs-lookup"><span data-stu-id="4761b-108">You can schedule when a batch job runs.</span></span> <span data-ttu-id="4761b-109">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="4761b-109">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

## <a name="to-run-a-batch-job"></a><span data-ttu-id="4761b-110">To run a batch job</span><span class="sxs-lookup"><span data-stu-id="4761b-110">To run a batch job</span></span>
1. <span data-ttu-id="4761b-111">To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4761b-111">To open the request page for the relevant batch job, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the batch job, and then choose the related link.</span></span>
2. <span data-ttu-id="4761b-112">If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.</span><span class="sxs-lookup"><span data-stu-id="4761b-112">If there is an **Options** FastTab for the batch job, fill in the fields to determine what the batch job will do.</span></span>
3. <span data-ttu-id="4761b-113">The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job.</span><span class="sxs-lookup"><span data-stu-id="4761b-113">The page may contain one or more FastTab with filters, which you can use to limit the data included in the batch job.</span></span> <span data-ttu-id="4761b-114">You can enter criteria in the suggested filters or add more filters.</span><span class="sxs-lookup"><span data-stu-id="4761b-114">You can enter criteria in the suggested filters or add more filters.</span></span>
4. <span data-ttu-id="4761b-115">Choose the **OK** button to start the batch job.</span><span class="sxs-lookup"><span data-stu-id="4761b-115">Choose the **OK** button to start the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="4761b-116">See Also</span><span class="sxs-lookup"><span data-stu-id="4761b-116">See Also</span></span>
[<span data-ttu-id="4761b-117">Sorting, Searching, and Filtering Lists</span><span class="sxs-lookup"><span data-stu-id="4761b-117">Sorting, Searching, and Filtering Lists</span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="4761b-118">Use Job Queues to Schedule Tasks</span><span class="sxs-lookup"><span data-stu-id="4761b-118">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)  
<span data-ttu-id="4761b-119">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4761b-119">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]