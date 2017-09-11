---
title: Create Records of Incoming Documents| Microsoft Docs
description: You can create records of incoming documents, such as e-invoices, and manage OCR tasks, eCommerce, and document exchange.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 36e1acc3125e325a9fca8fdd9ce797ac50c065c1
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-create-incoming-document-records"></a><span data-ttu-id="3d5f2-103">How to: Create Incoming Document Records</span><span class="sxs-lookup"><span data-stu-id="3d5f2-103">How to: Create Incoming Document Records</span></span>
<span data-ttu-id="3d5f2-104">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-104">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="3d5f2-105">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-105">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="3d5f2-106">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-106">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span></span> <span data-ttu-id="3d5f2-107">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-107">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="3d5f2-108">Before you can use the Incoming Documents feature, you must perform the required setup.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-108">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="3d5f2-109">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="3d5f2-109">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="3d5f2-110">To approve or reject an incoming document</span><span class="sxs-lookup"><span data-stu-id="3d5f2-110">To approve or reject an incoming document</span></span>
<span data-ttu-id="3d5f2-111">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-111">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="3d5f2-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="3d5f2-113">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-113">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="3d5f2-114">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-114">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="3d5f2-115">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-115">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="3d5f2-116">To create an incoming document record by taking a photo</span><span class="sxs-lookup"><span data-stu-id="3d5f2-116">To create an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="3d5f2-117">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-117">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="3d5f2-118">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-118">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="3d5f2-119">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-119">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="3d5f2-120">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-120">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="3d5f2-121">The camera on the tablet or phone is activated.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-121">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="3d5f2-122">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-122">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="3d5f2-123">A new incoming document record is created, with the image attached.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-123">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="3d5f2-124">To attach an image to an incoming document record by taking a photo</span><span class="sxs-lookup"><span data-stu-id="3d5f2-124">To attach an image to an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="3d5f2-125">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-125">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="3d5f2-126">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-126">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="3d5f2-127">Open the card for an existing incoming document record.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-127">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="3d5f2-128">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-128">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="3d5f2-129">The camera on the tablet or phone is activated.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-129">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="3d5f2-130">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-130">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="3d5f2-131">The image is attached to the incoming document record.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-131">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="3d5f2-132">To create an incoming document record manually</span><span class="sxs-lookup"><span data-stu-id="3d5f2-132">To create an incoming document record manually</span></span>
1. <span data-ttu-id="3d5f2-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="3d5f2-134">Choose the **Create from File** action.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-134">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="3d5f2-135">In the **Insert File** window, select a file, and then choose **Open**.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-135">In the **Insert File** window, select a file, and then choose **Open**.</span></span>

    <span data-ttu-id="3d5f2-136">The file is automatically attached.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-136">The file is automatically attached.</span></span>
4. <span data-ttu-id="3d5f2-137">Alternatively, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-137">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="3d5f2-138">To attach a file, choose the **Attach File** action.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-138">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="3d5f2-139">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-139">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="3d5f2-140">In the **Incoming Document** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="3d5f2-140">In the **Incoming Document** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a><span data-ttu-id="3d5f2-141">See Also</span><span class="sxs-lookup"><span data-stu-id="3d5f2-141">See Also</span></span>
[<span data-ttu-id="3d5f2-142">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="3d5f2-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="3d5f2-143">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="3d5f2-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="3d5f2-144">Purchasing</span><span class="sxs-lookup"><span data-stu-id="3d5f2-144">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="3d5f2-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3d5f2-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

