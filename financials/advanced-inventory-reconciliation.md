---
title: 'Advanced: Inventory Reconciliation| Microsoft Docs'
description: Describes how your inventory value in reconciled with the general ledger.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: post inventory cost to G/L, reconcile inventory
ms.date: 02/15/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 7eb07530fe80f871ef113c95e48bf89da6c29db0
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
## <a name="advanced-inventory-reconciliation"></a>Advanced: Inventory Reconciliation
When you post inventory transactions, such as sales shipments, purchase invoices, or inventory adjustments, the changed item costs are recorded in item value entries. To reflect this change of inventory value in your financial books, the inventory costs are automatically posted to the related inventory accounts in the general ledger. For each inventory transaction that you post, the appropriate values are posted to the inventory account, adjustment account, and COGS account in the general ledger.

Even though inventory costs are automatically posted to the general ledger, it is still necessary to ensure that the costs of goods are forwarded to the related outbound sales transaction, especially in situations where you sell goods before you invoice the purchase of those goods. This is referred to as cost adjustment. Item costs are automatically adjusted when you post item transactions, but you can also adjust item costs manually. For more information, see [How to: Adjust Item Costs](inventory-how-adjust-item-costs.md).

## <a name="see-also"></a>See Also
[Inventory](inventory-manage-inventory.md)  
[Advanced: Best Price Calculation](advanced-best-price-calculation.md)

