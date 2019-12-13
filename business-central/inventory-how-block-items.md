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
ms.date: 12/04/2019
ms.author: sgroespe
ms.openlocfilehash: 0218cf1b4982b9e8c5b5c2817590bc5ebd8f1941
ms.sourcegitcommit: b6e506a45a1cd632294bafa1c959746cc3a144f6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/06/2019
ms.locfileid: "2896068"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="83750-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="83750-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="83750-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="83750-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="83750-105">The following table illustrates what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="83750-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="83750-106">Option</span><span class="sxs-lookup"><span data-stu-id="83750-106">Option</span></span>|<span data-ttu-id="83750-107">Description</span><span class="sxs-lookup"><span data-stu-id="83750-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="83750-108">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="83750-108">**Sales Blocked**</span></span>|<span data-ttu-id="83750-109">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="83750-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="83750-110">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="83750-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="83750-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="83750-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="83750-112">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="83750-112">**Blocked**</span></span>|<span data-ttu-id="83750-113">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="83750-113">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="83750-114">Blocked items can be returned.</span><span class="sxs-lookup"><span data-stu-id="83750-114">Blocked items can be returned.</span></span> <span data-ttu-id="83750-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span><span class="sxs-lookup"><span data-stu-id="83750-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

<span data-ttu-id="83750-116">When you use the **Copy Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span><span class="sxs-lookup"><span data-stu-id="83750-116">When you use the **Copy Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span></span> <span data-ttu-id="83750-117">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span><span class="sxs-lookup"><span data-stu-id="83750-117">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="83750-118">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="83750-118">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="83750-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="83750-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="83750-120">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="83750-120">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="83750-121">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="83750-121">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="83750-122">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="83750-122">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="83750-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="83750-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="83750-124">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="83750-124">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="83750-125">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="83750-125">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="83750-126">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="83750-126">To block an item from being posted</span></span>
1. <span data-ttu-id="83750-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="83750-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="83750-128">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="83750-128">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="83750-129">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="83750-129">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="83750-130">See Also</span><span class="sxs-lookup"><span data-stu-id="83750-130">See Also</span></span>  
[<span data-ttu-id="83750-131">Register New Items</span><span class="sxs-lookup"><span data-stu-id="83750-131">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="83750-132">Inventory</span><span class="sxs-lookup"><span data-stu-id="83750-132">Inventory</span></span>](inventory-manage-inventory.md)  
