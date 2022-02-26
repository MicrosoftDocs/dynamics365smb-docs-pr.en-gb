---
title: Optional Activities for Closing Periods
description: This topic outlines the optional processes and activities for closing accounting periods in Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: overview
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 9442b0617691098b32e5012a5a708e14fe5a0187
ms.sourcegitcommit: 8464b37c4f1e5819aed81d9cfdc382fc3d0762fc
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/19/2022
ms.locfileid: "8012032"
---
# <a name="overview-of-tasks-to-close-accounting-periods"></a>Overview of Tasks to Close Accounting Periods

[!INCLUDE[prod_short](includes/prod_short.md)] does not force you to close periods, however, there are many period-end (month-end) activities that you can do. This topic provides an overview of optional processes and activities for closing periods.  

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

## <a name="fixed-assets"></a>Fixed Assets

* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.

## <a name="intercompany"></a>Intercompany

* Process Intercompany Transactions

## <a name="calculate-and-process-sales-tax"></a>Calculate and Process VAT

* Complete Tax Statements.  

## <a name="see-also"></a>See Also

[Closing Years and Periods](year-close-years-periods.md)  
[Closing Books](year-close-books.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]