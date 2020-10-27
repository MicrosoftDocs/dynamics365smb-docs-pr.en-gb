---
title: Correct or Cancel a Posted Sales Invoice | Microsoft Docs
description: Describes how to correct, undo, or cancel a posted sales invoice and apply a sales credit memo.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3803ce840569d1b1668db64879e68395ee6f3a65
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3926304"
---
# <a name="correct-or-cancel-unpaid-sales-invoices"></a><span data-ttu-id="fc6da-103">Correct or Cancel Unpaid Sales Invoices</span><span class="sxs-lookup"><span data-stu-id="fc6da-103">Correct or Cancel Unpaid Sales Invoices</span></span>

<span data-ttu-id="fc6da-104">You can correct or cancel a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-104">You can correct or cancel a posted sales invoice.</span></span> <span data-ttu-id="fc6da-105">This is useful if you make a mistake or if the customer requests a change.</span><span class="sxs-lookup"><span data-stu-id="fc6da-105">This is useful if you make a mistake or if the customer requests a change.</span></span>

> [!NOTE]  
> <span data-ttu-id="fc6da-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span><span class="sxs-lookup"><span data-stu-id="fc6da-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span></span> <span data-ttu-id="fc6da-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span><span class="sxs-lookup"><span data-stu-id="fc6da-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span></span> <span data-ttu-id="fc6da-108">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="fc6da-108">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>

<span data-ttu-id="fc6da-109">On the **Posted Sales Invoice** page, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span><span class="sxs-lookup"><span data-stu-id="fc6da-109">On the **Posted Sales Invoice** page, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span></span>

| <span data-ttu-id="fc6da-110">Action</span><span class="sxs-lookup"><span data-stu-id="fc6da-110">Action</span></span> | <span data-ttu-id="fc6da-111">Description</span><span class="sxs-lookup"><span data-stu-id="fc6da-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="fc6da-112">**Correct**</span><span class="sxs-lookup"><span data-stu-id="fc6da-112">**Correct**</span></span> |<span data-ttu-id="fc6da-113">The posted sales invoice is cancelled.</span><span class="sxs-lookup"><span data-stu-id="fc6da-113">The posted sales invoice is canceled.</span></span> <span data-ttu-id="fc6da-114">A new sales invoice with the same information is created.</span><span class="sxs-lookup"><span data-stu-id="fc6da-114">A new sales invoice with the same information is created.</span></span> <span data-ttu-id="fc6da-115">You can make the correction and then continue the sales process.</span><span class="sxs-lookup"><span data-stu-id="fc6da-115">You can make the correction and then continue the sales process.</span></span> <span data-ttu-id="fc6da-116">The new sales invoice has a different number than the initial sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-116">The new sales invoice has a different number than the initial sales invoice.</span></span> <span data-ttu-id="fc6da-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="fc6da-118">On the initial posted sales invoice, the Cancelled and Paid check boxes are selected.</span><span class="sxs-lookup"><span data-stu-id="fc6da-118">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |
| <span data-ttu-id="fc6da-119">**Cancel**</span><span class="sxs-lookup"><span data-stu-id="fc6da-119">**Cancel**</span></span> |<span data-ttu-id="fc6da-120">The posted sales invoice is cancelled.</span><span class="sxs-lookup"><span data-stu-id="fc6da-120">The posted sales invoice is canceled.</span></span> <span data-ttu-id="fc6da-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="fc6da-122">On the initial posted sales invoice, the Cancelled and Paid check boxes are selected.</span><span class="sxs-lookup"><span data-stu-id="fc6da-122">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |

<span data-ttu-id="fc6da-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="fc6da-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span></span> <span data-ttu-id="fc6da-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="fc6da-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span></span>  

> [!TIP]
> <span data-ttu-id="fc6da-125">If you have posted a prepayment invoice for a sales invoice that you then correct or cancel, you must correct or cancel the prepayment as well.</span><span class="sxs-lookup"><span data-stu-id="fc6da-125">If you have posted a prepayment invoice for a sales invoice that you then correct or cancel, you must correct or cancel the prepayment as well.</span></span> <span data-ttu-id="fc6da-126">For more information, see [Correct Prepayments](finance-how-to-correct-prepayments.md).</span><span class="sxs-lookup"><span data-stu-id="fc6da-126">For more information, see [Correct Prepayments](finance-how-to-correct-prepayments.md).</span></span>

