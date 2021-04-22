---
title: How to Convert Service Contracts | Microsoft Docs
description: Because the VAT rate change tool cannot convert service contracts, these contracts must be converted manually. This topic describes several alternative methods that you can use for service contract conversion.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3da6d4144b1e35da864de7b69a425bb65800b2cb
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5770745"
---
# <a name="convert-service-contracts-that-include-vat-amounts"></a><span data-ttu-id="492db-104">Convert Service Contracts that Include VAT Amounts</span><span class="sxs-lookup"><span data-stu-id="492db-104">Convert Service Contracts that Include VAT Amounts</span></span>
<span data-ttu-id="492db-105">Because the VAT rate change tool cannot convert service contracts, these contracts must be converted manually.</span><span class="sxs-lookup"><span data-stu-id="492db-105">Because the VAT rate change tool cannot convert service contracts, these contracts must be converted manually.</span></span> <span data-ttu-id="492db-106">This topic describes several alternative methods that you can use for service contract conversion.</span><span class="sxs-lookup"><span data-stu-id="492db-106">This topic describes several alternative methods that you can use for service contract conversion.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="492db-107">This topic provides a high-level workflow.</span><span class="sxs-lookup"><span data-stu-id="492db-107">This topic provides a high-level workflow.</span></span>  

 <span data-ttu-id="492db-108">The following procedure describes how to correct an invoice for a prepaid service contract that has been created a year in advance.</span><span class="sxs-lookup"><span data-stu-id="492db-108">The following procedure describes how to correct an invoice for a prepaid service contract that has been created a year in advance.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="492db-109">For this example, you must change your work date to 01.01.2017.</span><span class="sxs-lookup"><span data-stu-id="492db-109">For this example, you must change your work date to 01.01.2017.</span></span>  

### <a name="to-correct-an-invoice-for-a-prepaid-service-contract"></a><span data-ttu-id="492db-110">To correct an invoice for a prepaid service contract</span><span class="sxs-lookup"><span data-stu-id="492db-110">To correct an invoice for a prepaid service contract</span></span>  
1. <span data-ttu-id="492db-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contract Management**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="492db-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contract Management**, and then choose the related link.</span></span>  
2. <span data-ttu-id="492db-112">Under **Lists**, choose **Service Contracts**.</span><span class="sxs-lookup"><span data-stu-id="492db-112">Under **Lists**, choose **Service Contracts**.</span></span>  
3. <span data-ttu-id="492db-113">Create a new prepaid service contract.</span><span class="sxs-lookup"><span data-stu-id="492db-113">Create a new prepaid service contract.</span></span> <span data-ttu-id="492db-114">Enter a start date of **01.01.2017** and an invoice period year for customer **20000**.</span><span class="sxs-lookup"><span data-stu-id="492db-114">Enter a start date of **01.01.2017** and an invoice period year for customer **20000**.</span></span>  
4. <span data-ttu-id="492db-115">To sign the contract, choose the **Sign Contract** action.</span><span class="sxs-lookup"><span data-stu-id="492db-115">To sign the contract, choose the **Sign Contract** action.</span></span>  
5. <span data-ttu-id="492db-116">Create a service invoice.</span><span class="sxs-lookup"><span data-stu-id="492db-116">Create a service invoice.</span></span>
6. <span data-ttu-id="492db-117">The invoice is listed as an unposted service invoice.</span><span class="sxs-lookup"><span data-stu-id="492db-117">The invoice is listed as an unposted service invoice.</span></span> <span data-ttu-id="492db-118">To view the service invoice, choose the **Service** action, choose the **Contract Management** action, and then choose the **Service Invoices** action.</span><span class="sxs-lookup"><span data-stu-id="492db-118">To view the service invoice, choose the **Service** action, choose the **Contract Management** action, and then choose the **Service Invoices** action.</span></span>  
7. <span data-ttu-id="492db-119">Post the service invoice.</span><span class="sxs-lookup"><span data-stu-id="492db-119">Post the service invoice.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="492db-120">Do not change the unposted service invoice.</span><span class="sxs-lookup"><span data-stu-id="492db-120">Do not change the unposted service invoice.</span></span> <span data-ttu-id="492db-121">Since the service ledger entries are created when the invoice is created, a change in the unposted invoice will not change the already created service ledger entries.</span><span class="sxs-lookup"><span data-stu-id="492db-121">Since the service ledger entries are created when the invoice is created, a change in the unposted invoice will not change the already created service ledger entries.</span></span> <span data-ttu-id="492db-122">However, the VAT entries are created when the invoice is posted.</span><span class="sxs-lookup"><span data-stu-id="492db-122">However, the VAT entries are created when the invoice is posted.</span></span> <span data-ttu-id="492db-123">This lets you change the general product posting group and the GSP product posting group on the unposted service invoice.</span><span class="sxs-lookup"><span data-stu-id="492db-123">This lets you change the general product posting group and the GSP product posting group on the unposted service invoice.</span></span>  

