---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/23/2020
ms.author: sgroespe
ms.openlocfilehash: 09047315c701bd2076f59b6c3f4840ba95eb06cc
ms.sourcegitcommit: 63102669366eb26f9c32729848170bc2e5c4d6ae
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/25/2020
ms.locfileid: "3503551"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="4a7fe-103">Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4a7fe-103">Set Up Incoming Documents</span></span>

<span data-ttu-id="4a7fe-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="4a7fe-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span></span>

<span data-ttu-id="4a7fe-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="4a7fe-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="4a7fe-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="4a7fe-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="4a7fe-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="4a7fe-110">To set up the Incoming Documents feature</span><span class="sxs-lookup"><span data-stu-id="4a7fe-110">To set up the Incoming Documents feature</span></span>

1. <span data-ttu-id="4a7fe-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="4a7fe-112">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="4a7fe-113">As part of the setup, you must decide if you want to require approval of incoming documents.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-113">As part of the setup, you must decide if you want to require approval of incoming documents.</span></span> <span data-ttu-id="4a7fe-114">To require approval, you must set up approvers and approval workflows.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-114">To require approval, you must set up approvers and approval workflows.</span></span> <span data-ttu-id="4a7fe-115">If your organisation does not intend to require approval, you can skip the next section.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-115">If your organization does not intend to require approval, you can skip the next section.</span></span>  

<span data-ttu-id="4a7fe-116">Finally, you if you use a service to convert PDF or image files representing incoming documents, you must it set up.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-116">Finally, you if you use a service to convert PDF or image files representing incoming documents, you must it set up.</span></span> <span data-ttu-id="4a7fe-117">Otherwise, you can also skip that section.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-117">Otherwise, you can also skip that section.</span></span>  

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="4a7fe-118">To set up approvers of incoming document records</span><span class="sxs-lookup"><span data-stu-id="4a7fe-118">To set up approvers of incoming document records</span></span>

<span data-ttu-id="4a7fe-119">Approvers of incoming documents must be set up as approval workflow users.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-119">Approvers of incoming documents must be set up as approval workflow users.</span></span>

<span data-ttu-id="4a7fe-120">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-120">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span></span> <span data-ttu-id="4a7fe-121">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-121">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span></span> <span data-ttu-id="4a7fe-122">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="4a7fe-122">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="4a7fe-123">To set up an OCR service</span><span class="sxs-lookup"><span data-stu-id="4a7fe-123">To set up an OCR service</span></span>

1. <span data-ttu-id="4a7fe-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="4a7fe-125">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="4a7fe-126">You login data is automatically encrypted.</span><span class="sxs-lookup"><span data-stu-id="4a7fe-126">You login data is automatically encrypted.</span></span>

<span data-ttu-id="4a7fe-127">For more information, see [Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).</span><span class="sxs-lookup"><span data-stu-id="4a7fe-127">For more information, see [Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="4a7fe-128">See Also</span><span class="sxs-lookup"><span data-stu-id="4a7fe-128">See Also</span></span>

[<span data-ttu-id="4a7fe-129">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4a7fe-129">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="4a7fe-130">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="4a7fe-130">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="4a7fe-131">Purchasing</span><span class="sxs-lookup"><span data-stu-id="4a7fe-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="4a7fe-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4a7fe-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
