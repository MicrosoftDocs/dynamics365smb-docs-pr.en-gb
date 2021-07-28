---
title: Breaking Bulk with Directed Put-away and Pick
description: Learn how to enable automatic breaking bulk with directed put-away and pick, as well as breakbulking in picks, putaways, movements, and more.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/25/2021
ms.author: edupont
ms.openlocfilehash: a3e992b86b2c53393ee385fd4abde05bd2b915f2
ms.sourcegitcommit: e562b45fda20ff88230e086caa6587913eddae26
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/30/2021
ms.locfileid: "6324846"
---
# <a name="enable-automatic-breaking-bulk-with-directed-put-away-and-pick"></a>Enable Automatic Breaking Bulk with Directed Put-away and Pick
For locations that use directed put-away and pick, [!INCLUDE[prod_short](includes/prod_short.md)] can, in various situations, automatically breakbulk, that is, break a larger unit of measurement into smaller units of measurement, when it creates warehouse instructions that fulfil the needs of source documents, works orders, or internal picks and put-aways. To breakbulk sometimes also means gathering smaller units of measurement, if necessary, to meet outbound requests by breaking the larger unit of measurement on the source document or works order into the smaller units of measurement that are available in the warehouse.   

## <a name="breakbulking-in-picks"></a>Breakbulking in Picks  
If you want to store items in several different units of measurement and allow them to be automatically combined as needed in the picking process, select the **Allow Breakbulk** field on the location card.  

To fulfil a task, application automatically looks for an item in the same unit of measurement. But if it cannot find this form of the item, and this field is selected, application will suggest that you break a larger unit of measurement into the unit of measurement that is needed.  

If the system can only find smaller units of measurement, it will suggest that you gather items to fulfil the quantity on the shipment or works order. In effect, it breaks the larger unit of measurement on the source document into smaller units for picking.  

## <a name="breakbulking-in-put-aways"></a>Breakbulking in Put-aways  
In the warehouse put-away, application automatically suggests Place action lines in the put-away unit of measurement, for example, pieces, even though the items arrive in a different unit of measurement.  

## <a name="breakbulking-in-movements"></a>Breakbulking in Movements  
The application also breakbulks automatically in replenishment movements, if the **Allow Breakbulk** field is selected on the **Option** FastTab on the **Calculate Bin Replenishment** page.  

You can view the results of the conversion process from one unit of measurement to another as intermediate breakbulk lines in the put-away, pick, or movement instructions.  

> [!NOTE]  
>  If you select the **Set Breakbulk Filter** field on the warehouse instruction header, application will hide the breakbulk lines whenever the larger unit of measurement is going to be completely used. For example, if a pallet is 12 pieces and you are going to use all 12 pieces, the pick will then direct you to take 1 pallet and place 12 pieces. However, if you have to pick only 9 pieces, then the breakbulk lines will not be hidden, even if you have selected the **Breakbulk Filter** field, because you have to place the remaining three pieces somewhere in the warehouse.  

> [!NOTE]  
>  If you want your units of measurement to perform optimally in the warehouse, also in connection with the breakbulk functionality, you should wherever possible try to:  
>   
> - Set up the base unit of measurement for an item as the smallest unit of measurement that you expect to handle in your warehouse processes.  
> - Set up your alternative units of measurement for the item as multiples of the base unit of measurement.  

## <a name="see-also"></a>See Also  
[Warehouse Management](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]