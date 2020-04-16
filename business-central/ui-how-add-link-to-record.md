---
title: Add Attachments, Links, and Notes on Records| Microsoft Docs
description: Attach a hyperlink to a document or website to a specific record, such as a customer or document.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c5d9dcc46e05cef21961e20008227a1a35b737af
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3193892"
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a><span data-ttu-id="262ee-103">Manage Attachments, Links, and Notes on Cards and Documents</span><span class="sxs-lookup"><span data-stu-id="262ee-103">Manage Attachments, Links, and Notes on Cards and Documents</span></span>

<span data-ttu-id="262ee-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span><span class="sxs-lookup"><span data-stu-id="262ee-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span></span> <span data-ttu-id="262ee-105">For links and notes, you can also do this on the list page by first selecting the related line.</span><span class="sxs-lookup"><span data-stu-id="262ee-105">For links and notes, you can also do this on the list page by first selecting the related line.</span></span>

<span data-ttu-id="262ee-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="262ee-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span></span> <span data-ttu-id="262ee-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span><span class="sxs-lookup"><span data-stu-id="262ee-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span></span>

<span data-ttu-id="262ee-108">Attachments, links, and notes stay attached as the card or document is processed into other counties, such as from an ongoing sales order to a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="262ee-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span></span> <span data-ttu-id="262ee-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span><span class="sxs-lookup"><span data-stu-id="262ee-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span></span>

> [!NOTE]
> <span data-ttu-id="262ee-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span><span class="sxs-lookup"><span data-stu-id="262ee-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span></span> <span data-ttu-id="262ee-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span><span class="sxs-lookup"><span data-stu-id="262ee-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span></span>

## <a name="to-attach-a-file-to-a-purchase-invoice"></a><span data-ttu-id="262ee-112">To attach a file to a purchase invoice</span><span class="sxs-lookup"><span data-stu-id="262ee-112">To attach a file to a purchase invoice</span></span>
<span data-ttu-id="262ee-113">You can attach any type of file, containing text, image, or video, to a card or document.</span><span class="sxs-lookup"><span data-stu-id="262ee-113">You can attach any type of file, containing text, image, or video, to a card or document.</span></span> <span data-ttu-id="262ee-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="262ee-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="262ee-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="262ee-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span></span>

<span data-ttu-id="262ee-116">The following procedure is based on a purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="262ee-116">The following procedure is based on a purchase invoice.</span></span> <span data-ttu-id="262ee-117">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="262ee-117">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="262ee-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="262ee-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="262ee-119">Open the sales order that you want to attach a file to.</span><span class="sxs-lookup"><span data-stu-id="262ee-119">Open the sales order that you want to attach a file to.</span></span>
3. <span data-ttu-id="262ee-120">In the FactBox, open the **Attachments** tab.</span><span class="sxs-lookup"><span data-stu-id="262ee-120">In the FactBox, open the **Attachments** tab.</span></span>
4. <span data-ttu-id="262ee-121">Choose the value behind the **Documents** field, such as "0".</span><span class="sxs-lookup"><span data-stu-id="262ee-121">Choose the value behind the **Documents** field, such as "0".</span></span>
5. <span data-ttu-id="262ee-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** button.</span><span class="sxs-lookup"><span data-stu-id="262ee-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** button.</span></span>
5. <span data-ttu-id="262ee-123">Select a file from any location, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="262ee-123">Select a file from any location, and then choose the **Open** button.</span></span>

<span data-ttu-id="262ee-124">The file is now attached to the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="262ee-124">The file is now attached to the purchase invoice.</span></span>

## <a name="to-save-a-document-as-a-pdf-attachment"></a><span data-ttu-id="262ee-125">To save a document as a PDF attachment</span><span class="sxs-lookup"><span data-stu-id="262ee-125">To save a document as a PDF attachment</span></span>
<span data-ttu-id="262ee-126">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span><span class="sxs-lookup"><span data-stu-id="262ee-126">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span></span> <span data-ttu-id="262ee-127">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span><span class="sxs-lookup"><span data-stu-id="262ee-127">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span></span>

<span data-ttu-id="262ee-128">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="262ee-128">The following procedure is based on a sales order.</span></span> <span data-ttu-id="262ee-129">The steps are similar for all supported documents.</span><span class="sxs-lookup"><span data-stu-id="262ee-129">The steps are similar for all supported documents.</span></span>

1. <span data-ttu-id="262ee-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="262ee-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="262ee-131">Select a sales order, and then choose the **Attach as PDF** action.</span><span class="sxs-lookup"><span data-stu-id="262ee-131">Select a sales order, and then choose the **Attach as PDF** action.</span></span>

