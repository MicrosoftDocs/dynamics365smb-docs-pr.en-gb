---
title: Design Details - Prioritising Orders | Microsoft Docs
description: Read about how to prioritise to meet both demand and supply requirements.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 6e09ad64750493f99210d47516410d8471a83011
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-prioritizing-orders"></a>Design Details: Prioritising Orders
Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week. But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand. Likewise, it will suggest what source of supply should be applied before applying other sources of supply. This is done according to order priorities.  
  
Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:  
  
## <a name="priorities-on-the-demand-side"></a>Priorities on the Demand Side  
1. Already shipped: Item Ledger Entry  
2. Purchase Return Order  
3. Sales Order  
4. Service Order  
5. Production Component Need  
6. Assembly Order Line  
7. Outbound Transfer Order  
8. Blanket Order (that has not already been consumed by related sales orders)  
9. Forecast (that has not already been consumed by other sales orders)  
  
> [!NOTE]  
>  Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned. If not reserved, purchase returns play a role in the availability and are highly prioritised to avoid that the planning system suggests a supply order just to serve a purchase return.  
  
## <a name="priorities-on-the-supply-side"></a>Priorities on the Supply Side  
1. Already in inventory: Item Ledger Entry (Planning Flexibility = None)  
2. Sales Return Order (Planning Flexibility = None)  
3. Inbound Transfer Order  
4. Production Order  
5. Assembly Order  
6. Purchase Order  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a>Priority Related to the State of Demand and Supply  
Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority. For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:  
  
1. Partly handled (Planning Flexibility = None)  
2. Already in process in the warehouse (Planning Flexibility = None)  
3. Released – all order types (Planning Flexibility = Unlimited)  
4. Firm Planned Production Order (Planning Flexibility = Unlimited)  
5. Planned/Open – all order types (Planning Flexibility = Unlimited)  
  
## <a name="see-also"></a>See Also  
[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)   
[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)
