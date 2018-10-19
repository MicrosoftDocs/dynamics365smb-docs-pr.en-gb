---
title: How to Plan Warehouse Movements in Worksheets | Microsoft Docs
description: Plan movements in the worksheet using a bin replenishment function or manually planning the lines that you want to create as movement instructions.
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
ms.openlocfilehash: d66ad263235d7f123f731263b0f13a009a1e20fd
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="plan-warehouse-movements-in-worksheets"></a><span data-ttu-id="6bbdc-103">Plan Warehouse Movements in Worksheets</span><span class="sxs-lookup"><span data-stu-id="6bbdc-103">Plan Warehouse Movements in Worksheets</span></span>
<span data-ttu-id="6bbdc-104">Plan movements in the worksheet using a bin replenishment function or manually planning the lines that you want to create as movement instructions.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-104">Plan movements in the worksheet using a bin replenishment function or manually planning the lines that you want to create as movement instructions.</span></span>  

## <a name="to-calculate-a-replenishment-movement"></a><span data-ttu-id="6bbdc-105">To calculate a replenishment movement</span><span class="sxs-lookup"><span data-stu-id="6bbdc-105">To calculate a replenishment movement</span></span>  
<span data-ttu-id="6bbdc-106">As the warehouse ships items out to customers, the bins with the highest bin rankings contain fewer and fewer items.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-106">As the warehouse ships items out to customers, the bins with the highest bin rankings contain fewer and fewer items.</span></span> <span data-ttu-id="6bbdc-107">To fill up these high-ranking pick bins with items from other bins, run the **Calculate Bin Replenishment** function in the **Movement Worksheet** window</span><span class="sxs-lookup"><span data-stu-id="6bbdc-107">To fill up these high-ranking pick bins with items from other bins, run the **Calculate Bin Replenishment** function in the **Movement Worksheet** window</span></span>

