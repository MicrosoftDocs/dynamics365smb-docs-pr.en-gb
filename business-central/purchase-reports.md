---
title: Purchase Reports and Analytics
description: See which purchase reports and analytics are available in the standard version of Business Central so that you can keep track of your business.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 3f818e556b2ebe3f50189b0057f1302a5598d904
ms.sourcegitcommit: a486aa1760519c380b8cdc8fdf614bed306b65ea
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/13/2021
ms.locfileid: "6543177"
---
# <a name="purchase-reports-and-analytics-in-business-central"></a>Purchase Reports and Analytics in Business Central

Purchase reporting in [!INCLUDE [prod_short](includes/prod_short.md)] allows procurement and business professionals to get insights and statistics about current and past purchase activities.  

## <a name="reports"></a>Reports

The following table describes some of the key reports in purchase reporting.

|Report |Object ID|Description  |
|---------|---------|---------|
|**Purchase statistics**|312|[!INCLUDE [reports-purchase-statistics](includes/reports-purchase-statistics.md)]|
|**Supplier – Top 10 list**|311|Shows information on purchases from suppliers for a selected period. You can choose the number of suppliers that are included in the report.<br>The suppliers are sorted in order of amount, and you can choose whether they are sorted by purchase amount or balance. The report gives a quick overview of the suppliers from which you purchase the most or to which you owe the most.|
|**Supplier Item catalogue** or **Item/supplier catalogue**|320 or 720|Displays a list of the suppliers for the selected items or items for selected suppliers. For each combination of item and supplier, it shows direct unit cost, lead time calculation and the supplier's item number.<br>In the US, Canada, and Mexico, this report is not available. Instead, use the **Item/Supplier catalogue** (10164) report.|
|**Supplier/Item Purchases**|313|Shows a list of item entries for each supplier in a selected period. The report contains information on invoiced quantity, amount and possible discounts. It can be used, for example, to analyse a company's item purchases and to show whether there is a relationship between discounts and item purchases.|
|**Stock Cost and price list**|716|Displays a list of price information for the selected items or stockkeeping units: direct unit cost, last direct cost, unit price, profit percentage, and profit.|
|**Stock Availability Plan**|707|If you would like to have an overview about specific items/stockkeeping units and their availability. This report will show you cumulated values such as gross requirements, scheduled and planned receipts, the stock, and so on. |
|**Stock Supplier Purchases**|714|Displays a list of the suppliers that your company has purchased items from within a selected period. It shows invoiced quantity, amount and discount. The report can be used to analyse a company's item purchases.|
|**Stock Purchase Orders**|709|Displays a list of items on order from suppliers. It also shows the expected receipt date and the quantity and amount on back orders. For example, use the report to see when items should be received, and whether a reminder of a back order should be issued|
|**Purchase Reservation Availability**|409|Shows the availability of items for shipment on purchase documents, for example return orders. You determine whether the report indicates the status of each document or of each purchase line. <br>When you print the report, you can also update the quantity that is available for shipment in the **Qty. to Receive** field on the purchase lines. On purchase credit memos and negative purchase order lines, the **Qty. to Receive** field contains the quantity to ship.. Then you can use the report to determine which documents to ship. **Note**: This report is not available for advanced warehouse functionality.|
<!--|**Supplier detailed ageing**|11006| DACH specific: A report which could be used by the team leader of your purchased department as will the accounting. Here you will have an overview about the unpaid supplier invoices including the due dates, currencies and amounts. Basis is the open supplier ledger entries.| -->




## <a name="tasks"></a>Tasks

The following articles describe some of the key tasks for analysing the state of your business:

* [Create Analysis Reports](bi-how-create-analysis-views-reports.md)  
* [View the Availability of Items](inventory-how-availability-overview.md)  


## <a name="see-also"></a>See also 

[Setting Up Purchase](purchasing-setup-purchasing.md)  
[Purchasing](purchasing-manage-purchasing.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
