---
title: How to Work with Inventory Periods | Microsoft Docs
description: You can control the timeframe in which people can post post changes to inventory by defining inventory periods.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 309de0c582e125eb4bf5fb5b0c6b901adb1d0bfc
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "929248"
---
# <a name="work-with-inventory-periods"></a><span data-ttu-id="29b2c-103">Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="29b2c-103">Work with Inventory Periods</span></span>
<span data-ttu-id="29b2c-104">Inventory periods define a period of time in which you can post changes to inventory.</span><span class="sxs-lookup"><span data-stu-id="29b2c-104">Inventory periods define a period of time in which you can post changes to inventory.</span></span> <span data-ttu-id="29b2c-105">An inventory period is defined by the date on which it ends, or the ending date.</span><span class="sxs-lookup"><span data-stu-id="29b2c-105">An inventory period is defined by the date on which it ends, or the ending date.</span></span> <span data-ttu-id="29b2c-106">When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date.</span><span class="sxs-lookup"><span data-stu-id="29b2c-106">When you close an inventory period, you cannot post any changes to inventory, either expected or invoiced, before this ending date.</span></span> <span data-ttu-id="29b2c-107">You cannot post any new values to inventory before the ending date.</span><span class="sxs-lookup"><span data-stu-id="29b2c-107">You cannot post any new values to inventory before the ending date.</span></span> <span data-ttu-id="29b2c-108">If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.</span><span class="sxs-lookup"><span data-stu-id="29b2c-108">If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.</span></span>  

<span data-ttu-id="29b2c-109">The following sections describe how to:</span><span class="sxs-lookup"><span data-stu-id="29b2c-109">The following sections describe how to:</span></span>  

* <span data-ttu-id="29b2c-110">Create inventory periods.</span><span class="sxs-lookup"><span data-stu-id="29b2c-110">Create inventory periods.</span></span>  
* <span data-ttu-id="29b2c-111">Close inventory periods.</span><span class="sxs-lookup"><span data-stu-id="29b2c-111">Close inventory periods.</span></span>  
* <span data-ttu-id="29b2c-112">Reopen inventory periods.</span><span class="sxs-lookup"><span data-stu-id="29b2c-112">Reopen inventory periods.</span></span>  

## <a name="to-create-an-inventory-period"></a><span data-ttu-id="29b2c-113">To create an inventory period</span><span class="sxs-lookup"><span data-stu-id="29b2c-113">To create an inventory period</span></span>  
1. <span data-ttu-id="29b2c-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="29b2c-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="29b2c-115">Create a new line.</span><span class="sxs-lookup"><span data-stu-id="29b2c-115">Create a new line.</span></span>  
3. <span data-ttu-id="29b2c-116">In the **Ending Date** field, enter the last date in the inventory period that you want to define.</span><span class="sxs-lookup"><span data-stu-id="29b2c-116">In the **Ending Date** field, enter the last date in the inventory period that you want to define.</span></span> <span data-ttu-id="29b2c-117">When the period is closed, you will not be able to post inventory changes before this date.</span><span class="sxs-lookup"><span data-stu-id="29b2c-117">When the period is closed, you will not be able to post inventory changes before this date.</span></span>  
4. <span data-ttu-id="29b2c-118">Enter a descriptive name in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="29b2c-118">Enter a descriptive name in the **Name** field.</span></span> <span data-ttu-id="29b2c-119">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="29b2c-119">Choose the **OK** button.</span></span>  

## <a name="closing-inventory-periods"></a><span data-ttu-id="29b2c-120">Closing Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="29b2c-120">Closing Inventory Periods</span></span>  
<span data-ttu-id="29b2c-121">The **Closed** field indicates whether or not the inventory period is closed to inventory value changes.</span><span class="sxs-lookup"><span data-stu-id="29b2c-121">The **Closed** field indicates whether or not the inventory period is closed to inventory value changes.</span></span> <span data-ttu-id="29b2c-122">You cannot edit this field.</span><span class="sxs-lookup"><span data-stu-id="29b2c-122">You cannot edit this field.</span></span>  

<span data-ttu-id="29b2c-123">You can close any inventory period, provided that the following is true:</span><span class="sxs-lookup"><span data-stu-id="29b2c-123">You can close any inventory period, provided that the following is true:</span></span>  

* <span data-ttu-id="29b2c-124">There are no open outbound item ledger entries, meaning negative inventory, in that period.</span><span class="sxs-lookup"><span data-stu-id="29b2c-124">There are no open outbound item ledger entries, meaning negative inventory, in that period.</span></span>  
* <span data-ttu-id="29b2c-125">The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.</span><span class="sxs-lookup"><span data-stu-id="29b2c-125">The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.</span></span>  

<span data-ttu-id="29b2c-126">This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.</span><span class="sxs-lookup"><span data-stu-id="29b2c-126">This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in inventory.</span></span>  

