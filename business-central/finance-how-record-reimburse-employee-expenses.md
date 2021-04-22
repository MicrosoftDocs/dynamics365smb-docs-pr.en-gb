---
title: Record and Reimburse Employees' Business-Related Expenses | Microsoft Docs
description: Post employees' expenses with the general journal to the employee's account and later post a payment to the employee's bank account to reimburse for the business-related expense.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: edef774738233890af240b20622cc40585d79116
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783829"
---
# <a name="record-and-reimburse-employees-expenses"></a><span data-ttu-id="0bebb-103">Record and Reimburse Employees' Expenses</span><span class="sxs-lookup"><span data-stu-id="0bebb-103">Record and Reimburse Employees' Expenses</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="0bebb-104">supports transactions for employee in a similar way as for vendors.</span><span class="sxs-lookup"><span data-stu-id="0bebb-104">supports transactions for employee in a similar way as for vendors.</span></span> <span data-ttu-id="0bebb-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0bebb-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span></span>

> [!NOTE]  
> <span data-ttu-id="0bebb-106">Employee transactions can be posted in the local currency only.</span><span class="sxs-lookup"><span data-stu-id="0bebb-106">Employee transactions can be posted in the local currency only.</span></span> <span data-ttu-id="0bebb-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span><span class="sxs-lookup"><span data-stu-id="0bebb-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span></span>

<span data-ttu-id="0bebb-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span><span class="sxs-lookup"><span data-stu-id="0bebb-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span></span> <span data-ttu-id="0bebb-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span><span class="sxs-lookup"><span data-stu-id="0bebb-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span></span>  

> [!TIP]
> <span data-ttu-id="0bebb-110">This article explains how to record the expense in the books and how to reimburse the employee.</span><span class="sxs-lookup"><span data-stu-id="0bebb-110">This article explains how to record the expense in the books and how to reimburse the employee.</span></span> <span data-ttu-id="0bebb-111">Your organisation may have a portal or app where employees can submit their expense reports.</span><span class="sxs-lookup"><span data-stu-id="0bebb-111">Your organization may have a portal or app where employees can submit their expense reports.</span></span>

## <a name="to-record-an-employees-expense"></a><span data-ttu-id="0bebb-112">To record an employee's expense</span><span class="sxs-lookup"><span data-stu-id="0bebb-112">To record an employee's expense</span></span>
<span data-ttu-id="0bebb-113">You post employees' expenses on the **General Journal** page.</span><span class="sxs-lookup"><span data-stu-id="0bebb-113">You post employees' expenses on the **General Journal** page.</span></span>
1. <span data-ttu-id="0bebb-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0bebb-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="0bebb-115">Open the relevant general journal batch.</span><span class="sxs-lookup"><span data-stu-id="0bebb-115">Open the relevant general journal batch.</span></span> <span data-ttu-id="0bebb-116">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="0bebb-116">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="0bebb-117">On a new journal line, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0bebb-117">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="0bebb-118">Repeat step 3 for all the expenses that the employee has incurred.</span><span class="sxs-lookup"><span data-stu-id="0bebb-118">Repeat step 3 for all the expenses that the employee has incurred.</span></span>

    > [!TIP]  
    > <span data-ttu-id="0bebb-119">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span><span class="sxs-lookup"><span data-stu-id="0bebb-119">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="0bebb-120">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span><span class="sxs-lookup"><span data-stu-id="0bebb-120">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span></span>
5. <span data-ttu-id="0bebb-121">Choose the **Post** action to record the expenses on the employee's account.</span><span class="sxs-lookup"><span data-stu-id="0bebb-121">Choose the **Post** action to record the expenses on the employee's account.</span></span>

## <a name="to-reimburse-an-employee"></a><span data-ttu-id="0bebb-122">To reimburse an employee</span><span class="sxs-lookup"><span data-stu-id="0bebb-122">To reimburse an employee</span></span>
<span data-ttu-id="0bebb-123">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span><span class="sxs-lookup"><span data-stu-id="0bebb-123">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span></span>
1. <span data-ttu-id="0bebb-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0bebb-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="0bebb-125">Open the relevant payment journal batch.</span><span class="sxs-lookup"><span data-stu-id="0bebb-125">Open the relevant payment journal batch.</span></span> <span data-ttu-id="0bebb-126">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="0bebb-126">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="0bebb-127">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0bebb-127">Fill in the fields as necessary.</span></span> <span data-ttu-id="0bebb-128">For more information, see [Making Payments](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="0bebb-128">For more information, see [Making Payments](payables-make-payments.md).</span></span>
4. <span data-ttu-id="0bebb-129">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span><span class="sxs-lookup"><span data-stu-id="0bebb-129">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span></span>
5. <span data-ttu-id="0bebb-130">Choose the **Post** action to register the reimbursement.</span><span class="sxs-lookup"><span data-stu-id="0bebb-130">Choose the **Post** action to register the reimbursement.</span></span>  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a><span data-ttu-id="0bebb-131">To reconcile reimbursements with employee ledger entries</span><span class="sxs-lookup"><span data-stu-id="0bebb-131">To reconcile reimbursements with employee ledger entries</span></span>
<span data-ttu-id="0bebb-132">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span><span class="sxs-lookup"><span data-stu-id="0bebb-132">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span></span> <span data-ttu-id="0bebb-133">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="0bebb-133">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span> <span data-ttu-id="0bebb-134">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span><span class="sxs-lookup"><span data-stu-id="0bebb-134">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span></span> <span data-ttu-id="0bebb-135">For more information, see the related [Reconcile Vendor Payments with the Payment Journal or from Vendor Ledger Entries](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="0bebb-135">For more information, see the related [Reconcile Vendor Payments with the Payment Journal or from Vendor Ledger Entries](payables-how-apply-purchase-transactions-manually.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="0bebb-136">See Also</span><span class="sxs-lookup"><span data-stu-id="0bebb-136">See Also</span></span>
[<span data-ttu-id="0bebb-137">Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="0bebb-137">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="0bebb-138">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="0bebb-138">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="0bebb-139">Reverse Journal Postings and Undo Receipts/Shipments</span><span class="sxs-lookup"><span data-stu-id="0bebb-139">Reverse Journal Postings and Undo Receipts/Shipments</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="0bebb-140">Finance</span><span class="sxs-lookup"><span data-stu-id="0bebb-140">Finance</span></span>](finance.md)  
<span data-ttu-id="0bebb-141">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0bebb-141">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]