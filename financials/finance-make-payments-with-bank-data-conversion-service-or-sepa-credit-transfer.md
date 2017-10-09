---
title: Choose the method of electronic payments | Microsoft Docs
description: Process payments to your vendors by exporting a file together with the payment information from the journal lines.
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: bbb38f7d4a4b7d1b63cfceef2640172d7b69e364
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a><span data-ttu-id="8f6c2-103">Make Payments with Bank Data Conversion Service or SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="8f6c2-103">Make Payments with Bank Data Conversion Service or SEPA Credit Transfer</span></span>
<span data-ttu-id="8f6c2-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span></span> <span data-ttu-id="8f6c2-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="8f6c2-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span></span>   

 <span data-ttu-id="8f6c2-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span></span> <span data-ttu-id="8f6c2-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8f6c2-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span></span>  

 <span data-ttu-id="8f6c2-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="8f6c2-111">**To**</span><span class="sxs-lookup"><span data-stu-id="8f6c2-111">**To**</span></span>|<span data-ttu-id="8f6c2-112">**See**</span><span class="sxs-lookup"><span data-stu-id="8f6c2-112">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="8f6c2-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span></span>|[<span data-ttu-id="8f6c2-114">How to: Set Up the Bank Data Conversion Service</span><span class="sxs-lookup"><span data-stu-id="8f6c2-114">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-statement-service.md)|  
|<span data-ttu-id="8f6c2-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span></span>|[<span data-ttu-id="8f6c2-116">How to: Set Up SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="8f6c2-116">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)|  
|<span data-ttu-id="8f6c2-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span></span>|[<span data-ttu-id="8f6c2-118">Manage Payables</span><span class="sxs-lookup"><span data-stu-id="8f6c2-118">Manage Payables</span></span>](payables-manage-payables.md)|  
|<span data-ttu-id="8f6c2-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span></span>|[<span data-ttu-id="8f6c2-120">How to: Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="8f6c2-120">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="8f6c2-121">Review which payments have been exported and into which files.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-121">Review which payments have been exported and into which files.</span></span>|<span data-ttu-id="8f6c2-122">Credit Transfer Registers</span><span class="sxs-lookup"><span data-stu-id="8f6c2-122">Credit Transfer Registers</span></span>|  
|<span data-ttu-id="8f6c2-123">When the electronic payment is successfully processed by the bank, post the payments.</span><span class="sxs-lookup"><span data-stu-id="8f6c2-123">When the electronic payment is successfully processed by the bank, post the payments.</span></span>|[<span data-ttu-id="8f6c2-124">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="8f6c2-124">Working with General Journals</span></span>](ui-work-general-journals.md)|  

## <a name="see-also"></a><span data-ttu-id="8f6c2-125">See Also</span><span class="sxs-lookup"><span data-stu-id="8f6c2-125">See Also</span></span>  
[<span data-ttu-id="8f6c2-126">How to: Set Up the Bank Data Conversion Service</span><span class="sxs-lookup"><span data-stu-id="8f6c2-126">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-statement-service.md)  
[<span data-ttu-id="8f6c2-127">How to: Set Up SEPA Credit Transfer</span><span class="sxs-lookup"><span data-stu-id="8f6c2-127">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)  
<span data-ttu-id="8f6c2-128">[Manage Payables](payables-manage-payables.md) </span><span class="sxs-lookup"><span data-stu-id="8f6c2-128">[Manage Payables](payables-manage-payables.md) </span></span>  
[<span data-ttu-id="8f6c2-129">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="8f6c2-129">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="8f6c2-130">Collect Payments with SEPA Direct Debit</span><span class="sxs-lookup"><span data-stu-id="8f6c2-130">Collect Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   

