---
title: Create Records of Incoming Documents| Microsoft Docs
description: You can create records of incoming documents, such as e-invoices, and manage OCR tasks, eCommerce, and document exchange.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: daca27c051c8bdefe9a0424bca4699446ee9c84f
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3188608"
---
# <a name="create-incoming-document-records"></a><span data-ttu-id="e4651-103">Create Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="e4651-103">Create Incoming Document Records</span></span>
<span data-ttu-id="e4651-104">On the **Incoming Documents** page, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="e4651-104">On the **Incoming Documents** page, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="e4651-105">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="e4651-105">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="e4651-106">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span><span class="sxs-lookup"><span data-stu-id="e4651-106">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span></span> <span data-ttu-id="e4651-107">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span><span class="sxs-lookup"><span data-stu-id="e4651-107">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="e4651-108">Before you can use the Incoming Documents feature, you must perform the required setup.</span><span class="sxs-lookup"><span data-stu-id="e4651-108">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="e4651-109">For more information, see [Set Up Incoming Documents](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="e4651-109">For more information, see [Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="e4651-110">To approve or reject an incoming document</span><span class="sxs-lookup"><span data-stu-id="e4651-110">To approve or reject an incoming document</span></span>
<span data-ttu-id="e4651-111">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span><span class="sxs-lookup"><span data-stu-id="e4651-111">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="e4651-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4651-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4651-113">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span><span class="sxs-lookup"><span data-stu-id="e4651-113">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="e4651-114">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span><span class="sxs-lookup"><span data-stu-id="e4651-114">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="e4651-115">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span><span class="sxs-lookup"><span data-stu-id="e4651-115">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="e4651-116">To create an incoming document record by taking a photo</span><span class="sxs-lookup"><span data-stu-id="e4651-116">To create an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="e4651-117">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span><span class="sxs-lookup"><span data-stu-id="e4651-117">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="e4651-118">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span><span class="sxs-lookup"><span data-stu-id="e4651-118">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="e4651-119">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span><span class="sxs-lookup"><span data-stu-id="e4651-119">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="e4651-120">On the **Incoming Documents** page, choose the ellipsis button, and then choose **Create from Camera**.</span><span class="sxs-lookup"><span data-stu-id="e4651-120">On the **Incoming Documents** page, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="e4651-121">The camera on the tablet or phone is activated.</span><span class="sxs-lookup"><span data-stu-id="e4651-121">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="e4651-122">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e4651-122">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

    <span data-ttu-id="e4651-123">A new incoming document record is created, with the image attached.</span><span class="sxs-lookup"><span data-stu-id="e4651-123">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="e4651-124">To attach an image to an incoming document record by taking a photo</span><span class="sxs-lookup"><span data-stu-id="e4651-124">To attach an image to an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="e4651-125">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span><span class="sxs-lookup"><span data-stu-id="e4651-125">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="e4651-126">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span><span class="sxs-lookup"><span data-stu-id="e4651-126">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="e4651-127">Open the card for an existing incoming document record.</span><span class="sxs-lookup"><span data-stu-id="e4651-127">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="e4651-128">On the **Incoming Document** page, choose the ellipsis button, and then choose **Attach Image from Camera**.</span><span class="sxs-lookup"><span data-stu-id="e4651-128">On the **Incoming Document** page, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="e4651-129">The camera on the tablet or phone is activated.</span><span class="sxs-lookup"><span data-stu-id="e4651-129">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="e4651-130">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e4651-130">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

    <span data-ttu-id="e4651-131">The image is attached to the incoming document record.</span><span class="sxs-lookup"><span data-stu-id="e4651-131">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="e4651-132">To create an incoming document record manually</span><span class="sxs-lookup"><span data-stu-id="e4651-132">To create an incoming document record manually</span></span>
1. <span data-ttu-id="e4651-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e4651-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="e4651-134">Choose the **Create from File** action.</span><span class="sxs-lookup"><span data-stu-id="e4651-134">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="e4651-135">On the **Insert File** page, select a file, and then choose **Open**.</span><span class="sxs-lookup"><span data-stu-id="e4651-135">On the **Insert File** page, select a file, and then choose **Open**.</span></span> <span data-ttu-id="e4651-136">The file is automatically attached.</span><span class="sxs-lookup"><span data-stu-id="e4651-136">The file is automatically attached.</span></span>
4. <span data-ttu-id="e4651-137">Alternatively, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="e4651-137">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="e4651-138">To attach a file, choose the **Attach File** action.</span><span class="sxs-lookup"><span data-stu-id="e4651-138">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="e4651-139">On the **Insert File** page, select the file that represents the incoming document in question, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="e4651-139">On the **Insert File** page, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="e4651-140">On the **Incoming Document** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e4651-140">On the **Incoming Document** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a><span data-ttu-id="e4651-141">See Also</span><span class="sxs-lookup"><span data-stu-id="e4651-141">See Also</span></span>
[<span data-ttu-id="e4651-142">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="e4651-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="e4651-143">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="e4651-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="e4651-144">Purchasing</span><span class="sxs-lookup"><span data-stu-id="e4651-144">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="e4651-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e4651-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
