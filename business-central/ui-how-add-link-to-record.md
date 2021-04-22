---
title: Add Attachments, Links, and Notes on Records| Microsoft Docs
description: Attach a hyperlink to a document or website to a specific record, such as a customer or document.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3acc0113cb14170b84363ab40a803da8b7551c75
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771142"
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a><span data-ttu-id="e4bb1-103">Manage Attachments, Links, and Notes on Cards and Documents</span><span class="sxs-lookup"><span data-stu-id="e4bb1-103">Manage Attachments, Links, and Notes on Cards and Documents</span></span>

<span data-ttu-id="e4bb1-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span></span> <span data-ttu-id="e4bb1-105">For links and notes, you can also do this on the list page by first selecting the related line.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-105">For links and notes, you can also do this on the list page by first selecting the related line.</span></span>

<span data-ttu-id="e4bb1-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span></span> <span data-ttu-id="e4bb1-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span></span>

<span data-ttu-id="e4bb1-108">Attachments, links, and notes stay attached as the card or document is processed into other counties, such as from an ongoing sales order to a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span></span> <span data-ttu-id="e4bb1-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span></span>

> [!NOTE]
> <span data-ttu-id="e4bb1-110">When you partially ship and invoice a sales or purchase order, the attachment will only be attached to the final invoice of the order.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-110">When you partially ship and invoice a sales or purchase order, the attachment will only be attached to the final invoice of the order.</span></span> <span data-ttu-id="e4bb1-111">Similarly, when you invoice using the Deferrals feature, the attachment is attached to the G/L entries for the document but not for the deferral entries.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-111">Similarly, when you invoice using the Deferrals feature, the attachment is attached to the G/L entries for the document but not for the deferral entries.</span></span>
>
> <span data-ttu-id="e4bb1-112">If you delete an order before it is invoiced, the attachment is also removed.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-112">If you delete an order before it is invoiced, the attachment is also removed.</span></span> <span data-ttu-id="e4bb1-113">When you invoice purchase orders using the Get Receipt Lines action from a purchase invoice, the attachment on the purchase orders is not added to the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-113">When you invoice purchase orders using the Get Receipt Lines action from a purchase invoice, the attachment on the purchase orders is not added to the purchase invoice.</span></span>

## <a name="to-attach-a-file-to-a-purchase-invoice"></a><span data-ttu-id="e4bb1-114">To attach a file to a purchase invoice</span><span class="sxs-lookup"><span data-stu-id="e4bb1-114">To attach a file to a purchase invoice</span></span>
<span data-ttu-id="e4bb1-115">You can attach any type of file, containing text, image, or video, to a card or document.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-115">You can attach any type of file, containing text, image, or video, to a card or document.</span></span> <span data-ttu-id="e4bb1-116">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="e4bb1-116">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="e4bb1-117">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="e4bb1-117">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span></span>

<span data-ttu-id="e4bb1-118">The following procedure is based on a purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-118">The following procedure is based on a purchase invoice.</span></span> <span data-ttu-id="e4bb1-119">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-119">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="e4bb1-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4bb1-121">Open the sales order that you want to attach a file to.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-121">Open the sales order that you want to attach a file to.</span></span>
3. <span data-ttu-id="e4bb1-122">In the FactBox, open the **Attachments** tab.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-122">In the FactBox, open the **Attachments** tab.</span></span>
4. <span data-ttu-id="e4bb1-123">Choose the value behind the **Documents** field, such as "0".</span><span class="sxs-lookup"><span data-stu-id="e4bb1-123">Choose the value behind the **Documents** field, such as "0".</span></span>
5. <span data-ttu-id="e4bb1-124">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** action.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-124">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** action.</span></span>
5. <span data-ttu-id="e4bb1-125">Select a file from any location, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-125">Select a file from any location, and then choose the **Open** button.</span></span>

<span data-ttu-id="e4bb1-126">The file is now attached to the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-126">The file is now attached to the purchase invoice.</span></span>

## <a name="to-view-an-attached-file"></a><span data-ttu-id="e4bb1-127">To view an attached file</span><span class="sxs-lookup"><span data-stu-id="e4bb1-127">To view an attached file</span></span>
1. <span data-ttu-id="e4bb1-128">In the FactBox, open the **Attachments** tab.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-128">In the FactBox, open the **Attachments** tab.</span></span>
2. <span data-ttu-id="e4bb1-129">Choose the value behind the **Documents** field, such as "1".</span><span class="sxs-lookup"><span data-stu-id="e4bb1-129">Choose the value behind the **Documents** field, such as "1".</span></span>
3. <span data-ttu-id="e4bb1-130">On the **Attached Documents** page, choose the **Preview** action.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-130">On the **Attached Documents** page, choose the **Preview** action.</span></span>
4. <span data-ttu-id="e4bb1-131">Open the downloaded file.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-131">Open the downloaded file.</span></span>

