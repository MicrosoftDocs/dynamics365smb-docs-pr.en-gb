---
title: Manage FA Budgets| Microsoft Docs
description: You set up information about future investments, disposals, and depreciation of fixed assets to help prepare budgets and forecasts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: forecast
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 2185a1fc40ddae772e20994f6531b02d7e703e17
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-manage-budgets-for-fixed-assets"></a><span data-ttu-id="e43c2-103">How to: Manage Budgets for Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="e43c2-103">How to: Manage Budgets for Fixed Assets</span></span>
<span data-ttu-id="e43c2-104">You can set up budgeted fixed assets.</span><span class="sxs-lookup"><span data-stu-id="e43c2-104">You can set up budgeted fixed assets.</span></span> <span data-ttu-id="e43c2-105">For example, this lets you include anticipated acquisitions and sales in reports.</span><span class="sxs-lookup"><span data-stu-id="e43c2-105">For example, this lets you include anticipated acquisitions and sales in reports.</span></span>  

<span data-ttu-id="e43c2-106">To prepare your budgeted income statement, budgeted balance sheet, and cash budget, you need information about future investments, disposals and depreciation of fixed assets.</span><span class="sxs-lookup"><span data-stu-id="e43c2-106">To prepare your budgeted income statement, budgeted balance sheet, and cash budget, you need information about future investments, disposals and depreciation of fixed assets.</span></span> <span data-ttu-id="e43c2-107">You can get this information from the **Fixed Asset - Projected Value** report.</span><span class="sxs-lookup"><span data-stu-id="e43c2-107">You can get this information from the **Fixed Asset - Projected Value** report.</span></span> <span data-ttu-id="e43c2-108">Before you print this report, you must prepare the budget.</span><span class="sxs-lookup"><span data-stu-id="e43c2-108">Before you print this report, you must prepare the budget.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="e43c2-109">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="e43c2-109">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="e43c2-110">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="e43c2-110">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a><span data-ttu-id="e43c2-111">To budget the acquisition cost of a fixed asset</span><span class="sxs-lookup"><span data-stu-id="e43c2-111">To budget the acquisition cost of a fixed asset</span></span>
<span data-ttu-id="e43c2-112">To prepare a budget, you have to set up fixed asset cards for fixed assets that you intend to buy in the future.</span><span class="sxs-lookup"><span data-stu-id="e43c2-112">To prepare a budget, you have to set up fixed asset cards for fixed assets that you intend to buy in the future.</span></span> <span data-ttu-id="e43c2-113">The budget fixed assets are set up as ordinary fixed assets, but it must be set up to not post to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="e43c2-113">The budget fixed assets are set up as ordinary fixed assets, but it must be set up to not post to the general ledger.</span></span>

<span data-ttu-id="e43c2-114">When you post the acquisition cost, you enter the number of the budgeted fixed asset in the **Budgeted FA No.**</span><span class="sxs-lookup"><span data-stu-id="e43c2-114">When you post the acquisition cost, you enter the number of the budgeted fixed asset in the **Budgeted FA No.**</span></span> <span data-ttu-id="e43c2-115">field.</span><span class="sxs-lookup"><span data-stu-id="e43c2-115">field.</span></span> <span data-ttu-id="e43c2-116">This will post an acquisition cost with an opposite sign for the budgeted asset.</span><span class="sxs-lookup"><span data-stu-id="e43c2-116">This will post an acquisition cost with an opposite sign for the budgeted asset.</span></span> <span data-ttu-id="e43c2-117">This means that the total acquisition cost on the budgeted asset is the difference between the budgeted and the actual acquisition cost.</span><span class="sxs-lookup"><span data-stu-id="e43c2-117">This means that the total acquisition cost on the budgeted asset is the difference between the budgeted and the actual acquisition cost.</span></span>

