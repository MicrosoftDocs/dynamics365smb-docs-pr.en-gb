---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 00bfa89376a361bedc71ba76630906d761989ead
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5384606"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="716b5-103">Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="716b5-103">Set Up Incoming Documents</span></span>

<span data-ttu-id="716b5-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span><span class="sxs-lookup"><span data-stu-id="716b5-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="716b5-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span><span class="sxs-lookup"><span data-stu-id="716b5-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span></span>

<span data-ttu-id="716b5-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[prod_short](includes/prod_short.md)], you must first set up the OCR feature and enable the service.</span><span class="sxs-lookup"><span data-stu-id="716b5-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[prod_short](includes/prod_short.md)], you must first set up the OCR feature and enable the service.</span></span> <span data-ttu-id="716b5-107">Choose a service package that is appropriate for your organisation and/or country/region.</span><span class="sxs-lookup"><span data-stu-id="716b5-107">Choose a service package that is appropriate for your organization and/or country/region.</span></span> <span data-ttu-id="716b5-108">Alternatively, you can create entries manually to represent the external documents.</span><span class="sxs-lookup"><span data-stu-id="716b5-108">Alternatively, you can create entries manually to represent the external documents.</span></span>  

<span data-ttu-id="716b5-109">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="716b5-109">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="716b5-110">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="716b5-110">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="716b5-111">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="716b5-111">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="716b5-112">To set up the Incoming Documents feature</span><span class="sxs-lookup"><span data-stu-id="716b5-112">To set up the Incoming Documents feature</span></span>

1. <span data-ttu-id="716b5-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="716b5-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="716b5-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="716b5-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="716b5-115">As part of the setup, you must decide if you want to require approval of incoming documents.</span><span class="sxs-lookup"><span data-stu-id="716b5-115">As part of the setup, you must decide if you want to require approval of incoming documents.</span></span> <span data-ttu-id="716b5-116">To require approval, you must set up approvers and approval workflows.</span><span class="sxs-lookup"><span data-stu-id="716b5-116">To require approval, you must set up approvers and approval workflows.</span></span> <span data-ttu-id="716b5-117">If your organisation does not intend to require approval, you can skip the next section.</span><span class="sxs-lookup"><span data-stu-id="716b5-117">If your organization does not intend to require approval, you can skip the next section.</span></span>  

<span data-ttu-id="716b5-118">Finally, you if you use a service to convert PDF or image files representing incoming documents, you must it set up.</span><span class="sxs-lookup"><span data-stu-id="716b5-118">Finally, you if you use a service to convert PDF or image files representing incoming documents, you must it set up.</span></span> <span data-ttu-id="716b5-119">Otherwise, you can also skip that section.</span><span class="sxs-lookup"><span data-stu-id="716b5-119">Otherwise, you can also skip that section.</span></span>  

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="716b5-120">To set up approvers of incoming document records</span><span class="sxs-lookup"><span data-stu-id="716b5-120">To set up approvers of incoming document records</span></span>

<span data-ttu-id="716b5-121">Optionally, set up an approval process for the incoming documents.</span><span class="sxs-lookup"><span data-stu-id="716b5-121">Optionally, set up an approval process for the incoming documents.</span></span> <span data-ttu-id="716b5-122">Approvers of incoming documents must be set up as approval workflow users.</span><span class="sxs-lookup"><span data-stu-id="716b5-122">Approvers of incoming documents must be set up as approval workflow users.</span></span>

<span data-ttu-id="716b5-123">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span><span class="sxs-lookup"><span data-stu-id="716b5-123">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span></span> <span data-ttu-id="716b5-124">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span><span class="sxs-lookup"><span data-stu-id="716b5-124">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span></span> <span data-ttu-id="716b5-125">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="716b5-125">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="716b5-126">To set up an OCR service</span><span class="sxs-lookup"><span data-stu-id="716b5-126">To set up an OCR service</span></span>

1. <span data-ttu-id="716b5-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="716b5-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="716b5-128">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="716b5-128">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="716b5-129">You login data is automatically encrypted.</span><span class="sxs-lookup"><span data-stu-id="716b5-129">You login data is automatically encrypted.</span></span>

<span data-ttu-id="716b5-130">For more information, see [Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).</span><span class="sxs-lookup"><span data-stu-id="716b5-130">For more information, see [Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="716b5-131">See Also</span><span class="sxs-lookup"><span data-stu-id="716b5-131">See Also</span></span>

[<span data-ttu-id="716b5-132">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="716b5-132">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="716b5-133">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="716b5-133">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="716b5-134">Purchasing</span><span class="sxs-lookup"><span data-stu-id="716b5-134">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="716b5-135">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="716b5-135">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]