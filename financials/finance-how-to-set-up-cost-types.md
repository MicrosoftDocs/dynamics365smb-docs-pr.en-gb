---
title: How to Set Up a Chart of Cost Types | Microsoft Docs
description: Chart of cost types are similar to the chart of accounts in the general ledger.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger, accounts
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: c89170fd159428d771df105ca16a1d91d29651e4
ms.contentlocale: en-gb
ms.lasthandoff: 04/16/2018

---
# <a name="set-up-cost-types"></a><span data-ttu-id="747fa-103">Set Up Cost Types</span><span class="sxs-lookup"><span data-stu-id="747fa-103">Set Up Cost Types</span></span>
<span data-ttu-id="747fa-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="747fa-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span></span> <span data-ttu-id="747fa-105">You can set up the chart of cost types in the following ways:</span><span class="sxs-lookup"><span data-stu-id="747fa-105">You can set up the chart of cost types in the following ways:</span></span>  

-   <span data-ttu-id="747fa-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="747fa-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span></span> <span data-ttu-id="747fa-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="747fa-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span></span> <span data-ttu-id="747fa-108">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="747fa-108">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="747fa-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="747fa-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span></span> <span data-ttu-id="747fa-110">You must create each new cost type individually.</span><span class="sxs-lookup"><span data-stu-id="747fa-110">You must create each new cost type individually.</span></span>  

## <a name="to-transfer-the-general-ledger-chart-of-accounts-to-the-chart-of-cost-types"></a><span data-ttu-id="747fa-111">To transfer the general ledger chart of accounts to the chart of cost types</span><span class="sxs-lookup"><span data-stu-id="747fa-111">To transfer the general ledger chart of accounts to the chart of cost types</span></span>  
1.  <span data-ttu-id="747fa-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="747fa-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="747fa-113">Choose the **Get Cost Types from Chart of Accounts** action.</span><span class="sxs-lookup"><span data-stu-id="747fa-113">Choose the **Get Cost Types from Chart of Accounts** action.</span></span> <span data-ttu-id="747fa-114">In the dialogue box, choose the **Yes** button to confirm the transfer.</span><span class="sxs-lookup"><span data-stu-id="747fa-114">In the dialog box, choose the **Yes** button to confirm the transfer.</span></span> <span data-ttu-id="747fa-115">The function uses the chart of accounts to create a chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="747fa-115">The function uses the chart of accounts to create a chart of cost types.</span></span>  

    <span data-ttu-id="747fa-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span><span class="sxs-lookup"><span data-stu-id="747fa-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span></span> <span data-ttu-id="747fa-117">You can change the chart of cost types, as necessary.</span><span class="sxs-lookup"><span data-stu-id="747fa-117">You can change the chart of cost types, as necessary.</span></span> <span data-ttu-id="747fa-118">For example, you can delete duplicate existing cost types.</span><span class="sxs-lookup"><span data-stu-id="747fa-118">For example, you can delete duplicate existing cost types.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="747fa-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="747fa-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span></span> <span data-ttu-id="747fa-120">The **No.**</span><span class="sxs-lookup"><span data-stu-id="747fa-120">The **No.**</span></span> <span data-ttu-id="747fa-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="747fa-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span></span> <span data-ttu-id="747fa-122">The function runs automatically before transferring general ledger entries to cost accounting.</span><span class="sxs-lookup"><span data-stu-id="747fa-122">The function runs automatically before transferring general ledger entries to cost accounting.</span></span>  

## <a name="to-set-up-new-cost-types-in-the-chart-of-cost-types-window"></a><span data-ttu-id="747fa-123">To set up new cost types in the Chart of Cost Types window</span><span class="sxs-lookup"><span data-stu-id="747fa-123">To set up new cost types in the Chart of Cost Types window</span></span>  
1. <span data-ttu-id="747fa-124">Open the **Chart of Cost Types** window in edit mode.</span><span class="sxs-lookup"><span data-stu-id="747fa-124">Open the **Chart of Cost Types** window in edit mode.</span></span>  
2. <span data-ttu-id="747fa-125">Fill in the fields as described as necessary.</span><span class="sxs-lookup"><span data-stu-id="747fa-125">Fill in the fields as described as necessary.</span></span> [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

   > [!NOTE]  
   >  <span data-ttu-id="747fa-126">You can set up and maintain cost types in either the **Cost Type Card** window or in the **Chart of Cost Types** window.</span><span class="sxs-lookup"><span data-stu-id="747fa-126">You can set up and maintain cost types in either the **Cost Type Card** window or in the **Chart of Cost Types** window.</span></span> <span data-ttu-id="747fa-127">In this procedure, you set up cost types in the **Chart of Cost Types** window.</span><span class="sxs-lookup"><span data-stu-id="747fa-127">In this procedure, you set up cost types in the **Chart of Cost Types** window.</span></span>

3. <span data-ttu-id="747fa-128">After you have created all cost types, choose the **Indent Cost Types** action.</span><span class="sxs-lookup"><span data-stu-id="747fa-128">After you have created all cost types, choose the **Indent Cost Types** action.</span></span> <span data-ttu-id="747fa-129">In the dialogue box, choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="747fa-129">In the dialog box, choose the **Yes** button.</span></span>  
4. <span data-ttu-id="747fa-130">Link the new cost type to the corresponding general ledger account.</span><span class="sxs-lookup"><span data-stu-id="747fa-130">Link the new cost type to the corresponding general ledger account.</span></span>  

   > [!IMPORTANT]  
   >  <span data-ttu-id="747fa-131">If you have entered definitions in the **Totalling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="747fa-131">If you have entered definitions in the **Totaling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="to-update-cost-types"></a><span data-ttu-id="747fa-132">To update cost types</span><span class="sxs-lookup"><span data-stu-id="747fa-132">To update cost types</span></span>  
1.  <span data-ttu-id="747fa-133">In the **Cost Accounting Setup** window, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span><span class="sxs-lookup"><span data-stu-id="747fa-133">In the **Cost Accounting Setup** window, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span></span>  
2.  <span data-ttu-id="747fa-134">In the **Align G/L Account** field, you can choose from the following options.</span><span class="sxs-lookup"><span data-stu-id="747fa-134">In the **Align G/L Account** field, you can choose from the following options.</span></span>  

- <span data-ttu-id="747fa-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="747fa-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="747fa-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="747fa-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="747fa-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="747fa-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="747fa-138">See Also</span><span class="sxs-lookup"><span data-stu-id="747fa-138">See Also</span></span>  
[<span data-ttu-id="747fa-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="747fa-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="747fa-140">[Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="747fa-140">[Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md) </span></span>  
<span data-ttu-id="747fa-141">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="747fa-141">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span></span>  
<span data-ttu-id="747fa-142">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span><span class="sxs-lookup"><span data-stu-id="747fa-142">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span></span>  
<span data-ttu-id="747fa-143">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="747fa-143">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="747fa-144">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="747fa-144">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="747fa-145">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="747fa-145">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="747fa-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="747fa-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

