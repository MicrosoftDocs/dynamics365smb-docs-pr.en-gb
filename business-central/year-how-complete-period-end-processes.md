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
# <a name="overview-of-tasks-to-close-accounting-periods"></a>Overview of Tasks to Close Accounting Periods
[!INCLUDE[d365fin](includes/d365fin_md.md)] does not force you to close periods, however, there are many period-end (month-end) activities that you can do. This topic provides an overview of optional processes and activities for closing periods.  

## <a name="general-ledger"></a>General Ledger
* Specify system-wide and user-specific posting periods.  

    This specifies the dates between which you allow posting. Depending on your business, you may want to allow posting at the start of the period, or toward the end. For more information, see [Specify Posting Periods](finance-how-specify-posting-periods.md).  
* Make all necessary G/L adjustments.  
* Update and post Recurring Journals.  
  <!--* Process Consolidations-->
* Run account schedules as follows:  
  * Open the **Account Schedule** page, and then choose the **Print** action.  

## <a name="sales-and-receivables"></a>Sales and Receivables
* Post all sales orders, invoices, credit memos, and return orders.  
* Post all cash receipt journals.  
* Update and post recurring journals that are related to sales and receivables.  
* Reconcile accounts receivable to the general ledger.  
* Run the **Delete Invoiced Sales Orders** batch job.  

## <a name="purchases-and-payables"></a>Purchases and Payables
* Post all purchase orders, invoices, credit memos, and return orders.  
* Post all payment journals.  
* Update and post recurring journals that are related to purchases & payables.  
* Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.  
* Run the **Delete Invoiced Purchase Orders** batch job.  

Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.

Intercompany
* Process Intercompany Transactions

## <a name="calculate-and-process-sales-tax"></a>Calculate and Process VAT
* Complete Tax Statements.  

## <a name="see-also"></a>See Also
[Closing Years and Periods](year-close-years-periods.md)  
[Closing Books](year-close-books.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
