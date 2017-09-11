---
title: Record and Adjust Resource Usage and Prices| Microsoft Docs
description: Describes how you can record the resource usage or consumption associated with a job, to keep track and manage costs, prices, and work types.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 48692c9837007c6dd9c3891f0940b6f15b1d6541
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="60cc3-103">How to: Use Resources for Jobs</span><span class="sxs-lookup"><span data-stu-id="60cc3-103">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="60cc3-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span><span class="sxs-lookup"><span data-stu-id="60cc3-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="60cc3-105">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="60cc3-105">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="60cc3-106">You can also post the usage of a resource in a resource journal.</span><span class="sxs-lookup"><span data-stu-id="60cc3-106">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="60cc3-107">Entries posted in a resource journal have no effect on the general ledger.</span><span class="sxs-lookup"><span data-stu-id="60cc3-107">Entries posted in a resource journal have no effect on the general ledger.</span></span>

> [!NOTE]  
>   <span data-ttu-id="60cc3-108">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="60cc3-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="60cc3-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="60cc3-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="60cc3-110">To assign resources to jobs</span><span class="sxs-lookup"><span data-stu-id="60cc3-110">To assign resources to jobs</span></span>
<span data-ttu-id="60cc3-111">You assign resources to jobs by creating job planning lines for the job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-111">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="60cc3-112">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="60cc3-112">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="60cc3-113">To record resource usage for a job</span><span class="sxs-lookup"><span data-stu-id="60cc3-113">To record resource usage for a job</span></span>
1. <span data-ttu-id="60cc3-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="60cc3-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="60cc3-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="60cc3-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="60cc3-116">When the journal is complete, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="60cc3-116">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="60cc3-117">To adjust resource prices</span><span class="sxs-lookup"><span data-stu-id="60cc3-117">To adjust resource prices</span></span>
<span data-ttu-id="60cc3-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="60cc3-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="60cc3-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="60cc3-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="60cc3-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="60cc3-121">This batch job does not create or adjust alternate costs or prices for resources.</span><span class="sxs-lookup"><span data-stu-id="60cc3-121">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="60cc3-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="60cc3-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="60cc3-124">To get resource price change suggestions based on existing alternate prices</span><span class="sxs-lookup"><span data-stu-id="60cc3-124">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="60cc3-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="60cc3-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="60cc3-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="60cc3-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="60cc3-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="60cc3-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="60cc3-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="60cc3-128">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="60cc3-129">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-129">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="60cc3-130">To get resource price change suggestions based on standard prices</span><span class="sxs-lookup"><span data-stu-id="60cc3-130">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="60cc3-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="60cc3-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="60cc3-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="60cc3-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="60cc3-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="60cc3-134">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="60cc3-134">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="60cc3-135">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-135">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="60cc3-136">To get resource price change suggestions based on alternate prices</span><span class="sxs-lookup"><span data-stu-id="60cc3-136">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="60cc3-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span><span class="sxs-lookup"><span data-stu-id="60cc3-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="60cc3-138">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="60cc3-138">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="60cc3-139">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="60cc3-139">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="60cc3-140">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="60cc3-140">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="60cc3-141">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span><span class="sxs-lookup"><span data-stu-id="60cc3-141">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="60cc3-142">See Also</span><span class="sxs-lookup"><span data-stu-id="60cc3-142">See Also</span></span>
[<span data-ttu-id="60cc3-143">Project Management</span><span class="sxs-lookup"><span data-stu-id="60cc3-143">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="60cc3-144">Finance</span><span class="sxs-lookup"><span data-stu-id="60cc3-144">Finance</span></span>](finance.md)  
<span data-ttu-id="60cc3-145">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="60cc3-145">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="60cc3-146">[Sales](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="60cc3-146">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="60cc3-147">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="60cc3-147">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

