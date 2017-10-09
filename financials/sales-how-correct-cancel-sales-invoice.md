---
title: Correct or Cancel a Posted Sales Invoice | Microsoft Docs
description: Describes how to correct, undo, or cancel a posted sales invoice and apply a sales credit memo.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 08/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 6de89bc0865fbe8617e33288b9c0c8fe7da802ef
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-correct-or-cancel-unpaid-sales-invoices"></a><span data-ttu-id="6a72d-103">How to: Correct or Cancel Unpaid Sales Invoices</span><span class="sxs-lookup"><span data-stu-id="6a72d-103">How to: Correct or Cancel Unpaid Sales Invoices</span></span>
<span data-ttu-id="6a72d-104">You can correct or cancel a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-104">You can correct or cancel a posted sales invoice.</span></span> <span data-ttu-id="6a72d-105">This is useful if you make a mistake or if the customer requests a change.</span><span class="sxs-lookup"><span data-stu-id="6a72d-105">This is useful if you make a mistake or if the customer requests a change.</span></span>

> [!NOTE]  
>   <span data-ttu-id="6a72d-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span><span class="sxs-lookup"><span data-stu-id="6a72d-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span></span> <span data-ttu-id="6a72d-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span><span class="sxs-lookup"><span data-stu-id="6a72d-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span></span> <span data-ttu-id="6a72d-108">For more information, see [How to: Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="6a72d-108">For more information, see [How to: Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>

<span data-ttu-id="6a72d-109">In the **Posted Sales Invoice** window, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span><span class="sxs-lookup"><span data-stu-id="6a72d-109">In the **Posted Sales Invoice** window, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span></span>

| <span data-ttu-id="6a72d-110">Action</span><span class="sxs-lookup"><span data-stu-id="6a72d-110">Action</span></span> | <span data-ttu-id="6a72d-111">Description</span><span class="sxs-lookup"><span data-stu-id="6a72d-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="6a72d-112">**Correct**</span><span class="sxs-lookup"><span data-stu-id="6a72d-112">**Correct**</span></span> |<span data-ttu-id="6a72d-113">The posted sales invoice is cancelled.</span><span class="sxs-lookup"><span data-stu-id="6a72d-113">The posted sales invoice is canceled.</span></span> <span data-ttu-id="6a72d-114">A new sales invoice with the same information is created.</span><span class="sxs-lookup"><span data-stu-id="6a72d-114">A new sales invoice with the same information is created.</span></span> <span data-ttu-id="6a72d-115">You can make the correction and then continue the sales process.</span><span class="sxs-lookup"><span data-stu-id="6a72d-115">You can make the correction and then continue the sales process.</span></span> <span data-ttu-id="6a72d-116">The new sales invoice has a different number than the initial sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-116">The new sales invoice has a different number than the initial sales invoice.</span></span> <span data-ttu-id="6a72d-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="6a72d-118">On the initial posted sales invoice, the Cancelled and Paid check boxes are selected.</span><span class="sxs-lookup"><span data-stu-id="6a72d-118">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |
| <span data-ttu-id="6a72d-119">**Cancel**</span><span class="sxs-lookup"><span data-stu-id="6a72d-119">**Cancel**</span></span> |<span data-ttu-id="6a72d-120">The posted sales invoice is cancelled.</span><span class="sxs-lookup"><span data-stu-id="6a72d-120">The posted sales invoice is canceled.</span></span> <span data-ttu-id="6a72d-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="6a72d-122">On the initial posted sales invoice, the Cancelled and Paid check boxes are selected.</span><span class="sxs-lookup"><span data-stu-id="6a72d-122">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |

<span data-ttu-id="6a72d-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="6a72d-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span></span> <span data-ttu-id="6a72d-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="6a72d-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span></span>

## <a name="to-correct-a-posted-sales-invoice"></a><span data-ttu-id="6a72d-125">To correct a posted sales invoice</span><span class="sxs-lookup"><span data-stu-id="6a72d-125">To correct a posted sales invoice</span></span>
1. <span data-ttu-id="6a72d-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6a72d-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6a72d-127">Select the posted sales invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="6a72d-127">Select the posted sales invoice that you want to correct.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="6a72d-128">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="6a72d-128">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="6a72d-129">In the **Posted Sales Invoice** window, choose the **Correct** action.</span><span class="sxs-lookup"><span data-stu-id="6a72d-129">In the **Posted Sales Invoice** window, choose the **Correct** action.</span></span>  
4. <span data-ttu-id="6a72d-130">A new sales invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="6a72d-130">A new sales invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="6a72d-131">The **Cancelled** field on the initial posted sales invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="6a72d-131">The **Canceled** field on the initial posted sales invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="6a72d-132">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-132">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span>
5. <span data-ttu-id="6a72d-133">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-133">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="to-cancel-a-posted-sales-invoice"></a><span data-ttu-id="6a72d-134">To cancel a posted sales invoice</span><span class="sxs-lookup"><span data-stu-id="6a72d-134">To cancel a posted sales invoice</span></span>
1. <span data-ttu-id="6a72d-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6a72d-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6a72d-136">Select the posted sales invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="6a72d-136">Select the posted sales invoice that you want to cancel.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="6a72d-137">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="6a72d-137">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="6a72d-138">In the **Posted Sales Invoice** window, choose the **Cancel** action.</span><span class="sxs-lookup"><span data-stu-id="6a72d-138">In the **Posted Sales Invoice** window, choose the **Cancel** action.</span></span>

    <span data-ttu-id="6a72d-139">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-139">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="6a72d-140">The **Cancelled** field on the initial posted sales invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="6a72d-140">The **Canceled** field on the initial posted sales invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="6a72d-141">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6a72d-141">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="6a72d-142">See Also</span><span class="sxs-lookup"><span data-stu-id="6a72d-142">See Also</span></span>
[<span data-ttu-id="6a72d-143">Sales</span><span class="sxs-lookup"><span data-stu-id="6a72d-143">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="6a72d-144">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="6a72d-144">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="6a72d-145">How to: Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="6a72d-145">How to: Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="6a72d-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6a72d-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

