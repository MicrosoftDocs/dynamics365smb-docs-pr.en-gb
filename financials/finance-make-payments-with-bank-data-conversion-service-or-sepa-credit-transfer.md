---
title: Make Payments with Bank Data Conversion Service or SEPA Credit Transfer | Microsoft Docs
description: Process payments to your vendors by exporting a file together with the payment information from the journal lines.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/17/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa56764b5f3210229ad21eae6891fb201462209c
ms.openlocfilehash: 0760b5480b3c2de9bc370526bd87da2c9a492d92
ms.contentlocale: en-gb
ms.lasthandoff: 12/14/2017

---
# <a name="making-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a><span data-ttu-id="c92f7-103">Making Payments with Bank Data Conversion Service or SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="c92f7-103">Making Payments with Bank Data Conversion Service or SEPA Credit Transfer</span></span>
<span data-ttu-id="c92f7-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span><span class="sxs-lookup"><span data-stu-id="c92f7-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span></span> <span data-ttu-id="c92f7-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span><span class="sxs-lookup"><span data-stu-id="c92f7-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="c92f7-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span><span class="sxs-lookup"><span data-stu-id="c92f7-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span></span>   

 <span data-ttu-id="c92f7-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span><span class="sxs-lookup"><span data-stu-id="c92f7-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span></span> <span data-ttu-id="c92f7-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span><span class="sxs-lookup"><span data-stu-id="c92f7-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c92f7-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span><span class="sxs-lookup"><span data-stu-id="c92f7-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span></span>  

 <span data-ttu-id="c92f7-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="c92f7-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="c92f7-111">**To**</span><span class="sxs-lookup"><span data-stu-id="c92f7-111">**To**</span></span>|<span data-ttu-id="c92f7-112">**See**</span><span class="sxs-lookup"><span data-stu-id="c92f7-112">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="c92f7-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span><span class="sxs-lookup"><span data-stu-id="c92f7-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span></span>|[<span data-ttu-id="c92f7-114">How to: Set Up the Bank Data Conversion Service</span><span class="sxs-lookup"><span data-stu-id="c92f7-114">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-statement-service.md)|  
|<span data-ttu-id="c92f7-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span><span class="sxs-lookup"><span data-stu-id="c92f7-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span></span>|[<span data-ttu-id="c92f7-116">How to: Set Up SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="c92f7-116">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)|  
|<span data-ttu-id="c92f7-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span><span class="sxs-lookup"><span data-stu-id="c92f7-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span></span>|[<span data-ttu-id="c92f7-118">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="c92f7-118">Managing Payables</span></span>](payables-manage-payables.md)|  
|<span data-ttu-id="c92f7-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span><span class="sxs-lookup"><span data-stu-id="c92f7-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span></span>|[<span data-ttu-id="c92f7-120">How to: Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="c92f7-120">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="c92f7-121">When the electronic payment is successfully processed by the bank, post the payments.</span><span class="sxs-lookup"><span data-stu-id="c92f7-121">When the electronic payment is successfully processed by the bank, post the payments.</span></span>|[<span data-ttu-id="c92f7-122">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="c92f7-122">Working with General Journals</span></span>](ui-work-general-journals.md)|  

## <a name="see-also"></a><span data-ttu-id="c92f7-123">See Also</span><span class="sxs-lookup"><span data-stu-id="c92f7-123">See Also</span></span>  
[<span data-ttu-id="c92f7-124">How to: Set Up the Bank Data Conversion Service</span><span class="sxs-lookup"><span data-stu-id="c92f7-124">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-statement-service.md)  
[<span data-ttu-id="c92f7-125">How to: Set Up SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="c92f7-125">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)  
<span data-ttu-id="c92f7-126">[Managing Payables](payables-manage-payables.md) </span><span class="sxs-lookup"><span data-stu-id="c92f7-126">[Managing Payables](payables-manage-payables.md) </span></span>  
[<span data-ttu-id="c92f7-127">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="c92f7-127">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="c92f7-128">Collecting Payments with SEPA Direct Debit</span><span class="sxs-lookup"><span data-stu-id="c92f7-128">Collecting Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   

