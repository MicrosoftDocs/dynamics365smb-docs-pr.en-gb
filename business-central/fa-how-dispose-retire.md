---
title: Dispose or Retire FA| Microsoft Docs
description: You must post a disposal value when you scrap, sell, or retire a fixed asset.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: scrap
ms.date: 06/04/2020
ms.author: edupont
ms.openlocfilehash: 29293e957617fea91c9a8e8b8c1f988b06104494
ms.sourcegitcommit: ccae3ff6aaeaa52db9d6456042acdede19fb9f7b
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/08/2020
ms.locfileid: "3435214"
---
# <a name="dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="d318d-103">Dispose of or Retire Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d318d-103">Dispose of or Retire Fixed Assets</span></span>

<span data-ttu-id="d318d-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span><span class="sxs-lookup"><span data-stu-id="d318d-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="d318d-105">A disposal entry must be the last entry posted for a fixed asset.</span><span class="sxs-lookup"><span data-stu-id="d318d-105">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="d318d-106">For partially disposed fixed assets, you can post more than one disposal entry.</span><span class="sxs-lookup"><span data-stu-id="d318d-106">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="d318d-107">The total of all posted disposal amounts must be a credit amount.</span><span class="sxs-lookup"><span data-stu-id="d318d-107">The total of all posted disposal amounts must be a credit amount.</span></span>  

> [!NOTE]  
> <span data-ttu-id="d318d-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span><span class="sxs-lookup"><span data-stu-id="d318d-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="d318d-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="d318d-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

<span data-ttu-id="d318d-110">The following steps assume that you have already set up the relevant posting groups in the **FA Posting Groups** page.</span><span class="sxs-lookup"><span data-stu-id="d318d-110">The following steps assume that you have already set up the relevant posting groups in the **FA Posting Groups** page.</span></span> <span data-ttu-id="d318d-111">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="d318d-111">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="d318d-112">To post a disposal from the fixed asset G/L journal</span><span class="sxs-lookup"><span data-stu-id="d318d-112">To post a disposal from the fixed asset G/L journal</span></span>

1. <span data-ttu-id="d318d-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d318d-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d318d-114">Create an initial journal line and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="d318d-114">Create an initial journal line and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="d318d-115">In the **FA Posting Type** field, select **Disposal**.</span><span class="sxs-lookup"><span data-stu-id="d318d-115">In the **FA Posting Type** field, select **Disposal**.</span></span>  
4. <span data-ttu-id="d318d-116">Choose the **Insert FA Bal. Account** action.</span><span class="sxs-lookup"><span data-stu-id="d318d-116">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="d318d-117">A second journal line is created for the balancing account that is set up for disposal posting.</span><span class="sxs-lookup"><span data-stu-id="d318d-117">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="d318d-118">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span><span class="sxs-lookup"><span data-stu-id="d318d-118">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="d318d-119">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="d318d-119">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
5. <span data-ttu-id="d318d-120">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="d318d-120">Choose the **Post** action.</span></span>  

<span data-ttu-id="d318d-121">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span><span class="sxs-lookup"><span data-stu-id="d318d-121">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="d318d-122">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="d318d-122">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>  

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="d318d-123">To view disposal ledger entries</span><span class="sxs-lookup"><span data-stu-id="d318d-123">To view disposal ledger entries</span></span>
<span data-ttu-id="d318d-124">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span><span class="sxs-lookup"><span data-stu-id="d318d-124">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>  

1. <span data-ttu-id="d318d-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d318d-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d318d-126">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="d318d-126">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>  
3. <span data-ttu-id="d318d-127">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="d318d-127">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>  
4. <span data-ttu-id="d318d-128">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span><span class="sxs-lookup"><span data-stu-id="d318d-128">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span></span>  
5. <span data-ttu-id="d318d-129">On the **Navigate** page, select the general ledger entry line, and then choose the **Show** action.</span><span class="sxs-lookup"><span data-stu-id="d318d-129">On the **Navigate** page, select the general ledger entry line, and then choose the **Show** action.</span></span>  

<span data-ttu-id="d318d-130">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span><span class="sxs-lookup"><span data-stu-id="d318d-130">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d318d-131">See Also</span><span class="sxs-lookup"><span data-stu-id="d318d-131">See Also</span></span>

[<span data-ttu-id="d318d-132">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d318d-132">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="d318d-133">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="d318d-133">Setting Up Fixed Assets</span></span>](fa-setup.md)  
<span data-ttu-id="d318d-134">[To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="d318d-134">[To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
[<span data-ttu-id="d318d-135">Finance</span><span class="sxs-lookup"><span data-stu-id="d318d-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="d318d-136">Getting Started</span><span class="sxs-lookup"><span data-stu-id="d318d-136">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="d318d-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d318d-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
