---
title: How to Block Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c453a10f30d2a45f6d4641bda8b24ee3659b1a32
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3182307"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="e2167-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="e2167-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="e2167-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="e2167-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="e2167-105">The following table illustrates what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="e2167-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="e2167-106">Option</span><span class="sxs-lookup"><span data-stu-id="e2167-106">Option</span></span>|<span data-ttu-id="e2167-107">Description</span><span class="sxs-lookup"><span data-stu-id="e2167-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="e2167-108">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="e2167-108">**Sales Blocked**</span></span>|<span data-ttu-id="e2167-109">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="e2167-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="e2167-110">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="e2167-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="e2167-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="e2167-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="e2167-112">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="e2167-112">**Blocked**</span></span>|<span data-ttu-id="e2167-113">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="e2167-113">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="e2167-114">Blocked items can be returned.</span><span class="sxs-lookup"><span data-stu-id="e2167-114">Blocked items can be returned.</span></span> <span data-ttu-id="e2167-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span><span class="sxs-lookup"><span data-stu-id="e2167-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

<span data-ttu-id="e2167-116">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span><span class="sxs-lookup"><span data-stu-id="e2167-116">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span></span> <span data-ttu-id="e2167-117">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span><span class="sxs-lookup"><span data-stu-id="e2167-117">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="e2167-118">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="e2167-118">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="e2167-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e2167-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e2167-120">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="e2167-120">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="e2167-121">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="e2167-121">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="e2167-122">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="e2167-122">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="e2167-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e2167-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e2167-124">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="e2167-124">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="e2167-125">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="e2167-125">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="e2167-126">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="e2167-126">To block an item from being posted</span></span>
1. <span data-ttu-id="e2167-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e2167-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="e2167-128">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="e2167-128">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="e2167-129">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="e2167-129">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="e2167-130">See Also</span><span class="sxs-lookup"><span data-stu-id="e2167-130">See Also</span></span>  
[<span data-ttu-id="e2167-131">Register New Items</span><span class="sxs-lookup"><span data-stu-id="e2167-131">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="e2167-132">Inventory</span><span class="sxs-lookup"><span data-stu-id="e2167-132">Inventory</span></span>](inventory-manage-inventory.md)  