<span data-ttu-id="262ee-132">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="262ee-132">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span></span> 

## <a name="to-add-a-link-from-an-item-card"></a><span data-ttu-id="262ee-133">To add a link from an item card</span><span class="sxs-lookup"><span data-stu-id="262ee-133">To add a link from an item card</span></span>
<span data-ttu-id="262ee-134">You can add a link from a card or document to any URL or path.</span><span class="sxs-lookup"><span data-stu-id="262ee-134">You can add a link from a card or document to any URL or path.</span></span> <span data-ttu-id="262ee-135">This is useful, for example, when you want to link an item card with the supplier's item catalogue.</span><span class="sxs-lookup"><span data-stu-id="262ee-135">This is useful, for example, when you want to link an item card with the supplier's item catalog.</span></span>

<span data-ttu-id="262ee-136">The following procedure is based on an item card.</span><span class="sxs-lookup"><span data-stu-id="262ee-136">The following procedure is based on an item card.</span></span> <span data-ttu-id="262ee-137">The steps are similar for all other supported cards and documents.</span><span class="sxs-lookup"><span data-stu-id="262ee-137">The steps are similar for all other supported cards and documents.</span></span>

1. <span data-ttu-id="262ee-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="262ee-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="262ee-139">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="262ee-139">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="262ee-140">In the **Links**, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="262ee-140">In the **Links**, choose the **+** icon.</span></span>
4. <span data-ttu-id="262ee-141">In the **Link Address** field, enter the link.</span><span class="sxs-lookup"><span data-stu-id="262ee-141">In the **Link Address** field, enter the link.</span></span>

    <span data-ttu-id="262ee-142">The link must be a valid internet or intranet URL.</span><span class="sxs-lookup"><span data-stu-id="262ee-142">The link must be a valid internet or intranet URL.</span></span>

5. <span data-ttu-id="262ee-143">In the **Description** field, enter any information about the link.</span><span class="sxs-lookup"><span data-stu-id="262ee-143">In the **Description** field, enter any information about the link.</span></span>  
6. <span data-ttu-id="262ee-144">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="262ee-144">Choose the **OK** button.</span></span>

<span data-ttu-id="262ee-145">The link is now attached to the item card.</span><span class="sxs-lookup"><span data-stu-id="262ee-145">The link is now attached to the item card.</span></span>  

## <a name="to-write-a-note-on-a-sales-order"></a><span data-ttu-id="262ee-146">To write a note on a sales order</span><span class="sxs-lookup"><span data-stu-id="262ee-146">To write a note on a sales order</span></span>
<span data-ttu-id="262ee-147">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span><span class="sxs-lookup"><span data-stu-id="262ee-147">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span></span> <span data-ttu-id="262ee-148">You can include file links and URLs in notes.</span><span class="sxs-lookup"><span data-stu-id="262ee-148">You can include file links and URLs in notes.</span></span>

> [!NOTE]
> <span data-ttu-id="262ee-149">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span><span class="sxs-lookup"><span data-stu-id="262ee-149">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span></span> <span data-ttu-id="262ee-150">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="262ee-150">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>

<span data-ttu-id="262ee-151">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="262ee-151">The following procedure is based on a sales order.</span></span> <span data-ttu-id="262ee-152">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="262ee-152">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="262ee-153">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="262ee-153">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="262ee-154">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="262ee-154">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="262ee-155">In the **Notes** section, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="262ee-155">In the **Notes** section, choose the **+** icon.</span></span>
4. <span data-ttu-id="262ee-156">In the **Note** field, write any text, such as "This is an urgent order.".</span><span class="sxs-lookup"><span data-stu-id="262ee-156">In the **Note** field, write any text, such as "This is an urgent order.".</span></span>
5. <span data-ttu-id="262ee-157">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="262ee-157">Choose the **OK** button.</span></span>

<span data-ttu-id="262ee-158">The note is now attached to the sales order.</span><span class="sxs-lookup"><span data-stu-id="262ee-158">The note is now attached to the sales order.</span></span>

## <a name="see-also"></a><span data-ttu-id="262ee-159">See Also</span><span class="sxs-lookup"><span data-stu-id="262ee-159">See Also</span></span>  
<span data-ttu-id="262ee-160">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="262ee-160">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="262ee-161">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="262ee-161">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="262ee-162">Setting Up Workflow Notifications</span><span class="sxs-lookup"><span data-stu-id="262ee-162">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)  
