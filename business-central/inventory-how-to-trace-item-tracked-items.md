---
title: Trace Item-Tracked Items
description: You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned. You can also find all current instances of a specific serial or lot number in the database. You do this by using the Item Tracing and the Find Entries features.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a425b974bf37b440de27f2b469694f9e8eac07de
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785707"
---
# <a name="trace-item-tracked-items"></a><span data-ttu-id="0eb17-105">Trace Item-Tracked Items</span><span class="sxs-lookup"><span data-stu-id="0eb17-105">Trace Item-Tracked Items</span></span>
<span data-ttu-id="0eb17-106">You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned.</span><span class="sxs-lookup"><span data-stu-id="0eb17-106">You can see where an item-tracked item was used, including how and when it was received or produced, transferred, sold, consumed, or returned.</span></span> <span data-ttu-id="0eb17-107">You can also find all current instances of a specific serial or lot number in the database.</span><span class="sxs-lookup"><span data-stu-id="0eb17-107">You can also find all current instances of a specific serial or lot number in the database.</span></span> <span data-ttu-id="0eb17-108">You do this by using the Item Tracing and the [Find Entries](ui-find-entries.md) features.</span><span class="sxs-lookup"><span data-stu-id="0eb17-108">You do this by using the Item Tracing and the [Find Entries](ui-find-entries.md) features.</span></span>  

<span data-ttu-id="0eb17-109">These features can be particularly useful in quality control when you need to find out which customers received products with a particular lot number or when you need to find out which lot a defective component came from.</span><span class="sxs-lookup"><span data-stu-id="0eb17-109">These features can be particularly useful in quality control when you need to find out which customers received products with a particular lot number or when you need to find out which lot a defective component came from.</span></span>  

 <span data-ttu-id="0eb17-110">On the **Item Tracing** page, you can trace forwards and backwards in a sequence of posted inventory transactions for the serial or lot number.</span><span class="sxs-lookup"><span data-stu-id="0eb17-110">On the **Item Tracing** page, you can trace forwards and backwards in a sequence of posted inventory transactions for the serial or lot number.</span></span>  

 <span data-ttu-id="0eb17-111">On the **Find Entries** page, you cannot see the sequence of transactions, but you can see all records of the serial or lot number, both posted entries and open records.</span><span class="sxs-lookup"><span data-stu-id="0eb17-111">On the **Find Entries** page, you cannot see the sequence of transactions, but you can see all records of the serial or lot number, both posted entries and open records.</span></span>  

 <span data-ttu-id="0eb17-112">The two features can be used in combination by transferring a traced serial or lot number to the **Find Entries** page to finish a complete trace scenario.</span><span class="sxs-lookup"><span data-stu-id="0eb17-112">The two features can be used in combination by transferring a traced serial or lot number to the **Find Entries** page to finish a complete trace scenario.</span></span> <span data-ttu-id="0eb17-113">For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span><span class="sxs-lookup"><span data-stu-id="0eb17-113">For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span></span>  

## <a name="to-trace-item-tracked-items"></a><span data-ttu-id="0eb17-114">To trace item-tracked items</span><span class="sxs-lookup"><span data-stu-id="0eb17-114">To trace item-tracked items</span></span>  

