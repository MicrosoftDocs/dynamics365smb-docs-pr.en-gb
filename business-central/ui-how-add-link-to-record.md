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
ms.date: 01/13/2020
ms.author: sgroespe
ms.openlocfilehash: 84d9c0768a457fd13a73b3d70d2b8c329098fe82
ms.sourcegitcommit: ead69ebe5b29927876a4fb23afb6c066f8854591
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/14/2020
ms.locfileid: "2953287"
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a><span data-ttu-id="9622a-103">Manage Attachments, Links, and Notes on Cards and Documents</span><span class="sxs-lookup"><span data-stu-id="9622a-103">Manage Attachments, Links, and Notes on Cards and Documents</span></span>

<span data-ttu-id="9622a-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span><span class="sxs-lookup"><span data-stu-id="9622a-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span></span> <span data-ttu-id="9622a-105">For links and notes, you can also do this on the list page by first selecting the related line.</span><span class="sxs-lookup"><span data-stu-id="9622a-105">For links and notes, you can also do this on the list page by first selecting the related line.</span></span>

<span data-ttu-id="9622a-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="9622a-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span></span> <span data-ttu-id="9622a-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span><span class="sxs-lookup"><span data-stu-id="9622a-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span></span>

<span data-ttu-id="9622a-108">Attachments, links, and notes stay attached as the card or document is processed into other counties, such as from an ongoing sales order to a posted sales invoice.</span><span class="sxs-lookup"><span data-stu-id="9622a-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span></span> <span data-ttu-id="9622a-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span><span class="sxs-lookup"><span data-stu-id="9622a-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span></span>

> [!NOTE]
> <span data-ttu-id="9622a-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span><span class="sxs-lookup"><span data-stu-id="9622a-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span></span> <span data-ttu-id="9622a-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span><span class="sxs-lookup"><span data-stu-id="9622a-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span></span>

## <a name="to-attach-a-file-to-a-purchase-invoice"></a><span data-ttu-id="9622a-112">To attach a file to a purchase invoice</span><span class="sxs-lookup"><span data-stu-id="9622a-112">To attach a file to a purchase invoice</span></span>
<span data-ttu-id="9622a-113">You can attach any type of file, containing text, image, or video, to a card or document.</span><span class="sxs-lookup"><span data-stu-id="9622a-113">You can attach any type of file, containing text, image, or video, to a card or document.</span></span> <span data-ttu-id="9622a-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="9622a-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="9622a-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="9622a-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span></span>

<span data-ttu-id="9622a-116">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="9622a-116">The following procedure is based on a sales order.</span></span> <span data-ttu-id="9622a-117">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="9622a-117">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="9622a-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9622a-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="9622a-119">Open the sales order that you want to attach a file to.</span><span class="sxs-lookup"><span data-stu-id="9622a-119">Open the sales order that you want to attach a file to.</span></span>
3. <span data-ttu-id="9622a-120">In the FactBox, open the **Attachments** tab.</span><span class="sxs-lookup"><span data-stu-id="9622a-120">In the FactBox, open the **Attachments** tab.</span></span>
4. <span data-ttu-id="9622a-121">Choose the value behind the **Documents** field, such as "0".</span><span class="sxs-lookup"><span data-stu-id="9622a-121">Choose the value behind the **Documents** field, such as "0".</span></span>
5. <span data-ttu-id="9622a-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** button.</span><span class="sxs-lookup"><span data-stu-id="9622a-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** button.</span></span>
5. <span data-ttu-id="9622a-123">Select a file from any location, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="9622a-123">Select a file from any location, and then choose the **Open** button.</span></span>

<span data-ttu-id="9622a-124">The file is now attached to the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="9622a-124">The file is now attached to the purchase invoice.</span></span>

## <a name="to-add-a-link-from-an-item-card"></a><span data-ttu-id="9622a-125">To add a link from an item card</span><span class="sxs-lookup"><span data-stu-id="9622a-125">To add a link from an item card</span></span>
<span data-ttu-id="9622a-126">You can add a link from a card or document to any URL or path.</span><span class="sxs-lookup"><span data-stu-id="9622a-126">You can add a link from a card or document to any URL or path.</span></span> <span data-ttu-id="9622a-127">This is useful, for example, when you want to link an item card with the supplier's item catalogue.</span><span class="sxs-lookup"><span data-stu-id="9622a-127">This is useful, for example, when you want to link an item card with the supplier's item catalog.</span></span>

