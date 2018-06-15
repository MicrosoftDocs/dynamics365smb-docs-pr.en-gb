---
title: Issue, Print, Cancel, and Void Checks| Microsoft Docs
description: Describes how to issue cheques using the payment journal, print cheques, and void or view cheque ledger entries in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment journal, print check, vendor payment, creditor, debt, balance due, AP
ms.date: 04/25/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: db28ad9a4adb45514b1d1287d269d8daefe64865
ms.openlocfilehash: 39b48fbd34b29db56b39712fbd2cbf5dc91fefc6
ms.contentlocale: en-gb
ms.lasthandoff: 04/26/2018

---
# <a name="make-check-payments"></a><span data-ttu-id="bc3a4-103">Make Cheque Payments</span><span class="sxs-lookup"><span data-stu-id="bc3a4-103">Make Check Payments</span></span>
<span data-ttu-id="bc3a4-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="bc3a4-104">You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="bc3a4-105">Both methods use the payment journal to issue checks to vendors.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-105">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="bc3a4-106">You can also void cheques and view cheque ledger entries.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-106">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="bc3a4-107">The following procedure shows how to pay a vendor with a computer cheque by applying the payment to the relevant vendor invoice, printing the cheque, and then posting the payment as paid.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-107">The following procedure shows how to pay a vendor with a computer checks by applying the payment to the relevant vendor invoice, printing the check, and then posting the payment as paid.</span></span> <span data-ttu-id="bc3a4-108">This results in positive vendor ledger entries, applied to negative bank ledger entries, and physical cheques for processing in the bank.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-108">This results in positive vendor ledger entries, applied to negative bank ledger entries, and physical checks for processing in the bank.</span></span>

<span data-ttu-id="bc3a4-109">You can pay with two types of cheque.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-109">You can pay with two types of checks.</span></span> <span data-ttu-id="bc3a4-110">For both types, the **Bal. Account Type** or the **Account Type** field must contain **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-110">For both types, the **Bal. Account Type** or the **Account Type** field must contain **Bank Account**.</span></span>

- <span data-ttu-id="bc3a4-111">**Computer Cheque**: Select this option if you want to print a cheque for the amount on the payment journal line.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-111">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="bc3a4-112">You must print the checks before you can post the journal lines.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-112">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="bc3a4-113">You can only select **Computer Cheque** if</span><span class="sxs-lookup"><span data-stu-id="bc3a4-113">You can only select **Computer Check** if</span></span>
- <span data-ttu-id="bc3a4-114">**Manual Cheque**: Select this option if you have created a cheque manually and want to create a corresponding cheque ledger entry for this amount.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-114">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="bc3a4-115">By using this option, you cannot print the cheque.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-115">By using this option, you cannot print the check.</span></span>

> [!NOTE]  
> <span data-ttu-id="bc3a4-116">To make sure that your bank only clears validated cheques and amounts, you can send them a file that contains vendor, cheque, and payment information.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-116">To make sure that your bank only clears validated checks and amounts, you can send them a file that contains vendor, check, and payment information.</span></span> <span data-ttu-id="bc3a4-117">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span><span class="sxs-lookup"><span data-stu-id="bc3a4-117">For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).</span></span>

<span data-ttu-id="bc3a4-118">Your printer must be correctly set up with the cheque forms, and you must define which cheque layout to use.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-118">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="bc3a4-119">For more information, see [Define Cheque Layouts](finance-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="bc3a4-119">For more information, see [Define Check Layouts](finance-how-define-check-layouts.md)</span></span>

## <a name="to-pay-a-vendor-invoice-with-a-computer-check"></a><span data-ttu-id="bc3a4-120">To pay a vendor invoice with a computer cheque</span><span class="sxs-lookup"><span data-stu-id="bc3a4-120">To pay a vendor invoice with a computer check</span></span>
<span data-ttu-id="bc3a4-121">The following describes how to pay a vendor by cheque.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-121">The following describes how to pay a vendor by check.</span></span> <span data-ttu-id="bc3a4-122">The steps are similar to refund a customer by cheque.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-122">The steps are similar to refund a customer by check.</span></span>