1.  <span data-ttu-id="0eb17-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Tracing**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0eb17-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Tracing**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0eb17-116">In the filter fields at the top of the page, enter the specific item numbers or a filter on the item numbers that you would like to trace.</span><span class="sxs-lookup"><span data-stu-id="0eb17-116">In the filter fields at the top of the page, enter the specific item numbers or a filter on the item numbers that you would like to trace.</span></span>  
3.  <span data-ttu-id="0eb17-117">In the **Show Components** field, select whether you would like to also see where the components for the items came from.</span><span class="sxs-lookup"><span data-stu-id="0eb17-117">In the **Show Components** field, select whether you would like to also see where the components for the items came from.</span></span> <span data-ttu-id="0eb17-118">Your options in this field are as follows.</span><span class="sxs-lookup"><span data-stu-id="0eb17-118">Your options in this field are as follows.</span></span>  

    |<span data-ttu-id="0eb17-119">Field</span><span class="sxs-lookup"><span data-stu-id="0eb17-119">Field</span></span>|<span data-ttu-id="0eb17-120">Description</span><span class="sxs-lookup"><span data-stu-id="0eb17-120">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="0eb17-121">**No**</span><span class="sxs-lookup"><span data-stu-id="0eb17-121">**No**</span></span>|<span data-ttu-id="0eb17-122">Select this option if you do not want to see any components.</span><span class="sxs-lookup"><span data-stu-id="0eb17-122">Select this option if you do not want to see any components.</span></span>|  
    |<span data-ttu-id="0eb17-123">**Item-tracked Only**</span><span class="sxs-lookup"><span data-stu-id="0eb17-123">**Item-tracked Only**</span></span>|<span data-ttu-id="0eb17-124">Select this option if you want to see only components that have lot or serial numbers.</span><span class="sxs-lookup"><span data-stu-id="0eb17-124">Select this option if you want to see only components that have lot or serial numbers.</span></span>|  
    |<span data-ttu-id="0eb17-125">**All**</span><span class="sxs-lookup"><span data-stu-id="0eb17-125">**All**</span></span>|<span data-ttu-id="0eb17-126">Select this option if you want to see all components.</span><span class="sxs-lookup"><span data-stu-id="0eb17-126">Select this option if you want to see all components.</span></span>|  

4.  <span data-ttu-id="0eb17-127">In the **Trace Method** field, select the method you would like to use for tracing the item.</span><span class="sxs-lookup"><span data-stu-id="0eb17-127">In the **Trace Method** field, select the method you would like to use for tracing the item.</span></span> <span data-ttu-id="0eb17-128">The options are as follows</span><span class="sxs-lookup"><span data-stu-id="0eb17-128">The options are as follows</span></span>  

    |<span data-ttu-id="0eb17-129">Field</span><span class="sxs-lookup"><span data-stu-id="0eb17-129">Field</span></span>|<span data-ttu-id="0eb17-130">Description</span><span class="sxs-lookup"><span data-stu-id="0eb17-130">Description</span></span>|  
    |----------------------------------|---------------------------------------|  
    |<span data-ttu-id="0eb17-131">**Usage->Origin**</span><span class="sxs-lookup"><span data-stu-id="0eb17-131">**Usage->Origin**</span></span>|<span data-ttu-id="0eb17-132">This method traces the item starting from where it was used to where it came from.</span><span class="sxs-lookup"><span data-stu-id="0eb17-132">This method traces the item starting from where it was used to where it came from.</span></span> <span data-ttu-id="0eb17-133">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the sales shipment line first, which you can then expand to see from which production order it came.</span><span class="sxs-lookup"><span data-stu-id="0eb17-133">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the sales shipment line first, which you can then expand to see from which production order it came.</span></span>|  
    |<span data-ttu-id="0eb17-134">**Origin->Usage**</span><span class="sxs-lookup"><span data-stu-id="0eb17-134">**Origin->Usage**</span></span>|<span data-ttu-id="0eb17-135">This method traces the item starting from where it came into inventory to where it was used.</span><span class="sxs-lookup"><span data-stu-id="0eb17-135">This method traces the item starting from where it came into inventory to where it was used.</span></span> <span data-ttu-id="0eb17-136">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the finished production order first, which you can then expand to see sale shipment lines where the item was used.</span><span class="sxs-lookup"><span data-stu-id="0eb17-136">For instance, if a manufactured item was sold to a customer, the **Item Tracing** page shows this with the finished production order first, which you can then expand to see sale shipment lines where the item was used.</span></span>|  

