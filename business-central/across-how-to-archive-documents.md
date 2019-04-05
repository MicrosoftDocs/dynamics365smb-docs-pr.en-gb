---
title: How to Archive Sales and Purchase Documents | Microsoft Docs
description: You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 02/14/2018
ms.author: sgroespe
ms.openlocfilehash: 2f05313d30aede255e4ef49065f0189d649ce93c
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "809538"
---
# <a name="archive-documents"></a><span data-ttu-id="b86f9-103">Archive Documents</span><span class="sxs-lookup"><span data-stu-id="b86f9-103">Archive Documents</span></span>
<span data-ttu-id="b86f9-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, for example because you want to save a copy of a document for reuse later.</span><span class="sxs-lookup"><span data-stu-id="b86f9-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, for example because you want to save a copy of a document for reuse later.</span></span> <span data-ttu-id="b86f9-105">You can archive a sales or purchase document several times, saving a different archived version each time.</span><span class="sxs-lookup"><span data-stu-id="b86f9-105">You can archive a sales or purchase document several times, saving a different archived version each time.</span></span>

<span data-ttu-id="b86f9-106">For archived documents where the original still exists and is not posted, you can use the **Restore** function to overwrite the original with the archived version of the document.</span><span class="sxs-lookup"><span data-stu-id="b86f9-106">For archived documents where the original still exists and is not posted, you can use the **Restore** function to overwrite the original with the archived version of the document.</span></span> <span data-ttu-id="b86f9-107">This is practical if you need to restore the contents of a document to an earlier state.</span><span class="sxs-lookup"><span data-stu-id="b86f9-107">This is practical if you need to restore the contents of a document to an earlier state.</span></span>

<span data-ttu-id="b86f9-108">For archived documents where the original is deleted, you can only reuse the content by copying the data, for example with the **Copy Document** function.</span><span class="sxs-lookup"><span data-stu-id="b86f9-108">For archived documents where the original is deleted, you can only reuse the content by copying the data, for example with the **Copy Document** function.</span></span>   

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="b86f9-109">To set up automatic document archiving</span><span class="sxs-lookup"><span data-stu-id="b86f9-109">To set up automatic document archiving</span></span>  
<span data-ttu-id="b86f9-110">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span><span class="sxs-lookup"><span data-stu-id="b86f9-110">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="b86f9-111">The following procedure describes how to set up automatic archiving of sales documents.</span><span class="sxs-lookup"><span data-stu-id="b86f9-111">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="b86f9-112">The steps are similar for purchase documents.</span><span class="sxs-lookup"><span data-stu-id="b86f9-112">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="b86f9-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b86f9-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="b86f9-114">On the **Sales & Receivables Setup** page, fill in the fields as follows.</span><span class="sxs-lookup"><span data-stu-id="b86f9-114">On the **Sales & Receivables Setup** page, fill in the fields as follows.</span></span>

