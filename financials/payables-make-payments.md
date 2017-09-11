---
title: Overview of Tasks to Manage Payments to Vendors| Microsoft Docs
description: Outlines tasks to manage payments to vendors or creditors, including posting payment lines and getting an overview of the balance due.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: d0b9020596484a8910db2f5720adfe159ad96fe7
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="make-payments"></a><span data-ttu-id="491cb-103">Make Payments</span><span class="sxs-lookup"><span data-stu-id="491cb-103">Make Payments</span></span>
<span data-ttu-id="491cb-104">When you make payments to vendors, you post the related payment lines in the **Payment Journal** window.</span><span class="sxs-lookup"><span data-stu-id="491cb-104">When you make payments to vendors, you post the related payment lines in the **Payment Journal** window.</span></span> <span data-ttu-id="491cb-105">You can use the **Suggest Vendor Payments** function to find payments that are due.</span><span class="sxs-lookup"><span data-stu-id="491cb-105">You can use the **Suggest Vendor Payments** function to find payments that are due.</span></span> <span data-ttu-id="491cb-106">You can also use the **Vendor - Summary Aging** report to get an overview of due payments.</span><span class="sxs-lookup"><span data-stu-id="491cb-106">You can also use the **Vendor - Summary Aging** report to get an overview of due payments.</span></span>

<span data-ttu-id="491cb-107">From the payment journal, you can print computer cheques or record when cheques are written.</span><span class="sxs-lookup"><span data-stu-id="491cb-107">From the payment journal, you can print computer checks or record when checks are written.</span></span> <span data-ttu-id="491cb-108">If you select **Computer Cheque** in the **Bank Payment Type** field, then any lines representing cheques must be printed before the payment journal can be posted.</span><span class="sxs-lookup"><span data-stu-id="491cb-108">If you select **Computer Check** in the **Bank Payment Type** field, then any lines representing checks must be printed before the payment journal can be posted.</span></span>

<span data-ttu-id="491cb-109">When the payments are posted, you can export them to a bank file for upload to your bank for processing.</span><span class="sxs-lookup"><span data-stu-id="491cb-109">When the payments are posted, you can export them to a bank file for upload to your bank for processing.</span></span>

<span data-ttu-id="491cb-110">After the payments are made at your bank, you must apply them to their related open vendor ledger entries.</span><span class="sxs-lookup"><span data-stu-id="491cb-110">After the payments are made at your bank, you must apply them to their related open vendor ledger entries.</span></span> <span data-ttu-id="491cb-111">You can do this manually or by importing a bank statement file and applying the payments automatically.</span><span class="sxs-lookup"><span data-stu-id="491cb-111">You can do this manually or by importing a bank statement file and applying the payments automatically.</span></span> <span data-ttu-id="491cb-112">For more information, see [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="491cb-112">For more information, see [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span>

<span data-ttu-id="491cb-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="491cb-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="491cb-114">To</span><span class="sxs-lookup"><span data-stu-id="491cb-114">To</span></span> | <span data-ttu-id="491cb-115">See</span><span class="sxs-lookup"><span data-stu-id="491cb-115">See</span></span> |
| --- | --- |
| <span data-ttu-id="491cb-116">Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity.</span><span class="sxs-lookup"><span data-stu-id="491cb-116">Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity.</span></span> |[<span data-ttu-id="491cb-117">How to: Suggest Vendor Payments</span><span class="sxs-lookup"><span data-stu-id="491cb-117">How to: Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md) |
| <span data-ttu-id="491cb-118">Issue cheques for payments, either as print-outs or as computer cheques.</span><span class="sxs-lookup"><span data-stu-id="491cb-118">Issue checks for payments, either as print-outs or as computer checks.</span></span> <span data-ttu-id="491cb-119">Void cheques before or after posting.</span><span class="sxs-lookup"><span data-stu-id="491cb-119">Void checks before or after posting.</span></span> |[<span data-ttu-id="491cb-120">How to: Work with Checks</span><span class="sxs-lookup"><span data-stu-id="491cb-120">How to: Work with Checks</span></span>](payables-how-work-checks.md) |
| <span data-ttu-id="491cb-121">Make sure that your bank only clears validated cheques and amounts by sending them a file that contains vendor, cheque, and payment information.</span><span class="sxs-lookup"><span data-stu-id="491cb-121">Make sure that your bank only clears validated checks and amounts by sending them a file that contains vendor, check, and payment information.</span></span> |[<span data-ttu-id="491cb-122">How to: Export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="491cb-122">How to: Export a Positive Pay file</span></span>](finance-how-positive-pay.md) |
|<span data-ttu-id="491cb-123">Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America.</span><span class="sxs-lookup"><span data-stu-id="491cb-123">Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America.</span></span> |[<span data-ttu-id="491cb-124">How to: Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="491cb-124">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  

## <a name="see-also"></a><span data-ttu-id="491cb-125">See Also</span><span class="sxs-lookup"><span data-stu-id="491cb-125">See Also</span></span>
[<span data-ttu-id="491cb-126">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="491cb-126">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="491cb-127">Purchasing</span><span class="sxs-lookup"><span data-stu-id="491cb-127">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="491cb-128">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="491cb-128">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="491cb-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="491cb-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

