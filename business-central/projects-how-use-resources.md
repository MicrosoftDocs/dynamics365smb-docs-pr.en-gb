---
title: Record and Adjust Resource Usage and Prices| Microsoft Docs
description: Describes how you can record the resource usage or consumption associated with a job, to keep track and manage costs, prices, and work types.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: fc51b47b71d37daaccc4133d648c90b84d5a3494
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "911772"
---
# <a name="use-resources-for-jobs"></a><span data-ttu-id="c5eae-103">Use Resources for Jobs</span><span class="sxs-lookup"><span data-stu-id="c5eae-103">Use Resources for Jobs</span></span>
<span data-ttu-id="c5eae-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span><span class="sxs-lookup"><span data-stu-id="c5eae-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="c5eae-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="c5eae-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="c5eae-106">You can also post the usage of a resource in a resource journal.</span><span class="sxs-lookup"><span data-stu-id="c5eae-106">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="c5eae-107">Entries posted in a resource journal have no effect on the general ledger.</span><span class="sxs-lookup"><span data-stu-id="c5eae-107">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="c5eae-108">To assign resources to jobs</span><span class="sxs-lookup"><span data-stu-id="c5eae-108">To assign resources to jobs</span></span>
<span data-ttu-id="c5eae-109">You assign resources to jobs by creating job planning lines for the job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-109">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="c5eae-110">For more information, see [Create Jobs](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="c5eae-110">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="c5eae-111">To record resource usage for a job</span><span class="sxs-lookup"><span data-stu-id="c5eae-111">To record resource usage for a job</span></span>
1. <span data-ttu-id="c5eae-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c5eae-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="c5eae-113">Open a relevant job journal batch, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="c5eae-113">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="c5eae-114">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="c5eae-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="c5eae-115">To adjust resource prices</span><span class="sxs-lookup"><span data-stu-id="c5eae-115">To adjust resource prices</span></span>
<span data-ttu-id="c5eae-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="c5eae-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c5eae-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="c5eae-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="c5eae-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="c5eae-119">This batch job does not create or adjust alternate costs or prices for resources.</span><span class="sxs-lookup"><span data-stu-id="c5eae-119">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="c5eae-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="c5eae-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="c5eae-122">To get resource price change suggestions based on existing alternate prices</span><span class="sxs-lookup"><span data-stu-id="c5eae-122">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="c5eae-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="c5eae-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="c5eae-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c5eae-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="c5eae-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="c5eae-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="c5eae-126">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="c5eae-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="c5eae-127">When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-127">When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="c5eae-128">To get resource price change suggestions based on standard prices</span><span class="sxs-lookup"><span data-stu-id="c5eae-128">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="c5eae-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="c5eae-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c5eae-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="c5eae-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="c5eae-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="c5eae-132">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="c5eae-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="c5eae-133">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-133">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="c5eae-134">To get resource price change suggestions based on alternate prices</span><span class="sxs-lookup"><span data-stu-id="c5eae-134">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="c5eae-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="c5eae-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="c5eae-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c5eae-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c5eae-137">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="c5eae-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="c5eae-138">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="c5eae-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="c5eae-139">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="c5eae-139">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="c5eae-140">See Also</span><span class="sxs-lookup"><span data-stu-id="c5eae-140">See Also</span></span>
[<span data-ttu-id="c5eae-141">Project Management</span><span class="sxs-lookup"><span data-stu-id="c5eae-141">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="c5eae-142">Finance</span><span class="sxs-lookup"><span data-stu-id="c5eae-142">Finance</span></span>](finance.md)  
<span data-ttu-id="c5eae-143">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="c5eae-143">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="c5eae-144">[Sales](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="c5eae-144">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="c5eae-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c5eae-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
