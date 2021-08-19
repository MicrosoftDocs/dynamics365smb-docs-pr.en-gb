---
title: Managing Stock Costs
description: Cost management is concerned with recording and reporting business operating costs and includes the reporting of manufacturing costs and stock costs.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: 561401c985fc0e2f25c4f6e719252d19e76e7fe8
ms.sourcegitcommit: 769d20d299155cba30c35636d02b2ef021e4ecc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/29/2021
ms.locfileid: "6688350"
---
# <a name="managing-inventory-costs"></a>Managing Stock Costs
Cost management, also referred to as “costing”, is concerned with recording and reporting business operating costs. It includes the reporting of manufacturing costs and stock costs, that is, the value of items.   

Central principles to understand are that costing methods define how items are valued when they leave stock, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that stock values must be posted to dedicated G/L accounts at regular intervals.

The following table describes a sequence of tasks, with links to the topics that describe them.

|**To**|**See**|  
|------------|-------------|  
|Read various conceptual information to understand the principles and definitions that govern the stock costing accounting functionality in [!INCLUDE[prod_short](includes/prod_short.md)].|[About Stock Costing](finance-learn-about-costing.md)|  
|Ensure that you know the cost of shipped items by assigning added item costs, such as freight, physical handling, insurance, and transportation that you incur after selling.|[Use Item Charges to Account for Additional Trade Costs](payables-how-assign-item-charges.md)|
|Learn about all mechanisms in the costing system.|[Design Details: Stock Costing](design-details-inventory-costing.md)|
|Read how stock periods help a company to control stock value over time by defining shorter periods that can be closed for posting as the financial year progresses.|[Work with Stock Periods](finance-how-to-work-with-inventory-periods.md)|
|Read why standard costs are often used by manufacturing companies as a valuation base for components and end items.|[About Calculating Standard Cost](finance-about-calculating-standard-cost.md)|
|Set up stock periods, costing methods, and rounding methods.|[Setting Up Stock Valuation and Costing](finance-set-up-inventory-valuation-and-costing.md)|
|Appreciate or depreciate the value of one or more items in stock by posting their current, calculated value.|[Revalue Stock](inventory-how-revalue-inventory.md)|
|Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.|[Adjust Item Costs](inventory-how-adjust-item-costs.md)|
|Use special costing functions for every-day item transactions in the item operations.|[Handling Stock and Manufacturing Costs](finance-handle-inventory-and-manufacturing-costs.md)|  
|Periodically update the standard costs of components, in assembly or production BOMs, and roll the new costs up to the parent item.|[Update Standard Costs](finance-how-to-update-standard-costs.md)|
|View and manually change certain item application entries that are created automatically during stock transactions.|[Remove and Reapply Item Ledger Entries](finance-how-to-remove-and-reapply-item-entries.md)|
|Perform period-end control and reporting tasks, such as calculate the value of stock and post costs to the general ledger.|[Reporting Costs and Reconciling with the General Ledger](finance-report-costs-and-reconcile-with-the-general-ledger.md)|
|Learn how you can use the job queue to move the tasks for adjusting stock cost or reconciling it with the general ledger to the background.|[Adjust and Reconcile Stock Cost with General Ledger with Job Queue](finance-manage-inventory-costs.md)|

## <a name="see-also"></a>See Also  
 [Finance](finance.md)  
 [Stock](inventory-manage-inventory.md)   
 [Sales](sales-manage-sales.md)   
 [Purchasing](purchasing-manage-purchasing.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]