---
title: Create Works Orders from Sales Orders
description: You can create works orders from sales orders.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/28/2021
ms.author: edupont
ms.openlocfilehash: 438f4d4e1833ba607ceedb9f5d9450c0a4dbb680
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115243"
---
# <a name="create-production-orders-from-sales-orders"></a>Create Works Orders from Sales Orders
You can create works orders for produced items directly from sales orders.  

## <a name="to-create-a-production-order-from-a-sales-order"></a>To create a works order from a sales order  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.  
2.  Select the sales order you want to create a works order for.  
3.  Choose the **Planning** action. On the **Sales Order Planning** page, you can view the availability of the sales order item.  
4.  Choose the **Create Prod. Order** action.  
5.  Select the status and order type.  
6.  Choose the **Yes** button to create one or more works orders for the lines that have **Prod. Order** in their **Replenishment System** field.


> [!NOTE]  
> Demand lines in the created works order that have **Prod. Order** in their **Replenishment System** field represent underlying works orders. After you have generated these works orders, remember to identify any unfulfilled component demand for them using the **Order Planning** page or the **Replan** function from created orders. 

## <a name="order-type"></a>Order type  
You can choose between two ways to create the works orders as outlined in the following table.

|Option|Description|
|------|-----------|
|Item Order|One works order is created for each needed works order that is represented by a line in the **Sales Order Planning** window.|
|Project Order|One works order is created for all needed works orders order that are represented by lines in the **Sales Order Planning** window. |

When you use project orders, the **Source Type** field of the works order contains **Sales Header** and the order has multiple lines, one for each sales line item that must be produced.  


## <a name="see-also"></a>See Also  
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Manufacturing](production-manage-manufacturing.md)    
[Stock](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Design Details: Supply Planning](design-details-supply-planning.md)   
[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
