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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 16d052c67a2d9b5513e9dac901dfeddce0527512
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749425"
---
# <a name="dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="86629-103">Dispose of or Retire Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="86629-103">Dispose of or Retire Fixed Assets</span></span>

<span data-ttu-id="86629-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span><span class="sxs-lookup"><span data-stu-id="86629-104">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="86629-105">A disposal entry must be the last entry posted for a fixed asset.</span><span class="sxs-lookup"><span data-stu-id="86629-105">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="86629-106">For partially disposed fixed assets, you can post more than one disposal entry.</span><span class="sxs-lookup"><span data-stu-id="86629-106">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="86629-107">The total of all posted disposal amounts must be a credit amount.</span><span class="sxs-lookup"><span data-stu-id="86629-107">The total of all posted disposal amounts must be a credit amount.</span></span>  

> [!NOTE]  
> <span data-ttu-id="86629-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span><span class="sxs-lookup"><span data-stu-id="86629-108">If you trade-in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="86629-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="86629-109">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

<span data-ttu-id="86629-110">The following steps assume that you have already set up the relevant posting groups in the **FA Posting Groups** page.</span><span class="sxs-lookup"><span data-stu-id="86629-110">The following steps assume that you have already set up the relevant posting groups in the **FA Posting Groups** page.</span></span> <span data-ttu-id="86629-111">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="86629-111">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="86629-112">To post a disposal from the fixed asset G/L journal</span><span class="sxs-lookup"><span data-stu-id="86629-112">To post a disposal from the fixed asset G/L journal</span></span>

1. <span data-ttu-id="86629-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="86629-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Asset G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="86629-114">Create an initial journal line and fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="86629-114">Create an initial journal line and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="86629-115">In the **FA Posting Type** field, select **Disposal**.</span><span class="sxs-lookup"><span data-stu-id="86629-115">In the **FA Posting Type** field, select **Disposal**.</span></span>  
4. <span data-ttu-id="86629-116">Choose the **Insert FA Bal. Account** action.</span><span class="sxs-lookup"><span data-stu-id="86629-116">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="86629-117">A second journal line is created for the balancing account that is set up for disposal posting.</span><span class="sxs-lookup"><span data-stu-id="86629-117">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="86629-118">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span><span class="sxs-lookup"><span data-stu-id="86629-118">Step 4 only works if you have set up the following: On the **FA Posting Group Card** page for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="86629-119">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="86629-119">For more information, see [To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
5. <span data-ttu-id="86629-120">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="86629-120">Choose the **Post** action.</span></span>  

<span data-ttu-id="86629-121">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span><span class="sxs-lookup"><span data-stu-id="86629-121">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="86629-122">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="86629-122">For more information, see [Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>  

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="86629-123">To view disposal ledger entries</span><span class="sxs-lookup"><span data-stu-id="86629-123">To view disposal ledger entries</span></span>
<span data-ttu-id="86629-124">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span><span class="sxs-lookup"><span data-stu-id="86629-124">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>  

1. <span data-ttu-id="86629-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="86629-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="86629-126">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="86629-126">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>  
3. <span data-ttu-id="86629-127">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="86629-127">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>  
4. <span data-ttu-id="86629-128">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Find Entries** action.</span><span class="sxs-lookup"><span data-stu-id="86629-128">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Find Entries** action.</span></span>  
5. <span data-ttu-id="86629-129">On the **Find Entries** page, select the general ledger entry line, and then choose the **Show Related Entries** action.</span><span class="sxs-lookup"><span data-stu-id="86629-129">On the **Find Entries** page, select the general ledger entry line, and then choose the **Show Related Entries** action.</span></span>  

<span data-ttu-id="86629-130">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span><span class="sxs-lookup"><span data-stu-id="86629-130">The **General Ledger Entries** page opens where you can see the entries that the disposal posting resulted in.</span></span>  

## <a name="see-also"></a><span data-ttu-id="86629-131">See Also</span><span class="sxs-lookup"><span data-stu-id="86629-131">See Also</span></span>

[<span data-ttu-id="86629-132">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="86629-132">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="86629-133">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="86629-133">Setting Up Fixed Assets</span></span>](fa-setup.md)  
<span data-ttu-id="86629-134">[To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span><span class="sxs-lookup"><span data-stu-id="86629-134">[To set up fixed asset posting groups](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups).</span></span>  
[<span data-ttu-id="86629-135">Finance</span><span class="sxs-lookup"><span data-stu-id="86629-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="86629-136">Getting Started</span><span class="sxs-lookup"><span data-stu-id="86629-136">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="86629-137">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="86629-137">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="86629-138">Find Entries</span><span class="sxs-lookup"><span data-stu-id="86629-138">Find Entries</span></span>](ui-find-entries.md)  