## <a name="to-correct-a-posted-sales-invoice"></a><span data-ttu-id="fc6da-127">To correct a posted sales invoice</span><span class="sxs-lookup"><span data-stu-id="fc6da-127">To correct a posted sales invoice</span></span>

1. <span data-ttu-id="fc6da-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Invoices** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fc6da-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Invoices** , and then choose the related link.</span></span>  
2. <span data-ttu-id="fc6da-129">Select the posted sales invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="fc6da-129">Select the posted sales invoice that you want to correct.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="fc6da-130">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="fc6da-130">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="fc6da-131">On the **Posted Sales Invoice** page, choose the **Correct** action.</span><span class="sxs-lookup"><span data-stu-id="fc6da-131">On the **Posted Sales Invoice** page, choose the **Correct** action.</span></span>  
4. <span data-ttu-id="fc6da-132">A new sales invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="fc6da-132">A new sales invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="fc6da-133">The **Cancelled** field on the initial posted sales invoice is changed to **Yes** .</span><span class="sxs-lookup"><span data-stu-id="fc6da-133">The **Canceled** field on the initial posted sales invoice is changed to **Yes** .</span></span>

    <span data-ttu-id="fc6da-134">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-134">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span>
5. <span data-ttu-id="fc6da-135">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-135">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="to-cancel-a-posted-sales-invoice"></a><span data-ttu-id="fc6da-136">To cancel a posted sales invoice</span><span class="sxs-lookup"><span data-stu-id="fc6da-136">To cancel a posted sales invoice</span></span>

1. <span data-ttu-id="fc6da-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Invoices** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fc6da-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Invoices** , and then choose the related link.</span></span>  
2. <span data-ttu-id="fc6da-138">Select the posted sales invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="fc6da-138">Select the posted sales invoice that you want to cancel.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="fc6da-139">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="fc6da-139">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="fc6da-140">On the **Posted Sales Invoice** page, choose the **Cancel** action.</span><span class="sxs-lookup"><span data-stu-id="fc6da-140">On the **Posted Sales Invoice** page, choose the **Cancel** action.</span></span>

    <span data-ttu-id="fc6da-141">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-141">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="fc6da-142">The **Cancelled** field on the initial posted sales invoice is changed to **Yes** .</span><span class="sxs-lookup"><span data-stu-id="fc6da-142">The **Canceled** field on the initial posted sales invoice is changed to **Yes** .</span></span>
4. <span data-ttu-id="fc6da-143">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="fc6da-143">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

### <a name="partial-invoice-posting-also-supported"></a><span data-ttu-id="fc6da-144">Partial Invoice Posting also Supported</span><span class="sxs-lookup"><span data-stu-id="fc6da-144">Partial Invoice Posting also Supported</span></span>

<span data-ttu-id="fc6da-145">If the cancellation is related to a partial invoice posting, then the originating sales order line is updated to reflect the cancelled invoiced quantity.</span><span class="sxs-lookup"><span data-stu-id="fc6da-145">If the cancellation is related to a partial invoice posting, then the originating sales order line is updated to reflect the canceled invoiced quantity.</span></span> <span data-ttu-id="fc6da-146">The **Qty. to Invoice** and **Qty. Invoiced** fields on the related sales order line are reset to the values before the partial posting.</span><span class="sxs-lookup"><span data-stu-id="fc6da-146">The **Qty. to Invoice** and **Qty. Invoiced** fields on the related sales order line are reset to the values before the partial posting.</span></span>

## <a name="see-also"></a><span data-ttu-id="fc6da-147">See Also</span><span class="sxs-lookup"><span data-stu-id="fc6da-147">See Also</span></span>

[<span data-ttu-id="fc6da-148">Sales</span><span class="sxs-lookup"><span data-stu-id="fc6da-148">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="fc6da-149">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="fc6da-149">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="fc6da-150">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="fc6da-150">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="fc6da-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fc6da-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
