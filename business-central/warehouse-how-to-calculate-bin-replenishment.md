---
title: Calculate Bin Replenishment
description: When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.search.form: 7315, 7351
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 0f2653087df90ca6801f0d2e972f142e1f65b889
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/19/2022
ms.locfileid: "9530819"
---
# <a name="calculate-bin-replenishment"></a>Calculate Bin Replenishment

When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away. Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings. Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.  

But inventory does not always arrive in a steady trickle. Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost. Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.  

It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.  

Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.  

## <a name="to-replenish-pick-bins"></a>To replenish pick bins

1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.  
2.  Choose the **Calculate Bin Replenishment** action to open the report request page.  
3.  Fill in the batch job request page to limit the scope of the replenishment suggestions that will be calculated. For example, you might be concerned with particular items, zones, or bins.  
4.  Choose the **OK** button. Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.  
5.  If you want to perform all the suggested replenishments, choose the **Create Movement** action. Employees can now find instructions in the **Movements** menu item, carry them out and register them.  
6.  If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.  

The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.  

> [!NOTE]  
>  If the following conditions are met for an item:  
>   
>  -   The item has an expiration date, and  
> -   The **Pick According to FEFO** field on the location card is selected, and  
> -   You use the **Calculate Bin Replenishment** functionality  
>   
>  then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.  

## <a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/move-items/)

## <a name="see-also"></a>See also 

[Warehouse Management](warehouse-manage-warehouse.md)  
[Picking by FEFO](warehouse-picking-by-fefo.md)  
[Inventory](inventory-manage-inventory.md)  
[Setting Up Warehouse Management](warehouse-setup-warehouse.md)  
[Assembly Management](assembly-assemble-items.md)  
[Design Details: Warehouse Management](design-details-warehouse-management.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
