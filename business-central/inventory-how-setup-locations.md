---
title: Set Up a Location Card and Define Transfer Routes
description: You create a location card for each place you store stock items, for example, a warehouse or distribution centre, and set up routes to transfer items between locations.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/01/2021
ms.author: edupont
ms.openlocfilehash: 0319f0c64dd46610aa82705257091bd9478ac14f
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184331"
---
# <a name="set-up-locations"></a>Set Up Locations

If you buy, store, or sell items at more than one place or warehouse, you must set up each location with a location card and define transfer routes. [!INCLUDE [prod_short](includes/prod_short.md)] uses locations to help keep track of stock in both simpler cases and the more complex warehouse processes.

You can then create document lines for a specific location, view availability by location, and transfer stock between locations. For more information, see [Manage Stock](inventory-manage-inventory.md).
<br><br>  
  
> [!Video https://www.microsoft.com/videoplayer/embed/RE4aQvq?rel=0]

## <a name="location-cards"></a>Location cards

The location card specifies information about a location, such as a warehouse or distribution centre. You give each location a name and a code that represents the location. You can then enter the location code in other parts of the program when you want to record transactions for a given location.  

You can enter information about bins and warehouse policies for each location. Based on the warehouse policies you select, you can use the options on the **Bins** FastTab to define the bins that will be used as default bins when you are performing transactions. If you are using directed put-away and pick, you use most of the options on the **Bin Policies** FastTab to define how you would like to use the various advanced warehousing features.  

Some option fields are greyed and disabled by other settings in the **Location Card** page to restrict unsupported setup combinations.  

Choose the **Zones** or **Bins** action to view information about zones and bins that may be defined for the location.

### <a name="to-create-a-location-card"></a>To create a location card

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.
2. Choose the **New** action.
3. On the **Location Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Repeat steps 2 and 3 for every location where you want to keep stock.

> [!NOTE]  
> Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes. The fields are not relevant for companies that do not require the more complex warehouse functionality. For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).

You can change the configuration of a location later, but you cannot edit the setup of locations that have item ledger entries.  

Next, if you have multiple locations, you can define transfer routes between locations.  

### <a name="to-create-a-transfer-route"></a>To create a transfer route

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Routes**, and then choose the related link.
2. Alternatively, from any **Location Card** page, choose the **Transfer Routes** action.
3. Choose the **New** action.
4. On the **Location Card** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

You can now transfer stock items between two locations. For more information, see [Transfer Stock Between Locations](inventory-how-transfer-between-locations.md).    

## <a name="bins"></a>Bins

Bins represent the basic warehouse structure and are used to make suggestions about the placement of items. When you have created your bins, you can define precisely the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents. Bins are predominantly used in basic and advance warehouse operations. If you manage stock in a more simple setup, you probably do not need bins.

To use the bin functionality at a location, you first activate the functionality on the **Location** card by selecting the **Bins Mandatory** field on the **Warehouse** FastTab. Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.

> [!NOTE]
> Before you can specify bin codes on the location card, the bin codes must be created.

For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md) and [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).  

## <a name="zones"></a>Zones

If you want to structure your bins under zones, you can do that in the **Zones** page.

[!INCLUDE [prod_short](includes/prod_short.md)] copies the fields that you set for any particular zone to the bins within it. This way, you can assign a zone to a bin or a bin template (bin creation filter), and several other fields are then filled in automatically.

However, you can choose to set up just one zone and to organise your warehouse according to bins alone. For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).  

## <a name="see-also"></a>See Also

[Manage Stock](inventory-manage-inventory.md)  
[Transfer Stock Between Locations](inventory-how-transfer-between-locations.md)  
[Create Bins](warehouse-how-to-create-individual-bins.md)  
[Set Up Bin Types](warehouse-how-to-set-up-bin-types.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[General Business Functionality](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]