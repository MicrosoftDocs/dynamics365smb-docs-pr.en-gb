---
title: Pick Production or Assembly in Basic Warehouse
description: When your warehouse location requires pick processing but not shipment processing, use the Stock Pick page to organise and record picking the components.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/24/2021
ms.author: edupont
ms.openlocfilehash: c3827bb8ab272b38972c17d79933ce0aa187e32d
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6445804"
---
# <a name="pick-for-production-or-assembly-in-basic-warehouse-configurations"></a>Pick for Production or Assembly in Basic Warehouse Configurations
How you put away your pick components for production or assembly orders depends on how your warehouse is set up as a location. For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).


## <a name="pick-for-production-in-basic-warehouse-configurations"></a>Pick for Production in Basic Warehouse Configurations
Flushishing method also affects the flow of components in production. For more information, see [Flush Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).

In advanced warehouse configurations where locations require both picks and shipments, you must use the **Warehouse Pick** page to bring components with flushing method set to *Manual*, *Pick + Forward*, *Pick + Backward* to works orders. For more information, see [Pick for Production or Assembly in Advanced Warehouse Configurations](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md).

In basic warehouse configurations where the location requires pick processing but not shipment processing, you can also use the **Stock Pick** page to organise and record the picking of components with flushing method set to *Manual*. When you register a stock pick for an internal operation, such as production, the consumption of the picked components is posted at the same time. Alternatively you can use **Stock Movement** with reference to a source document to bring components with flushing method set to *Manual*, *Pick + Forward*, *Pick + Backward* to works orders.

When production operations are integrated with warehouse processes, either by bins or by directed put-aways and picks, the bin from which the components are consumed is the bin that is defined on each works order component line. All required components must be available in that bin. Otherwise, the manual or flushed consumption posting is stopped for that component.

**Stock Movement** with references to the source document and **Warehouse pick** cannot be used to pick components with flushing methods *Forward* and *Backward*. **Stock Pick** cannot be used to pick components with any flushing method but *Manual*. To handle remaining components, use **Stock Movement** without reference to a source document. For more information, see [Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).

> [!NOTE]  
>  The following important differences exist between stock picks, stock movements, and warehouse picks:  
>   
>  -   When you register a stock pick for an internal operation, such as production, the consumption of the picked components is posted at the same time. When you register a stock movement or warehouse pick for an internal operation, you only record the physical movement of the required components to a bin in the operation area without posting the consumption.  
> -   When you use stock picks, the **Bin Code** field on a works order component line defines the *take* bin from where components are decreased when posting consumption. When you use stock movements or warehouse pick, the **Bin Code** field on works order component lines defines the *place* bin in the operation area where the warehouse worker must place the components.  

A system precondition for picking, or moving, components for source documents is that an outbound warehouse request exists to notify the warehouse area of the component need. The outbound warehouse request is created whenever the works order status is changed to Released or when a released works order is created.  

## <a name="to-pick-production-components-in-basic-warehouse-configurations-using-inventory-pick"></a>To pick production components in basic warehouse configurations using Stock Pick
In basic warehouse configurations where the location is set up to use picking only, you can pick components for production activities with the **Stock Pick** page. For more information, see [Pick Items with Stock Picks](warehouse-how-to-pick-items-with-inventory-picks.md).

1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stock Picks**, and then choose the related link.  
2.  To access the works order components, choose the **Get Source Documents** action, and then select the released works order.  
3.  Perform the pick, and then record the actual picking information in the **Qty. to Handle** field.  
4.  When the lines are ready for posting, choose the **Post** action. The posting creates the necessary warehouse entries and posts the consumption of the items.  

You can also create an **Stock Pick** directly from the released works order. Choose the **Create Stock Put-away/Pick/Movement** action, select the **Create Invt. Pick** check box, and then choose the **OK** button.

Alternatively, you can use the **Stock Movement** with reference to the source document to move items between bins. You will need to register consumption separately. For more information, see [Batch Post Production Consumption](production-how-to-post-consumption.md)

## <a name="pick-for-assembly-in-basic-warehouse-configurations"></a>Pick for Assembly in Basic Warehouse Configurations
In advanced warehouse configurations where locations require both picks and shipments, you must use the **Warehouse Pick** page to bring components to assembly orders. For more information, see [Pick for Production or Assembly in Advanced Warehouse Configurations](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md).

In basic warehouse configurations, you can also pick for assembly orders with the **Stock Movement** page. 

In basic warehouse configurations where the location requires pick processing but not shipment processing, the **Stock Pick** page is also used to pick, assemble, and ship for sales order where items must be assembled before they can be shipped. For more information, see [Handling Assemble-to-Order Item with Stock Picks](warehouse-how-to-pick-for-production.md#handling-assemble-to-order-items-with-inventory-picks).  

## <a name="handling-assemble-to-order-items-with-inventory-picks"></a>Handling Assemble-to-Order Items with Stock Picks
The **Stock Pick** page is also used to pick and ship for sales where items must be assembled before they can be shipped. For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).

Items to be shipped are not physically present in a bin until they are assembled and posted as output to a bin in the assembly area. This means that picking assemble-to-order items for shipment follows a special flow. From a bin, warehouse workers take the assembly items to the shipping dock and then post the stock pick. The posted stock pick then posts the assembly output, the component consumption, and the sales shipment.

You can set up [!INCLUDE[prod_short](includes/prod_short.md)] to automatically create a stock movement when the stock pick for the assembly item is created. To enable this, you must select the **Create Movements Automatically** field on the **Assembly Setup** page. For more information, see [Move Components to an Operation Area in Basic Warehousing](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).

Stock pick lines for sales items are created in different ways depending on whether none, some, or all of the sales line quantities are assembled to order.

In regular sales where you use stock picks to post shipment of stock quantities, one stock pick line, or several if the item is placed in different bins, is created for each sales order line. This pick line is based on the quantity in the **Qty. to Ship** field.

In assemble-to-order sales where the full quantity on the sales order line is assembled to order, one stock pick line is created for that quantity. This means that the value in the Quantity to Assemble field is the same as the value in the **Qty. to Ship** field. The **Assemble to Order** field is selected on the line.

If an assembly output flow is set up for the location, then the value in the **Asm.-to-Order Shpt. Bin Code** field or the value in the **From-Assembly Bin Code** field, in that order, is inserted in the **Bin Code** field on the stock pick line.

If no bin code is specified on the sales order line, and no assembly output flow is set up for the location, then the **Bin Code** field on the stock pick line is empty. The warehouse worker must open the **Bin Contents** page and select the bin where the assembly items are assembled.

In combination scenarios, where a part of the quantity must first be assembled and another must be picked from stock, a minimum of two stock pick lines are created. One pick line is for the assemble-to-order quantity. The other pick line depends on which bins can fulfil the remaining quantity from stock. Bin codes on the two lines are filled in different ways as described for the two different sales types respectively. For more information, see the “Combination Scenarios” section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).

## <a name="filling-the-consumption-bin"></a>Filling the Consumption Bin
This flow chart shows how the **Bin Code** field on works order component lines is filled according to your location setup.

![Bin flow chart.](media/binflow.png "BinFlow")

## <a name="see-also"></a>See Also
[Warehouse Management](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)     
[Assembly Management](assembly-assemble-items.md)    
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
