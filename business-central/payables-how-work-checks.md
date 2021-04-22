---
title: Issue, Print, Cancel, and Void Checks| Microsoft Docs
description: Describes how to issue cheques using the payment journal, print cheques, and void or view cheque ledger entries in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment journal, print check, vendor payment, creditor, debt, balance due, AP
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 6d2f204daefe5ed9473d64592d67e3c4cf026bce
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775097"
---
# <a name="make-check-payments"></a><span data-ttu-id="5e0cd-103">Make Cheque Payments</span><span class="sxs-lookup"><span data-stu-id="5e0cd-103">Make Check Payments</span></span>

<span data-ttu-id="5e0cd-104">You can issue electronic and manual checks in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="5e0cd-104">You can issue electronic and manual checks in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="5e0cd-105">Both methods use the payment journal to issue checks to vendors.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-105">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="5e0cd-106">You can also void cheques and view cheque ledger entries.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-106">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="5e0cd-107">The following procedure shows how to pay a vendor with a computer cheque by applying the payment to the relevant vendor invoice, printing the cheque, and then posting the payment as paid.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-107">The following procedure shows how to pay a vendor with a computer checks by applying the payment to the relevant vendor invoice, printing the check, and then posting the payment as paid.</span></span> <span data-ttu-id="5e0cd-108">This results in positive vendor ledger entries, applied to negative bank ledger entries, and physical cheques for processing in the bank.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-108">This results in positive vendor ledger entries, applied to negative bank ledger entries, and physical checks for processing in the bank.</span></span>

<span data-ttu-id="5e0cd-109">You can pay with two types of cheque.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-109">You can pay with two types of checks.</span></span> <span data-ttu-id="5e0cd-110">For both types, the **Bal. Account Type** or the **Account Type** field must contain **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-110">For both types, the **Bal. Account Type** or the **Account Type** field must contain **Bank Account**.</span></span>

- <span data-ttu-id="5e0cd-111">**Computer Cheque**: Select this option if you want to print a cheque for the amount on the payment journal line.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-111">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="5e0cd-112">You must print the cheques before you can post the journal lines.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-112">You must print the checks before you can post the journal lines.</span></span>
- <span data-ttu-id="5e0cd-113">**Manual Cheque**: Select this option if you have created a cheque manually and want to create a corresponding cheque ledger entry for this amount.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-113">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="5e0cd-114">By using this option, you cannot print the cheque.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-114">By using this option, you cannot print the check.</span></span>

> [!NOTE]  
> <span data-ttu-id="5e0cd-115">To make sure that your bank only clears validated cheques and amounts, you can send them a file that contains vendor, cheque, and payment information.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-115">To make sure that your bank only clears validated checks and amounts, you can send them a file that contains vendor, check, and payment information.</span></span> <span data-ttu-id="5e0cd-116">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span><span class="sxs-lookup"><span data-stu-id="5e0cd-116">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5e0cd-117">Your printer must be correctly set up with the cheque forms, and you must define which cheque layout to use.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-117">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="5e0cd-118">For more information, see [Select a Cheque Layout](finance-how-define-check-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="5e0cd-118">For more information, see [Select a Check Layout](finance-how-define-check-layouts.md).</span></span> <span data-ttu-id="5e0cd-119">Alternatively, you can send the cheque as a PDF file, for example.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-119">Alternatively, you can send the check as a PDF file, for example.</span></span>  

<span data-ttu-id="5e0cd-120">You can print up to 10 invoices on a page for a cheque stub.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-120">You can print up to 10 invoices on a page for a check stub.</span></span> <span data-ttu-id="5e0cd-121">If a cheque applies to more than 10 invoices, when you print the stub we void the cheque on the first page and print the word VOID on the cheque.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-121">If a check applies to more than 10 invoices, when you print the stub we void the check on the first page and print the word VOID on the check.</span></span> <span data-ttu-id="5e0cd-122">We then print the remainder of the invoices and the total cheque amount on the second page.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-122">We then print the remainder of the invoices and the total check amount on the second page.</span></span>

## <a name="to-pay-a-vendor-invoice-with-a-computer-check"></a><span data-ttu-id="5e0cd-123">To pay a vendor invoice with a computer cheque</span><span class="sxs-lookup"><span data-stu-id="5e0cd-123">To pay a vendor invoice with a computer check</span></span>
<span data-ttu-id="5e0cd-124">The following describes how to pay a vendor by cheque.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-124">The following describes how to pay a vendor by check.</span></span> <span data-ttu-id="5e0cd-125">The steps are similar to refund a customer by cheque.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-125">The steps are similar to refund a customer by check.</span></span>

