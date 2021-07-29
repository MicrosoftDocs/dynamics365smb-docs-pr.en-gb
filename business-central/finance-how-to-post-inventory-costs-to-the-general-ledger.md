---
title: How to Post Stock Costs to the General Ledger
description: At the end of accounting periods a sequence of cost control and auditing tasks must be performed to report a correct and balanced stock value.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: 74a2e257df3306a76d777559a5a157aa2b9ddec9
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6442142"
---
# <a name="reconcile-inventory-costs-with-the-general-ledger"></a>Reconcile Stock Costs with the General Ledger
When you post stock transactions, such as sales shipments, purchase invoices, or stock adjustments, the changed item costs are recorded in item value entries. To reflect this change of stock value in your financial books, the stock costs are automatically posted to the related stock accounts in the general ledger. For each stock transaction that you post, the appropriate values are posted to the stock account, adjustment account, and COGS account in the general ledger.

Automatic cost posting is defined by the **Automatic Cost Posting** field on the **Stock Setup** page.

Even though stock costs are automatically posted to the general ledger, it is still necessary to ensure that the costs of goods are forwarded to the related outbound sales transaction, especially in situations where you sell goods before you invoice the purchase of those goods. This is referred to as cost adjustment. Item costs are automatically adjusted when you post item transactions, but you can also adjust item costs manually. For more information, see [Adjust Item Costs](inventory-how-adjust-item-costs.md).

## <a name="to-post-inventory-costs-manually"></a>To post stock costs manually
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Post Stock Cost to G/L**, and then choose the related link.
2. Post stock costs to the general ledger manually by running the batch job. When you run this batch job, general ledger entries are created on the basis of value entries. You can post the entries so that they are summarized per posting group.

> [!NOTE]  
> When you run this batch job, you might encounter errors having to do with missing setup or incompatible dimension setup. If the batch job encounters errors in the dimension setup, it overrides these errors and uses the dimensions of the value entry. For any other errors, the batch job skips posting the value entries and lists them at the end of the report in a section titled “Skipped Entries.” To post these entries, you must fix the errors.

To see a list of errors before running the posting batch job, you can run the **Post Invt. Cost to G/L - Test** report. The test report lists all the errors encountered during a test posting. You can then fix the errors, and run the stock cost posting batch job without skipping any entries.

If you would like to simply get an overview of what values could be posted to the general ledger without actually performing the posting, you can run the **Post Stock Cost to G/L** batch job without actually posting the values to the general ledger. You do this by clearing the check mark from the **Post** field on the request page. This way, when you run the batch job, the report is produced showing the values that are ready to be posted to the general ledger, but they are not posted.

## <a name="to-audit-the-reconciliation-between-the-inventory-ledger-and-the-general-ledger"></a>To audit the reconciliation between the stock ledger and the general ledger
The **Stock - G/L Reconciliation** page provides the following:

- Exposes reconciliation differences by comparing what is recorded in G/L and what is recorded in the stock ledger (value entries).
- Displays unreconciled cost amounts in the value entries in the stock ledger as if they were mapped to corresponding stock-related accounts in G/L and compares those to the totals actually recorded in the same accounts in G/L.
- Reflects the double entry structure of G/L by visually presenting data as such. For example, a COGS entry has a corresponding stock entry.
- Lets users drill down and see the entries that make up the cost amounts.
- Includes filters to narrow the analysis by date, item, and location.
- Explains reasons for reconciliation differences in informative messages.


The **Name** column on the far left in the grid lists the various G/L account types that are associated with stock.

The **Stock**, **Stock (Interim)**, and **WIP Stock** columns show the invoiced, non-invoiced, and WIP totals of each G/L account type. These are calculated from value entries, that is, they are projected onto the G/L account types where they will end when they are eventually posted to G/L.

The **Total** column shows the sum (in bold font) of the value entry amounts in the three stock columns.

The **G/L Total** column shows the amounts (in bold font) for each G/L account type that exists in G/L. These are calculated from G/L entries, that is, they represent stock costs already posted to G/L.

The **Difference** column represents the difference between the value in the **G/L Total** and **Total** fields.

In the top of the **Stock - G/L Reconciliation** page, you can enter filters to limit, for example, the period of time for which you want information.

If you select the **Show Warning** check box and if there are any discrepancies between the stock totals and G/L totals, application shows messages in the **Warning** field of the grid that explain the discrepancy. If you choose the Warning field, application gives you more information on what the warning means.

When you have entered all relevant filters, choose the **Show Matrix** action. The data is calculated and the matrix page appears.

On the far left column in the grid, you see the various general ledger account types that are associated with stock. The grid then shows the invoiced, non-invoiced (interim), and WIP stock totals for each of these account types. These totals are calculated from the value entries.

The next columns show the totals for the same account types calculated from the general ledger entries.

Choose the amount in any of the total fields to see the stock report entries that were used to calculate the totals. For stock totals, the stock report entries are the sums of the value entries for the items. For the G/L totals, the stock report entries are the sums from the general ledger entries.

## <a name="reporting-costs-and-reconciling-with-the-general-ledger"></a>Reporting Costs and Reconciling with the General Ledger
Other reports, tracing functions, and a special reconciliation tool are available to the auditor or controller responsible for reporting a correct and balanced stock value to the finance department.

The following table describes them.    

|**To**|**See**|  
|------------|-------------|  
|View the stock value of selected items, including information about the quantities and values of increases and decreases in stock over a selected period.|**Stock Valuation** report|  
|View the stock value of selected works orders in your WIP (work in progress) stock, such as the quantities and values of consumption, capacity usage, and output in ongoing works orders.|**Stock Valuation - WIP** report|  
|View the stock value of selected items, including their actual and expected cost on the date specified.|**Invt. Valuation - Cost Spec.** report|  
|Use a report to analyze the reasons for cost variances or to gain insight into the cost shares of sold items (COGS).|**Cost Shares Breakdown** report|  

## <a name="see-also"></a>See Also  
[Managing Stock Costs](finance-manage-inventory-costs.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Sales](sales-manage-sales.md)    
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]