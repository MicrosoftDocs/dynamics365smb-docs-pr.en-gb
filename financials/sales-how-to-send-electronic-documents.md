---
title: Send Electronic Documents | Microsoft Docs
description: learn how to send invoices electronically.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: fae5e37b8f1fcca84a474b2eac2039f7fc6d8245
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="send-electronic-documents"></a><span data-ttu-id="5fe53-103">Send Electronic Documents</span><span class="sxs-lookup"><span data-stu-id="5fe53-103">Send Electronic Documents</span></span>
<span data-ttu-id="5fe53-104">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports sending electronic invoices and credit memos in the PEPPOL format, which is supported by the largest document exchange service providers.</span><span class="sxs-lookup"><span data-stu-id="5fe53-104">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports sending electronic invoices and credit memos in the PEPPOL format, which is supported by the largest document exchange service providers.</span></span> <span data-ttu-id="5fe53-105">A document exchange service provider dispatches electronic documents between trading partners.</span><span class="sxs-lookup"><span data-stu-id="5fe53-105">A document exchange service provider dispatches electronic documents between trading partners.</span></span> <span data-ttu-id="5fe53-106">To provide support for other electronic document formats, you use the data exchange framework.</span><span class="sxs-lookup"><span data-stu-id="5fe53-106">To provide support for other electronic document formats, you use the data exchange framework.</span></span>  

 <span data-ttu-id="5fe53-107">In the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)], a document exchange service is preconfigured and ready to be set up for your company.</span><span class="sxs-lookup"><span data-stu-id="5fe53-107">In the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)], a document exchange service is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="5fe53-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span><span class="sxs-lookup"><span data-stu-id="5fe53-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span></span>  

 <span data-ttu-id="5fe53-109">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialogue box from where you can also set up the customer’s default document sending profile.</span><span class="sxs-lookup"><span data-stu-id="5fe53-109">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box from where you can also set up the customer’s default document sending profile.</span></span> <span data-ttu-id="5fe53-110">First, you must set up various master data, such as company information, customers, items, and units of measure.</span><span class="sxs-lookup"><span data-stu-id="5fe53-110">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="5fe53-111">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span><span class="sxs-lookup"><span data-stu-id="5fe53-111">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span></span>  

### <a name="to-send-an-electronic-sales-invoice"></a><span data-ttu-id="5fe53-112">To send an electronic sales invoice</span><span class="sxs-lookup"><span data-stu-id="5fe53-112">To send an electronic sales invoice</span></span>  

1.  <span data-ttu-id="5fe53-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5fe53-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="5fe53-114">Create a new sales invoice.</span><span class="sxs-lookup"><span data-stu-id="5fe53-114">Create a new sales invoice.</span></span>  

3.  <span data-ttu-id="5fe53-115">When the sales invoice is ready to be invoiced, on the **Actions** tab, in the **Posting** group, choose **Post and Send**.</span><span class="sxs-lookup"><span data-stu-id="5fe53-115">When the sales invoice is ready to be invoiced, on the **Actions** tab, in the **Posting** group, choose **Post and Send**.</span></span>  

     <span data-ttu-id="5fe53-116">If the customer’s default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialogue box and you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span><span class="sxs-lookup"><span data-stu-id="5fe53-116">If the customer’s default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialog box and you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span></span>  

4.  <span data-ttu-id="5fe53-117">In the **Post and Send Confirmation** dialogue box, choose the AssistEdit button to the right of the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="5fe53-117">In the **Post and Send Confirmation** dialog box, choose the AssistEdit button to the right of the **Send Document to** field.</span></span>  

5.  <span data-ttu-id="5fe53-118">In the **Send Document to** dialogue box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span><span class="sxs-lookup"><span data-stu-id="5fe53-118">In the **Send Document to** dialog box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span></span>  

6.  <span data-ttu-id="5fe53-119">In the **Format** field, choose **PEPPOL**.</span><span class="sxs-lookup"><span data-stu-id="5fe53-119">In the **Format** field, choose **PEPPOL**.</span></span>  

7.  <span data-ttu-id="5fe53-120">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="5fe53-120">Choose the **OK** button.</span></span> <span data-ttu-id="5fe53-121">The **Post and Send Confirmation** dialogue box appears.</span><span class="sxs-lookup"><span data-stu-id="5fe53-121">The **Post and Send Confirmation** dialog box appears.</span></span> <span data-ttu-id="5fe53-122">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span><span class="sxs-lookup"><span data-stu-id="5fe53-122">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span></span>  

8.  <span data-ttu-id="5fe53-123">Choose the **Yes** button.</span><span class="sxs-lookup"><span data-stu-id="5fe53-123">Choose the **Yes** button.</span></span>  

     <span data-ttu-id="5fe53-124">The sales invoice is posted and sent to the customer as an electronic document in the PEPPOL format.</span><span class="sxs-lookup"><span data-stu-id="5fe53-124">The sales invoice is posted and sent to the customer as an electronic document in the PEPPOL format.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="5fe53-125">You can also send a posted sales invoice as an electronic document.</span><span class="sxs-lookup"><span data-stu-id="5fe53-125">You can also send a posted sales invoice as an electronic document.</span></span> <span data-ttu-id="5fe53-126">The procedure is the same as described in this topic for non-posted sales documents.</span><span class="sxs-lookup"><span data-stu-id="5fe53-126">The procedure is the same as described in this topic for non-posted sales documents.</span></span> <span data-ttu-id="5fe53-127">In the **Posted Sales Invoice** window, on the **Actions** tab, in the **General** group, choose **Activity Log** to view the status of the electronic document.</span><span class="sxs-lookup"><span data-stu-id="5fe53-127">In the **Posted Sales Invoice** window, on the **Actions** tab, in the **General** group, choose **Activity Log** to view the status of the electronic document.</span></span> <span data-ttu-id="5fe53-128">For more information, see **Activity Log**.</span><span class="sxs-lookup"><span data-stu-id="5fe53-128">For more information, see **Activity Log**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5fe53-129">See Also</span><span class="sxs-lookup"><span data-stu-id="5fe53-129">See Also</span></span>  
[<span data-ttu-id="5fe53-130">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="5fe53-130">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="5fe53-131">Set Up Document Sending Profiles</span><span class="sxs-lookup"><span data-stu-id="5fe53-131">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md)  
[<span data-ttu-id="5fe53-132">Set Up Electronic Document Sending and Receiving</span><span class="sxs-lookup"><span data-stu-id="5fe53-132">Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[<span data-ttu-id="5fe53-133">Set Up a Document Exchange Service</span><span class="sxs-lookup"><span data-stu-id="5fe53-133">Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)  
[<span data-ttu-id="5fe53-134">Set Up Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="5fe53-134">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="5fe53-135">Exchanging Data Electronically</span><span class="sxs-lookup"><span data-stu-id="5fe53-135">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
[<span data-ttu-id="5fe53-136">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="5fe53-136">General Business Functionality</span></span>](ui-across-business-areas.md)  

