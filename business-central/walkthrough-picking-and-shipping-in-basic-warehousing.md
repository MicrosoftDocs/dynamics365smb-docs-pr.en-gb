---
title: Picking and Shipping in Basic Warehouse Configurations
description: In Business Central, the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.
author: jill-kotel-andersson
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: e1763e6288c8b8218955049ba7ef4c461ee5164e
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214660"
---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a>Walkthrough: Picking and Shipping in Basic Warehouse Configurations

<!-- [!INCLUDE[complete_sample_data](includes/complete_sample_data.md)] -->

In [!INCLUDE[prod_short](includes/prod_short.md)], the outbound processes for picking and shipping can be performed in four ways using different functionalities depending on the warehouse complexity level.  

|Method|Inbound process|Bins|Picks|Shipments|Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Post pick and shipment from the order line|X|||2|  
|B|Post pick and shipment from an stock pick document||X||3|  
|C|Post pick and shipment from a warehouse shipment document|||X|4/5/6|  
|D|Post pick from a warehouse pick document and post shipment from a warehouse shipment document||X|X|4/5/6|  

For more information, see [Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md).  

The following walkthrough demonstrates method B in the previous table.  

## <a name="about-this-walkthrough"></a>About This Walkthrough

In basic warehouse configurations where your location is set up to require pick processing but not ship processing, you use the **Stock Pick** page to record and post pick and ship information for your outbound source documents. The outbound source document can be a sales order, purchase return order, outbound transfer order, or a works order with component need.  

This walkthrough demonstrates the following tasks:  

- Setting up SOUTH location for stock picks.  
- Creating a sales order for customer 10000 for 30 Amsterdam Lamps.  
- Releasing the sales order for warehouse handling.  
- Creating an stock pick based on a released source document.  
- Registering the warehouse movement from the warehouse and at the same time posting the sales shipment for the source sales order.  

## <a name="roles"></a>Roles

This walkthrough demonstrates tasks that are performed by the following user roles:  

- Warehouse Manager  
- Order Processor  
- Warehouse Worker  

<!-- ## Prerequisites

To complete this walkthrough, you will need:  

- For [!INCLUDE[prod_short](includes/prod_short.md)] online, a company based on the **Advanced Evaluation - Complete Sample Data** option in a sandbox environment. For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, CRONUS installed.
 -->

## <a name="story"></a>Story

Ellen, the warehouse manager at CRONUS, sets up SOUTH warehouse for basic pick handling where warehouse workers process outbound orders individually. Susan, the order processor, creates a sales order for 30 units of item 1928-S to be shipped to customer 10000 from the SOUTH Warehouse. John, the warehouse worker must make sure that the shipment is prepared and delivered to the customer. John manages all involved tasks on the **Stock Pick** page, which automatically points to the bins where 1928-S is stored.

[!INCLUDE[set_up_location.md](includes/set_up_location.md)]

### <a name="setting-up-the-bin-codes"></a>Setting Up the Bin Codes
Once you have the location set up, you must add two bins.

#### <a name="to-setup-the-bin-codes"></a>To setup the bin codes

1. Select the **Bins** action.
2. Create two bins, with the codes *S-01-0001* and *S-01-0002*.

### <a name="making-yourself-a-warehouse-employee-at-location-south"></a>Making Yourself a Warehouse Employee at Location SOUTH

In order to use this functionality, you must add yourself to the location as a warehouse worker. 

#### <a name="to-make-yourself-a-warehouse-employee"></a>To make yourself a warehouse employee

  1. Choose the ![Lightbulb that opens the Tell Me feature first](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.  
  2. Choose the **User ID** field, and select your own user account on the **Warehouse Employees** page.
  3. In the **Location Code** field, choose SOUTH.  
  4. Select the **Default** field, and then select the **Yes** button.  

### <a name="making-item-1928-s-available"></a>Making Item 1928-S Available

To make item 1928-S available at the SOUTH location follow these steps:  

  1. Choose the ![Lightbulb that opens the Tell Me feature second](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Journals**, and then choose the related link.  
  2. Open the default journal, and then create two item journal lines with the following information about the work date (January 23).  

        |Entry Type|Item Number|Location Code|Bin Code|Quantity|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |Positive Adjmt.|1928-S|SOUTH|S-01-0001|20|  
        |Positive Adjmt.|1928-S|SOUTH|S-01-0002|20|  

        By default, the **Bin Code** field on the sales lines are hidden, so you must display it. To do this you need to personalise the page. For more information, see [To start personalising a page through the Personalising banner](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).

  3. Choose **Actions**, then **Posting**, and then choose **Post**.  
  4. Select the **Yes** button.  

## <a name="creating-the-sales-order"></a>Creating the Sales Order

Sales orders are the most common type of outbound source document.  

### <a name="to-create-the-sales-order"></a>To create the sales order

1. Choose the ![Lightbulb that opens the Tell Me feature third](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.  
2. Choose the **New** action.  
3. Create a sales order for customer 10000 on the work date (January 23) with the following sales order line.  

    |Item|Location Code|Quantity|  
    |----|-------------|--------|  
    |1928-S|SOUTH|30|  

     Proceed to notify the warehouse that the sales order is ready for warehouse handling.  

4. Choose the **Release** action.  

    John proceeds to pick and ship the sold items.  

## <a name="picking-and-shipping-items"></a>Picking and Shipping Items

On the **Stock Pick** page, you can manage all outbound warehouse activities for a specific source document, such as a sales order. [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

### <a name="to-pick-and-ship-items"></a>To pick and ship items

1. Choose the ![Lightbulb that opens the Tell Me feature fourth](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stock Picks**, and then choose the related link.  
2. Choose the **New** action.  

    Make sure that the **No.** field on the **General** FastTab is filled in.
3. Select the **Source Document** field, and then select **Sales Order**.  
4. Select the **Source No.** field, select the line for the sale to customer 10000, and then choose the **OK** button.  

    Alternatively, choose the **Get Source Document** action, and then select the sales order.  
5. Choose the **Autofill Qty. to Handle** action.  

    Alternatively, in the **Qty. to Handle** field, enter 10 and 20 respectively on the two stock pick lines.  
6. Choose the **Post** action, select **Ship**, and then choose the **OK** button.  

    The 30 Amsterdam Lamps are now registered as picked from bins S-01-0001 and S-01-0002, and a negative item ledger entry is created reflecting the posted sales shipment.  

## <a name="see-also"></a>See Also

[Pick Items with Stock Picks](warehouse-how-to-pick-items-with-inventory-picks.md)  
[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md)  
[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)  
[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  
[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md)  
[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)  
[Design Details: Outbound Warehouse Flow](design-details-outbound-warehouse-flow.md)  
[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
