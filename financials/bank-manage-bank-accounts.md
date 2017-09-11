---
title: Manage Bank Accounts| Microsoft Docs
description: You must regularly reconcile bank ledger entries in Financials with the related bank transactions in your bank accounts.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: dcefa921d7e8b901d906085e6bce01d6e0aa6ac4
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="managing-bank-accounts"></a><span data-ttu-id="3fda8-103">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="3fda8-103">Managing Bank Accounts</span></span>
<span data-ttu-id="3fda8-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span><span class="sxs-lookup"><span data-stu-id="3fda8-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="3fda8-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span><span class="sxs-lookup"><span data-stu-id="3fda8-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="3fda8-106">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports cheque ledger entries.</span><span class="sxs-lookup"><span data-stu-id="3fda8-106">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="3fda8-107">In both cases, you fill in the windows by importing the bank statement into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3fda8-107">In both cases, you fill in the windows by importing the bank statement into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="3fda8-108">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span><span class="sxs-lookup"><span data-stu-id="3fda8-108">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span></span> <span data-ttu-id="3fda8-109">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span><span class="sxs-lookup"><span data-stu-id="3fda8-109">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="3fda8-110">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span><span class="sxs-lookup"><span data-stu-id="3fda8-110">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="3fda8-111">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span><span class="sxs-lookup"><span data-stu-id="3fda8-111">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="3fda8-112">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="3fda8-112">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="3fda8-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="3fda8-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="3fda8-114">To</span><span class="sxs-lookup"><span data-stu-id="3fda8-114">To</span></span> | <span data-ttu-id="3fda8-115">See</span><span class="sxs-lookup"><span data-stu-id="3fda8-115">See</span></span> |
| --- | --- |
| <span data-ttu-id="3fda8-116">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span><span class="sxs-lookup"><span data-stu-id="3fda8-116">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span> |[<span data-ttu-id="3fda8-117">Apply Payments Automatically and Reconcile Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="3fda8-117">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="3fda8-118">Reconcile bank accounts, including cheque ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span><span class="sxs-lookup"><span data-stu-id="3fda8-118">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span> |[<span data-ttu-id="3fda8-119">How to: Reconcile Bank Accounts Separately</span><span class="sxs-lookup"><span data-stu-id="3fda8-119">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="3fda8-120">Post transfers between bank accounts in the same currency or in different currencies.</span><span class="sxs-lookup"><span data-stu-id="3fda8-120">Post transfers between bank accounts in the same currency or in different currencies.</span></span> |[<span data-ttu-id="3fda8-121">How to: Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="3fda8-121">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a><span data-ttu-id="3fda8-122">See Also</span><span class="sxs-lookup"><span data-stu-id="3fda8-122">See Also</span></span>
[<span data-ttu-id="3fda8-123">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="3fda8-123">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="3fda8-124">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="3fda8-124">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="3fda8-125">[Managing Payables](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="3fda8-125">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="3fda8-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3fda8-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="3fda8-127">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="3fda8-127">General Business Functionality</span></span>](ui-across-business-areas.md)  

