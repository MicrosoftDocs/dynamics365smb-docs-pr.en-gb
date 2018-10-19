---
title: Set Up Incoming Documents| Microsoft Docs
description: Use the Incoming Documents feature to create electronic documents, manage OCR tasks, import invoices, and convert image files.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 35911fe862a016546954d6912b3cf12896d23fdd
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="31016-103">Set Up Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="31016-103">Set Up Incoming Documents</span></span>
<span data-ttu-id="31016-104">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span><span class="sxs-lookup"><span data-stu-id="31016-104">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="31016-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span><span class="sxs-lookup"><span data-stu-id="31016-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="31016-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span><span class="sxs-lookup"><span data-stu-id="31016-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="31016-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span><span class="sxs-lookup"><span data-stu-id="31016-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="31016-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span><span class="sxs-lookup"><span data-stu-id="31016-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="31016-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="31016-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="31016-110">To set up the Incoming Documents feature</span><span class="sxs-lookup"><span data-stu-id="31016-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="31016-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="31016-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="31016-112">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="31016-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="31016-113">To set up approvers of incoming document records</span><span class="sxs-lookup"><span data-stu-id="31016-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="31016-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="31016-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="31016-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span><span class="sxs-lookup"><span data-stu-id="31016-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="31016-116">The **Incoming Document Approvers** window shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="31016-116">The **Incoming Document Approvers** window shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
3. <span data-ttu-id="31016-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span><span class="sxs-lookup"><span data-stu-id="31016-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="31016-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span><span class="sxs-lookup"><span data-stu-id="31016-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

> [!NOTE]  
>   <span data-ttu-id="31016-119">This approval setup is not related to approval workflows.</span><span class="sxs-lookup"><span data-stu-id="31016-119">This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="31016-120">For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="31016-120">For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="31016-121">To set up an OCR service</span><span class="sxs-lookup"><span data-stu-id="31016-121">To set up an OCR service</span></span>
1. <span data-ttu-id="31016-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="31016-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="31016-123">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="31016-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="31016-124">You login data is automatically encrypted.</span><span class="sxs-lookup"><span data-stu-id="31016-124">You login data is automatically encrypted.</span></span>

## <a name="see-also"></a><span data-ttu-id="31016-125">See Also</span><span class="sxs-lookup"><span data-stu-id="31016-125">See Also</span></span>
[<span data-ttu-id="31016-126">Process Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="31016-126">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="31016-127">Incoming Documents</span><span class="sxs-lookup"><span data-stu-id="31016-127">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="31016-128">Purchasing</span><span class="sxs-lookup"><span data-stu-id="31016-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="31016-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="31016-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

