---
title: Understanding Item Types
description: You can adjust the stock valuation of an item using the FIFO or Average costing methods when item costs change for reasons other than transactions.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: 2541f509d02a584620c83903c3b92983aba1c2a8
ms.sourcegitcommit: e562b45fda20ff88230e086caa6587913eddae26
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/30/2021
ms.locfileid: "6322801"
---
# <a name="about-item-types"></a>About Item Types
In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system. Three options exist:

|Option|Typical Purpose|
|------|-----------|
|Stock|A physical unit, such as a bicycle, for full business support.|
|Non-Stock|A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.|
|Service|A labour time unit, such as a consultancy hour, for limited business support.|

The **Stock** type involves full tracking of stock quantity and value. Therefore, all item transaction nature codes are supported, and items of type Stock can be used with all item-handling features.

The **Service** and **Non-Stock** types do not involve tracking of stock quantity and value. Therefore, only selected item transaction nature codes and features are supported.

The three item types support the following features respectively.

|Item Type|Sales|Purchasing|Job Consumption|Service Consumption|Assembly Consumption|Production Consumption|Assembly Output|Production Output|Location Transfer|Physical Counting|Stock Revaluation|Stock Costing|Item Tracking|Reservation|Warehousing|Planning|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|Stock|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|Non-Stock|Yes|Yes|Yes|Yes|Yes|Yes|No|No|No|No|No|No|No|No|No|No|
|Service|Yes|Yes|Yes|No|No|No|No|No|No|No|No|No|No|No|No|No|

## <a name="costing-methods-for-types-of-items"></a>Costing Methods for Types of Items
When you post stock transactions, the quantity and value changes to the stock are recorded in the item ledger entries and the value entries, respectively. 

For stock items, the cost is recorded in the **Cost Amount (Actual)** field on the **Value Entries** page, and when it is reconciled to the general ledger the cost will be shown in the **Cost Posted to G/L** field. For more information, see [Design Details: Stock Costing](design-details-inventory-costing.md).

For non-stock and service items the cost is recorded in the **Cost Amount (Non-Invtbl.)** field on the **Value Entries** page. For non-stock and service items the cost is specified on the sales, assembly, and production documents and journals. The default cost can be specified in the **Unit Cost** field on the **Item Card** and **Stockkeeping Unit** pages. Costs for these types of items are not reconciled to the general ledger. 

## <a name="catalog-and-service-items"></a>Catalogue and Service Items
Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalogue items. Catalogue items are not to be mistaken with regular items of type Non-Stock. For more information, see [Work with Catalogue Items](inventory-how-work-nonstock-items.md).

Customers' items that you perform service on, such as a printer, are called service items. Service items have nothing to do with regular or catalogue items. However, service components can be regular items. For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Setting Up Stock](inventory-setup-inventory.md)  
[Managing Stock Costs](finance-manage-inventory-costs.md)  
[Stock](inventory-manage-inventory.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]