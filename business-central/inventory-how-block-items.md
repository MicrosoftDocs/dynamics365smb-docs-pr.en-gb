---
title: How to Block Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 8c98e4b893783c795a49e05ab04dc70b03161c6a
ms.sourcegitcommit: bf5f89dfaf5ad9f8f9902941cf3dac3e9f3553e5
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/22/2019
ms.locfileid: "1594264"
---
# <a name="block-items-from-sales-or-purchasing"></a><span data-ttu-id="ed6e2-103">Block Items from Sales or Purchasing</span><span class="sxs-lookup"><span data-stu-id="ed6e2-103">Block Items from Sales or Purchasing</span></span>
<span data-ttu-id="ed6e2-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-104">You can block an item from being entered on sales or purchase lines, and you can block it from being posted in any transaction.</span></span>  

<span data-ttu-id="ed6e2-105">The following table illustrates what occurs when items are blocked.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-105">The following table illustrates what occurs when items are blocked.</span></span>  

|<span data-ttu-id="ed6e2-106">Option</span><span class="sxs-lookup"><span data-stu-id="ed6e2-106">Option</span></span>|<span data-ttu-id="ed6e2-107">Description</span><span class="sxs-lookup"><span data-stu-id="ed6e2-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="ed6e2-108">**Sales Blocked**</span><span class="sxs-lookup"><span data-stu-id="ed6e2-108">**Sales Blocked**</span></span>|<span data-ttu-id="ed6e2-109">You cannot enter the item in a sales document or in a sales item journal.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-109">You cannot enter the item in a sales document or in a sales item journal.</span></span>|  
|<span data-ttu-id="ed6e2-110">**Purchasing Blocked**</span><span class="sxs-lookup"><span data-stu-id="ed6e2-110">**Purchasing Blocked**</span></span>|<span data-ttu-id="ed6e2-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-111">You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.</span></span>|  
|<span data-ttu-id="ed6e2-112">**Blocked**</span><span class="sxs-lookup"><span data-stu-id="ed6e2-112">**Blocked**</span></span>|<span data-ttu-id="ed6e2-113">You cannot use the item for any item transaction.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-113">You cannot use the item for any item transaction.</span></span>|  

> [!NOTE]
> <span data-ttu-id="ed6e2-114">Blocked items can be returned.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-114">Blocked items can be returned.</span></span> <span data-ttu-id="ed6e2-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-115">This means that none of the above settings apply when the item is used on return orders and credit memos.</span></span>

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a><span data-ttu-id="ed6e2-116">To block an item from being entered on sales lines</span><span class="sxs-lookup"><span data-stu-id="ed6e2-116">To block an item from being entered on sales lines</span></span>  

1.  <span data-ttu-id="ed6e2-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ed6e2-118">Select the item that you want to block, and then select the **Sales Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-118">Select the item that you want to block, and then select the **Sales Blocked** check box.</span></span>  

<span data-ttu-id="ed6e2-119">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-119">If you try to enter the item on a sales document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a><span data-ttu-id="ed6e2-120">To block an item from being entered on purchase lines</span><span class="sxs-lookup"><span data-stu-id="ed6e2-120">To block an item from being entered on purchase lines</span></span>  

1.  <span data-ttu-id="ed6e2-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ed6e2-122">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-122">Select the item that you want to block, and then select the **Purchasing Blocked** check box.</span></span>  

<span data-ttu-id="ed6e2-123">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-123">If you try to enter the item on a purchase document or journal line, you will now get an error message that the item is blocked.</span></span>

## <a name="to-block-an-item-from-being-posted"></a><span data-ttu-id="ed6e2-124">To block an item from being posted</span><span class="sxs-lookup"><span data-stu-id="ed6e2-124">To block an item from being posted</span></span>
1. <span data-ttu-id="ed6e2-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="ed6e2-126">Select the item that you want to block, and then select the **Blocked** check box.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-126">Select the item that you want to block, and then select the **Blocked** check box.</span></span>

<span data-ttu-id="ed6e2-127">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span><span class="sxs-lookup"><span data-stu-id="ed6e2-127">If you try to post any type of transaction for the item, you will now get an error message that the item is blocked.</span></span>

## <a name="see-also"></a><span data-ttu-id="ed6e2-128">See Also</span><span class="sxs-lookup"><span data-stu-id="ed6e2-128">See Also</span></span>  
[<span data-ttu-id="ed6e2-129">Register New Items</span><span class="sxs-lookup"><span data-stu-id="ed6e2-129">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="ed6e2-130">Inventory</span><span class="sxs-lookup"><span data-stu-id="ed6e2-130">Inventory</span></span>](inventory-manage-inventory.md)  
