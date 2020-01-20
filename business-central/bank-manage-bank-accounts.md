---
title: Manage Bank Accounts| Microsoft Docs
description: You must regularly reconcile bank ledger entries with the related bank transactions in your bank accounts.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 01/10/2020
ms.author: sgroespe
ms.openlocfilehash: 0d1a38468f5d07a1170027bc728ba16996f2b782
ms.sourcegitcommit: 2f741f442226b8be74586e355f283f365e43220f
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/10/2020
ms.locfileid: "2947244"
---
# <a name="reconciling-bank-accounts"></a><span data-ttu-id="ec657-103">Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="ec657-103">Reconciling Bank Accounts</span></span>
<span data-ttu-id="ec657-104">A bank reconciliation should be completed at regular intervals for all your bank accounts to ensure that the company's cash records are correct.</span><span class="sxs-lookup"><span data-stu-id="ec657-104">A bank reconciliation should be completed at regular intervals for all your bank accounts to ensure that the company's cash records are correct.</span></span> <span data-ttu-id="ec657-105">You do this by comparing and matching entries in your internal bank accounts with bank transactions at your bank, and then posting the balances to your internal bank accounts to make totals available to finance managers.</span><span class="sxs-lookup"><span data-stu-id="ec657-105">You do this by comparing and matching entries in your internal bank accounts with bank transactions at your bank, and then posting the balances to your internal bank accounts to make totals available to finance managers.</span></span> <span data-ttu-id="ec657-106">Bank reconciliation is also a practical way to discover and resolve missing payments and bookkeeping errors.</span><span class="sxs-lookup"><span data-stu-id="ec657-106">Bank reconciliation is also a practical way to discover and resolve missing payments and bookkeeping errors.</span></span>

<span data-ttu-id="ec657-107">You can perform the task on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span><span class="sxs-lookup"><span data-stu-id="ec657-107">You can perform the task on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span></span> <span data-ttu-id="ec657-108">Alternatively, you can perform this task on the **Payment Reconciliation Journal** page as part of processing the payments that are represented on a bank statement.</span><span class="sxs-lookup"><span data-stu-id="ec657-108">Alternatively, you can perform this task on the **Payment Reconciliation Journal** page as part of processing the payments that are represented on a bank statement.</span></span> <span data-ttu-id="ec657-109">On both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span><span class="sxs-lookup"><span data-stu-id="ec657-109">On both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span></span>

> [!NOTE]  
> <span data-ttu-id="ec657-110">In North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for cheques and deposits but does not offer import of bank statement files.</span><span class="sxs-lookup"><span data-stu-id="ec657-110">In North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for checks and deposits but does not offer import of bank statement files.</span></span> <span data-ttu-id="ec657-111">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span><span class="sxs-lookup"><span data-stu-id="ec657-111">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span></span> <span data-ttu-id="ec657-112">For more information, see the "Reconcile Bank Accounts" section under United States Local Functionality.</span><span class="sxs-lookup"><span data-stu-id="ec657-112">For more information, see the "Reconcile Bank Accounts" section under United States Local Functionality.</span></span>

<span data-ttu-id="ec657-113">Before you can manage your bank accounts within [!INCLUDE[d365fin](includes/d365fin_md.md)], you must set each bank account up as a bank account card.</span><span class="sxs-lookup"><span data-stu-id="ec657-113">Before you can manage your bank accounts within [!INCLUDE[d365fin](includes/d365fin_md.md)], you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="ec657-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span><span class="sxs-lookup"><span data-stu-id="ec657-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="ec657-115">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="ec657-115">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="ec657-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="ec657-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="ec657-117">To</span><span class="sxs-lookup"><span data-stu-id="ec657-117">To</span></span> | <span data-ttu-id="ec657-118">See</span><span class="sxs-lookup"><span data-stu-id="ec657-118">See</span></span> |
| --- | --- |
| <span data-ttu-id="ec657-119">Reconcile bank accounts as a separate task on the **Bank Acc. Reconciliation** page.</span><span class="sxs-lookup"><span data-stu-id="ec657-119">Reconcile bank accounts as a separate task on the **Bank Acc. Reconciliation** page.</span></span> |[<span data-ttu-id="ec657-120">Reconcile Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="ec657-120">Reconcile Bank Accounts</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="ec657-121">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span><span class="sxs-lookup"><span data-stu-id="ec657-121">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span></span> |[<span data-ttu-id="ec657-122">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="ec657-122">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |

## <a name="see-related-training-at-microsoft-learnlearnpathsreconcile-bank-accounts-dynamics-365-business-central"></a><span data-ttu-id="ec657-123">See Related Training at [Microsoft Learn](/learn/paths/reconcile-bank-accounts-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="ec657-123">See Related Training at [Microsoft Learn](/learn/paths/reconcile-bank-accounts-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="ec657-124">See Also</span><span class="sxs-lookup"><span data-stu-id="ec657-124">See Also</span></span>
[<span data-ttu-id="ec657-125">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="ec657-125">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="ec657-126">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="ec657-126">Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)  
[<span data-ttu-id="ec657-127">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="ec657-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="ec657-128">[Managing Payables](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="ec657-128">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="ec657-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ec657-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="ec657-130">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="ec657-130">General Business Functionality</span></span>](ui-across-business-areas.md)
