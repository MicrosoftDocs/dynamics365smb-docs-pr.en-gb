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
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 9e5fe99fe822ca94758a3030659bf484f917fcaa
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2308387"
---
# <a name="managing-bank-accounts"></a><span data-ttu-id="91748-103">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="91748-103">Managing Bank Accounts</span></span>
<span data-ttu-id="91748-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span><span class="sxs-lookup"><span data-stu-id="91748-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="91748-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span><span class="sxs-lookup"><span data-stu-id="91748-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="91748-106">Alternatively, you can perform the task separately from payment processing, on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span><span class="sxs-lookup"><span data-stu-id="91748-106">Alternatively, you can perform the task separately from payment processing, on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span></span> <span data-ttu-id="91748-107">In both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span><span class="sxs-lookup"><span data-stu-id="91748-107">In both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span></span>

> [!NOTE]  
> <span data-ttu-id="91748-108">In North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for cheques and deposits but does not offer import of bank statement files.</span><span class="sxs-lookup"><span data-stu-id="91748-108">In North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for checks and deposits but does not offer import of bank statement files.</span></span> <span data-ttu-id="91748-109">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span><span class="sxs-lookup"><span data-stu-id="91748-109">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span></span> <span data-ttu-id="91748-110">For more information, see the "Reconcile Bank Accounts" section under United States Local Functionality.</span><span class="sxs-lookup"><span data-stu-id="91748-110">For more information, see the "Reconcile Bank Accounts" section under United States Local Functionality.</span></span>

<span data-ttu-id="91748-111">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span><span class="sxs-lookup"><span data-stu-id="91748-111">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span></span> <span data-ttu-id="91748-112">You perform this task on the **General Journal** page, in different ways depending on the currency of the funds.</span><span class="sxs-lookup"><span data-stu-id="91748-112">You perform this task on the **General Journal** page, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="91748-113">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span><span class="sxs-lookup"><span data-stu-id="91748-113">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="91748-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span><span class="sxs-lookup"><span data-stu-id="91748-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="91748-115">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="91748-115">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="91748-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="91748-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="91748-117">To</span><span class="sxs-lookup"><span data-stu-id="91748-117">To</span></span> | <span data-ttu-id="91748-118">See</span><span class="sxs-lookup"><span data-stu-id="91748-118">See</span></span> |
| --- | --- |
| <span data-ttu-id="91748-119">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span><span class="sxs-lookup"><span data-stu-id="91748-119">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span></span> |[<span data-ttu-id="91748-120">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="91748-120">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="91748-121">Reconcile bank accounts, including cheque ledger entries, as a separate task on the **Bank Acc. Reconciliation** page.</span><span class="sxs-lookup"><span data-stu-id="91748-121">Reconcile bank accounts, including check ledger entries, as a separate task on the **Bank Acc. Reconciliation** page.</span></span> |[<span data-ttu-id="91748-122">Reconcile Bank Accounts Separately</span><span class="sxs-lookup"><span data-stu-id="91748-122">Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="91748-123">Post transfers between bank accounts in the same currency or in different currencies.</span><span class="sxs-lookup"><span data-stu-id="91748-123">Post transfers between bank accounts in the same currency or in different currencies.</span></span> |[<span data-ttu-id="91748-124">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="91748-124">Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a><span data-ttu-id="91748-125">See Also</span><span class="sxs-lookup"><span data-stu-id="91748-125">See Also</span></span>
[<span data-ttu-id="91748-126">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="91748-126">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="91748-127">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="91748-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="91748-128">[Managing Payables](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="91748-128">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="91748-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="91748-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="91748-130">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="91748-130">General Business Functionality</span></span>](ui-across-business-areas.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 