1. <span data-ttu-id="5e0cd-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="5e0cd-127">Fill in the payment journal lines.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-127">Fill in the payment journal lines.</span></span> <span data-ttu-id="5e0cd-128">For more information, see [Record Payments and Refunds](payables-how-post-payments-refunds.md).</span><span class="sxs-lookup"><span data-stu-id="5e0cd-128">For more information, see [Record Payments and Refunds](payables-how-post-payments-refunds.md).</span></span>
3. <span data-ttu-id="5e0cd-129">In the **Payment Method Code** field, select **Cheque**.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-129">In the **Payment Method Code** field, select **Check**.</span></span>
4. <span data-ttu-id="5e0cd-130">In the **Bank Payment Type** field, select **Computer Cheque**.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-130">In the **Bank Payment Type** field, select **Computer Check**.</span></span>
5. <span data-ttu-id="5e0cd-131">Choose the **Print Cheque** action.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-131">Choose the **Print Check** action.</span></span>
6. <span data-ttu-id="5e0cd-132">On the **Cheque** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-132">On the **Check** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. <span data-ttu-id="5e0cd-133">If your printer is set up to print cheques, choose the **Print** button.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-133">If your printer is set up to print checks, choose the **Print** button.</span></span> <span data-ttu-id="5e0cd-134">Otherwise, choose the **Send to** button, select the **PDF Document** option, choose the **OK** button, and then print the PDF document.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-134">Otherwise, choose the **Send to** button, select the **PDF Document** option, choose the **OK** button, and then print the PDF document.</span></span>

    <span data-ttu-id="5e0cd-135">The physical cheques can now be sent to the vendors for processing.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-135">The physical checks can now be sent to the vendors for processing.</span></span> <span data-ttu-id="5e0cd-136">Proceed to post the payment as applied to the vendor and thereby paid in the system.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-136">Proceed to post the payment as applied to the vendor and thereby paid in the system.</span></span>
8. <span data-ttu-id="5e0cd-137">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-137">Choose the **Post** action.</span></span>

<span data-ttu-id="5e0cd-138">Fully applied vendor ledger entries and bank ledger entries are created.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-138">Fully applied vendor ledger entries and bank ledger entries are created.</span></span>

> [!NOTE]  
> <span data-ttu-id="5e0cd-139">If you want to print and pay cheques in more than one currency from different bank accounts, you must run the **Print Cheque** batch job separately for each currency and specify the appropriate bank account.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-139">If you want to print and pay checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="5e0cd-140">To cancel printed cheques that are not posted</span><span class="sxs-lookup"><span data-stu-id="5e0cd-140">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="5e0cd-141">You can cancel non-posted cheques after they have been printed by using the **Void Cheque** action on the **Payment Journal** page.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-141">You can cancel non-posted checks after they have been printed by using the **Void Check** action on the **Payment Journal** page.</span></span>

1. <span data-ttu-id="5e0cd-142">On the **Payment Journal** page, choose the **Void Cheque**, and then choose which cheques to cancel.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-142">On the **Payment Journal** page, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="5e0cd-143">To void cheques</span><span class="sxs-lookup"><span data-stu-id="5e0cd-143">To void checks</span></span>

<span data-ttu-id="5e0cd-144">When cheque payment have been posted, you can only cancel (void) cheques from the resulting bank ledger entries.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-144">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5e0cd-145">If the cheque is applied to an invoice, unapply the cheque first so that the invoice can be repaid, and then void the cheque.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-145">If the check is applied to an invoice, unapply the check first so that the invoice can be repaid, and then void the check.</span></span> <span data-ttu-id="5e0cd-146">If the cheque was printed and did not pay an invoice, then choose **Void Cheque Only** as described in this section.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-146">If the check was printed and did not pay an invoice, then choose **Void Check Only** as described in this section.</span></span>

1. <span data-ttu-id="5e0cd-147">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-147">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="5e0cd-148">Select the relevant bank account, choose the **Edit** action, and then choose the **Cheque Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-148">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="5e0cd-149">On the **Cheque Ledger Entries** page, choose the **Void Cheque** action.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-149">On the **Check Ledger Entries** page, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="5e0cd-150">Select the **Void Cheque Only** check box.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-150">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="5e0cd-151">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-151">Choose the **OK** button.</span></span>

## <a name="to-view-a-summary-of-posted-checks"></a><span data-ttu-id="5e0cd-152">To view a summary of posted cheques</span><span class="sxs-lookup"><span data-stu-id="5e0cd-152">To view a summary of posted checks</span></span>
<span data-ttu-id="5e0cd-153">If you want to review posted cheques, for example to verify multiple cheques paid to one vendor, you can use the **Bank Account - Cheque Details** report.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-153">If you want to review posted checks, for example to verify multiple checks paid to one vendor, you can use the **Bank Account - Check Details** report.</span></span>
1. <span data-ttu-id="5e0cd-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Account - Cheque Details**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Account - Check Details**, and then choose the related link.</span></span>
2. <span data-ttu-id="5e0cd-155">Set filters as relevant, and then choose the **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="5e0cd-155">Set filters as relevant, and then choose the **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="5e0cd-156">See Also</span><span class="sxs-lookup"><span data-stu-id="5e0cd-156">See Also</span></span>
[<span data-ttu-id="5e0cd-157">Making Payments</span><span class="sxs-lookup"><span data-stu-id="5e0cd-157">Making Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="5e0cd-158">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="5e0cd-158">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="5e0cd-159">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="5e0cd-159">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="5e0cd-160">Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="5e0cd-160">Export a Positive Pay file</span></span>](finance-how-positive-pay.md)  
<span data-ttu-id="5e0cd-161">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5e0cd-161">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]