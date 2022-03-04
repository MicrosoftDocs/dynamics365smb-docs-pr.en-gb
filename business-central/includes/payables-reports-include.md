---
author: edupont04
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: c2f5f4c264150802920169139c90c0456f9a27c4
ms.sourcegitcommit: cdb57f14960f58b1d36a1b373fbf35dfed5fad9e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/23/2022
ms.locfileid: "8334857"
---
The following table describes some of the key reports in purchase ledger reporting.

| Report | Description | Id | 
|--|--|--|
| [Aged Accounts Payable](https://businesscentral.dynamics.com?report=322) |Shows overdue balances for suppliers in overdue time intervals. The overdue amounts can be shown by due date, posting date, or by document date as needed. You can choose to show the amounts in local currency (LCY) and print details of the overdue documents. The time intervals can have headings with dates or with number of dates overdue, relative to the specified ageing by type.<br>This report is the main report for reconciling supplier ledger to G/L. Assuming that you have not allowed direct posting to the accounts used in the supplier posting groups' payables account, this report is a specification of the amounts you find in the general ledger.| 322|
| [Vendor - Balance to Date](https://businesscentral.dynamics.com?report=321) | Shows the supplier balance by the ending date of the specified date range. You can choose to display the supplier balance in your local currency (LCY). Select the **Include Unapplied Entries** field to show entries that have been closed by the ending date but have been un-applied (opened) at a later date. Select the **Show Entries with Zero Balance** to show suppliers with a balance of zero by the ending date of the date filter. The date filter applies to the detailed supplier ledger entries for the entries in the report. If you have payments later than the ending date that have been applied to invoices in within the date range, the invoices will appear in the report as they have not been closed as by the ending date. | 321 |
| [Vendor - Trial Balance](https://businesscentral.dynamics.com?report=329) | Shows the net changes for suppliers for the period specified in the date filter as well as the net change year-to-date for the financial year corresponding to the period selected. The report is grouped by supplier posting groups and will give a different view of the supplier ledger than the **Aged Purchase Ledger** report. **Note**: If you haven't set up any accounting period, the system will not know what financial year to use and will either show year-to-date from the most recent financial year defined or just select the period, which may or may not be from beginning of a year.|329 | 
| [Vendor - Detail Trial Balance](https://businesscentral.dynamics.com?report=304) | Shows all the supplier ledger entries within the specified date filter. The report shows the supplier's beginning balances relative to the date filter. | 304 | 
| [Purchase Statistics](https://businesscentral.dynamics.com?report=312) |[!INCLUDE [reports-purchase-statistics](reports-purchase-statistics.md)]<br>This report can also be used in purchase ledger as it's easier to do a quick look-up of posted payments, discounts, and other transactions for a given supplier.| 312 |
| [Vendor - Summary Ageing](https://businesscentral.dynamics.com?report=305)| Legacy report for aged purchase ledger. We recommend that you use **Aged Accounts Payables** report instead. You can choose a period length and a date to use as set *overdue per* date.|305| 
| [Payments on Hold](https://businesscentral.dynamics.com?report=319)| Shows supplier ledger entries where the **On Hold** field is not blank.| 319 |
| [Vendor Pre-Payment Journal](https://businesscentral.dynamics.com?report=317)|Shows the payment journal with payment discount and tolerance information. The report can be used to check payments before creating payment files and posting the journal. **Note**: The report will show payment discounts incorrectly when multiple credit memos have been used in an application. In this case, the payment discount for the additional credit memos will be shown as an un-applied amount.| 317 |
| [Vendor - List](https://businesscentral.dynamics.com?report=301)|Shows various kinds of basic information for suppliers, such as supplier posting group, discount and payment information, priority level and the supplier's default currency, and the supplier's current balance (in LCY). The report can be used, for example, to maintain the information in the Supplier table.|301|