<span data-ttu-id="9622a-128">The following procedure is based on an item card.</span><span class="sxs-lookup"><span data-stu-id="9622a-128">The following procedure is based on an item card.</span></span> <span data-ttu-id="9622a-129">The steps are similar for all other supported cards and documents.</span><span class="sxs-lookup"><span data-stu-id="9622a-129">The steps are similar for all other supported cards and documents.</span></span>

1. <span data-ttu-id="9622a-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9622a-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="9622a-131">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="9622a-131">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="9622a-132">In the **Links**, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="9622a-132">In the **Links**, choose the **+** icon.</span></span>
4. <span data-ttu-id="9622a-133">In the **Link Address** field, enter the link.</span><span class="sxs-lookup"><span data-stu-id="9622a-133">In the **Link Address** field, enter the link.</span></span>

    <span data-ttu-id="9622a-134">The link must be a valid internet or intranet URL.</span><span class="sxs-lookup"><span data-stu-id="9622a-134">The link must be a valid internet or intranet URL.</span></span>

5. <span data-ttu-id="9622a-135">In the **Description** field, enter any information about the link.</span><span class="sxs-lookup"><span data-stu-id="9622a-135">In the **Description** field, enter any information about the link.</span></span>  
6. <span data-ttu-id="9622a-136">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9622a-136">Choose the **OK** button.</span></span>

<span data-ttu-id="9622a-137">The link is now attached to the item card.</span><span class="sxs-lookup"><span data-stu-id="9622a-137">The link is now attached to the item card.</span></span>  

## <a name="to-write-a-note-on-a-sales-order"></a><span data-ttu-id="9622a-138">To write a note on a sales order</span><span class="sxs-lookup"><span data-stu-id="9622a-138">To write a note on a sales order</span></span>
<span data-ttu-id="9622a-139">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span><span class="sxs-lookup"><span data-stu-id="9622a-139">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span></span> <span data-ttu-id="9622a-140">You can include file links and URLs in notes.</span><span class="sxs-lookup"><span data-stu-id="9622a-140">You can include file links and URLs in notes.</span></span>

> [!NOTE]
> <span data-ttu-id="9622a-141">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span><span class="sxs-lookup"><span data-stu-id="9622a-141">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span></span> <span data-ttu-id="9622a-142">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="9622a-142">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>

<span data-ttu-id="9622a-143">The following procedure is based on a sales order.</span><span class="sxs-lookup"><span data-stu-id="9622a-143">The following procedure is based on a sales order.</span></span> <span data-ttu-id="9622a-144">The steps are similar for all other supported documents and cards.</span><span class="sxs-lookup"><span data-stu-id="9622a-144">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="9622a-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9622a-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="9622a-146">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span><span class="sxs-lookup"><span data-stu-id="9622a-146">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="9622a-147">In the **Notes** section, choose the **+** icon.</span><span class="sxs-lookup"><span data-stu-id="9622a-147">In the **Notes** section, choose the **+** icon.</span></span>
4. <span data-ttu-id="9622a-148">In the **Note** field, write any text, such as "This is an urgent order.".</span><span class="sxs-lookup"><span data-stu-id="9622a-148">In the **Note** field, write any text, such as "This is an urgent order.".</span></span>
5. <span data-ttu-id="9622a-149">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9622a-149">Choose the **OK** button.</span></span>

<span data-ttu-id="9622a-150">The note is now attached to the sales order.</span><span class="sxs-lookup"><span data-stu-id="9622a-150">The note is now attached to the sales order.</span></span>

## <a name="see-also"></a><span data-ttu-id="9622a-151">See Also</span><span class="sxs-lookup"><span data-stu-id="9622a-151">See Also</span></span>  
<span data-ttu-id="9622a-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9622a-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="9622a-153">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="9622a-153">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="9622a-154">Setting Up Workflow Notifications</span><span class="sxs-lookup"><span data-stu-id="9622a-154">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)  
