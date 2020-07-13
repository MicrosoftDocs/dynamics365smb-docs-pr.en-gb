---
title: How to Combine Receipts | Microsoft Docs
description: If you want to invoice more than one purchase receipt at a time, you can use the Combine Receipts function.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/02/2020
ms.author: sgroespe
ms.openlocfilehash: f5b3c47ab430b89c2f747f73bc427e045a902992
ms.sourcegitcommit: 506a433298fc3629231cfa98f64a2d1428094fde
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/03/2020
ms.locfileid: "3534678"
---
# <a name="combine-receipts-on-a-single-invoice"></a><span data-ttu-id="8c793-103">Combine Receipts on a Single Invoice</span><span class="sxs-lookup"><span data-stu-id="8c793-103">Combine Receipts on a Single Invoice</span></span>

<span data-ttu-id="8c793-104">If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.</span><span class="sxs-lookup"><span data-stu-id="8c793-104">If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.</span></span>  

<span data-ttu-id="8c793-105">Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted.</span><span class="sxs-lookup"><span data-stu-id="8c793-105">Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted.</span></span> <span data-ttu-id="8c793-106">In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.</span><span class="sxs-lookup"><span data-stu-id="8c793-106">In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.</span></span>  

<span data-ttu-id="8c793-107">When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines.</span><span class="sxs-lookup"><span data-stu-id="8c793-107">When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines.</span></span> <span data-ttu-id="8c793-108">The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity.</span><span class="sxs-lookup"><span data-stu-id="8c793-108">The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity.</span></span> <span data-ttu-id="8c793-109">However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.</span><span class="sxs-lookup"><span data-stu-id="8c793-109">However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.</span></span>  

> [!NOTE]
> <span data-ttu-id="8c793-110">The resulting purchase invoice cannot later be corrected or cancelled.</span><span class="sxs-lookup"><span data-stu-id="8c793-110">The resulting purchase invoice cannot later be corrected or canceled.</span></span> <span data-ttu-id="8c793-111">If you want to modify a purchase invoice that is created in this way, you must use purchase credit memos.</span><span class="sxs-lookup"><span data-stu-id="8c793-111">If you want to modify a purchase invoice that is created in this way, you must use purchase credit memos.</span></span> <span data-ttu-id="8c793-112">For more information, see [Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="8c793-112">For more information, see [Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).</span></span>

## <a name="to-combine-receipts"></a><span data-ttu-id="8c793-113">To combine receipts</span><span class="sxs-lookup"><span data-stu-id="8c793-113">To combine receipts</span></span>

1. <span data-ttu-id="8c793-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8c793-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8c793-115">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="8c793-115">Choose the **New** action.</span></span> <span data-ttu-id="8c793-116">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="8c793-116">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>  
3. <span data-ttu-id="8c793-117">On the **Lines** FastTab, choose the **Get Receipt Lines** action.</span><span class="sxs-lookup"><span data-stu-id="8c793-117">On the **Lines** FastTab, choose the **Get Receipt Lines** action.</span></span>  
4. <span data-ttu-id="8c793-118">Select multiple receipt lines that you want to include in the invoice.</span><span class="sxs-lookup"><span data-stu-id="8c793-118">Select multiple receipt lines that you want to include in the invoice.</span></span>  

    <span data-ttu-id="8c793-119">If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.</span><span class="sxs-lookup"><span data-stu-id="8c793-119">If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.</span></span>  
5. <span data-ttu-id="8c793-120">To post the invoice, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="8c793-120">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a><span data-ttu-id="8c793-121">To remove open purchase orders after combined receipt posting</span><span class="sxs-lookup"><span data-stu-id="8c793-121">To remove open purchase orders after combined receipt posting</span></span>

1. <span data-ttu-id="8c793-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.</span><span class="sxs-lookup"><span data-stu-id="8c793-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.</span></span>  
2. <span data-ttu-id="8c793-123">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="8c793-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="8c793-124">.</span><span class="sxs-lookup"><span data-stu-id="8c793-124">.</span></span>
3. <span data-ttu-id="8c793-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="8c793-125">Choose the **OK** button.</span></span>  

<span data-ttu-id="8c793-126">Alternatively, delete the individual orders manually.</span><span class="sxs-lookup"><span data-stu-id="8c793-126">Alternatively, delete the individual orders manually.</span></span>

<span data-ttu-id="8c793-127">Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.</span><span class="sxs-lookup"><span data-stu-id="8c793-127">Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="8c793-128">See Also</span><span class="sxs-lookup"><span data-stu-id="8c793-128">See Also</span></span>

[<span data-ttu-id="8c793-129">Purchasing</span><span class="sxs-lookup"><span data-stu-id="8c793-129">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="8c793-130">Correct or Cancel Unpaid Purchase Invoices</span><span class="sxs-lookup"><span data-stu-id="8c793-130">Correct or Cancel Unpaid Purchase Invoices</span></span>](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
<span data-ttu-id="8c793-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8c793-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
