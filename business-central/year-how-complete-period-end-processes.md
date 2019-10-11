---
title: Optional Activities for Closing Periods | Microsoft Docs
description: This topic outlines the optional processes and activities for closing accounting periods in Business Central.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 10/01/2019
ms.author: jswymer
ms.openlocfilehash: 1912a3e1731c2a6a86c5fd5eb93c7e2bf2ff8a1b
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2313791"
---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><span data-ttu-id="2ae9a-103">Overview of Tasks to Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="2ae9a-103">Overview of Tasks to Close Accounting Periods</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="2ae9a-104">does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-104">does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span></span> <span data-ttu-id="2ae9a-105">This topic provides an overview of optional processes and activities for closing periods.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-105">This topic provides an overview of optional processes and activities for closing periods.</span></span>  

## <a name="general-ledger"></a><span data-ttu-id="2ae9a-106">General Ledger</span><span class="sxs-lookup"><span data-stu-id="2ae9a-106">General Ledger</span></span>
* <span data-ttu-id="2ae9a-107">Specify system-wide and user-specific posting periods.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-107">Specify system-wide and user-specific posting periods.</span></span>  

    <span data-ttu-id="2ae9a-108">This specifies the dates between which you allow posting.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-108">This specifies the dates between which you allow posting.</span></span> <span data-ttu-id="2ae9a-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span></span> <span data-ttu-id="2ae9a-110">For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="2ae9a-110">For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).</span></span>  
* <span data-ttu-id="2ae9a-111">Make all necessary G/L adjustments.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-111">Make all necessary G/L adjustments.</span></span>  
* <span data-ttu-id="2ae9a-112">Update and post Recurring Journals.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-112">Update and post Recurring Journals.</span></span>  
  <!--* Process Consolidations-->
* <span data-ttu-id="2ae9a-113">Run account schedules as follows:</span><span class="sxs-lookup"><span data-stu-id="2ae9a-113">Run account schedules as follows:</span></span>  
  * <span data-ttu-id="2ae9a-114">Open the **Account Schedule** page, and then choose the **Print** action.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-114">Open the **Account Schedule** page, and then choose the **Print** action.</span></span>  

## <a name="sales-and-receivables"></a><span data-ttu-id="2ae9a-115">Sales and Receivables</span><span class="sxs-lookup"><span data-stu-id="2ae9a-115">Sales and Receivables</span></span>
* <span data-ttu-id="2ae9a-116">Post all sales orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="2ae9a-117">Post all cash receipt journals.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-117">Post all cash receipt journals.</span></span>  
* <span data-ttu-id="2ae9a-118">Update and post recurring journals that are related to sales and receivables.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-118">Update and post recurring journals that are related to sales and receivables.</span></span>  
* <span data-ttu-id="2ae9a-119">Reconcile accounts receivable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-119">Reconcile accounts receivable to the general ledger.</span></span>  
* <span data-ttu-id="2ae9a-120">Run the **Delete Invoiced Sales Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>  

## <a name="purchases-and-payables"></a><span data-ttu-id="2ae9a-121">Purchases and Payables</span><span class="sxs-lookup"><span data-stu-id="2ae9a-121">Purchases and Payables</span></span>
* <span data-ttu-id="2ae9a-122">Post all purchase orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="2ae9a-123">Post all payment journals.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-123">Post all payment journals.</span></span>  
* <span data-ttu-id="2ae9a-124">Update and post recurring journals that are related to purchases & payables.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-124">Update and post recurring journals that are related to purchases & payables.</span></span>  
* <span data-ttu-id="2ae9a-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>  
* <span data-ttu-id="2ae9a-126">Run the **Delete Invoiced Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>  

<span data-ttu-id="2ae9a-127">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="2ae9a-127">Fixed Assets</span></span>
* <span data-ttu-id="2ae9a-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span></span>
* <span data-ttu-id="2ae9a-129">Post adjustments.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-129">Post adjustments.</span></span>
* <span data-ttu-id="2ae9a-130">Post appreciation.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-130">Post appreciation.</span></span>
* <span data-ttu-id="2ae9a-131">Post depreciation.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-131">Post depreciation.</span></span>
* <span data-ttu-id="2ae9a-132">Update and post the recurring fixed asset journal.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-132">Update and post the recurring fixed asset journal.</span></span>

<span data-ttu-id="2ae9a-133">Intercompany</span><span class="sxs-lookup"><span data-stu-id="2ae9a-133">Intercompany</span></span>
* <span data-ttu-id="2ae9a-134">Process Intercompany Transactions</span><span class="sxs-lookup"><span data-stu-id="2ae9a-134">Process Intercompany Transactions</span></span>

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="2ae9a-135">Calculate and Process VAT</span><span class="sxs-lookup"><span data-stu-id="2ae9a-135">Calculate and Process Sales Tax</span></span>
* <span data-ttu-id="2ae9a-136">Complete Tax Statements.</span><span class="sxs-lookup"><span data-stu-id="2ae9a-136">Complete Tax Statements.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2ae9a-137">See Also</span><span class="sxs-lookup"><span data-stu-id="2ae9a-137">See Also</span></span>
[<span data-ttu-id="2ae9a-138">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="2ae9a-138">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="2ae9a-139">Closing Books</span><span class="sxs-lookup"><span data-stu-id="2ae9a-139">Closing Books</span></span>](year-close-books.md)  
<span data-ttu-id="2ae9a-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2ae9a-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
