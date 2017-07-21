---
title: Manually Adjust the Costs of Items| Microsoft Docs
description: You can adjust the inventory valuation of an item using the FIFO or Average costing methods, for example, when item costs change for reasons other than transactions.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost adjustment, cost forwarding, costing method, inventory valuation, costing
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: a1f682b60b7b9ae402c27093f13aa3db2368ed5b
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-adjust-item-costs-manually"></a>How to: Adjust Item Costs Manually
The cost of an item (inventory value) that you purchase and later sell may change during its lifetime, for example because a freight cost is added to its purchase cost after you have sold the item. Cost adjustment is especially relevant in situations where you sell goods before you invoice the purchase of those goods. To always know the correct inventory value, item costs must therefore regularly be adjusted. This ensures that sales and profit statistics are up to date and that financial KPIs are correct.

In [!INCLUDE[d365fin](includes/d365fin_md.md)], item costs are automatically adjusted every time that an inventory transaction occurs, such as when posting a purchase invoice for an item.

You can also use a function to manually adjust the costs of one or more items. This is useful, for example, when you know that item costs have changed for other reasons than item transactions.

Item costs are adjusted by the FIFO or Average costing method, depending on your selection in the **Set Up My Company** assisted setup. For more information, see [Getting Ready for Doing Business](ui-get-ready-business.md).  

If you use the FIFO costing method, then an item’s unit cost is the actual value of any receipt of the item. Inventory is valuated with the assumption that the first items placed in inventory are sold first.

If you use the Average costing method, then an item’s unit cost is calculated as the average unit cost at each point in time after a purchase. Inventory is valuated with the assumption that all inventories are sold simultaneously.

The cost adjustment function processes only value entries that have not yet been adjusted. If the function encounters a situation where changed inbound costs need to be forwarded to associated outbound entries, then new adjustment value entries are created, which are based on the information in the original value entries but contain the adjustment amount. The cost adjustment function uses the posting date of the original value entry in the adjustment entry, unless that date is in a closed inventory period. In that case, the program uses the starting date of the next open inventory period. If inventory periods are not used, then the date in the **Allow Posting From** field in the **General Ledger Setup** window will define when the adjustment entry is posted.

Changes in inventory value from trade are automatically reconciled with your financial books when you post item transactions. For more information, see the "Inventory Reconciliation" section in [Inventory](inventory-manage-inventory.md).

## <a name="to-adjust-item-costs-manually"></a>To adjust item costs manually
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Cost - Item Entries**, and then choose the related link.
2. In the **Adjust Cost - Item Entries** window, specify which items to adjust costs for.
3. Choose the **OK** button.

## <a name="see-also"></a>See Also
[Inventory](inventory-manage-inventory.md)  
[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