### <a name="to-close-an-inventory-period"></a><span data-ttu-id="29b2c-127">To close an inventory period</span><span class="sxs-lookup"><span data-stu-id="29b2c-127">To close an inventory period</span></span>  
1. <span data-ttu-id="29b2c-128">Before closing an inventory period, run the **Adjust Cost – Item Entries** batch job to ensure that all cost adjustments are posted.</span><span class="sxs-lookup"><span data-stu-id="29b2c-128">Before closing an inventory period, run the **Adjust Cost – Item Entries** batch job to ensure that all cost adjustments are posted.</span></span> <span data-ttu-id="29b2c-129">On the **Actions** tab, in the **Functions** group, choose **Adjust Cost – Item Entries**.</span><span class="sxs-lookup"><span data-stu-id="29b2c-129">On the **Actions** tab, in the **Functions** group, choose **Adjust Cost – Item Entries**.</span></span>  

     <span data-ttu-id="29b2c-130">Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.</span><span class="sxs-lookup"><span data-stu-id="29b2c-130">Run the **Close Inventory Period – Test** report to determine if there are any open outbound item entries within the inventory period or any items whose cost has not yet been adjusted.</span></span>  
2. <span data-ttu-id="29b2c-131">Choose the **Close Inventory Period – Test** action.</span><span class="sxs-lookup"><span data-stu-id="29b2c-131">Choose the **Close Inventory Period – Test** action.</span></span>  

     <span data-ttu-id="29b2c-132">Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="29b2c-132">Run the **Post Inventory Cost to G/L** batch job to ensure that all costs are posted to the general ledger.</span></span>  
3. <span data-ttu-id="29b2c-133">Choose the **Post Inventory to G/L** action.</span><span class="sxs-lookup"><span data-stu-id="29b2c-133">Choose the **Post Inventory to G/L** action.</span></span>  
4. <span data-ttu-id="29b2c-134">On the **Inventory Periods** page, select the inventory period you want to close.</span><span class="sxs-lookup"><span data-stu-id="29b2c-134">On the **Inventory Periods** page, select the inventory period you want to close.</span></span>  
5. <span data-ttu-id="29b2c-135">Choose the **Close Period** action.</span><span class="sxs-lookup"><span data-stu-id="29b2c-135">Choose the **Close Period** action.</span></span> <span data-ttu-id="29b2c-136">After the inventory period has been closed, you cannot post inventory changes before the ending date.</span><span class="sxs-lookup"><span data-stu-id="29b2c-136">After the inventory period has been closed, you cannot post inventory changes before the ending date.</span></span> <span data-ttu-id="29b2c-137">The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.</span><span class="sxs-lookup"><span data-stu-id="29b2c-137">The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the inventory period.</span></span>  
6. <span data-ttu-id="29b2c-138">Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.</span><span class="sxs-lookup"><span data-stu-id="29b2c-138">Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.</span></span>  
7. <span data-ttu-id="29b2c-139">The inventory period is closed and a confirmation message is displayed when it is finished.</span><span class="sxs-lookup"><span data-stu-id="29b2c-139">The inventory period is closed and a confirmation message is displayed when it is finished.</span></span>  

## <a name="reopening-inventory-periods"></a><span data-ttu-id="29b2c-140">Reopening Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="29b2c-140">Reopening Inventory Periods</span></span>  
<span data-ttu-id="29b2c-141">After you have closed the inventory period, you cannot delete the inventory period.</span><span class="sxs-lookup"><span data-stu-id="29b2c-141">After you have closed the inventory period, you cannot delete the inventory period.</span></span> <span data-ttu-id="29b2c-142">You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period.</span><span class="sxs-lookup"><span data-stu-id="29b2c-142">You can, however, reopen it, if you would like to allow posting before the ending date of the inventory period.</span></span> <span data-ttu-id="29b2c-143">Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.</span><span class="sxs-lookup"><span data-stu-id="29b2c-143">Reopening a period also reopens all inventory periods with ending dates later than the period you reopen.</span></span>  

### <a name="to-reopen-an-inventory-period"></a><span data-ttu-id="29b2c-144">To reopen an inventory period</span><span class="sxs-lookup"><span data-stu-id="29b2c-144">To reopen an inventory period</span></span>  
1. <span data-ttu-id="29b2c-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="29b2c-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Periods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="29b2c-146">Select the inventory period you want to reopen.</span><span class="sxs-lookup"><span data-stu-id="29b2c-146">Select the inventory period you want to reopen.</span></span>  
3. <span data-ttu-id="29b2c-147">Choose the **Reopen Period** period action.</span><span class="sxs-lookup"><span data-stu-id="29b2c-147">Choose the **Reopen Period** period action.</span></span> <span data-ttu-id="29b2c-148">Confirm that you want to reopen the period.</span><span class="sxs-lookup"><span data-stu-id="29b2c-148">Confirm that you want to reopen the period.</span></span>  
4. <span data-ttu-id="29b2c-149">All inventory periods with ending dates later than the period you selected are reopened.</span><span class="sxs-lookup"><span data-stu-id="29b2c-149">All inventory periods with ending dates later than the period you selected are reopened.</span></span>  

## <a name="see-also"></a><span data-ttu-id="29b2c-150">See Also</span><span class="sxs-lookup"><span data-stu-id="29b2c-150">See Also</span></span>  
[<span data-ttu-id="29b2c-151">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="29b2c-151">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="29b2c-152">Finance</span><span class="sxs-lookup"><span data-stu-id="29b2c-152">Finance</span></span>](finance.md)  
[<span data-ttu-id="29b2c-153">Inventory</span><span class="sxs-lookup"><span data-stu-id="29b2c-153">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="29b2c-154">Working with Financials</span><span class="sxs-lookup"><span data-stu-id="29b2c-154">Working with Financials</span></span>](ui-work-product.md)
