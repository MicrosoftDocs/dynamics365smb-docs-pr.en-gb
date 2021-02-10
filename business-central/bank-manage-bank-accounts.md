---
title: Manage Bank Accounts| Microsoft Docs
description: You must regularly reconcile bank ledger entries with the related bank transactions in your bank accounts.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7eb749c17ea9f17b3ef7c7c29c5dc9037fcbaf9c
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4752337"
---
# <a name="reconciling-bank-accounts"></a><span data-ttu-id="dabcc-103">Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="dabcc-103">Reconciling Bank Accounts</span></span>

<span data-ttu-id="dabcc-104">A bank reconciliation should be completed at regular intervals for all your bank accounts to ensure that the company's cash records are correct.</span><span class="sxs-lookup"><span data-stu-id="dabcc-104">A bank reconciliation should be completed at regular intervals for all your bank accounts to ensure that the company's cash records are correct.</span></span> <span data-ttu-id="dabcc-105">You do this by comparing and matching entries in your internal bank accounts with bank transactions at your bank, and then posting the balances to your internal bank accounts to make totals available to finance managers.</span><span class="sxs-lookup"><span data-stu-id="dabcc-105">You do this by comparing and matching entries in your internal bank accounts with bank transactions at your bank, and then posting the balances to your internal bank accounts to make totals available to finance managers.</span></span> <span data-ttu-id="dabcc-106">Bank reconciliation is also a practical way to discover and resolve missing payments and bookkeeping errors.</span><span class="sxs-lookup"><span data-stu-id="dabcc-106">Bank reconciliation is also a practical way to discover and resolve missing payments and bookkeeping errors.</span></span>

<span data-ttu-id="dabcc-107">You can perform the task on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span><span class="sxs-lookup"><span data-stu-id="dabcc-107">You can perform the task on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span></span> <span data-ttu-id="dabcc-108">Alternatively, you can perform this task on the **Payment Reconciliation Journal** page as part of processing the payments that are represented on a bank statement.</span><span class="sxs-lookup"><span data-stu-id="dabcc-108">Alternatively, you can perform this task on the **Payment Reconciliation Journal** page as part of processing the payments that are represented on a bank statement.</span></span> <span data-ttu-id="dabcc-109">On both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span><span class="sxs-lookup"><span data-stu-id="dabcc-109">On both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span></span>

> [!NOTE]  
> <span data-ttu-id="dabcc-110">In the North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for cheques and deposits but does not offer import of bank statement files.</span><span class="sxs-lookup"><span data-stu-id="dabcc-110">In the North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for checks and deposits but does not offer import of bank statement files.</span></span> <span data-ttu-id="dabcc-111">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span><span class="sxs-lookup"><span data-stu-id="dabcc-111">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span></span> <span data-ttu-id="dabcc-112">For more information, see [Reconcile Bank Accounts](LocalFunctionality/UnitedStates/how-to-reconcile-bank-accounts.md) under United States Local Functionality.</span><span class="sxs-lookup"><span data-stu-id="dabcc-112">For more information, see [Reconcile Bank Accounts](LocalFunctionality/UnitedStates/how-to-reconcile-bank-accounts.md) under United States Local Functionality.</span></span>

<span data-ttu-id="dabcc-113">Before you can manage your bank accounts within [!INCLUDE[prod_short](includes/prod_short.md)], you must set each bank account up as a bank account card.</span><span class="sxs-lookup"><span data-stu-id="dabcc-113">Before you can manage your bank accounts within [!INCLUDE[prod_short](includes/prod_short.md)], you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="dabcc-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span><span class="sxs-lookup"><span data-stu-id="dabcc-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="dabcc-115">For more information, see [Setting Up Banking](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="dabcc-115">For more information, see [Setting Up Banking](bank-setup-banking.md).</span></span>

<span data-ttu-id="dabcc-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="dabcc-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="dabcc-117">To</span><span class="sxs-lookup"><span data-stu-id="dabcc-117">To</span></span> | <span data-ttu-id="dabcc-118">See</span><span class="sxs-lookup"><span data-stu-id="dabcc-118">See</span></span> |
| --- | --- |
| <span data-ttu-id="dabcc-119">Reconcile bank accounts as a separate task on the **Bank Acc. Reconciliation** page.</span><span class="sxs-lookup"><span data-stu-id="dabcc-119">Reconcile bank accounts as a separate task on the **Bank Acc. Reconciliation** page.</span></span> |[<span data-ttu-id="dabcc-120">Reconcile Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="dabcc-120">Reconcile Bank Accounts</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="dabcc-121">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span><span class="sxs-lookup"><span data-stu-id="dabcc-121">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span></span> |[<span data-ttu-id="dabcc-122">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="dabcc-122">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |

> [!TIP]
> <span data-ttu-id="dabcc-123">Use bank reconciliation to help verify that your books are up-to-date, and do not post the reconciliation until you are satisfied with the reconciliation.</span><span class="sxs-lookup"><span data-stu-id="dabcc-123">Use bank reconciliation to help verify that your books are up-to-date, and do not post the reconciliation until you are satisfied with the reconciliation.</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="dabcc-124">See Related Training at [Microsoft Learn](/learn/paths/reconcile-bank-accounts-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="dabcc-124">See Related Training at [Microsoft Learn](/learn/paths/reconcile-bank-accounts-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="dabcc-125">See Also</span><span class="sxs-lookup"><span data-stu-id="dabcc-125">See Also</span></span>

[<span data-ttu-id="dabcc-126">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="dabcc-126">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="dabcc-127">Reconcile Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="dabcc-127">Reconcile Bank Accounts</span></span>](bank-how-reconcile-bank-accounts-separately.md)  
[<span data-ttu-id="dabcc-128">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="dabcc-128">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[<span data-ttu-id="dabcc-129">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="dabcc-129">Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)  
[<span data-ttu-id="dabcc-130">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="dabcc-130">Managing Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="dabcc-131">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="dabcc-131">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="dabcc-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dabcc-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="dabcc-133">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="dabcc-133">General Business Functionality</span></span>](ui-across-business-areas.md)