1.  <span data-ttu-id="6bbdc-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6bbdc-109">Choose the **Calculate Bin Replenishment** action.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-109">Choose the **Calculate Bin Replenishment** action.</span></span>  

    [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="6bbdc-110">creates lines that indicate precisely how you should move items from the low-ranking bins to the higher-ranking bins.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-110">creates lines that indicate precisely how you should move items from the low-ranking bins to the higher-ranking bins.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6bbdc-111">A movement is suggested according to FEFO when you activate the **Create Movement** function if the following conditions are met for an item:</span><span class="sxs-lookup"><span data-stu-id="6bbdc-111">A movement is suggested according to FEFO when you activate the **Create Movement** function if the following conditions are met for an item:</span></span>  
    >   
    >  -   <span data-ttu-id="6bbdc-112">The item has an expiration date.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-112">The item has an expiration date.</span></span>  
    > -   <span data-ttu-id="6bbdc-113">The **Pick According to FEFO** check box on the location card is selected.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-113">The **Pick According to FEFO** check box on the location card is selected.</span></span>  
    > -   <span data-ttu-id="6bbdc-114">The **Bin Mandatory** check box on the location card is selected.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-114">The **Bin Mandatory** check box on the location card is selected.</span></span>  
    > -   <span data-ttu-id="6bbdc-115">The **From Zone** and **From Bin** fields are blank.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-115">The **From Zone** and **From Bin** fields are blank.</span></span>  

    <span data-ttu-id="6bbdc-116">For more information, see [Picking by FEFO](warehouse-picking-by-fefo.md).</span><span class="sxs-lookup"><span data-stu-id="6bbdc-116">For more information, see [Picking by FEFO](warehouse-picking-by-fefo.md).</span></span>  

3.  <span data-ttu-id="6bbdc-117">Look through the lines and change them if necessary, or delete some of them if there is not enough time to perform them all.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-117">Look through the lines and change them if necessary, or delete some of them if there is not enough time to perform them all.</span></span>  
4.  <span data-ttu-id="6bbdc-118">Choose the **Create Movement** action to make a warehouse instruction for action by warehouse employees.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-118">Choose the **Create Movement** action to make a warehouse instruction for action by warehouse employees.</span></span>  

## <a name="to-move-the-entire-contents-of-one-or-more-bins-by-using-the-get-bin-content-function"></a><span data-ttu-id="6bbdc-119">To move the entire contents of one or more bins by using the Get Bin Content function</span><span class="sxs-lookup"><span data-stu-id="6bbdc-119">To move the entire contents of one or more bins by using the Get Bin Content function</span></span>  
<span data-ttu-id="6bbdc-120">You can also use the movement worksheet to plan other movement of inventory within the warehouse.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-120">You can also use the movement worksheet to plan other movement of inventory within the warehouse.</span></span> <span data-ttu-id="6bbdc-121">For example, when you want to place items in a bin for quality control, you can use the movement worksheet to plan this action and then create a movement to make instructions for an employee.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-121">For example, when you want to place items in a bin for quality control, you can use the movement worksheet to plan this action and then create a movement to make instructions for an employee.</span></span>  

1.  <span data-ttu-id="6bbdc-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6bbdc-123">Choose the **Get Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-123">Choose the **Get Bin Content** action.</span></span> <span data-ttu-id="6bbdc-124">Use the request window to filter which bins and items you want to appear on the movement worksheet lines.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-124">Use the request window to filter which bins and items you want to appear on the movement worksheet lines.</span></span>  
3.  <span data-ttu-id="6bbdc-125">Fill in the relevant fields in the batch job request window.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-125">Fill in the relevant fields in the batch job request window.</span></span> <span data-ttu-id="6bbdc-126">For example, if you want to see the bin content of all the bins in a certain zone at the location, fill in the **Zone Code** field.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-126">For example, if you want to see the bin content of all the bins in a certain zone at the location, fill in the **Zone Code** field.</span></span> <span data-ttu-id="6bbdc-127">If you want to retrieve lines for each bin that contains a particular item, fill in the **Item No.** field.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-127">If you want to retrieve lines for each bin that contains a particular item, fill in the **Item No.** field.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6bbdc-128">You cannot manually move items in or out of a bin of bin type RECEIVE, because items that are in a RECEIVE-type bin must be registered as being put away before they are part of available inventory.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-128">You cannot manually move items in or out of a bin of bin type RECEIVE, because items that are in a RECEIVE-type bin must be registered as being put away before they are part of available inventory.</span></span>  

4.  <span data-ttu-id="6bbdc-129">If you are retrieving many lines, choose **Sort** to select a sorting method to determine the order the lines will appear in the worksheet, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-129">If you are retrieving many lines, choose **Sort** to select a sorting method to determine the order the lines will appear in the worksheet, and then choose the **OK** button.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6bbdc-130">Movement lines are retrieved according to FEFO when you activate the **Get Bin Content** function if the following conditions are met for an item:</span><span class="sxs-lookup"><span data-stu-id="6bbdc-130">Movement lines are retrieved according to FEFO when you activate the **Get Bin Content** function if the following conditions are met for an item:</span></span>  
    >   
    >  -   <span data-ttu-id="6bbdc-131">The item has an expiration date.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-131">The item has an expiration date.</span></span>  
    > -   <span data-ttu-id="6bbdc-132">The **Pick According to FEFO** check box on the location card is selected.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-132">The **Pick According to FEFO** check box on the location card is selected.</span></span>  
    > -   <span data-ttu-id="6bbdc-133">The **Bin Mandatory** check box on the location card is selected.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-133">The **Bin Mandatory** check box on the location card is selected.</span></span>  
    > -   <span data-ttu-id="6bbdc-134">The **From Zone** and **From Bin** fields are blank.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-134">The **From Zone** and **From Bin** fields are blank.</span></span>  

5.  <span data-ttu-id="6bbdc-135">Complete some of the retrieved lines to reflect the changes you want to make.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-135">Complete some of the retrieved lines to reflect the changes you want to make.</span></span> <span data-ttu-id="6bbdc-136">For each item that you want to move, you must fill in the **Item No.**, **From Bin Code**, **To Bin Code**, and **Quantity** fields.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-136">For each item that you want to move, you must fill in the **Item No.**, **From Bin Code**, **To Bin Code**, and **Quantity** fields.</span></span>  
6.  <span data-ttu-id="6bbdc-137">Delete the incomplete lines that you used for information.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-137">Delete the incomplete lines that you used for information.</span></span>  
7.  <span data-ttu-id="6bbdc-138">Once the movement worksheet lines accurately reflect how the movement action should be carried out by the warehouse employee, choose the **Create Movement** action to create the instructions for the employee.</span><span class="sxs-lookup"><span data-stu-id="6bbdc-138">Once the movement worksheet lines accurately reflect how the movement action should be carried out by the warehouse employee, choose the **Create Movement** action to create the instructions for the employee.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6bbdc-139">See Also</span><span class="sxs-lookup"><span data-stu-id="6bbdc-139">See Also</span></span>  
[<span data-ttu-id="6bbdc-140">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="6bbdc-140">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="6bbdc-141">Inventory</span><span class="sxs-lookup"><span data-stu-id="6bbdc-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="6bbdc-142">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="6bbdc-142">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="6bbdc-143">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="6bbdc-143">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="6bbdc-144">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="6bbdc-144">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="6bbdc-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6bbdc-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

