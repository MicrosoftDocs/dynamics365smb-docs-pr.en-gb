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
ms.author: sgroespe
ms.openlocfilehash: 467b43b14f1905018c2a26a06c15abc5a0a17e99
ms.sourcegitcommit: 4545bb597dd9dc4c563b30af762977ee1d815497
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/29/2020
ms.locfileid: "3410651"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="0d105-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="0d105-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="0d105-104">You can block an item from being entered on lines in sales or purchase documents, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="0d105-104">You can block an item from being entered on lines in sales or purchase documents, and you can block it from being posted in any transaction.</span></span> <span data-ttu-id="0d105-105">For example, this is useful when an item has a known defect.</span><span class="sxs-lookup"><span data-stu-id="0d105-105">For example, this is useful when an item has a known defect.</span></span> <span data-ttu-id="0d105-106">If someone chooses a blocked item on a sales or purchase document a message will inform them that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="0d105-106">If someone chooses a blocked item on a sales or purchase document a message will inform them that the item is blocked.</span></span>

<span data-ttu-id="0d105-107">The following table describes what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="0d105-107">The following table describes what occurs when items are blocked.</span></span>  

|<span data-ttu-id="0d105-108">Option</span><span class="sxs-lookup"><span data-stu-id="0d105-108">Option</span></span>|<span data-ttu-id="0d105-109">Description</span><span class="sxs-lookup"><span data-stu-id="0d105-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="0d105-110">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="0d105-110">**Sales Blocked**</span></span>|<span data-ttu-id="0d105-111">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="0d105-111">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="0d105-112">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="0d105-112">**Purchasing Blocked**</span></span>|<span data-ttu-id="0d105-113">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="0d105-113">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="0d105-114">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="0d105-114">**Blocked**</span></span>|<span data-ttu-id="0d105-115">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="0d105-115">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="0d105-116">Blocked items can be returned.</span><span class="sxs-lookup"><span data-stu-id="0d105-116">Blocked items can be returned.</span></span> <span data-ttu-id="0d105-117">This means that none of the above settings apply when the item is used on return orders and credit memos.</span><span class="sxs-lookup"><span data-stu-id="0d105-117">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

<span data-ttu-id="0d105-118">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span><span class="sxs-lookup"><span data-stu-id="0d105-118">When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked.</span></span> <span data-ttu-id="0d105-119">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span><span class="sxs-lookup"><span data-stu-id="0d105-119">The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="0d105-120">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="0d105-120">To block an item from being entered on sales lines</span></span>  
1.  <span data-ttu-id="0d105-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d105-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0d105-122">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="0d105-122">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="0d105-123">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="0d105-123">To block an item from being entered on purchase lines</span></span>  
1.  <span data-ttu-id="0d105-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d105-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0d105-125">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="0d105-125">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="0d105-126">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="0d105-126">To block an item from being posted</span></span>
1. <span data-ttu-id="0d105-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d105-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="0d105-128">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="0d105-128">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d105-129">See Also</span><span class="sxs-lookup"><span data-stu-id="0d105-129">See Also</span></span>  
[<span data-ttu-id="0d105-130">Register New Items</span><span class="sxs-lookup"><span data-stu-id="0d105-130">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="0d105-131">Inventory</span><span class="sxs-lookup"><span data-stu-id="0d105-131">Inventory</span></span>](inventory-manage-inventory.md)  
