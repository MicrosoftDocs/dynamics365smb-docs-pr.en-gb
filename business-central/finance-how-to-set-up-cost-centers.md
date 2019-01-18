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
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-set-up-cost-accounting
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 252ebf514635ada8e07bfb1e950d0cff156d0bfc
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="set-up-cost-centers"></a><span data-ttu-id="04f12-104">Set Up Cost Centres</span><span class="sxs-lookup"><span data-stu-id="04f12-104">Set Up Cost Centers</span></span>
<span data-ttu-id="04f12-105">Cost centres are departments that are responsible for costs and income.</span><span class="sxs-lookup"><span data-stu-id="04f12-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="04f12-106">The chart of cost centres is similar to the dimension information for the general ledger.</span><span class="sxs-lookup"><span data-stu-id="04f12-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="04f12-107">You can set up the chart of cost centres in the following ways:</span><span class="sxs-lookup"><span data-stu-id="04f12-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="04f12-108">Transfer dimension values in the general ledger to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="04f12-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="04f12-109">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="04f12-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="04f12-110">Create a new chart of cost centre that is independent of the general ledger or add a new cost centre to an existing chart of cost centre.</span><span class="sxs-lookup"><span data-stu-id="04f12-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="04f12-111">You must create each cost centre individually.</span><span class="sxs-lookup"><span data-stu-id="04f12-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="04f12-112">To transfer dimension values in the general ledger to the chart of cost centres</span><span class="sxs-lookup"><span data-stu-id="04f12-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="04f12-113">Set up a dimension to be the cost centre dimension on the **Update Cost Acctg. Dimensions** page.</span><span class="sxs-lookup"><span data-stu-id="04f12-113">Set up a dimension to be the cost center dimension on the **Update Cost Acctg. Dimensions** page.</span></span> <span data-ttu-id="04f12-114">Only the values from this dimension are transferred.</span><span class="sxs-lookup"><span data-stu-id="04f12-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="04f12-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centres**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="04f12-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="04f12-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centres from Dimension** to transfer dimension values to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="04f12-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="04f12-117">The function transfers the dimension values that you defined in step 1.</span><span class="sxs-lookup"><span data-stu-id="04f12-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="04f12-118">You can set up the **Align Cost Centre Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost centres.</span><span class="sxs-lookup"><span data-stu-id="04f12-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="04f12-119">You cannot define a synchronisation of the chart of cost centres to dimension values from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="04f12-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="04f12-120">The chart of cost centres now contains all specified dimension values from the general ledger and includes titles and subtotals.</span><span class="sxs-lookup"><span data-stu-id="04f12-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-page"></a><span data-ttu-id="04f12-121">To create new cost centres in the Chart of Cost Centres page</span><span class="sxs-lookup"><span data-stu-id="04f12-121">To create new cost centers in the Chart of Cost Centers page</span></span>  
<span data-ttu-id="04f12-122">You can set up and maintain cost centres in either the **Cost Centre Card** card or on the **Chart of Cost Centres** page.</span><span class="sxs-lookup"><span data-stu-id="04f12-122">You can set up and maintain cost centers in either the **Cost Center Card** card or on the **Chart of Cost Centers** page.</span></span> <span data-ttu-id="04f12-123">In this procedure, you set up cost centres on the **Chart of Cost Centres** page.</span><span class="sxs-lookup"><span data-stu-id="04f12-123">In this procedure, you set up cost centers on the **Chart of Cost Centers** page.</span></span>  

1. <span data-ttu-id="04f12-124">Open the **Chart of Cost Centres** page in edit mode.</span><span class="sxs-lookup"><span data-stu-id="04f12-124">Open the **Chart of Cost Centers** page in edit mode.</span></span>  
2. <span data-ttu-id="04f12-125">In the **Code** field, enter the cost center code.</span><span class="sxs-lookup"><span data-stu-id="04f12-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="04f12-126">All cost centres must have a code.</span><span class="sxs-lookup"><span data-stu-id="04f12-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="04f12-127">In the **Name** field, enter the cost center name.</span><span class="sxs-lookup"><span data-stu-id="04f12-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="04f12-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost centre.</span><span class="sxs-lookup"><span data-stu-id="04f12-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="04f12-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span><span class="sxs-lookup"><span data-stu-id="04f12-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="04f12-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span><span class="sxs-lookup"><span data-stu-id="04f12-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="04f12-131">For cost centres of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span><span class="sxs-lookup"><span data-stu-id="04f12-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="04f12-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span><span class="sxs-lookup"><span data-stu-id="04f12-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="04f12-133">Choose the next empty line to create a new cost centre, and then repeat steps 2 through 5.</span><span class="sxs-lookup"><span data-stu-id="04f12-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="04f12-134">After you have set up all the cost centres, choose the **Indent Cost Centres** action.</span><span class="sxs-lookup"><span data-stu-id="04f12-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="04f12-135">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="04f12-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="04f12-136">If you have entered definitions in the **Totalling** fields for **End-Total** cost centres before you run the indent function, then you must enter them again.</span><span class="sxs-lookup"><span data-stu-id="04f12-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="04f12-137">The function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="04f12-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="04f12-138">See Also</span><span class="sxs-lookup"><span data-stu-id="04f12-138">See Also</span></span>  
[<span data-ttu-id="04f12-139">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="04f12-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="04f12-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="04f12-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="04f12-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="04f12-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="04f12-142">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="04f12-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="04f12-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="04f12-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

