---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 12/09/2019
ms.author: sgroespe
ms.openlocfilehash: e67ca1c0b26d7e4a81e53854ca31efc64a366c3f
ms.sourcegitcommit: 3d128a00358668b3fdd105ebf4604ca4e2b6743c
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/20/2019
ms.locfileid: "2910499"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="23fa0-103">Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="23fa0-103">Set Up Incoming Documents</span></span>
<span data-ttu-id="23fa0-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span><span class="sxs-lookup"><span data-stu-id="23fa0-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="23fa0-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span><span class="sxs-lookup"><span data-stu-id="23fa0-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span></span>

<span data-ttu-id="23fa0-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span><span class="sxs-lookup"><span data-stu-id="23fa0-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="23fa0-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="23fa0-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="23fa0-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="23fa0-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="23fa0-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="23fa0-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="23fa0-110">To set up the Incoming Documents feature</span><span class="sxs-lookup"><span data-stu-id="23fa0-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="23fa0-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="23fa0-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="23fa0-112">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="23fa0-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="23fa0-113">To set up approvers of incoming document records</span><span class="sxs-lookup"><span data-stu-id="23fa0-113">To set up approvers of incoming document records</span></span>
<span data-ttu-id="23fa0-114">Approvers of incoming documents must be set up as approval workflow users.</span><span class="sxs-lookup"><span data-stu-id="23fa0-114">Approvers of incoming documents must be set up as approval workflow users.</span></span>

<span data-ttu-id="23fa0-115">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span><span class="sxs-lookup"><span data-stu-id="23fa0-115">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span></span> <span data-ttu-id="23fa0-116">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span><span class="sxs-lookup"><span data-stu-id="23fa0-116">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span></span> <span data-ttu-id="23fa0-117">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="23fa0-117">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="23fa0-118">To set up an OCR service</span><span class="sxs-lookup"><span data-stu-id="23fa0-118">To set up an OCR service</span></span>
1. <span data-ttu-id="23fa0-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="23fa0-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="23fa0-120">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="23fa0-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="23fa0-121">You login data is automatically encrypted.</span><span class="sxs-lookup"><span data-stu-id="23fa0-121">You login data is automatically encrypted.</span></span>

## <a name="see-also"></a><span data-ttu-id="23fa0-122">See Also</span><span class="sxs-lookup"><span data-stu-id="23fa0-122">See Also</span></span>
[<span data-ttu-id="23fa0-123">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="23fa0-123">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="23fa0-124">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="23fa0-124">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="23fa0-125">Purchasing</span><span class="sxs-lookup"><span data-stu-id="23fa0-125">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="23fa0-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="23fa0-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
