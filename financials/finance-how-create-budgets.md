---
title: Creating  Budgets| Microsoft Docs
description: Describes hos to create budgets to forecast different financial activities and assign dimensions for business intelligence purposes.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 7dfd3cc7efe00b48a39982bb220ccc21b7409da4
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-create--budgets"></a><span data-ttu-id="1e3e5-103">How to: Create  Budgets</span><span class="sxs-lookup"><span data-stu-id="1e3e5-103">How to: Create  Budgets</span></span>
<span data-ttu-id="1e3e5-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span></span> <span data-ttu-id="1e3e5-105">First, you set up the budget name and enter the budget figures.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-105">First, you set up the budget name and enter the budget figures.</span></span> <span data-ttu-id="1e3e5-106">The budget name is then included on all the budget entries you create.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-106">The budget name is then included on all the budget entries you create.</span></span>  

 <span data-ttu-id="1e3e5-107">When you create a budget, you can define four dimensions for each budget.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-107">When you create a budget, you can define four dimensions for each budget.</span></span> <span data-ttu-id="1e3e5-108">These budget\-specific dimensions are called budget dimensions.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-108">These budget\-specific dimensions are called budget dimensions.</span></span> <span data-ttu-id="1e3e5-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span></span> <span data-ttu-id="1e3e5-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span></span> <span data-ttu-id="1e3e5-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="1e3e5-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

 <span data-ttu-id="1e3e5-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analysing budgeted versus actual amounts in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="1e3e5-113">For more information, see [Business Intelligence](bi.md).</span><span class="sxs-lookup"><span data-stu-id="1e3e5-113">For more information, see [Business Intelligence](bi.md).</span></span>   

 > [!NOTE]  
>   <span data-ttu-id="1e3e5-114">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-114">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="1e3e5-115">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="1e3e5-115">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>  

### <a name="to-create-a-new-budget"></a><span data-ttu-id="1e3e5-116">To create a new budget</span><span class="sxs-lookup"><span data-stu-id="1e3e5-116">To create a new budget</span></span>  

1. <span data-ttu-id="1e3e5-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1e3e5-118">Choose the **Edit List** action, and then fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-118">Choose the **Edit List** action, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="1e3e5-119">Choose the **Edit Budget** action.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-119">Choose the **Edit Budget** action.</span></span>
4. <span data-ttu-id="1e3e5-120">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-120">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span></span>  

    <span data-ttu-id="1e3e5-121">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-121">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span></span> <span data-ttu-id="1e3e5-122">Because the budget name has just been created, there are no entries that match the filter.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-122">Because the budget name has just been created, there are no entries that match the filter.</span></span> <span data-ttu-id="1e3e5-123">Therefore, the window is empty.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-123">Therefore, the window is empty.</span></span>  
5. <span data-ttu-id="1e3e5-124">To enter an amount, choose the relevant cell in the matrix.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-124">To enter an amount, choose the relevant cell in the matrix.</span></span> <span data-ttu-id="1e3e5-125">The **G/L Budget Entries** window opens.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-125">The **G/L Budget Entries** window opens.</span></span>  
6. <span data-ttu-id="1e3e5-126">Create a new line and fill in the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-126">Create a new line and fill in the **Amount** field.</span></span> <span data-ttu-id="1e3e5-127">Close the **G/L Budget Entries** window.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-127">Close the **G/L Budget Entries** window.</span></span>  
7. <span data-ttu-id="1e3e5-128">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-128">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1e3e5-129">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span><span class="sxs-lookup"><span data-stu-id="1e3e5-129">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span></span>   

## <a name="see-also"></a><span data-ttu-id="1e3e5-130">See Also</span><span class="sxs-lookup"><span data-stu-id="1e3e5-130">See Also</span></span>
[<span data-ttu-id="1e3e5-131">Finance</span><span class="sxs-lookup"><span data-stu-id="1e3e5-131">Finance</span></span>](finance.md)  
[<span data-ttu-id="1e3e5-132">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="1e3e5-132">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="1e3e5-133">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="1e3e5-133">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="1e3e5-134">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="1e3e5-134">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="1e3e5-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1e3e5-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