1. <span data-ttu-id="e43c2-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e43c2-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="e43c2-119">Choose the **New** action to create a new fixed asset card for the budgeted fixed asset.</span><span class="sxs-lookup"><span data-stu-id="e43c2-119">Choose the **New** action to create a new fixed asset card for the budgeted fixed asset.</span></span>
3. <span data-ttu-id="e43c2-120">Select the **Budgeted Asset** check box to prevent posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="e43c2-120">Select the **Budgeted Asset** check box to prevent posting to the general ledger.</span></span>
4. <span data-ttu-id="e43c2-121">Fill in the remaining fields, assign a depreciation book, and then post the first acquisition cost with the budgeted fixed asset entered in the **Budgeted FA No.**</span><span class="sxs-lookup"><span data-stu-id="e43c2-121">Fill in the remaining fields, assign a depreciation book, and then post the first acquisition cost with the budgeted fixed asset entered in the **Budgeted FA No.**</span></span> <span data-ttu-id="e43c2-122">field on the journal line.</span><span class="sxs-lookup"><span data-stu-id="e43c2-122">field on the journal line.</span></span> <span data-ttu-id="e43c2-123">For more information, see [How to: Acquire Fixed Assets](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="e43c2-123">For more information, see [How to: Acquire Fixed Assets](fa-how-acquire.md).</span></span>

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a><span data-ttu-id="e43c2-124">To budget the disposal of a fixed asset</span><span class="sxs-lookup"><span data-stu-id="e43c2-124">To budget the disposal of a fixed asset</span></span>
<span data-ttu-id="e43c2-125">If you plan to sell assets within the budget period, you can enter information about sales price and sales date.</span><span class="sxs-lookup"><span data-stu-id="e43c2-125">If you plan to sell assets within the budget period, you can enter information about sales price and sales date.</span></span>

1. <span data-ttu-id="e43c2-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e43c2-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="e43c2-127">Select the fixed asset to be disposed of, and then choose the **Depreciation Books** action.</span><span class="sxs-lookup"><span data-stu-id="e43c2-127">Select the fixed asset to be disposed of, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="e43c2-128">In the **FA Depreciation Books** window, fill in the **Projected Disposal Date** and **Projected Proceeds on Disposal** fields.</span><span class="sxs-lookup"><span data-stu-id="e43c2-128">In the **FA Depreciation Books** window, fill in the **Projected Disposal Date** and **Projected Proceeds on Disposal** fields.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-projected-disposal-values"></a><span data-ttu-id="e43c2-129">To view projected disposal values</span><span class="sxs-lookup"><span data-stu-id="e43c2-129">To view projected disposal values</span></span>
<span data-ttu-id="e43c2-130">To see the projected disposal values and have the gain and loss calculated, you can use the **FA Projected Value** report.</span><span class="sxs-lookup"><span data-stu-id="e43c2-130">To see the projected disposal values and have the gain and loss calculated, you can use the **FA Projected Value** report.</span></span>

1. <span data-ttu-id="e43c2-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Projected Value**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e43c2-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Projected Value**, and then choose the related link.</span></span>
2. <span data-ttu-id="e43c2-132">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e43c2-132">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="e43c2-133">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="e43c2-133">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-budget-depreciation"></a><span data-ttu-id="e43c2-134">To budget depreciation</span><span class="sxs-lookup"><span data-stu-id="e43c2-134">To budget depreciation</span></span>
<span data-ttu-id="e43c2-135">You can use the **Fixed Asset - Projected Value** report to calculate future depreciation.</span><span class="sxs-lookup"><span data-stu-id="e43c2-135">You can use the **Fixed Asset - Projected Value** report to calculate future depreciation.</span></span> <span data-ttu-id="e43c2-136">The report shows the book value and accumulated depreciation at the start of the selected period, changes during the period, and the book value and accumulated depreciation at the end of the selected period.</span><span class="sxs-lookup"><span data-stu-id="e43c2-136">The report shows the book value and accumulated depreciation at the start of the selected period, changes during the period, and the book value and accumulated depreciation at the end of the selected period.</span></span>

1. <span data-ttu-id="e43c2-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Projected Value**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e43c2-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Projected Value**, and then choose the related link.</span></span>
2. <span data-ttu-id="e43c2-138">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e43c2-138">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="e43c2-139">To see total values for all assets, clear the **Print per Fixed Asset** check box.</span><span class="sxs-lookup"><span data-stu-id="e43c2-139">To see total values for all assets, clear the **Print per Fixed Asset** check box.</span></span>
4. <span data-ttu-id="e43c2-140">Leave the **Fixed Asset** FastTab blank to have all assets included.</span><span class="sxs-lookup"><span data-stu-id="e43c2-140">Leave the **Fixed Asset** FastTab blank to have all assets included.</span></span> <span data-ttu-id="e43c2-141">In the **Budgeted Asset** field, enter **No** to exclude budgeted assets or **Yes** to see budgeted assets only.</span><span class="sxs-lookup"><span data-stu-id="e43c2-141">In the **Budgeted Asset** field, enter **No** to exclude budgeted assets or **Yes** to see budgeted assets only.</span></span>
5. <span data-ttu-id="e43c2-142">Choose the **Print** or **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="e43c2-142">Choose the **Print** or **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="e43c2-143">See Also</span><span class="sxs-lookup"><span data-stu-id="e43c2-143">See Also</span></span>
[<span data-ttu-id="e43c2-144">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="e43c2-144">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="e43c2-145">Setting Up Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="e43c2-145">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="e43c2-146">Finance</span><span class="sxs-lookup"><span data-stu-id="e43c2-146">Finance</span></span>](finance.md)  
<span data-ttu-id="e43c2-147">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="e43c2-147">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="e43c2-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e43c2-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

