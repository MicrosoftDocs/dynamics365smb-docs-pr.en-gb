---
title: How to Set Up Cost Objects | Microsoft Docs
description: Learn how to set up cost objects, which are similar to dimensions for the general ledger.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: finance-set-up-cost-accounting
ms.openlocfilehash: ae2ca5b4c6f63a004d42c2ae1ef9f0efa95dd02c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2306035"
---
# <a name="set-up-cost-objects"></a><span data-ttu-id="50bec-103">Set Up Cost Objects</span><span class="sxs-lookup"><span data-stu-id="50bec-103">Set Up Cost Objects</span></span>
<span data-ttu-id="50bec-104">Cost objects are projects, products, or services of a company.</span><span class="sxs-lookup"><span data-stu-id="50bec-104">Cost objects are projects, products, or services of a company.</span></span> <span data-ttu-id="50bec-105">The chart of cost objects is similar to the dimension information for the general ledger.</span><span class="sxs-lookup"><span data-stu-id="50bec-105">The chart of cost objects is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="50bec-106">You can set up the chart of cost objects in the following ways:</span><span class="sxs-lookup"><span data-stu-id="50bec-106">You can set up the chart of cost objects in the following ways:</span></span>  

* <span data-ttu-id="50bec-107">Transfer dimension values in the general ledger to the chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="50bec-107">Transfer dimension values in the general ledger to the chart of cost objects.</span></span> <span data-ttu-id="50bec-108">You can make any necessary adjustments after the transfer.</span><span class="sxs-lookup"><span data-stu-id="50bec-108">You can make any necessary adjustments after the transfer.</span></span>  
* <span data-ttu-id="50bec-109">Create a new chart of cost object that is independent of the general ledger or add a new cost object to an existing chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="50bec-109">Create a new chart of cost object that is independent of the general ledger or add a new cost object to an existing chart of cost objects.</span></span> <span data-ttu-id="50bec-110">You must create each cost object individually.</span><span class="sxs-lookup"><span data-stu-id="50bec-110">You must create each cost object individually.</span></span>  

## <a name="to-transfer-dimension-values-from-the-general-ledger-to-the-chart-of-cost-objects"></a><span data-ttu-id="50bec-111">To transfer dimension values from the general ledger to the chart of cost objects</span><span class="sxs-lookup"><span data-stu-id="50bec-111">To transfer dimension values from the general ledger to the chart of cost objects</span></span>  
1.  <span data-ttu-id="50bec-112">Set a dimension to be the cost object dimension on the **Update CA Dimensions** page.</span><span class="sxs-lookup"><span data-stu-id="50bec-112">Set a dimension to be the cost object dimension on the **Update CA Dimensions** page.</span></span> <span data-ttu-id="50bec-113">Only the values from this dimension are transferred.</span><span class="sxs-lookup"><span data-stu-id="50bec-113">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="50bec-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Objects**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="50bec-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Objects**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="50bec-115">Choose the **Get Cost Objects from Dimension** action to transfer dimension values to the chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="50bec-115">Choose the **Get Cost Objects from Dimension** action to transfer dimension values to the chart of cost objects.</span></span> <span data-ttu-id="50bec-116">The function transfers the dimension values that you defined in step 1.</span><span class="sxs-lookup"><span data-stu-id="50bec-116">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="50bec-117">You can set up the **Align Cost Object Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost objects.</span><span class="sxs-lookup"><span data-stu-id="50bec-117">You can set up the **Align Cost Object Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost objects.</span></span> <span data-ttu-id="50bec-118">You cannot define a synchronisation of the chart of cost objects to dimension values from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="50bec-118">You cannot define a synchronization of the chart of cost objects to dimension values from the general ledger.</span></span>  

<span data-ttu-id="50bec-119">The chart of cost objects now contains all specified dimension values from the general ledger and includes titles and subtotals.</span><span class="sxs-lookup"><span data-stu-id="50bec-119">The chart of cost objects now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-objects-in-the-chart-of-cost-objects-page"></a><span data-ttu-id="50bec-120">To create new cost objects in the Chart of Cost Objects page</span><span class="sxs-lookup"><span data-stu-id="50bec-120">To create new cost objects in the Chart of Cost Objects page</span></span>  
<span data-ttu-id="50bec-121">You can set up and maintain cost objects in either the **Cost Object Card** card or on the **Chart of Cost Objects** page.</span><span class="sxs-lookup"><span data-stu-id="50bec-121">You can set up and maintain cost objects in either the **Cost Object Card** card or on the **Chart of Cost Objects** page.</span></span> <span data-ttu-id="50bec-122">In this procedure, you set up cost objects on the **Chart of Cost Objects** page.</span><span class="sxs-lookup"><span data-stu-id="50bec-122">In this procedure, you set up cost objects on the **Chart of Cost Objects** page.</span></span>  