### <a name="to-create-a-credit-memo-for-vat-difference"></a><span data-ttu-id="492db-124">To create a credit memo for VAT difference</span><span class="sxs-lookup"><span data-stu-id="492db-124">To create a credit memo for VAT difference</span></span>  
<span data-ttu-id="492db-125">The following procedure describes how to create a credit memo that only includes the VAT difference for the already invoiced period starting on **01.07.2017**.</span><span class="sxs-lookup"><span data-stu-id="492db-125">The following procedure describes how to create a credit memo that only includes the VAT difference for the already invoiced period starting on **01.07.2017**.</span></span> <span data-ttu-id="492db-126">In this example, the VAT amount is only posted to the Financial Management module, not to the Service Management module.</span><span class="sxs-lookup"><span data-stu-id="492db-126">In this example, the VAT amount is only posted to the Financial Management module, not to the Service Management module.</span></span> <span data-ttu-id="492db-127">The VAT entries that are linked to the service ledger entry will not be corrected.</span><span class="sxs-lookup"><span data-stu-id="492db-127">The VAT entries that are linked to the service ledger entry will not be corrected.</span></span>  

1. <span data-ttu-id="492db-128">Create a new general ledger account for the VAT difference.</span><span class="sxs-lookup"><span data-stu-id="492db-128">Create a new general ledger account for the VAT difference.</span></span> <span data-ttu-id="492db-129">This account will be used for direct posting of the VAT correction.</span><span class="sxs-lookup"><span data-stu-id="492db-129">This account will be used for direct posting of the VAT correction.</span></span>  
2. <span data-ttu-id="492db-130">Add a new line to the VAT posting setup.</span><span class="sxs-lookup"><span data-stu-id="492db-130">Add a new line to the VAT posting setup.</span></span>  

### <a name="to-create-contract-expiration-dates-in-contract-lines"></a><span data-ttu-id="492db-131">To create contract expiration dates in contract lines</span><span class="sxs-lookup"><span data-stu-id="492db-131">To create contract expiration dates in contract lines</span></span>  
<span data-ttu-id="492db-132">The following procedure describes how to create new contracts by working with contract expiration dates in service contract lines.</span><span class="sxs-lookup"><span data-stu-id="492db-132">The following procedure describes how to create new contracts by working with contract expiration dates in service contract lines.</span></span>  

1. <span data-ttu-id="492db-133">On the **Service Contract** page, set the contract expiration date to **30.06.2017**.</span><span class="sxs-lookup"><span data-stu-id="492db-133">On the **Service Contract** page, set the contract expiration date to **30.06.2017**.</span></span>  
2. <span data-ttu-id="492db-134">Choose the **Create Credit Memo** action to automatically create a credit memo for July 2017 to December 2017.</span><span class="sxs-lookup"><span data-stu-id="492db-134">Choose the **Create Credit Memo** action to automatically create a credit memo for July 2017 to December 2017.</span></span>  
3. <span data-ttu-id="492db-135">Because the contract has expired, you need to create a new contract for the period with the new VAT rate for July 1, 2017 to December 31, 2017.</span><span class="sxs-lookup"><span data-stu-id="492db-135">Because the contract has expired, you need to create a new contract for the period with the new VAT rate for July 1, 2017 to December 31, 2017.</span></span>  

