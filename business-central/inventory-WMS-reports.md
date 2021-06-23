---
title: Stock and Warehouse Reports and Analytics
description: See which stock and warehouse reports and analytics are available in the standard version of Business Central so that you can keep track of your business.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 8a4418699f28acd3ede80616ba69c56f50781e43
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216411"
---
# <a name="inventory-and-warehouse-reports-and-analytics-in-business-central"></a>Stock and Warehouse Reports and Analytics in Business Central

Stock and warehouse reporting in [!INCLUDE [prod_short](includes/prod_short.md)] allows stock and business professionals to get insights and statistics about current and past stock and warehouse activities.  

## <a name="reports"></a>Reports

The following table describes some of the key reports in stock and warehouse reporting.

|Report |Object ID|Description  |
|---------|---------|---------|
|**Stock Availability Plan**|707|If you would like to have an overview about specific items/stockkeeping units and their availability. This report shows cumulated values like gross requirements, scheduled and planned receipts, the stock, and so on. |
|**Stock Valuation**|1001|Displays stock valuation for selected items in your stock. The report also shows information about the value of increases and decreases in stock over time.|
|**Item Expiration - Quantity**|5809|Shows an overview of the quantities of selected items in your stock whose expiration dates fall within a certain period. The list shows the number of units of the selected item that will expire in a given time period. For each of the items that you specify when setting up the report, the printed document shows the number of units that will expire during each of three periods of equal length and the total stock quantity of the selected item.<br>You can specify what is included in the report by setting filters. If you do not set any filters, the report will include all your records. The quantities in the report reflect only the quantities of the item for which expiration dates have been defined.|
|**Item Age Composition - Quantity** or **Item Age Composition - Value**|5807 or 5808|Shows an overview of the current age composition of selected items in your stock. The list shows the number of units or value of the selected item that were added to or removed from stock and at which point in time. Items can be added to or removed from stock as a result of purchases, sales, and positive and negative adjustments.|
|**Stock Cost and price list**|716|Displays a list of price information for the selected items or stockkeeping units: direct unit cost, last direct cost, unit price, profit percentage, and profit. |
|**Warehouse Bin List**|7319|Shows an overview of warehouse bins, their setup, and the quantity of items within the bins. This report can be used for all locations, which have “bin” as mandatory field. |
|**Warehouse Shipment Status**|7313|Shows an overview of open source documents with items shipped or due for shipping per location. This report can be used for all locations, were **Required Shipments** is enabled. **Warehouse Shipment Status** shows locations, bin codes, document status, quantities.|
|**Stock Picking List**|813|Displays a list of the sales orders in which an item is included. The following information is shown for each item: sales order line with customer's name, variant code, location code, bin code, shipment date, quantity to be shipped, and unit of measurement. The quantity to be shipped is totalled for each item. The report can be used when items will be collected from the stock.<br>NOTE: this functionality is not available for advanced warehouse functionality.|
|**Warehouse Adjustment Bin**|7320|This special report is meant only for an advanced warehouse and shows the remaining quantities that are still stored in the adjustment bin itself. Normally this specific bin should be empty. The only reason when this bin will be filled is as result of physical counting process or if quantities of items had been removed or added to the warehouse|


## <a name="tasks"></a>Tasks

The following articles describe some of the key tasks for analysing the state of your business:

* [Create Analysis Reports](bi-how-create-analysis-views-reports.md)  
* [View the Availability of Items](inventory-how-availability-overview.md)


## <a name="see-also"></a>See also 

[Setting Up Stock](inventory-setup-inventory.md)  
[Stock](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Warehouse Management](warehouse-manage-warehouse.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
