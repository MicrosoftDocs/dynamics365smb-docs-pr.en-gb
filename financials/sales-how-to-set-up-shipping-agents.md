---
title: How to Set Up Shipping Agents | Microsoft Docs
description: You can set up a code for each of your shipping agents and enter information about them.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 84a5d9eb8757dc82834c17327ffbb510cd15fa1a
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-shipping-agents"></a>How to: Set Up Shipping Agents
You can set up a code for each of your shipping agents and enter information about them.  

If you enter an Internet address for the shipping agent, and the agent provides package tracking services on the Internet, you can use the automatic package tracking feature. For more information, see [How to: Track Packages](sales-how-track-packages.md).

When you set up shipping agents on your sales orders, you can also specify the services that each shipping agent offers.  
For each shipping agent, you can set up an unlimited number of services, and you can specify a shipping time for each service.  

When you have assigned a shipping agent service to a sales order line, the shipping time of the service will be included in the order promising calculation, for that line. For more information, see [How to: Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).

## <a name="to-set-up-a-shipping-agent"></a>To set up a shipping agent  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Shipping Agents**, and then choose the related link.  
2.  Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].  
3.  Choose the **Shipping Agent Services** action.
4. In the **Shipping Agent Services**, fill in the fields as necessary.

> [!NOTE]  
>  If you delete the shipping agent on the order line, the shipping agent service code is also deleted. The contents of fields that were based in part on the shipping agent service are recalculated.  

## <a name="see-also"></a>See Also
[How to: Track Packages](sales-how-track-packages.md)    
[Warehouse Management](warehouse-manage-warehouse.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

