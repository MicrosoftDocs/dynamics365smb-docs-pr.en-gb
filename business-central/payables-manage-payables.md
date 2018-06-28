---
title: Overview of Tasks to Manage Accounts Payable| Microsoft Docs
description: Outlines tasks to manage accounts payable, for example, paying creditors or applying outgoing payments to ledger entries to close invoices or credit memos.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 06/28/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2286b728a464943841b192031cfea13644441013
ms.openlocfilehash: 730596534df93b7aa16f7975b5c5b1307a7f571a
ms.contentlocale: en-gb
ms.lasthandoff: 06/28/2018

---
# <a name="managing-payables"></a><span data-ttu-id="4aa52-103">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="4aa52-103">Managing Payables</span></span>
<span data-ttu-id="4aa52-104">A big part of managing accounts payable is paying your vendors, or reimbursing your employees for expenses.</span><span class="sxs-lookup"><span data-stu-id="4aa52-104">A big part of managing accounts payable is paying your vendors, or reimbursing your employees for expenses.</span></span> <span data-ttu-id="4aa52-105">You can use functions to add payments lines for purchase invoices that are due in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="4aa52-105">You can use functions to add payments lines for purchase invoices that are due in the **Payment Journal** window.</span></span> <span data-ttu-id="4aa52-106">To send transactions to your bank, you can export multiple payment journal lines to a file, and then upload the file to your bank.</span><span class="sxs-lookup"><span data-stu-id="4aa52-106">To send transactions to your bank, you can export multiple payment journal lines to a file, and then upload the file to your bank.</span></span> <span data-ttu-id="4aa52-107">You can also make payments by cheque, including transmitting cheques as electronic payments.</span><span class="sxs-lookup"><span data-stu-id="4aa52-107">You can also make payments by check, including transmitting checks as electronic payments.</span></span>

<span data-ttu-id="4aa52-108">Another typical task is to apply outgoing payments to their related vendor or employee ledger entries in order to close purchase invoices, purchase credit memos, or employee accounts as paid.</span><span class="sxs-lookup"><span data-stu-id="4aa52-108">Another typical task is to apply outgoing payments to their related vendor or employee ledger entries in order to close purchase invoices, purchase credit memos, or employee accounts as paid.</span></span> <span data-ttu-id="4aa52-109">You can do this in the **Payment Reconciliation Journal** window by importing a bank statement file to register the payments.</span><span class="sxs-lookup"><span data-stu-id="4aa52-109">You can do this in the **Payment Reconciliation Journal** window by importing a bank statement file to register the payments.</span></span> <span data-ttu-id="4aa52-110">The payments are applied to open vendor, customer, or employee ledger entries by matching payment text and entry information.</span><span class="sxs-lookup"><span data-stu-id="4aa52-110">The payments are applied to open vendor, customer, or employee ledger entries by matching payment text and entry information.</span></span> <span data-ttu-id="4aa52-111">There are various ways to review and change the matches before you post the journal.</span><span class="sxs-lookup"><span data-stu-id="4aa52-111">There are various ways to review and change the matches before you post the journal.</span></span> <span data-ttu-id="4aa52-112">You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal.</span><span class="sxs-lookup"><span data-stu-id="4aa52-112">You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal.</span></span> <span data-ttu-id="4aa52-113">The bank account is automatically reconciled when all payments are applied.</span><span class="sxs-lookup"><span data-stu-id="4aa52-113">The bank account is automatically reconciled when all payments are applied.</span></span>

<span data-ttu-id="4aa52-114">Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor or employee ledger entries.</span><span class="sxs-lookup"><span data-stu-id="4aa52-114">Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor or employee ledger entries.</span></span>

<span data-ttu-id="4aa52-115">The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="4aa52-115">The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.</span></span>

| <span data-ttu-id="4aa52-116">To</span><span class="sxs-lookup"><span data-stu-id="4aa52-116">To</span></span> | <span data-ttu-id="4aa52-117">See</span><span class="sxs-lookup"><span data-stu-id="4aa52-117">See</span></span> |
| --- | --- |
| <span data-ttu-id="4aa52-118">Generate due vendor payments or employee reimbursements, prepare cheque payments, and export payments to a bank file when posting.</span><span class="sxs-lookup"><span data-stu-id="4aa52-118">Generate due vendor payments or employee reimbursements, prepare check payments, and export payments to a bank file when posting.</span></span> |[<span data-ttu-id="4aa52-119">Making Payments</span><span class="sxs-lookup"><span data-stu-id="4aa52-119">Making Payments</span></span>](payables-make-payments.md) |
| <span data-ttu-id="4aa52-120">Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file.</span><span class="sxs-lookup"><span data-stu-id="4aa52-120">Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file.</span></span> |[<span data-ttu-id="4aa52-121">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="4aa52-121">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="4aa52-122">Apply vendor payments to unpaid purchase invoices manually.</span><span class="sxs-lookup"><span data-stu-id="4aa52-122">Apply vendor payments to unpaid purchase invoices manually.</span></span> |[<span data-ttu-id="4aa52-123">Reconcile Vendor Payments Manually</span><span class="sxs-lookup"><span data-stu-id="4aa52-123">Reconcile Vendor Payments Manually</span></span>](payables-how-apply-purchase-transactions-manually.md) |
|<span data-ttu-id="4aa52-124">Ensure correct inventory valuation by assigning added item costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing.</span><span class="sxs-lookup"><span data-stu-id="4aa52-124">Ensure correct inventory valuation by assigning added item costs, such as freight, physical handling, insurance, and transportation that you incur when purchasing.</span></span>|[<span data-ttu-id="4aa52-125">Use Item Charges to Account for Additional Trade Costs</span><span class="sxs-lookup"><span data-stu-id="4aa52-125">Use Item Charges to Account for Additional Trade Costs</span></span>](payables-how-assign-item-charges.md)|

## <a name="see-also"></a><span data-ttu-id="4aa52-126">See Also</span><span class="sxs-lookup"><span data-stu-id="4aa52-126">See Also</span></span>
[<span data-ttu-id="4aa52-127">Purchasing</span><span class="sxs-lookup"><span data-stu-id="4aa52-127">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="4aa52-128">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="4aa52-128">Managing Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="4aa52-129">Use Item Charges to Account for Additional Trade Costs</span><span class="sxs-lookup"><span data-stu-id="4aa52-129">Use Item Charges to Account for Additional Trade Costs</span></span>](payables-how-assign-item-charges.md)  
[<span data-ttu-id="4aa52-130">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="4aa52-130">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="4aa52-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4aa52-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 

