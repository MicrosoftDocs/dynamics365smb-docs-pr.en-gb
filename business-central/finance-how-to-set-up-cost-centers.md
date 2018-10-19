---
title: How to Set Up Cost Centres | Microsoft Docs
description: Cost centres are departments that are responsible for costs and income. The chart of cost centres is similar to the dimension information for the general ledger.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 7362518cbade8132fb07f49e7b2e9be67c4bce29
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-cost-centers"></a><span data-ttu-id="afa92-104">Set Up Cost Centres</span><span class="sxs-lookup"><span data-stu-id="afa92-104">Set Up Cost Centers</span></span>
<span data-ttu-id="afa92-105">Cost centres are departments that are responsible for costs and income.</span><span class="sxs-lookup"><span data-stu-id="afa92-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="afa92-106">The chart of cost centres is similar to the dimension information for the general ledger.</span><span class="sxs-lookup"><span data-stu-id="afa92-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="afa92-107">You can set up the chart of cost centres in the following ways:</span><span class="sxs-lookup"><span data-stu-id="afa92-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="afa92-108">Transfer dimension values in the general ledger to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="afa92-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="afa92-109">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="afa92-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="afa92-110">Create a new chart of cost centre that is independent of the general ledger or add a new cost centre to an existing chart of cost centre.</span><span class="sxs-lookup"><span data-stu-id="afa92-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="afa92-111">You must create each cost centre individually.</span><span class="sxs-lookup"><span data-stu-id="afa92-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="afa92-112">To transfer dimension values in the general ledger to the chart of cost centres</span><span class="sxs-lookup"><span data-stu-id="afa92-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="afa92-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span><span class="sxs-lookup"><span data-stu-id="afa92-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span></span> <span data-ttu-id="afa92-114">Only the values from this dimension are transferred.</span><span class="sxs-lookup"><span data-stu-id="afa92-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="afa92-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centres**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="afa92-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="afa92-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centres from Dimension** to transfer dimension values to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="afa92-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="afa92-117">The function transfers the dimension values that you defined in step 1.</span><span class="sxs-lookup"><span data-stu-id="afa92-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="afa92-118">You can set up the **Align Cost Centre Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="afa92-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="afa92-119">You cannot define a synchronisation of the chart of cost centres to dimension values from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="afa92-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="afa92-120">The chart of cost centres now contains all specified dimension values from the general ledger and includes titles and subtotals.</span><span class="sxs-lookup"><span data-stu-id="afa92-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a><span data-ttu-id="afa92-121">To create new cost centers in the Chart of Cost Centers window</span><span class="sxs-lookup"><span data-stu-id="afa92-121">To create new cost centers in the Chart of Cost Centers window</span></span>  
<span data-ttu-id="afa92-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span><span class="sxs-lookup"><span data-stu-id="afa92-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span></span> <span data-ttu-id="afa92-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span><span class="sxs-lookup"><span data-stu-id="afa92-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span></span>  

1. <span data-ttu-id="afa92-124">Open the **Chart of Cost Centers** window in edit mode.</span><span class="sxs-lookup"><span data-stu-id="afa92-124">Open the **Chart of Cost Centers** window in edit mode.</span></span>  
2. <span data-ttu-id="afa92-125">In the **Code** field, enter the cost center code.</span><span class="sxs-lookup"><span data-stu-id="afa92-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="afa92-126">All cost centres must have a code.</span><span class="sxs-lookup"><span data-stu-id="afa92-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="afa92-127">In the **Name** field, enter the cost center name.</span><span class="sxs-lookup"><span data-stu-id="afa92-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="afa92-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost centre.</span><span class="sxs-lookup"><span data-stu-id="afa92-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="afa92-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span><span class="sxs-lookup"><span data-stu-id="afa92-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="afa92-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span><span class="sxs-lookup"><span data-stu-id="afa92-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="afa92-131">For cost centres of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span><span class="sxs-lookup"><span data-stu-id="afa92-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="afa92-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span><span class="sxs-lookup"><span data-stu-id="afa92-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="afa92-133">Choose the next empty line to create a new cost centre, and then repeat steps 2 through 5.</span><span class="sxs-lookup"><span data-stu-id="afa92-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="afa92-134">After you have set up all the cost centres, choose the **Indent Cost Centres** action.</span><span class="sxs-lookup"><span data-stu-id="afa92-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="afa92-135">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="afa92-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="afa92-136">If you have entered definitions in the **Totalling** fields for **End-Total** cost centres before you run the indent function, then you must enter them again.</span><span class="sxs-lookup"><span data-stu-id="afa92-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="afa92-137">The function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="afa92-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="afa92-138">See Also</span><span class="sxs-lookup"><span data-stu-id="afa92-138">See Also</span></span>  
[<span data-ttu-id="afa92-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="afa92-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="afa92-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="afa92-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="afa92-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="afa92-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="afa92-142">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="afa92-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="afa92-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="afa92-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

