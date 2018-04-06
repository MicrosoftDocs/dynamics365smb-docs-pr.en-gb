---
title: Undo a Posting by Posting a Reversing Entry| Microsoft Docs
description: If you have made an erroneous posting in the general journal, then you can use the Reverse Transaction function to undo the posting with a correct audit trail.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 66fcd6282f02d5789b12b79467ec177817422c5c
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="reverse-postings"></a><span data-ttu-id="de3a2-103">Reverse Postings</span><span class="sxs-lookup"><span data-stu-id="de3a2-103">Reverse Postings</span></span>
<span data-ttu-id="de3a2-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span><span class="sxs-lookup"><span data-stu-id="de3a2-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="de3a2-105">After reversing an entry, you must make the correct entry.</span><span class="sxs-lookup"><span data-stu-id="de3a2-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="de3a2-106">You can only reverse entries that are posted from a general journal line.</span><span class="sxs-lookup"><span data-stu-id="de3a2-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="de3a2-107">An entry can only be reversed once.</span><span class="sxs-lookup"><span data-stu-id="de3a2-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="de3a2-108">For more information about posting from a general journal, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="de3a2-108">For more information about posting from a general journal, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="de3a2-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span><span class="sxs-lookup"><span data-stu-id="de3a2-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="de3a2-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span><span class="sxs-lookup"><span data-stu-id="de3a2-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="de3a2-111">To reverse the journal posting of a general ledger entry</span><span class="sxs-lookup"><span data-stu-id="de3a2-111">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="de3a2-112">You can reverse entries from all **Ledger Entries** windows.</span><span class="sxs-lookup"><span data-stu-id="de3a2-112">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="de3a2-113">The following procedure is based on the **General Ledger Entries** window.</span><span class="sxs-lookup"><span data-stu-id="de3a2-113">The following procedure is based on the **General Ledger Entries** window.</span></span>
1. <span data-ttu-id="de3a2-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="de3a2-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="de3a2-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span><span class="sxs-lookup"><span data-stu-id="de3a2-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="de3a2-116">Note that is must originate from a journal posting.</span><span class="sxs-lookup"><span data-stu-id="de3a2-116">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="de3a2-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span><span class="sxs-lookup"><span data-stu-id="de3a2-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="de3a2-118">Choose the **Yes** button on the confirmation message.</span><span class="sxs-lookup"><span data-stu-id="de3a2-118">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="de3a2-119">To undo a quantity posting on a posted purchase receipt</span><span class="sxs-lookup"><span data-stu-id="de3a2-119">To undo a quantity posting on a posted purchase receipt</span></span>  

1.  <span data-ttu-id="de3a2-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="de3a2-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="de3a2-121">Open the posted receipt that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="de3a2-121">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="de3a2-122">Select the line or lines that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="de3a2-122">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="de3a2-123">Choose **Undo Receipt** action.</span><span class="sxs-lookup"><span data-stu-id="de3a2-123">Choose **Undo Receipt** action.</span></span>

    <span data-ttu-id="de3a2-124">A corrective line is inserted under the selected receipt line.</span><span class="sxs-lookup"><span data-stu-id="de3a2-124">A corrective line is inserted under the selected receipt line.</span></span>  

    <span data-ttu-id="de3a2-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span><span class="sxs-lookup"><span data-stu-id="de3a2-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span></span>  

    <span data-ttu-id="de3a2-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span><span class="sxs-lookup"><span data-stu-id="de3a2-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="de3a2-127">To undo and then redo a quantity posting on a posted return shipment</span><span class="sxs-lookup"><span data-stu-id="de3a2-127">To undo and then redo a quantity posting on a posted return shipment</span></span>

1.  <span data-ttu-id="de3a2-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="de3a2-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="de3a2-129">Open the posted return shipment that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="de3a2-129">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="de3a2-130">Select the line or lines you want to undo.</span><span class="sxs-lookup"><span data-stu-id="de3a2-130">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="de3a2-131">Choose the **Undo Return Shipment** action.</span><span class="sxs-lookup"><span data-stu-id="de3a2-131">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="de3a2-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span><span class="sxs-lookup"><span data-stu-id="de3a2-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="de3a2-133">Now go back to the purchase return order to redo the posting.</span><span class="sxs-lookup"><span data-stu-id="de3a2-133">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="de3a2-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span><span class="sxs-lookup"><span data-stu-id="de3a2-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="de3a2-135">field.</span><span class="sxs-lookup"><span data-stu-id="de3a2-135">field.</span></span>  
6.  <span data-ttu-id="de3a2-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="de3a2-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then select the related link.</span></span>  
7.  <span data-ttu-id="de3a2-137">Open the return order in question, and then choose the **Reopen** action.</span><span class="sxs-lookup"><span data-stu-id="de3a2-137">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="de3a2-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span><span class="sxs-lookup"><span data-stu-id="de3a2-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="to-post-a-negative-entry"></a><span data-ttu-id="de3a2-139">To post a negative entry</span><span class="sxs-lookup"><span data-stu-id="de3a2-139">To post a negative entry</span></span>  
<span data-ttu-id="de3a2-140">You can use the **Correction** field to post a negative debit instead of a credit, or to post a negative credit instead of a debit on an account.</span><span class="sxs-lookup"><span data-stu-id="de3a2-140">You can use the **Correction** field to post a negative debit instead of a credit, or to post a negative credit instead of a debit on an account.</span></span> <span data-ttu-id="de3a2-141">To meet legal requirements, this field is visible by default in all journals.</span><span class="sxs-lookup"><span data-stu-id="de3a2-141">To meet legal requirements, this field is visible by default in all journals.</span></span> <span data-ttu-id="de3a2-142">The **Debit Amount** and **Credit Amount** fields include both the original entry, and the corrected entry.</span><span class="sxs-lookup"><span data-stu-id="de3a2-142">The **Debit Amount** and **Credit Amount** fields include both the original entry, and the corrected entry.</span></span> <span data-ttu-id="de3a2-143">These fields have no effect on the account balance.</span><span class="sxs-lookup"><span data-stu-id="de3a2-143">These fields have no effect on the account balance.</span></span>  

1.  <span data-ttu-id="de3a2-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link</span><span class="sxs-lookup"><span data-stu-id="de3a2-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link</span></span>  
2.  <span data-ttu-id="de3a2-145">In the **Batch Name** field, select the required batch name.</span><span class="sxs-lookup"><span data-stu-id="de3a2-145">In the **Batch Name** field, select the required batch name.</span></span>  
3.  <span data-ttu-id="de3a2-146">Enter information into the relevant fields.</span><span class="sxs-lookup"><span data-stu-id="de3a2-146">Enter information into the relevant fields.</span></span>  
4.  <span data-ttu-id="de3a2-147">In the journal line that you want to activate for negative entries, select the **Correction** check box.</span><span class="sxs-lookup"><span data-stu-id="de3a2-147">In the journal line that you want to activate for negative entries, select the **Correction** check box.</span></span>  
5.  <span data-ttu-id="de3a2-148">To post the journal, choose the **Post** action, and then choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="de3a2-148">To post the journal, choose the **Post** action, and then choose the **Yes** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="de3a2-149">See Also</span><span class="sxs-lookup"><span data-stu-id="de3a2-149">See Also</span></span>
[<span data-ttu-id="de3a2-150">Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="de3a2-150">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="de3a2-151">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="de3a2-151">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="de3a2-152">Finance</span><span class="sxs-lookup"><span data-stu-id="de3a2-152">Finance</span></span>](finance.md)  
<span data-ttu-id="de3a2-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="de3a2-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