|<span data-ttu-id="b86f9-115">Field</span><span class="sxs-lookup"><span data-stu-id="b86f9-115">Field</span></span>|<span data-ttu-id="b86f9-116">Description</span><span class="sxs-lookup"><span data-stu-id="b86f9-116">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="b86f9-117">**Archiving Sales Quotes**</span><span class="sxs-lookup"><span data-stu-id="b86f9-117">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="b86f9-118">**Never** to never archive sales quotes when they are deleted.</span><span class="sxs-lookup"><span data-stu-id="b86f9-118">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="b86f9-119">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span><span class="sxs-lookup"><span data-stu-id="b86f9-119">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="b86f9-120">**Always** to archive sales quotes automatically when they are deleted.</span><span class="sxs-lookup"><span data-stu-id="b86f9-120">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="b86f9-121">**Archiving Blanket Sales Orders**</span><span class="sxs-lookup"><span data-stu-id="b86f9-121">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="b86f9-122">Select to archive blanket sales orders automatically each time they are deleted.</span><span class="sxs-lookup"><span data-stu-id="b86f9-122">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="b86f9-123">**Arch. Orders and Ret. Orders**</span><span class="sxs-lookup"><span data-stu-id="b86f9-123">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="b86f9-124">Select to automatically archive sales orders each time they are deleted.</span><span class="sxs-lookup"><span data-stu-id="b86f9-124">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="b86f9-125">To archive a sales order</span><span class="sxs-lookup"><span data-stu-id="b86f9-125">To archive a sales order</span></span>
<span data-ttu-id="b86f9-126">The following procedure describes how to archive a sales order.</span><span class="sxs-lookup"><span data-stu-id="b86f9-126">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="b86f9-127">The steps are similar for all orders, blanket orders, return orders, and quotes.</span><span class="sxs-lookup"><span data-stu-id="b86f9-127">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="b86f9-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b86f9-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b86f9-129">Open a sales order that you want to archive.</span><span class="sxs-lookup"><span data-stu-id="b86f9-129">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="b86f9-130">Choose the **Archive Document** action.</span><span class="sxs-lookup"><span data-stu-id="b86f9-130">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="b86f9-131">The sales order is archived.</span><span class="sxs-lookup"><span data-stu-id="b86f9-131">The sales order is archived.</span></span> <span data-ttu-id="b86f9-132">You can view it on the **Archived Sales orders** page.</span><span class="sxs-lookup"><span data-stu-id="b86f9-132">You can view it on the **Archived Sales orders** page.</span></span>

## <a name="to-restore-a-non-posted-sales-order-from-the-archive"></a><span data-ttu-id="b86f9-133">To restore a non-posted sales order from the archive</span><span class="sxs-lookup"><span data-stu-id="b86f9-133">To restore a non-posted sales order from the archive</span></span>
<span data-ttu-id="b86f9-134">The following procedure describes how to bring the contents of an archived sales order back to the original sales order.</span><span class="sxs-lookup"><span data-stu-id="b86f9-134">The following procedure describes how to bring the contents of an archived sales order back to the original sales order.</span></span> <span data-ttu-id="b86f9-135">This is only possible when the original document has not been posted.</span><span class="sxs-lookup"><span data-stu-id="b86f9-135">This is only possible when the original document has not been posted.</span></span> <span data-ttu-id="b86f9-136">The steps are similar for all orders, blanket orders, return orders, and quotes.</span><span class="sxs-lookup"><span data-stu-id="b86f9-136">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1. <span data-ttu-id="b86f9-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b86f9-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="b86f9-138">Select the archived sales order, or version of it, that you want to restore, and then choose the **Restore** action.</span><span class="sxs-lookup"><span data-stu-id="b86f9-138">Select the archived sales order, or version of it, that you want to restore, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="b86f9-139">The contents of the original sales order is replaced with that of the selected archived version.</span><span class="sxs-lookup"><span data-stu-id="b86f9-139">The contents of the original sales order is replaced with that of the selected archived version.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="b86f9-140">To delete archived sales orders</span><span class="sxs-lookup"><span data-stu-id="b86f9-140">To delete archived sales orders</span></span>
<span data-ttu-id="b86f9-141">The following procedure describes how to delete archived sales orders.</span><span class="sxs-lookup"><span data-stu-id="b86f9-141">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="b86f9-142">The steps are similar for other archived sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="b86f9-142">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="b86f9-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b86f9-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b86f9-144">On the **Delete Archived Sales Order Versions** page, select the appropriate filters.</span><span class="sxs-lookup"><span data-stu-id="b86f9-144">On the **Delete Archived Sales Order Versions** page, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="b86f9-145">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b86f9-145">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="b86f9-146">See Also</span><span class="sxs-lookup"><span data-stu-id="b86f9-146">See Also</span></span>
[<span data-ttu-id="b86f9-147">Track Document Lines</span><span class="sxs-lookup"><span data-stu-id="b86f9-147">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="b86f9-148">Sales</span><span class="sxs-lookup"><span data-stu-id="b86f9-148">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="b86f9-149">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="b86f9-149">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="b86f9-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b86f9-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
