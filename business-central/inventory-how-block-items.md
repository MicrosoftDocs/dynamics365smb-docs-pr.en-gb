---
title: How to Block Items from Sales or Purchasing
description: You can prevent an item from being being used, for example, on sales or purchase documents.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: fb80cecd119cf061b3102d94f586da4c103bd21c
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3784820"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="8e545-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="8e545-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="8e545-104">You can block an item from being entered on lines in sales or purchase documents, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="8e545-104">You can block an item from being entered on lines in sales or purchase documents, and you can block it from being posted in any transaction.</span></span> <span data-ttu-id="8e545-105">For example, this is useful when an item has a known defect.</span><span class="sxs-lookup"><span data-stu-id="8e545-105">For example, this is useful when an item has a known defect.</span></span> <span data-ttu-id="8e545-106">If someone chooses a blocked item on a sales or purchase document a message will inform them that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="8e545-106">If someone chooses a blocked item on a sales or purchase document a message will inform them that the item is blocked.</span></span>

<span data-ttu-id="8e545-107">The following table describes what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="8e545-107">The following table describes what occurs when items are blocked.</span></span>  

|<span data-ttu-id="8e545-108">Option</span><span class="sxs-lookup"><span data-stu-id="8e545-108">Option</span></span>|<span data-ttu-id="8e545-109">Description</span><span class="sxs-lookup"><span data-stu-id="8e545-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="8e545-110">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="8e545-110">**Sales Blocked**</span></span>|<span data-ttu-id="8e545-111">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="8e545-111">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="8e545-112">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="8e545-112">**Purchasing Blocked**</span></span>|<span data-ttu-id="8e545-113">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="8e545-113">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="8e545-114">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="8e545-114">**Blocked**</span></span>|<span data-ttu-id="8e545-115">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="8e545-115">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="8e545-116">Blocked items can be returned.</span><span class="sxs-lookup"><span data-stu-id="8e545-116">Blocked items can be returned.</span></span> <span data-ttu-id="8e545-117">This means that none of the above settings apply when the item is used on return orders and credit memos.</span><span class="sxs-lookup"><span data-stu-id="8e545-117">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

<span data-ttu-id="8e545-118">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span><span class="sxs-lookup"><span data-stu-id="8e545-118">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span></span> <span data-ttu-id="8e545-119">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span><span class="sxs-lookup"><span data-stu-id="8e545-119">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="8e545-120">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="8e545-120">To block an item from being entered on sales lines</span></span>  
1.  <span data-ttu-id="8e545-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8e545-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8e545-122">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="8e545-122">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="8e545-123">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="8e545-123">To block an item from being entered on purchase lines</span></span>  
1.  <span data-ttu-id="8e545-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8e545-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8e545-125">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="8e545-125">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="8e545-126">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="8e545-126">To block an item from being posted</span></span>
1. <span data-ttu-id="8e545-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8e545-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="8e545-128">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="8e545-128">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

## <a name="see-also"></a><span data-ttu-id="8e545-129">See Also</span><span class="sxs-lookup"><span data-stu-id="8e545-129">See Also</span></span>  
[<span data-ttu-id="8e545-130">Register New Items</span><span class="sxs-lookup"><span data-stu-id="8e545-130">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="8e545-131">Inventory</span><span class="sxs-lookup"><span data-stu-id="8e545-131">Inventory</span></span>](inventory-manage-inventory.md)  
