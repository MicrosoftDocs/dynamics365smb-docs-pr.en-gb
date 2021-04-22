---
title: Send Electronic Documents
description: learn how to send invoices electronically.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8056aa66531740634fb155e0b3b4419a7f014ffc
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778379"
---
# <a name="send-electronic-documents"></a><span data-ttu-id="85809-103">Send Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="85809-103">Send Electronic Documents</span></span>

<span data-ttu-id="85809-104">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports sending electronic invoices and credit memos in the PEPPOL format, a format that the largest document exchange service providers support.</span><span class="sxs-lookup"><span data-stu-id="85809-104">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports sending electronic invoices and credit memos in the PEPPOL format, a format that the largest document exchange service providers support.</span></span> <span data-ttu-id="85809-105">A document exchange service provider dispatches electronic documents between trading partners.</span><span class="sxs-lookup"><span data-stu-id="85809-105">A document exchange service provider dispatches electronic documents between trading partners.</span></span> <span data-ttu-id="85809-106">To provide support for other electronic document formats, you use the data exchange framework.</span><span class="sxs-lookup"><span data-stu-id="85809-106">To provide support for other electronic document formats, you use the data exchange framework.</span></span>  

 <span data-ttu-id="85809-107">In the generic version of [!INCLUDE[prod_short](includes/prod_short.md)], a document exchange service is preconfigured and ready to be set up for your company.</span><span class="sxs-lookup"><span data-stu-id="85809-107">In the generic version of [!INCLUDE[prod_short](includes/prod_short.md)], a document exchange service is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="85809-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span><span class="sxs-lookup"><span data-stu-id="85809-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span></span> <span data-ttu-id="85809-109">However, in some cases, you must install an app.</span><span class="sxs-lookup"><span data-stu-id="85809-109">However, in some cases, you must install an app.</span></span> <span data-ttu-id="85809-110">For more information, see [Electronic Invoicing FAQ](faq-electronic-invoicing.yml).</span><span class="sxs-lookup"><span data-stu-id="85809-110">For more information, see [Electronic Invoicing FAQ](faq-electronic-invoicing.yml).</span></span>  

 <span data-ttu-id="85809-111">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialogue box.</span><span class="sxs-lookup"><span data-stu-id="85809-111">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box.</span></span> <span data-ttu-id="85809-112">You can also set up the customer's default document sending profile from that dialogue box.</span><span class="sxs-lookup"><span data-stu-id="85809-112">You can also set up the customer's default document sending profile from that dialog box.</span></span> <span data-ttu-id="85809-113">First, you must set up various master data, such as company information, customers, items, and units of measure.</span><span class="sxs-lookup"><span data-stu-id="85809-113">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="85809-114">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span><span class="sxs-lookup"><span data-stu-id="85809-114">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span></span>  

### <a name="to-send-an-electronic-sales-invoice"></a><span data-ttu-id="85809-115">To send an electronic sales invoice</span><span class="sxs-lookup"><span data-stu-id="85809-115">To send an electronic sales invoice</span></span>

1. <span data-ttu-id="85809-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="85809-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  

2. <span data-ttu-id="85809-117">Create a new sales invoice.</span><span class="sxs-lookup"><span data-stu-id="85809-117">Create a new sales invoice.</span></span>  

3. <span data-ttu-id="85809-118">When the sales invoice is ready to be invoiced, choose the **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="85809-118">When the sales invoice is ready to be invoiced, choose the **Post and Send** action.</span></span>  

     <span data-ttu-id="85809-119">If the customer's default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialogue box.</span><span class="sxs-lookup"><span data-stu-id="85809-119">If the customer's default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialog box.</span></span> <span data-ttu-id="85809-120">This way, you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span><span class="sxs-lookup"><span data-stu-id="85809-120">This way, you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span></span>  

4. <span data-ttu-id="85809-121">In the **Post and Send Confirmation** dialogue box, choose the AssistEdit button to the right of the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="85809-121">In the **Post and Send Confirmation** dialog box, choose the AssistEdit button to the right of the **Send Document to** field.</span></span>  

5. <span data-ttu-id="85809-122">In the **Send Document to** dialogue box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span><span class="sxs-lookup"><span data-stu-id="85809-122">In the **Send Document to** dialog box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span></span>  

6. <span data-ttu-id="85809-123">In the **Format** field, choose **PEPPOL**.</span><span class="sxs-lookup"><span data-stu-id="85809-123">In the **Format** field, choose **PEPPOL**.</span></span>  

7. <span data-ttu-id="85809-124">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="85809-124">Choose the **OK** button.</span></span> <span data-ttu-id="85809-125">The **Post and Send Confirmation** dialogue box appears.</span><span class="sxs-lookup"><span data-stu-id="85809-125">The **Post and Send Confirmation** dialog box appears.</span></span> <span data-ttu-id="85809-126">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="85809-126">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span></span>  

8. <span data-ttu-id="85809-127">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="85809-127">Choose the **Yes** button.</span></span>  

     <span data-ttu-id="85809-128">The sales invoice is posted and sent to the customer in the PEPPOL format.</span><span class="sxs-lookup"><span data-stu-id="85809-128">The sales invoice is posted and sent to the customer in the PEPPOL format.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="85809-129">You can also send a posted sales invoice as an electronic document.</span><span class="sxs-lookup"><span data-stu-id="85809-129">You can also send a posted sales invoice as an electronic document.</span></span> <span data-ttu-id="85809-130">The procedure is the same as described in this topic for non-posted sales documents.</span><span class="sxs-lookup"><span data-stu-id="85809-130">The procedure is the same as described in this topic for non-posted sales documents.</span></span> <span data-ttu-id="85809-131">On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.</span><span class="sxs-lookup"><span data-stu-id="85809-131">On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="85809-132">See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="85809-132">See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="85809-133">See Also</span><span class="sxs-lookup"><span data-stu-id="85809-133">See Also</span></span>

[<span data-ttu-id="85809-134">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="85809-134">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="85809-135">Set Up Document Sending Profiles</span><span class="sxs-lookup"><span data-stu-id="85809-135">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md)  
[<span data-ttu-id="85809-136">Set Up Electronic Document Sending and Receiving</span><span class="sxs-lookup"><span data-stu-id="85809-136">Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[<span data-ttu-id="85809-137">Set Up a Document Exchange Service</span><span class="sxs-lookup"><span data-stu-id="85809-137">Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)  
[<span data-ttu-id="85809-138">Set Up Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="85809-138">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="85809-139">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="85809-139">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
[<span data-ttu-id="85809-140">Electronic Invoicing FAQ</span><span class="sxs-lookup"><span data-stu-id="85809-140">Electronic Invoicing FAQ</span></span>](faq-electronic-invoicing.yml)  
[<span data-ttu-id="85809-141">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="85809-141">General Business Functionality</span></span>](ui-across-business-areas.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]