## <a name="to-save-a-document-as-a-pdf-attachment"></a><span data-ttu-id="e4bb1-132">To save a document as a PDF attachment</span><span class="sxs-lookup"><span data-stu-id="e4bb1-132">To save a document as a PDF attachment</span></span>
<span data-ttu-id="e4bb1-133">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-133">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span></span> <span data-ttu-id="e4bb1-134">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-134">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span></span>

<span data-ttu-id="e4bb1-135">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-135">The following procedure is based on a sales order.</span></span> <span data-ttu-id="e4bb1-136">The steps are similar for all supported documents.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-136">The steps are similar for all supported documents.</span></span>

1. <span data-ttu-id="e4bb1-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4bb1-138">Select a sales order, and then choose the **Attach as PDF** action.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-138">Select a sales order, and then choose the **Attach as PDF** action.</span></span>

<span data-ttu-id="e4bb1-139">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-139">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span></span>

## <a name="to-add-a-link-from-an-item-card"></a><span data-ttu-id="e4bb1-140">To add a link from an item card</span><span class="sxs-lookup"><span data-stu-id="e4bb1-140">To add a link from an item card</span></span>
<span data-ttu-id="e4bb1-141">You can add a link from a card or document to any URL or path.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-141">You can add a link from a card or document to any URL or path.</span></span> <span data-ttu-id="e4bb1-142">This is useful, for example, when you want to link an item card with the supplier's item catalogue.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-142">This is useful, for example, when you want to link an item card with the supplier's item catalog.</span></span>

<span data-ttu-id="e4bb1-143">The following procedure is based on an item card.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-143">The following procedure is based on an item card.</span></span> <span data-ttu-id="e4bb1-144">The steps are similar for all other supported cards and documents.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-144">The steps are similar for all other supported cards and documents.</span></span>

1. <span data-ttu-id="e4bb1-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4bb1-146">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-146">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="e4bb1-147">In the **Links**, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-147">In the **Links**, choose the **+** icon.</span></span>
4. <span data-ttu-id="e4bb1-148">In the **Link Address** field, enter the link.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-148">In the **Link Address** field, enter the link.</span></span>

    <span data-ttu-id="e4bb1-149">The link must be a valid internet or intranet URL.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-149">The link must be a valid internet or intranet URL.</span></span>

5. <span data-ttu-id="e4bb1-150">In the **Description** field, enter any information about the link.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-150">In the **Description** field, enter any information about the link.</span></span>  
6. <span data-ttu-id="e4bb1-151">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-151">Choose the **OK** button.</span></span>

<span data-ttu-id="e4bb1-152">The link is now attached to the item card.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-152">The link is now attached to the item card.</span></span>  

## <a name="to-write-a-note-on-a-sales-order"></a><span data-ttu-id="e4bb1-153">To write a note on a sales order</span><span class="sxs-lookup"><span data-stu-id="e4bb1-153">To write a note on a sales order</span></span>
<span data-ttu-id="e4bb1-154">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-154">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span></span> <span data-ttu-id="e4bb1-155">You can include file links and URLs in notes.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-155">You can include file links and URLs in notes.</span></span>

> [!NOTE]
> <span data-ttu-id="e4bb1-156">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-156">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span></span> <span data-ttu-id="e4bb1-157">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="e4bb1-157">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>

<span data-ttu-id="e4bb1-158">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-158">The following procedure is based on a sales order.</span></span> <span data-ttu-id="e4bb1-159">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-159">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="e4bb1-160">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-160">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4bb1-161">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-161">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="e4bb1-162">In the **Notes** section, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-162">In the **Notes** section, choose the **+** icon.</span></span>
4. <span data-ttu-id="e4bb1-163">In the **Note** field, write any text, such as "This is an urgent order.".</span><span class="sxs-lookup"><span data-stu-id="e4bb1-163">In the **Note** field, write any text, such as "This is an urgent order.".</span></span>
5. <span data-ttu-id="e4bb1-164">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-164">Choose the **OK** button.</span></span>

<span data-ttu-id="e4bb1-165">The note is now attached to the sales order.</span><span class="sxs-lookup"><span data-stu-id="e4bb1-165">The note is now attached to the sales order.</span></span>

## <a name="see-also"></a><span data-ttu-id="e4bb1-166">See Also</span><span class="sxs-lookup"><span data-stu-id="e4bb1-166">See Also</span></span>  
<span data-ttu-id="e4bb1-167">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e4bb1-167">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="e4bb1-168">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="e4bb1-168">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="e4bb1-169">Setting Up Workflow Notifications</span><span class="sxs-lookup"><span data-stu-id="e4bb1-169">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]