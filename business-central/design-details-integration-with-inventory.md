---
title: Design Details - Integration with Stock | Microsoft Docs
description: The Warehouse Management application area and the Stock application area interact with one another in physical stock and in stock or warehouse adjustment.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 94eb1e0efa5c2a7ab54c46627b9d09ded6fae13f
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215160"
---
# <a name="design-details-integration-with-inventory"></a>Design Details: Integration with Stock
The Warehouse Management application area and the Stock application area interact with one another in physical stock and in stock or warehouse adjustment.  
  
## <a name="physical-inventory"></a>Physical Stock  
 The **Whse. Phys. Stock Journal** page is used with the **Phys. Stock Journal** page for all advanced warehouse locations. The stock on bin level is calculated, and a printed list is provided for the warehouse employee. The list shows which items in which bins must be counted.  
  
 The warehouse employee enters the counted quantity on the **Whse. Phys. Stock journal** page and then posts the journal.  
  
 If the counted quantity is greater than the quantity on the journal line, a movement is posted for this difference from the default adjustment bin to the counted bin. This increases the quantity in the counted bin and decreases the quantity in the default adjustment bin.  
  
 If the quantity counted is less than the quantity on the journal line, a movement for this difference is posted from the counted bin to the default adjustment bin. This decreases the quantity in the counted bin and increases the quantity in the default adjustment bin.  
  
 In advanced warehouse configurations, the value in the **Quantity (Calculated)** field is retrieved from item ledger entries and the value in the **Quantity (Phys. Stock)** field is retrieved from warehouse entries, excluding the adjustment bin content. The **Quantity** field specifies the difference between the first two fields, which should be equal to the contents of the adjustment bin.  
  
 When you post the physical stock journal, the stock and the default adjustment bin are updated.  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a>Warehouse Adjustments to the Item Ledger  
 You use the **Item Journal** page and the **Calculate Whse. Adjustment** function to adjust stock on the item ledger in accordance with an adjustment that has been made to the item quantity in a warehouse bin. To create a link between the stock and the warehouse, you must define a default adjustment bin per location.  
  
 The default adjustment bin registers items in the warehouse when you post an increase for the stock. However, if you post a decrease, the quantity on the default bin is also decreased. In both cases, item ledger entries and warehouse entries are created.  
  
> [!NOTE]  
>  The adjustment bin is not included in the availability calculation.  
  
 If you want to adjust the bin content, you can use the warehouse item journal, from which you can enter the item number, zone code, bin code, and quantity that you want to adjust.  
  
 If you enter a positive quantity and post the line, then the stock stored in the bin increases, and the quantity of the default adjustment bin decreases correspondingly.  
  
## <a name="see-also"></a>See Also  
 [Design Details: Warehouse Management](design-details-warehouse-management.md)   
 [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]