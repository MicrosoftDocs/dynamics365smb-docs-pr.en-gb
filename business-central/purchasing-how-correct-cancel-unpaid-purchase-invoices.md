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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d6644b7df13c70143d239de68ec419bdd196bfe3
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3926929"
---
# <a name="correct-or-cancel-unpaid-purchase-invoices"></a><span data-ttu-id="bf69d-103">Correct or Cancel Unpaid Purchase Invoices</span><span class="sxs-lookup"><span data-stu-id="bf69d-103">Correct or Cancel Unpaid Purchase Invoices</span></span>

<span data-ttu-id="bf69d-104">You can correct or cancel a posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="bf69d-104">You can correct or cancel a posted purchase invoice.</span></span> <span data-ttu-id="bf69d-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span><span class="sxs-lookup"><span data-stu-id="bf69d-105">This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.</span></span>

<span data-ttu-id="bf69d-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span><span class="sxs-lookup"><span data-stu-id="bf69d-106">If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself.</span></span> <span data-ttu-id="bf69d-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span><span class="sxs-lookup"><span data-stu-id="bf69d-107">Instead, you must manually create a purchase credit memo to reverse the purchase, optionally managed with a purchase return order.</span></span> <span data-ttu-id="bf69d-108">The same applies if you want to modify a posted purchase invoice that was based on combined purchase receipts.</span><span class="sxs-lookup"><span data-stu-id="bf69d-108">The same applies if you want to modify a posted purchase invoice that was based on combined purchase receipts.</span></span> <span data-ttu-id="bf69d-109">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="bf69d-109">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="bf69d-110">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span><span class="sxs-lookup"><span data-stu-id="bf69d-110">On the **Posted Purchase Invoice** page, you can choose the **Correct** button or the **Cancel** button.</span></span> <span data-ttu-id="bf69d-111">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span><span class="sxs-lookup"><span data-stu-id="bf69d-111">When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted.</span></span> <span data-ttu-id="bf69d-112">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span><span class="sxs-lookup"><span data-stu-id="bf69d-112">This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail.</span></span> <span data-ttu-id="bf69d-113">In the following the use of **Correct** and **Cancel** is described.</span><span class="sxs-lookup"><span data-stu-id="bf69d-113">In the following the use of **Correct** and **Cancel** is described.</span></span>
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE4dhoc?rel=0]

## <a name="to-correct-a-posted-purchase-invoice"></a><span data-ttu-id="bf69d-114">To correct a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="bf69d-114">To correct a posted purchase invoice</span></span>
1. <span data-ttu-id="bf69d-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bf69d-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices** , and then choose the related link.</span></span>  
2. <span data-ttu-id="bf69d-116">Select the posted purchase invoice that you want to correct.</span><span class="sxs-lookup"><span data-stu-id="bf69d-116">Select the posted purchase invoice that you want to correct.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="bf69d-117">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span><span class="sxs-lookup"><span data-stu-id="bf69d-117">If the **Canceled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="bf69d-118">On the **Posted Purchase Invoice** page, choose **Correct** .</span><span class="sxs-lookup"><span data-stu-id="bf69d-118">On the **Posted Purchase Invoice** page, choose **Correct** .</span></span>

    <span data-ttu-id="bf69d-119">A new purchase invoice with the same information is created where you can make the correction.</span><span class="sxs-lookup"><span data-stu-id="bf69d-119">A new purchase invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="bf69d-120">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="bf69d-120">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span> <span data-ttu-id="bf69d-121">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes** .</span><span class="sxs-lookup"><span data-stu-id="bf69d-121">The **Canceled** field on the initial posted purchase invoice is changed to **Yes** .</span></span>

    <span data-ttu-id="bf69d-122">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="bf69d-122">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span>
4. <span data-ttu-id="bf69d-123">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="bf69d-123">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

## <a name="to-cancel-a-posted-purchase-invoice"></a><span data-ttu-id="bf69d-124">To cancel a posted purchase invoice</span><span class="sxs-lookup"><span data-stu-id="bf69d-124">To cancel a posted purchase invoice</span></span>
1. <span data-ttu-id="bf69d-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bf69d-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Invoices** , and then choose the related link.</span></span>  
2. <span data-ttu-id="bf69d-126">Select the posted purchase invoice that you want to cancel.</span><span class="sxs-lookup"><span data-stu-id="bf69d-126">Select the posted purchase invoice that you want to cancel.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="bf69d-127">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span><span class="sxs-lookup"><span data-stu-id="bf69d-127">If the **Canceled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="bf69d-128">On the **Posted Purchase Invoice** page, choose **Cancel** .</span><span class="sxs-lookup"><span data-stu-id="bf69d-128">On the **Posted Purchase Invoice** page, choose **Cancel** .</span></span>

    <span data-ttu-id="bf69d-129">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="bf69d-129">A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.</span></span> <span data-ttu-id="bf69d-130">The **Cancelled** field on the initial posted purchase invoice is changed to **Yes** .</span><span class="sxs-lookup"><span data-stu-id="bf69d-130">The **Canceled** field on the initial posted purchase invoice is changed to **Yes** .</span></span>
4. <span data-ttu-id="bf69d-131">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="bf69d-131">Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.</span></span>

### <a name="partial-invoice-posting-also-supported"></a><span data-ttu-id="bf69d-132">Partial Invoice Posting also Supported</span><span class="sxs-lookup"><span data-stu-id="bf69d-132">Partial Invoice Posting also Supported</span></span>
<span data-ttu-id="bf69d-133">If the cancellation is related to a partial invoice posting, then the originating purchase order line is updated to reflect the cancelled invoiced quantity.</span><span class="sxs-lookup"><span data-stu-id="bf69d-133">If the cancellation is related to a partial invoice posting, then the originating purchase order line is updated to reflect the canceled invoiced quantity.</span></span> <span data-ttu-id="bf69d-134">The **Qty. to Invoice** and **Qty. Invoiced** fields on the related purchase order line are reset to the values before the partial posting.</span><span class="sxs-lookup"><span data-stu-id="bf69d-134">The **Qty. to Invoice** and **Qty. Invoiced** fields on the related purchase order line are reset to the values before the partial posting.</span></span>

## <a name="see-also"></a><span data-ttu-id="bf69d-135">See Also</span><span class="sxs-lookup"><span data-stu-id="bf69d-135">See Also</span></span>
[<span data-ttu-id="bf69d-136">Purchasing</span><span class="sxs-lookup"><span data-stu-id="bf69d-136">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="bf69d-137">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="bf69d-137">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
<span data-ttu-id="bf69d-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bf69d-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