5.  <span data-ttu-id="0eb17-137">Choose the **Trace** action to run the trace.</span><span class="sxs-lookup"><span data-stu-id="0eb17-137">Choose the **Trace** action to run the trace.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0eb17-138">If you have received the same lot on more transactions, then the **Item Tracing** page may not show all transactions.</span><span class="sxs-lookup"><span data-stu-id="0eb17-138">If you have received the same lot on more transactions, then the **Item Tracing** page may not show all transactions.</span></span> <span data-ttu-id="0eb17-139">Only applied transactions are shown.</span><span class="sxs-lookup"><span data-stu-id="0eb17-139">Only applied transactions are shown.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0eb17-140">If additional transaction history under an item tracing line has already been traced by another line above it, then the **Already Traced** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="0eb17-140">If additional transaction history under an item tracing line has already been traced by another line above it, then the **Already Traced** check box is selected.</span></span> <span data-ttu-id="0eb17-141">To provide a simpler view, such underlying lines are not shown.</span><span class="sxs-lookup"><span data-stu-id="0eb17-141">To provide a simpler view, such underlying lines are not shown.</span></span>  
>   
>  <span data-ttu-id="0eb17-142">To find the item tracing lines where the transaction history has already been traced, choose the **Go to Already Traced** button.</span><span class="sxs-lookup"><span data-stu-id="0eb17-142">To find the item tracing lines where the transaction history has already been traced, choose the **Go to Already Traced** button.</span></span> <span data-ttu-id="0eb17-143">The item tracing line in question is selected, and all underlying lines are expanded.</span><span class="sxs-lookup"><span data-stu-id="0eb17-143">The item tracing line in question is selected, and all underlying lines are expanded.</span></span>  

## <a name="to-find-item-tracked-items-with-find-entries"></a><span data-ttu-id="0eb17-144">To find item-tracked items with Find Entries</span><span class="sxs-lookup"><span data-stu-id="0eb17-144">To find item-tracked items with Find Entries</span></span>  

1. <span data-ttu-id="0eb17-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="0eb17-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then select the related link.</span></span>  
2. <span data-ttu-id="0eb17-146">Choose **Actions** > **Find by** > **Find by Item Reference**.</span><span class="sxs-lookup"><span data-stu-id="0eb17-146">Choose **Actions** > **Find by** > **Find by Item Reference**.</span></span>
3. <span data-ttu-id="0eb17-147">In the **Serial No.** and **Lot No.** fields, enter the item tracking numbers that you want to trace.</span><span class="sxs-lookup"><span data-stu-id="0eb17-147">In the **Serial No.** and **Lot No.** fields, enter the item tracking numbers that you want to trace.</span></span>  
4. <span data-ttu-id="0eb17-148">Choose the **Find** action to find all instances of the serial or lot number in the database.</span><span class="sxs-lookup"><span data-stu-id="0eb17-148">Choose the **Find** action to find all instances of the serial or lot number in the database.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0eb17-149">See Also</span><span class="sxs-lookup"><span data-stu-id="0eb17-149">See Also</span></span>

[<span data-ttu-id="0eb17-150">Inventory</span><span class="sxs-lookup"><span data-stu-id="0eb17-150">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0eb17-151">Work with Serial, Lot, and Package Numbers</span><span class="sxs-lookup"><span data-stu-id="0eb17-151">Work with Serial, Lot, and Package Numbers</span></span>](inventory-how-work-item-tracking.md)  
[<span data-ttu-id="0eb17-152">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="0eb17-152">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)  
[<span data-ttu-id="0eb17-153">Design Details - Item Tracking and Reservations</span><span class="sxs-lookup"><span data-stu-id="0eb17-153">Design Details - Item Tracking and Reservations</span></span>](design-details-item-tracking-and-reservations.md)  
[<span data-ttu-id="0eb17-154">Reserve Items</span><span class="sxs-lookup"><span data-stu-id="0eb17-154">Reserve Items</span></span>](inventory-how-to-reserve-items.md)  
<span data-ttu-id="0eb17-155">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0eb17-155">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="0eb17-156">Walkthrough: Tracing Serial-Lot Numbers</span><span class="sxs-lookup"><span data-stu-id="0eb17-156">Walkthrough: Tracing Serial-Lot Numbers</span></span>](walkthrough-tracing-serial-lot-numbers.md)  
[<span data-ttu-id="0eb17-157">Find Entries</span><span class="sxs-lookup"><span data-stu-id="0eb17-157">Find Entries</span></span>](ui-find-entries.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]