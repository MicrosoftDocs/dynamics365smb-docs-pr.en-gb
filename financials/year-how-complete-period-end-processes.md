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
ms.date: 06/02/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 678cebc065594ed0ed6fea897676f109ff2c1dce
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><span data-ttu-id="d3294-103">Overview of Tasks to Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="d3294-103">Overview of Tasks to Close Accounting Periods</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="d3294-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span><span class="sxs-lookup"><span data-stu-id="d3294-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span></span> <span data-ttu-id="d3294-105">This topic provides an overview of optional processes and activities for closing periods.</span><span class="sxs-lookup"><span data-stu-id="d3294-105">This topic provides an overview of optional processes and activities for closing periods.</span></span>  

## <a name="general-ledger"></a><span data-ttu-id="d3294-106">General Ledger</span><span class="sxs-lookup"><span data-stu-id="d3294-106">General Ledger</span></span>
* <span data-ttu-id="d3294-107">Specify system-wide and user-specific posting periods.</span><span class="sxs-lookup"><span data-stu-id="d3294-107">Specify system-wide and user-specific posting periods.</span></span>  

    <span data-ttu-id="d3294-108">This specifies the dates between which you allow posting.</span><span class="sxs-lookup"><span data-stu-id="d3294-108">This specifies the dates between which you allow posting.</span></span> <span data-ttu-id="d3294-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span><span class="sxs-lookup"><span data-stu-id="d3294-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span></span> <span data-ttu-id="d3294-110">For more information, see [How to: Specify Posting Periods](finance-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="d3294-110">For more information, see [How to: Specify Posting Periods](finance-how-specify-posting-periods.md).</span></span>  
* <span data-ttu-id="d3294-111">Make all necessary G/L adjustments.</span><span class="sxs-lookup"><span data-stu-id="d3294-111">Make all necessary G/L adjustments.</span></span>  
* <span data-ttu-id="d3294-112">Update and post Recurring Journals.</span><span class="sxs-lookup"><span data-stu-id="d3294-112">Update and post Recurring Journals.</span></span>  
  <!--* Process Consolidations-->
* <span data-ttu-id="d3294-113">Run account schedules as follows:</span><span class="sxs-lookup"><span data-stu-id="d3294-113">Run account schedules as follows:</span></span>  
  * <span data-ttu-id="d3294-114">Open the **Account Schedule** window, and then choose the **Print** action.</span><span class="sxs-lookup"><span data-stu-id="d3294-114">Open the **Account Schedule** window, and then choose the **Print** action.</span></span>  

## <a name="sales-and-receivables"></a><span data-ttu-id="d3294-115">Sales and Receivables</span><span class="sxs-lookup"><span data-stu-id="d3294-115">Sales and Receivables</span></span>
* <span data-ttu-id="d3294-116">Post all sales orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="d3294-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="d3294-117">Post all cash receipt journals.</span><span class="sxs-lookup"><span data-stu-id="d3294-117">Post all cash receipt journals.</span></span>  
* <span data-ttu-id="d3294-118">Update and post recurring journals that are related to sales and receivables.</span><span class="sxs-lookup"><span data-stu-id="d3294-118">Update and post recurring journals that are related to sales and receivables.</span></span>  
* <span data-ttu-id="d3294-119">Reconcile accounts receivable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="d3294-119">Reconcile accounts receivable to the general ledger.</span></span>  
* <span data-ttu-id="d3294-120">Run the **Delete Invoiced Sales Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="d3294-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>  

## <a name="purchases-and-payables"></a><span data-ttu-id="d3294-121">Purchases and Payables</span><span class="sxs-lookup"><span data-stu-id="d3294-121">Purchases and Payables</span></span>
* <span data-ttu-id="d3294-122">Post all purchase orders, invoices, credit memos, and return orders.</span><span class="sxs-lookup"><span data-stu-id="d3294-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="d3294-123">Post all payment journals.</span><span class="sxs-lookup"><span data-stu-id="d3294-123">Post all payment journals.</span></span>  
* <span data-ttu-id="d3294-124">Update and post recurring journals that are related to purchases & payables.</span><span class="sxs-lookup"><span data-stu-id="d3294-124">Update and post recurring journals that are related to purchases & payables.</span></span>  
* <span data-ttu-id="d3294-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="d3294-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>  
* <span data-ttu-id="d3294-126">Run the **Delete Invoiced Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="d3294-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>  

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="d3294-127">Calculate and Process VAT</span><span class="sxs-lookup"><span data-stu-id="d3294-127">Calculate and Process Sales Tax</span></span>
* <span data-ttu-id="d3294-128">Complete Tax Statements.</span><span class="sxs-lookup"><span data-stu-id="d3294-128">Complete Tax Statements.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d3294-129">See Also</span><span class="sxs-lookup"><span data-stu-id="d3294-129">See Also</span></span>
[<span data-ttu-id="d3294-130">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="d3294-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="d3294-131">Closing Books</span><span class="sxs-lookup"><span data-stu-id="d3294-131">Closing Books</span></span>](year-close-books.md)  
<span data-ttu-id="d3294-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d3294-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

