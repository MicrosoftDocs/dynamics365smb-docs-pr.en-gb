---
title: Amend or Cancel Unpaid Purchase Invoices | Microsoft Docs
description: Explains how to correct, cancel, or undo a posted purchase invoice and automatically create a purchase credit memo.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 3d0d1234a6459b153a436ed2dfe9a3a2f667ab89
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3192754"
---
# <a name="correct-or-cancel-unpaid-purchase-invoices"></a><span data-ttu-id="be5a4-103">Correct or Cancel Unpaid Purchase Invoices</span><span class="sxs-lookup"><span data-stu-id="be5a4-103">Correct or Cancel Unpaid Purchase Invoices</span></span>
<span data-ttu-id="be5a4-104">You can correct or cancel a posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="be5a4-104">You can correct or cancel a posted purchase invoice.</span></span> <span data-ttu-id="be5a4-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span><span class="sxs-lookup"><span data-stu-id="be5a4-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span></span>

<span data-ttu-id="be5a4-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span><span class="sxs-lookup"><span data-stu-id="be5a4-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span></span> <span data-ttu-id="be5a4-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span><span class="sxs-lookup"><span data-stu-id="be5a4-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span></span> <span data-ttu-id="be5a4-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="be5a4-108">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="be5a4-109">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span><span class="sxs-lookup"><span data-stu-id="be5a4-109">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span></span> <span data-ttu-id="be5a4-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="be5a4-110">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span></span> <span data-ttu-id="be5a4-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="be5a4-111">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span></span> <span data-ttu-id="be5a4-112">In the following the use of **Correct** and **Cancel** is described.</span><span class="sxs-lookup"><span data-stu-id="be5a4-112">In the following the use of **Correct** and **Cancel** is described.</span></span>
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE4dhoc?rel=0]

## <a name="to-correct-a-posted-purchase-invoice"></a><span data-ttu-id="be5a4-113">To correct a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="be5a4-113">To correct a posted purchase invoice</span></span>
1. <span data-ttu-id="be5a4-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="be5a4-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="be5a4-115">Select the posted purchase invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="be5a4-115">Select the posted purchase invoice that you want to correct.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="be5a4-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="be5a4-116">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="be5a4-117">On the **Posted Purchase Invoice** page, choose **Correct**.</span><span class="sxs-lookup"><span data-stu-id="be5a4-117">On the **Posted Purchase Invoice** page, choose **Correct**.</span></span>

    <span data-ttu-id="be5a4-118">A new purchase invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="be5a4-118">A new purchase invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="be5a4-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="be5a4-119">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span> <span data-ttu-id="be5a4-120">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="be5a4-120">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="be5a4-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="be5a4-121">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span>
4. <span data-ttu-id="be5a4-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="be5a4-122">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="to-cancel-a-posted-purchase-invoice"></a><span data-ttu-id="be5a4-123">To cancel a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="be5a4-123">To cancel a posted purchase invoice</span></span>
1. <span data-ttu-id="be5a4-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="be5a4-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="be5a4-125">Select the posted purchase invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="be5a4-125">Select the posted purchase invoice that you want to cancel.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="be5a4-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="be5a4-126">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="be5a4-127">On the **Posted Purchase Invoice** page, choose **Cancel**.</span><span class="sxs-lookup"><span data-stu-id="be5a4-127">On the **Posted Purchase Invoice** page, choose **Cancel**.</span></span>

    <span data-ttu-id="be5a4-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="be5a4-128">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span> <span data-ttu-id="be5a4-129">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.</span><span class="sxs-lookup"><span data-stu-id="be5a4-129">The **Canceled** field on the initial posted purchase invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="be5a4-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="be5a4-130">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

### <a name="partial-invoice-posting-also-supported"></a><span data-ttu-id="be5a4-131">Partial Invoice Posting also Supported</span><span class="sxs-lookup"><span data-stu-id="be5a4-131">Partial Invoice Posting also Supported</span></span>
<span data-ttu-id="be5a4-132">If the cancellation is related to a partial invoice posting, then the originating purchase order line is updated to reflect the cancelled invoiced quantity.</span><span class="sxs-lookup"><span data-stu-id="be5a4-132">If the cancellation is related to a partial invoice posting, then the originating purchase order line is updated to reflect the canceled invoiced quantity.</span></span> <span data-ttu-id="be5a4-133">The **Qty. to Invoice** and **Qty. Invoiced** fields on the related purchase order line are reset to the values before the partial posting.</span><span class="sxs-lookup"><span data-stu-id="be5a4-133">The **Qty. to Invoice** and **Qty. Invoiced** fields on the related purchase order line are reset to the values before the partial posting.</span></span>

## <a name="see-also"></a><span data-ttu-id="be5a4-134">See Also</span><span class="sxs-lookup"><span data-stu-id="be5a4-134">See Also</span></span>
[<span data-ttu-id="be5a4-135">Purchasing</span><span class="sxs-lookup"><span data-stu-id="be5a4-135">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="be5a4-136">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="be5a4-136">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="be5a4-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="be5a4-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
