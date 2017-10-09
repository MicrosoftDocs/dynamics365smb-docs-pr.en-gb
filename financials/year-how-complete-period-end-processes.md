---
title: Optional Activities for Closing Periods | Microsoft Docs
description: This topic outlines the optional processes and activities for closing accounting periods in Financials.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 06/19/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: eea34afbee429d14ab150894729cb4ea3843bb2b
ms.openlocfilehash: ddc2dbda549414a7beecf5f307c525b53166fa15
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><span data-ttu-id="e049a-103">Overview of Tasks to Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="e049a-103">Overview of Tasks to Close Accounting Periods</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="e049a-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span><span class="sxs-lookup"><span data-stu-id="e049a-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span></span> <span data-ttu-id="e049a-105">This topic provides an overview of optional processes and activities for closing periods.</span><span class="sxs-lookup"><span data-stu-id="e049a-105">This topic provides an overview of optional processes and activities for closing periods.</span></span>  

## <a name="general-ledger"></a><span data-ttu-id="e049a-106">General Ledger</span><span class="sxs-lookup"><span data-stu-id="e049a-106">General Ledger</span></span>
* <span data-ttu-id="e049a-107">Specify system-wide and user-specific posting periods.</span><span class="sxs-lookup"><span data-stu-id="e049a-107">Specify system-wide and user-specific posting periods.</span></span>  

    <span data-ttu-id="e049a-108">This specifies the dates between which you allow posting.</span><span class="sxs-lookup"><span data-stu-id="e049a-108">This specifies the dates between which you allow posting.</span></span> <span data-ttu-id="e049a-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span><span class="sxs-lookup"><span data-stu-id="e049a-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span></span> <span data-ttu-id="e049a-110">For more information, see [How to: Specify Posting Periods](finance-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="e049a-110">For more information, see [How to: Specify Posting Periods](finance-how-specify-posting-periods.md).</span></span>  
* <span data-ttu-id="e049a-111">Make all necessary G/L adjustments.</span><span class="sxs-lookup"><span data-stu-id="e049a-111">Make all necessary G/L adjustments.</span></span>  
* <span data-ttu-id="e049a-112">Update and post Recurring Journals.</span><span class="sxs-lookup"><span data-stu-id="e049a-112">Update and post Recurring Journals.</span></span>  
  <!--* Process Consolidations-->
* <span data-ttu-id="e049a-113">Run account schedules as follows:</span><span class="sxs-lookup"><span data-stu-id="e049a-113">Run account schedules as follows:</span></span>  
  * <span data-ttu-id="e049a-114">Open the **Account Schedule** window, and then choose the **Print** action.</span><span class="sxs-lookup"><span data-stu-id="e049a-114">Open the **Account Schedule** window, and then choose the **Print** action.</span></span>  

## <a name="sales-and-receivables"></a><span data-ttu-id="e049a-115">Sales and Receivables</span><span class="sxs-lookup"><span data-stu-id="e049a-115">Sales and Receivables</span></span>
* <span data-ttu-id="e049a-116">Post all sales orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="e049a-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="e049a-117">Post all cash receipt journals.</span><span class="sxs-lookup"><span data-stu-id="e049a-117">Post all cash receipt journals.</span></span>  
* <span data-ttu-id="e049a-118">Update and post recurring journals that are related to sales and receivables.</span><span class="sxs-lookup"><span data-stu-id="e049a-118">Update and post recurring journals that are related to sales and receivables.</span></span>  
* <span data-ttu-id="e049a-119">Reconcile accounts receivable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="e049a-119">Reconcile accounts receivable to the general ledger.</span></span>  
* <span data-ttu-id="e049a-120">Run the **Delete Invoiced Sales Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="e049a-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>  

## <a name="purchases-and-payables"></a><span data-ttu-id="e049a-121">Purchases and Payables</span><span class="sxs-lookup"><span data-stu-id="e049a-121">Purchases and Payables</span></span>
* <span data-ttu-id="e049a-122">Post all purchase orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="e049a-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="e049a-123">Post all payment journals.</span><span class="sxs-lookup"><span data-stu-id="e049a-123">Post all payment journals.</span></span>  
* <span data-ttu-id="e049a-124">Update and post recurring journals that are related to purchases & payables.</span><span class="sxs-lookup"><span data-stu-id="e049a-124">Update and post recurring journals that are related to purchases & payables.</span></span>  
* <span data-ttu-id="e049a-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="e049a-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>  
* <span data-ttu-id="e049a-126">Run the **Delete Invoiced Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="e049a-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>  

<span data-ttu-id="e049a-127">Fixed Assets</span><span class="sxs-lookup"><span data-stu-id="e049a-127">Fixed Assets</span></span>
* <span data-ttu-id="e049a-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span><span class="sxs-lookup"><span data-stu-id="e049a-128">Post all maintenance costs have been posted through the fixed asset journals or invoices.</span></span>
* <span data-ttu-id="e049a-129">Post adjustments.</span><span class="sxs-lookup"><span data-stu-id="e049a-129">Post adjustments.</span></span>
* <span data-ttu-id="e049a-130">Post appreciation.</span><span class="sxs-lookup"><span data-stu-id="e049a-130">Post appreciation.</span></span>
* <span data-ttu-id="e049a-131">Post depreciation.</span><span class="sxs-lookup"><span data-stu-id="e049a-131">Post depreciation.</span></span>
* <span data-ttu-id="e049a-132">Update and post the recurring fixed asset journal.</span><span class="sxs-lookup"><span data-stu-id="e049a-132">Update and post the recurring fixed asset journal.</span></span>

<span data-ttu-id="e049a-133">Intercompany</span><span class="sxs-lookup"><span data-stu-id="e049a-133">Intercompany</span></span>
* <span data-ttu-id="e049a-134">Process Intercompany Transactions</span><span class="sxs-lookup"><span data-stu-id="e049a-134">Process Intercompany Transactions</span></span>

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="e049a-135">Calculate and Process VAT</span><span class="sxs-lookup"><span data-stu-id="e049a-135">Calculate and Process Sales Tax</span></span>
* <span data-ttu-id="e049a-136">Complete Tax Statements.</span><span class="sxs-lookup"><span data-stu-id="e049a-136">Complete Tax Statements.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e049a-137">See Also</span><span class="sxs-lookup"><span data-stu-id="e049a-137">See Also</span></span>
[<span data-ttu-id="e049a-138">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="e049a-138">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="e049a-139">Closing Books</span><span class="sxs-lookup"><span data-stu-id="e049a-139">Closing Books</span></span>](year-close-books.md)  
<span data-ttu-id="e049a-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e049a-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

