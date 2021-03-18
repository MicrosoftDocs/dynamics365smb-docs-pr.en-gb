---
title: Undo a Posting by Posting a Reversing Entry| Microsoft Docs
description: If you have made an erroneous posting in the general journal, then you can use the Reverse Transaction function to undo the posting with a correct audit trail.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fc74ce4f1496e106e9f6419ceedb0885bba75525
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5381374"
---
# <a name="reverse-journal-postings-and-undo-receiptsshipments"></a><span data-ttu-id="8d704-103">Reverse Journal Postings and Undo Receipts/Shipments</span><span class="sxs-lookup"><span data-stu-id="8d704-103">Reverse Journal Postings and Undo Receipts/Shipments</span></span>
<span data-ttu-id="8d704-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span><span class="sxs-lookup"><span data-stu-id="8d704-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="8d704-105">After reversing an entry, you must make the correct entry.</span><span class="sxs-lookup"><span data-stu-id="8d704-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="8d704-106">You can only reverse entries that are posted from a general journal line.</span><span class="sxs-lookup"><span data-stu-id="8d704-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="8d704-107">An entry can only be reversed once.</span><span class="sxs-lookup"><span data-stu-id="8d704-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="8d704-108">To undo a receipt or shipment posting, before they are posted as invoiced, you can use the **Undo** function on the posted document.</span><span class="sxs-lookup"><span data-stu-id="8d704-108">To undo a receipt or shipment posting, before they are posted as invoiced, you can use the **Undo** function on the posted document.</span></span> <span data-ttu-id="8d704-109">You can undo quantities of type **Item** and **Resource**.</span><span class="sxs-lookup"><span data-stu-id="8d704-109">You can undo quantities of type **Item** and **Resource**.</span></span>

<span data-ttu-id="8d704-110">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items, and posted it as received but not invoiced, then you can undo the posting.</span><span class="sxs-lookup"><span data-stu-id="8d704-110">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items, and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="8d704-111">If you have made an incorrect positive quantity posting, such as a sales shipment or a purchase return shipment with the wrong number of items, and posted it as shipped but not invoiced, then you can undo the posting.</span><span class="sxs-lookup"><span data-stu-id="8d704-111">If you have made an incorrect positive quantity posting, such as a sales shipment or a purchase return shipment with the wrong number of items, and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="8d704-112">To reverse the journal posting of a general ledger entry</span><span class="sxs-lookup"><span data-stu-id="8d704-112">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="8d704-113">You can reverse entries from all **Ledger Entries** pages.</span><span class="sxs-lookup"><span data-stu-id="8d704-113">You can reverse entries from all **Ledger Entries** pages.</span></span> <span data-ttu-id="8d704-114">The following procedure is based on the **General Ledger Entries** page.</span><span class="sxs-lookup"><span data-stu-id="8d704-114">The following procedure is based on the **General Ledger Entries** page.</span></span>
1. <span data-ttu-id="8d704-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Entries**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8d704-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="8d704-116">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span><span class="sxs-lookup"><span data-stu-id="8d704-116">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="8d704-117">Note that is must originate from a journal posting.</span><span class="sxs-lookup"><span data-stu-id="8d704-117">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="8d704-118">On the **Reverse Transaction Entries** page, choose the **Reverse** action.</span><span class="sxs-lookup"><span data-stu-id="8d704-118">On the **Reverse Transaction Entries** page, choose the **Reverse** action.</span></span>
4. <span data-ttu-id="8d704-119">Choose the **Yes** button on the confirmation message.</span><span class="sxs-lookup"><span data-stu-id="8d704-119">Choose the **Yes** button on the confirmation message.</span></span>

> [!NOTE]
> <span data-ttu-id="8d704-120">You cannot reverse entries that have been posted with information from a job, or which have realised gains and losses within the same transaction.</span><span class="sxs-lookup"><span data-stu-id="8d704-120">You cannot reverse entries that have been posted with information from a job, or which have realized gains and losses within the same transaction.</span></span>

## <a name="to-post-a-negative-entry"></a><span data-ttu-id="8d704-121">To post a negative entry</span><span class="sxs-lookup"><span data-stu-id="8d704-121">To post a negative entry</span></span>  
<span data-ttu-id="8d704-122">You can use the **Correction** field to post a negative debit instead of a credit, or to post a negative credit instead of a debit on an account.</span><span class="sxs-lookup"><span data-stu-id="8d704-122">You can use the **Correction** field to post a negative debit instead of a credit, or to post a negative credit instead of a debit on an account.</span></span> <span data-ttu-id="8d704-123">To meet legal requirements, this field is visible by default in all journals.</span><span class="sxs-lookup"><span data-stu-id="8d704-123">To meet legal requirements, this field is visible by default in all journals.</span></span> <span data-ttu-id="8d704-124">The **Debit Amount** and **Credit Amount** fields include both the original entry, and the corrected entry.</span><span class="sxs-lookup"><span data-stu-id="8d704-124">The **Debit Amount** and **Credit Amount** fields include both the original entry, and the corrected entry.</span></span> <span data-ttu-id="8d704-125">These fields have no effect on the account balance.</span><span class="sxs-lookup"><span data-stu-id="8d704-125">These fields have no effect on the account balance.</span></span>  

