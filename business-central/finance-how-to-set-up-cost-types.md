---
title: How to Set Up a Chart of Cost Types | Microsoft Docs
description: Chart of cost types are similar to the chart of accounts in the general ledger.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger, accounts
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-set-up-cost-accounting
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 2846967648f5c0e0b6015c7990a941642fc27323
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="set-up-cost-types"></a><span data-ttu-id="b3a4f-103">Set Up Cost Types</span><span class="sxs-lookup"><span data-stu-id="b3a4f-103">Set Up Cost Types</span></span>
<span data-ttu-id="b3a4f-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-104">The chart of cost types is similar to the chart of accounts in the general ledger.</span></span> <span data-ttu-id="b3a4f-105">You can set up the chart of cost types in the following ways:</span><span class="sxs-lookup"><span data-stu-id="b3a4f-105">You can set up the chart of cost types in the following ways:</span></span>  

-   <span data-ttu-id="b3a4f-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-106">Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts.</span></span> <span data-ttu-id="b3a4f-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-107">Then, you can transfer the general ledger chart of accounts to the chart of cost types.</span></span> <span data-ttu-id="b3a4f-108">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-108">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="b3a4f-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-109">Create new chart of cost types or add new cost types to existing chart of cost types.</span></span> <span data-ttu-id="b3a4f-110">You must create each new cost type individually.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-110">You must create each new cost type individually.</span></span>  

## <a name="to-transfer-the-general-ledger-chart-of-accounts-to-the-chart-of-cost-types"></a><span data-ttu-id="b3a4f-111">To transfer the general ledger chart of accounts to the chart of cost types</span><span class="sxs-lookup"><span data-stu-id="b3a4f-111">To transfer the general ledger chart of accounts to the chart of cost types</span></span>  
1.  <span data-ttu-id="b3a4f-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b3a4f-113">Choose the **Get Cost Types from Chart of Accounts** action.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-113">Choose the **Get Cost Types from Chart of Accounts** action.</span></span> <span data-ttu-id="b3a4f-114">In the dialogue box, choose the **Yes** button to confirm the transfer.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-114">In the dialog box, choose the **Yes** button to confirm the transfer.</span></span> <span data-ttu-id="b3a4f-115">The function uses the chart of accounts to create a chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-115">The function uses the chart of accounts to create a chart of cost types.</span></span>  

    <span data-ttu-id="b3a4f-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-116">The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals.</span></span> <span data-ttu-id="b3a4f-117">You can change the chart of cost types, as necessary.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-117">You can change the chart of cost types, as necessary.</span></span> <span data-ttu-id="b3a4f-118">For example, you can delete duplicate existing cost types.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-118">For example, you can delete duplicate existing cost types.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="b3a4f-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-119">The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types.</span></span> <span data-ttu-id="b3a4f-120">The **No.**</span><span class="sxs-lookup"><span data-stu-id="b3a4f-120">The **No.**</span></span> <span data-ttu-id="b3a4f-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-121">field is filled and verified to make sure that each general ledger account is related to only one cost type.</span></span> <span data-ttu-id="b3a4f-122">The function runs automatically before transferring general ledger entries to cost accounting.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-122">The function runs automatically before transferring general ledger entries to cost accounting.</span></span>  

## <a name="to-set-up-new-cost-types-in-the-chart-of-cost-types-page"></a><span data-ttu-id="b3a4f-123">To set up new cost types in the Chart of Cost Types page</span><span class="sxs-lookup"><span data-stu-id="b3a4f-123">To set up new cost types in the Chart of Cost Types page</span></span>  
1.  <span data-ttu-id="b3a4f-124">Open the **Chart of Cost Types** page in edit mode.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-124">Open the **Chart of Cost Types** page in edit mode.</span></span>  
2.  <span data-ttu-id="b3a4f-125">Fill in the fields as described as necessary.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-125">Fill in the fields as described as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >  <span data-ttu-id="b3a4f-126">You can set up and maintain cost types in either the **Cost Type Card** page or on the **Chart of Cost Types** page.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-126">You can set up and maintain cost types in either the **Cost Type Card** page or on the **Chart of Cost Types** page.</span></span> <span data-ttu-id="b3a4f-127">In this procedure, you set up cost types on the **Chart of Cost Types** page.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-127">In this procedure, you set up cost types on the **Chart of Cost Types** page.</span></span>

3.  <span data-ttu-id="b3a4f-128">After you have created all cost types, choose the **Indent Cost Types** action.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-128">After you have created all cost types, choose the **Indent Cost Types** action.</span></span> <span data-ttu-id="b3a4f-129">In the dialogue box, choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-129">In the dialog box, choose the **Yes** button.</span></span>  
4.  <span data-ttu-id="b3a4f-130">Link the new cost type to the corresponding general ledger account.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-130">Link the new cost type to the corresponding general ledger account.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="b3a4f-131">If you have entered definitions in the **Totalling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-131">If you have entered definitions in the **Totaling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="to-update-cost-types"></a><span data-ttu-id="b3a4f-132">To update cost types</span><span class="sxs-lookup"><span data-stu-id="b3a4f-132">To update cost types</span></span>  
1.  <span data-ttu-id="b3a4f-133">On the **Cost Accounting Setup** page, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-133">On the **Cost Accounting Setup** page, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.</span></span>  
2.  <span data-ttu-id="b3a4f-134">In the **Align G/L Account** field, you can choose from the following options.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-134">In the **Align G/L Account** field, you can choose from the following options.</span></span>  

- <span data-ttu-id="b3a4f-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-135">**No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="b3a4f-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-136">**Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.</span></span>  
- <span data-ttu-id="b3a4f-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="b3a4f-137">**Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b3a4f-138">See Also</span><span class="sxs-lookup"><span data-stu-id="b3a4f-138">See Also</span></span>  
[<span data-ttu-id="b3a4f-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="b3a4f-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="b3a4f-140">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="b3a4f-140">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span></span>  
<span data-ttu-id="b3a4f-141">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span><span class="sxs-lookup"><span data-stu-id="b3a4f-141">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span></span>  
<span data-ttu-id="b3a4f-142">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="b3a4f-142">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="b3a4f-143">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="b3a4f-143">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="b3a4f-144">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="b3a4f-144">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="b3a4f-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b3a4f-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