### <a name="to-create-a-new-credit-memo"></a><span data-ttu-id="492db-136">To create a new credit memo</span><span class="sxs-lookup"><span data-stu-id="492db-136">To create a new credit memo</span></span>  
<span data-ttu-id="492db-137">The following procedure describes how to create a new credit memo using the **Get Prepaid Contract Entries** batch job.</span><span class="sxs-lookup"><span data-stu-id="492db-137">The following procedure describes how to create a new credit memo using the **Get Prepaid Contract Entries** batch job.</span></span> <span data-ttu-id="492db-138">Entries that you do not want to correct from January 2017 to June 2017 will be deleted.</span><span class="sxs-lookup"><span data-stu-id="492db-138">Entries that you do not want to correct from January 2017 to June 2017 will be deleted.</span></span>  

1. <span data-ttu-id="492db-139">Run the VAT rate change tool on July 1, 2017.</span><span class="sxs-lookup"><span data-stu-id="492db-139">Run the VAT rate change tool on July 1, 2017.</span></span> <span data-ttu-id="492db-140">The general product posting group or the VAT product posting group is changed.</span><span class="sxs-lookup"><span data-stu-id="492db-140">The general product posting group or the VAT product posting group is changed.</span></span> <span data-ttu-id="492db-141">For more information, see [Work with VAT on Sales and Purchases](finance-work-with-vat.md).</span><span class="sxs-lookup"><span data-stu-id="492db-141">For more information, see [Work with VAT on Sales and Purchases](finance-work-with-vat.md).</span></span>  
2. <span data-ttu-id="492db-142">After running the VAT rate change tool, enter a contract expiration date for the service contract.</span><span class="sxs-lookup"><span data-stu-id="492db-142">After running the VAT rate change tool, enter a contract expiration date for the service contract.</span></span> <span data-ttu-id="492db-143">You can now delete the service contract line and create a new line that is identical to the old one.</span><span class="sxs-lookup"><span data-stu-id="492db-143">You can now delete the service contract line and create a new line that is identical to the old one.</span></span>  
3. <span data-ttu-id="492db-144">Create a new invoice for the period of January 2017 to December 2012 using the new VAT rate.</span><span class="sxs-lookup"><span data-stu-id="492db-144">Create a new invoice for the period of January 2017 to December 2012 using the new VAT rate.</span></span>  
4. <span data-ttu-id="492db-145">To create another credit memo, on the **Service Credit Memos** page, choose the **New** action to create a new service credit memo.</span><span class="sxs-lookup"><span data-stu-id="492db-145">To create another credit memo, on the **Service Credit Memos** page, choose the **New** action to create a new service credit memo.</span></span>  
5. <span data-ttu-id="492db-146">Choose the **Get Prepaid Contract Entries** action.</span><span class="sxs-lookup"><span data-stu-id="492db-146">Choose the **Get Prepaid Contract Entries** action.</span></span>  
6. <span data-ttu-id="492db-147">After the conversion is complete, VAT and service ledger entries will be correct.</span><span class="sxs-lookup"><span data-stu-id="492db-147">After the conversion is complete, VAT and service ledger entries will be correct.</span></span>  

## <a name="see-also"></a><span data-ttu-id="492db-148">See Also</span><span class="sxs-lookup"><span data-stu-id="492db-148">See Also</span></span>  
[<span data-ttu-id="492db-149">Work with Service Contracts and Service Contract Quotes</span><span class="sxs-lookup"><span data-stu-id="492db-149">Work with Service Contracts and Service Contract Quotes</span></span>](service-how-to-create-service-contracts-and-service-contract-quotes.md)  
[<span data-ttu-id="492db-150">Finance</span><span class="sxs-lookup"><span data-stu-id="492db-150">Finance</span></span>](finance.md)  
[<span data-ttu-id="492db-151">Report VAT to Tax Authorities</span><span class="sxs-lookup"><span data-stu-id="492db-151">Report VAT to Tax Authorities</span></span>](finance-how-report-vat.md)  
[<span data-ttu-id="492db-152">Work with VAT on Sales and Purchases</span><span class="sxs-lookup"><span data-stu-id="492db-152">Work with VAT on Sales and Purchases</span></span>](finance-work-with-vat.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]