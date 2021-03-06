---
title: Understanding Item Types| Microsoft Docs
description: You can adjust the inventory valuation of an item using the FIFO or Average costing methods, for example, when item costs change for reasons other than transactions.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: bbe603de91c78cf64b2e181136ea6214aa43c5c8
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786130"
---
# <a name="about-item-types"></a>About Item Types
In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system. Three options exist:

|Option|Typical Purpose|
|------|-----------|
|Inventory|A physical unit, such as a bicycle, for full business support.|
|Non-Inventory|A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.|
|Service|A labour time unit, such as a consultancy hour, for limited business support.|

The **Inventory** type involves full tracking of inventory quantity and value. Therefore, all item transaction nature codes are supported, and items of type Inventory can be used with all item-handling features.

The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value. Therefore, only selected item transaction nature codes and features are supported.

The three item types support the following features respectively.

|Item Type|Sales|Purchasing|Job Consumption|Service Consumption|Assembly Consumption|Production Consumption|Assembly Output|Production Output|Location Transfer|Physical Counting|Inventory Revaluation|Inventory Costing|Item Tracking|Reservation|Warehousing|Planning|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|Inventory|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Non-Inventory|Yes|Yes|Yes|Yes|Yes|Yes|No|No|No|No|No|No|No|No|No|No|
|Service|Yes|Yes|Yes|No|No|No|No|No|No|No|No|No|No|No|No|No|

## <a name="costing-methods-for-types-of-items"></a>Costing Methods for Types of Items
When you post inventory transactions, the quantity and value changes to the inventory are recorded in the item ledger entries and the value entries, respectively. 

For inventory items, the cost is recorded in the **Cost Amount (Actual)** field on the **Value Entries** page, and when it is reconciled to the general ledger the cost will be shown in the **Cost Posted to G/L** field. For more information, see [Design Details: Inventory Costing](design-details-inventory-costing.md).

For non-inventory and service items the cost is recorded in the **Cost Amount (Non-Invtbl.)** field on the **Value Entries** page. For non-inventory and service items the cost is specified on the sales, assembly, and production documents and journals. The default cost can be specified in the **Unit Cost** field on the **Item Card** and **Stockkeeping Unit** pages. Costs for these types of items are not reconciled to the general ledger. 

## <a name="catalog-and-service-items"></a>Catalogue and Service Items
Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalogue items. Catalogue items are not to be mistaken with regular items of type Non-Inventory. For more information, see [Work with Catalogue Items](inventory-how-work-nonstock-items.md).

Customers' items that you perform service on, such as a printer, are called service items. Service items have nothing to do with regular or catalogue items. However, service components can be regular items. For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Setting Up Inventory](inventory-setup-inventory.md)  
[Managing Inventory Costs](finance-manage-inventory-costs.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]