1.  <span data-ttu-id="50bec-123">Open the **Chart of Cost Objects** page in edit mode.</span><span class="sxs-lookup"><span data-stu-id="50bec-123">Open the **Chart of Cost Objects** page in edit mode.</span></span>  
2.  <span data-ttu-id="50bec-124">In the **Code** field, enter the cost object code.</span><span class="sxs-lookup"><span data-stu-id="50bec-124">In the **Code** field, enter the cost object code.</span></span> <span data-ttu-id="50bec-125">All cost objects must have a code.</span><span class="sxs-lookup"><span data-stu-id="50bec-125">All cost objects must have a code.</span></span>  
3.  <span data-ttu-id="50bec-126">In the **Name** field, enter the cost object name.</span><span class="sxs-lookup"><span data-stu-id="50bec-126">In the **Name** field, enter the cost object name.</span></span>  
4.  <span data-ttu-id="50bec-127">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost object.</span><span class="sxs-lookup"><span data-stu-id="50bec-127">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost object.</span></span>  

    * <span data-ttu-id="50bec-128">For cost objects of the **Total** line type, fill in the **Total From/To** field.</span><span class="sxs-lookup"><span data-stu-id="50bec-128">For cost objects of the **Total** line type, fill in the **Total From/To** field.</span></span> <span data-ttu-id="50bec-129">Use the **or** operator, which is a vertical line (**&#124;**), to set ranges of cost objects.</span><span class="sxs-lookup"><span data-stu-id="50bec-129">Use the **or** operator, which is a vertical line (**&#124;**), to set ranges of cost objects.</span></span>  
    * <span data-ttu-id="50bec-130">For cost objects of the **End-Total** line type, this field is filled in automatically when you use  the indent function.</span><span class="sxs-lookup"><span data-stu-id="50bec-130">For cost objects of the **End-Total** line type, this field is filled in automatically when you use  the indent function.</span></span>  
5.  <span data-ttu-id="50bec-131">Fill in the **Sorting Order** field.</span><span class="sxs-lookup"><span data-stu-id="50bec-131">Fill in the **Sorting Order** field.</span></span>  
6.  <span data-ttu-id="50bec-132">Chose the next empty line to create a new cost object, and then repeat steps 2 through 5.</span><span class="sxs-lookup"><span data-stu-id="50bec-132">Chose the next empty line to create a new cost object, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="50bec-133">After you have set up all the cost objects, choose the **Indent Cost Objects** action.</span><span class="sxs-lookup"><span data-stu-id="50bec-133">After you have set up all the cost objects, choose the **Indent Cost Objects** action.</span></span> <span data-ttu-id="50bec-134">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="50bec-134">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="50bec-135">If you have entered definitions in the **Total From/To** fields for **End-Total** cost objects before you run the indent function, then you must enter them again.</span><span class="sxs-lookup"><span data-stu-id="50bec-135">If you have entered definitions in the **Total From/To** fields for **End-Total** cost objects before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="50bec-136">The function overwrites the values in all **End-Total** fields.</span><span class="sxs-lookup"><span data-stu-id="50bec-136">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="50bec-137">See Also</span><span class="sxs-lookup"><span data-stu-id="50bec-137">See Also</span></span>  
[<span data-ttu-id="50bec-138">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="50bec-138">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="50bec-139">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="50bec-139">[Defining Cost Centers and Cost Objects for Chart of Accounts](finance-defining-cost-centers-and-cost-objects-for-chart-of-accounts.md) </span></span>  
<span data-ttu-id="50bec-140">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span><span class="sxs-lookup"><span data-stu-id="50bec-140">[Balances Between Cost Type, Cost Center, and Cost Object](finance-balances-between-cost-type-cost-center-and-cost-object.md) </span></span>  
<span data-ttu-id="50bec-141">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="50bec-141">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="50bec-142">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="50bec-142">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="50bec-143">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="50bec-143">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="50bec-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="50bec-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