1.  <span data-ttu-id="8d704-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link</span><span class="sxs-lookup"><span data-stu-id="8d704-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link</span></span>  
2.  <span data-ttu-id="8d704-127">In the **Batch Name** field, select the required batch name.</span><span class="sxs-lookup"><span data-stu-id="8d704-127">In the **Batch Name** field, select the required batch name.</span></span>  
3.  <span data-ttu-id="8d704-128">Enter information into the relevant fields.</span><span class="sxs-lookup"><span data-stu-id="8d704-128">Enter information into the relevant fields.</span></span>  
4.  <span data-ttu-id="8d704-129">In the journal line that you want to activate for negative entries, select the **Correction** check box.</span><span class="sxs-lookup"><span data-stu-id="8d704-129">In the journal line that you want to activate for negative entries, select the **Correction** check box.</span></span>  
5.  <span data-ttu-id="8d704-130">To post the journal, choose the **Post** action, and then choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="8d704-130">To post the journal, choose the **Post** action, and then choose the **Yes** button.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="8d704-131">To undo a quantity posting on a posted purchase receipt</span><span class="sxs-lookup"><span data-stu-id="8d704-131">To undo a quantity posting on a posted purchase receipt</span></span>  
<span data-ttu-id="8d704-132">The following described how to undo a posted receipt of items or resources.</span><span class="sxs-lookup"><span data-stu-id="8d704-132">The following described how to undo a posted receipt of items or resources.</span></span> <span data-ttu-id="8d704-133">The steps are similar for posted shipments.</span><span class="sxs-lookup"><span data-stu-id="8d704-133">The steps are similar for posted shipments.</span></span>

1.  <span data-ttu-id="8d704-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8d704-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8d704-135">Open the posted receipt that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="8d704-135">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="8d704-136">Select the line or lines that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="8d704-136">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="8d704-137">Choose **Undo Receipt** action.</span><span class="sxs-lookup"><span data-stu-id="8d704-137">Choose **Undo Receipt** action.</span></span>

<span data-ttu-id="8d704-138">A corrective line is inserted under the selected receipt line.</span><span class="sxs-lookup"><span data-stu-id="8d704-138">A corrective line is inserted under the selected receipt line.</span></span> <span data-ttu-id="8d704-139">If the quantity was received in a warehouse receipt, then a corrective line is inserted on the posted warehouse receipt.</span><span class="sxs-lookup"><span data-stu-id="8d704-139">If the quantity was received in a warehouse receipt, then a corrective line is inserted on the posted warehouse receipt.</span></span>  

<span data-ttu-id="8d704-140">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span><span class="sxs-lookup"><span data-stu-id="8d704-140">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="8d704-141">To undo and then redo a quantity posting on a posted return shipment</span><span class="sxs-lookup"><span data-stu-id="8d704-141">To undo and then redo a quantity posting on a posted return shipment</span></span>
<span data-ttu-id="8d704-142">The following describes how to undo a posted return shipment of items or resources and then repost the purchase return with a new quantity.</span><span class="sxs-lookup"><span data-stu-id="8d704-142">The following describes how to undo a posted return shipment of items or resources and then repost the purchase return with a new quantity.</span></span> <span data-ttu-id="8d704-143">The steps are similar for posted return receipts.</span><span class="sxs-lookup"><span data-stu-id="8d704-143">The steps are similar for posted return receipts.</span></span>

1.  <span data-ttu-id="8d704-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Return Shipments**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8d704-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8d704-145">Open the posted return shipment that you want to undo.</span><span class="sxs-lookup"><span data-stu-id="8d704-145">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="8d704-146">Select the line or lines you want to undo.</span><span class="sxs-lookup"><span data-stu-id="8d704-146">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="8d704-147">Choose the **Undo Return Shipment** action.</span><span class="sxs-lookup"><span data-stu-id="8d704-147">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="8d704-148">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span><span class="sxs-lookup"><span data-stu-id="8d704-148">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="8d704-149">Now go back to the purchase return order to redo the posting.</span><span class="sxs-lookup"><span data-stu-id="8d704-149">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="8d704-150">On the **Posted Return Shipment** page, take a note of the number in the **Return Order No.**</span><span class="sxs-lookup"><span data-stu-id="8d704-150">On the **Posted Return Shipment** page, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="8d704-151">field.</span><span class="sxs-lookup"><span data-stu-id="8d704-151">field.</span></span>  
6.  <span data-ttu-id="8d704-152">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Return Orders**, and then select the related link.</span><span class="sxs-lookup"><span data-stu-id="8d704-152">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Return Orders**, and then select the related link.</span></span>  
7.  <span data-ttu-id="8d704-153">Open the return order in question, and then choose the **Reopen** action.</span><span class="sxs-lookup"><span data-stu-id="8d704-153">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="8d704-154">Correct the entry in the **Quantity** field and post the purchase return order again.</span><span class="sxs-lookup"><span data-stu-id="8d704-154">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8d704-155">See Also</span><span class="sxs-lookup"><span data-stu-id="8d704-155">See Also</span></span>
[<span data-ttu-id="8d704-156">Undo Assembly Posting</span><span class="sxs-lookup"><span data-stu-id="8d704-156">Undo Assembly Posting</span></span>](assembly-how-to-undo-assembly-posting.md)  
[<span data-ttu-id="8d704-157">Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="8d704-157">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="8d704-158">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="8d704-158">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="8d704-159">Finance</span><span class="sxs-lookup"><span data-stu-id="8d704-159">Finance</span></span>](finance.md)  
<span data-ttu-id="8d704-160">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8d704-160">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]