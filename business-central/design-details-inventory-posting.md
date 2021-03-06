---
title: Design Details - Stock Posting | Microsoft Docs
description: Each stock transaction, such as a purchase receipt or a sales shipment, posts two entries of different types.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 120db7bf4336444f6cf726d0f784a86841dc3e11
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215960"
---
# <a name="design-details-inventory-posting"></a>Design Details: Stock Posting

Each stock transaction, such as a purchase receipt or a sales shipment, posts two entries of different types.  

|Entry type|Description|  
|----------|-----------|  
|Quantity|Reflects the change of quantity in stock. This information is stored in item ledger entries.<br /><br /> Accompanied by item application entries.|  
|Value|Reflects the change of stock value. This information is stored in value entries.<br /><br /> One or more value entries can exist for each item ledger entry or capacity ledger entry.<br /><br /> For information about capacity value entries related to the use of production or assembly resources, see [Design Details: Works Order Posting](design-details-production-order-posting.md).|  

 In relation to quantity postings, item application entries exist to link stock increase with stock decrease. This enables the costing engine to forward costs from increases to the related decreases and vice versa. For more information, see [Design Details: Item Application](design-details-item-application.md).  

 Item ledger entries, value entries, and item application entries are created as a result of posting an item journal line, either indirectly by posting an order line or directly in the Item Journal page.  

 At regular intervals, value entries that are created in the stock ledger are posted to the general ledger to reconcile the two ledgers for financial control reasons. For more information, see [Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md).  

 ![Entry flow when reconciling stock with G/L](media/design_details_inventory_costing_1_entry_flow.png "Entry flow when reconciling stock with G/L")  

## <a name="example"></a>Example

The following example shows how item ledger entries, value entries, and item application entries result in general ledger entries.  

 You post a purchase order as received and invoiced for 10 items with a direct unit cost of LCY 7 and an overhead rate of LCY 1. The posting date is 01-01-20. The following entries are created.  

### <a name="item-ledger-entries-1"></a>Item Ledger Entries (1)

|Posting Date|Entry Type|Cost Amount (Actual)|Quantity|Entry No.|  
|------------|----------|--------------------|--------|---------|  
|01-01-20|Purchase|80.00|10|1|  

### <a name="value-entries-1"></a>Value Entries (1)

|Posting Date|Entry Type|Cost Amount (Actual)|Item Ledger Entry No.|Entry No.|  
|------------|----------|--------------------|---------------------|---------|  
|01-01-20|Direct Cost|70.00|1|1|  
|01-01-20|Indirect Cost|10.00|1|2|  

### <a name="item-application-entries-1"></a>Item Application Entries (1)

|Entry No.|Item Ledger Entry No.|Inbound Item Entry No.|Outbound Item Entry No.|Quantity|  
|---------|---------------------|----------------------|-----------------------|--------|  
|1|1|1|0|10|  

 Next, you post a sale of 10 units of the item with a posting date of 01-15-20.  

### <a name="item-ledger-entries-2"></a>Item Ledger Entries (2)

|Posting Date|Entry Type|Cost Amount (Actual)|Quantity|Entry No.|  
|------------|----------|--------------------|--------|---------|  
|01-15-20|Sale|-80.00|-10|2|  

### <a name="value-entries-2"></a>Value Entries (2)

|Posting Date|Entry Type|Cost Amount (Actual)|Item Ledger Entry No.|Entry No.|  
|------------|----------|--------------------|---------------------|---------|  
|01-15-20|Direct Cost|-80.00|2|3|  

### <a name="item-application-entries-2"></a>Item Application Entries (2)

|Entry No.|Item Ledger Entry No.|Inbound Item Entry No.|Outbound Item Entry No.|Quantity|  
|---------|---------------------|----------------------|-----------------------|--------|  
|2|2|1|2|-10|  

At the end of the accounting period, you run the **Post Stock Cost to G/L** batch job to reconcile these stock transactions with the general ledger.  

 For more information, see [Design Details: Accounts in the General Ledger](design-details-accounts-in-the-general-ledger.md).  

 The following tables show the result of reconciling the stock transactions in this example with the general ledger.  

### <a name="value-entries-3"></a>Value Entries (3)  

|Posting Date|Entry Type|Cost Amount (Actual)|Cost Posted to G/L|Item Ledger Entry No.|Entry No.|  
|------------|----------|--------------------|------------------|---------------------|---------|  
|01-01-20|Direct Cost|70.00|70.00|1|1|  
|01-01-20|Indirect Cost|10.00|10.00|1|2|  
|01-15-20|Direct Cost|-80.00|-80.00|2|3|  

### <a name="general-ledger-entries-3"></a>General Ledger Entries (3)

|Posting Date|G/L Account|Account No. (En-US Demo)|Amount|Entry No.|  
|------------|-----------|------------------------|------|---------|  
|01-01-20|[Stock Account]|2130|70.00|1|  
|01-01-20|[Direct Cost Applied Account]|7291|-70.00|2|  
|01-01-20|[Stock Account]|2130|10.00|3|  
|01-01-07|[Overhead Applied Account]|7292|-10.00|4|  
|01-15-20|[Stock Account]|2130|-80.00|5|  
|01-15-20|[COGS Account]|7290|80.00|6|  

> [!NOTE]  
> The posting date of the general ledger entries is the same as for the related value entries.  
> 
> The **Cost Posted to G/L** field in the **Value Entry** table is filled.  

 The relation between value entries and general ledger entries is stored in the **G/L - Item Ledger Relation** table.  

### <a name="relation-entries-in-the-gl--item-ledger-relation-table-3"></a>Relation Entries in the G/L – Item Ledger Relation table (3)

|G/L Entry No.|Value Entry No.|G/L Register No.|  
|-------------|---------------|----------------|  
|1|1|1|  
|2|1|1|  
|3|2|1|  
|4|2|1|  
|5|3|1|  
|6|3|1|  

## <a name="assembly-and-production-posting"></a>Assembly and Production Posting

Capacity and resource ledger entries represent the time that is posted as consumed in production or assembly. These process costs are posted as value entries to the general ledger along with the involved material costs in a similar structure as described for item ledger entries in this topic.  

For more information, see [Design Details: Assembly Order Posting](design-details-assembly-order-posting.md).  

## <a name="see-also"></a>See Also

 [Design Details: Stock Costing](design-details-inventory-costing.md)  
 [Design Details: Accounts in the General Ledger](design-details-accounts-in-the-general-ledger.md)  
 [Design Details: Cost Components](design-details-cost-components.md) [Managing Stock Costs](finance-manage-inventory-costs.md)  
 [Finance](finance.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]