1. <span data-ttu-id="bc3a4-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="bc3a4-124">Fill in the payment journal lines.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-124">Fill in the payment journal lines.</span></span> <span data-ttu-id="bc3a4-125">For more information, see [Record Payments and Refunds](payables-how-post-payments-refunds.md).</span><span class="sxs-lookup"><span data-stu-id="bc3a4-125">For more information, see [Record Payments and Refunds](payables-how-post-payments-refunds.md).</span></span>
3. <span data-ttu-id="bc3a4-126">In the **Payment Method Code** field, select **Cheque**.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-126">In the **Payment Method Code** field, select **Check**.</span></span>
4. <span data-ttu-id="bc3a4-127">In the **Bank Payment Type** field, select **Computer Cheque**.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-127">In the **Bank Payment Type** field, select **Computer Check**.</span></span>
5. <span data-ttu-id="bc3a4-128">Choose the **Print Cheque** action.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-128">Choose the **Print Check** action.</span></span>
6. <span data-ttu-id="bc3a4-129">In the **Check** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-129">In the **Check** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. <span data-ttu-id="bc3a4-130">Choose the **Send to** button, select the **PDF Document** option, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-130">Choose the **Send to** button, select the **PDF Document** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="bc3a4-131">The physical cheques can now be brought to the bank for processing.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-131">The physical checks can now be brought to the bank for processing.</span></span> <span data-ttu-id="bc3a4-132">Proceed to post the payment as applied to the vendor and thereby paid in the system.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-132">Proceed to post the payment as applied to the vendor and thereby paid in the system.</span></span>
8. <span data-ttu-id="bc3a4-133">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-133">Choose the **Post** action.</span></span>

<span data-ttu-id="bc3a4-134">Fully applied vendor ledger entries and bank ledger entries are created.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-134">Fully applied vendor ledger entries and bank ledger entries are created.</span></span>

> [!NOTE]  
> <span data-ttu-id="bc3a4-135">If you want to print and pay cheques in more than one currency from different bank accounts, you must run the **Print Cheque** batch job separately for each currency and specify the appropriate bank account.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-135">If you want to print and pay checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="bc3a4-136">To cancel printed cheques that are not posted</span><span class="sxs-lookup"><span data-stu-id="bc3a4-136">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="bc3a4-137">You can cancel non-posted cheques after they have been printed by using the **Void Cheque** action in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-137">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>

1. <span data-ttu-id="bc3a4-138">In the **Payment Journal** window, choose the **Void Cheque**, and then choose which cheques to cancel.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-138">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="bc3a4-139">To void cheques</span><span class="sxs-lookup"><span data-stu-id="bc3a4-139">To void checks</span></span>
<span data-ttu-id="bc3a4-140">When cheque payment have been posted, you can only cancel (void) cheques from the resulting bank ledger entries.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-140">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="bc3a4-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="bc3a4-142">Select the relevant bank account, choose the **Edit** action, and then choose the **Cheque Ledger Entries** action.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-142">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="bc3a4-143">In the **Cheque Ledger Entries** window, choose the **Void Cheque** action.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-143">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="bc3a4-144">Select the **Void Cheque Only** check box.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-144">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="bc3a4-145">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-145">Choose the **OK** button.</span></span>

## <a name="to-view-a-summary-of-posted-checks"></a><span data-ttu-id="bc3a4-146">To view a summary of posted cheques</span><span class="sxs-lookup"><span data-stu-id="bc3a4-146">To view a summary of posted checks</span></span>
<span data-ttu-id="bc3a4-147">If you want to review posted cheques, for example to verify multiple cheques paid to one vendor, you can use the **Bank Account - Cheque Details** report.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-147">If you want to review posted checks, for example to verify multiple checks paid to one vendor, you can use the **Bank Account - Check Details** report.</span></span>
1. <span data-ttu-id="bc3a4-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Account - Cheque Details**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Account - Check Details**, and then choose the related link.</span></span>
2. <span data-ttu-id="bc3a4-149">Set filters as relevant, and then choose the **Preview** button.</span><span class="sxs-lookup"><span data-stu-id="bc3a4-149">Set filters as relevant, and then choose the **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="bc3a4-150">See Also</span><span class="sxs-lookup"><span data-stu-id="bc3a4-150">See Also</span></span>
[<span data-ttu-id="bc3a4-151">Making Payments</span><span class="sxs-lookup"><span data-stu-id="bc3a4-151">Making Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="bc3a4-152">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="bc3a4-152">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="bc3a4-153">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="bc3a4-153">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="bc3a4-154">Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="bc3a4-154">Export a Positive Pay file</span></span>](finance-how-positive-pay.md)  
<span data-ttu-id="bc3a4-155">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bc3a4-155">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

