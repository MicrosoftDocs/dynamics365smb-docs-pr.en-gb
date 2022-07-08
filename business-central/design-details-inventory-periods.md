---
title: Design Details - Stock Periods
description: Stock Periods helps avoid problems with balances and stock valuations by opening or closing stock periods to limit posting in a set period of time.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/15/2021
ms.author: edupont
ms.openlocfilehash: 77348fbf2ef37320b0bfa0ea56a0d395f9b4b142
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2022
ms.locfileid: "8133895"
---
# <a name="design-details-inventory-periods"></a>Design Details: Stock Periods
Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed. This can have adverse effects on accurate reporting, especially within global corporations. The Stock Periods feature can be used to avoid such problems by opening or closing stock periods to limit posting in a set period of time.  

 A stock period is a period of time, defined by an ending date, in which you post stock transactions. When you close a stock period, no value changes can be posted in the closed period. This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments. However, you can still apply to an open item ledger entry that falls in the closed period. For more information, see [Design Details: Item Application](design-details-item-application.md).  

 To make sure that all transaction entries in a closed period are final, the following conditions must be met before a stock period can close:  

-   All outbound item ledger entries in the period must be closed (no negative stock).  
-   All item costs in the period must be adjusted.  
-   All released and finished production orders in the period must be cost adjusted.  

 When you close a stock period, a stock period entry is created by using the number of the last item register that falls in the stock period. In addition, the time, date, and user code of the user closing the period are recorded in the stock period entry. By using this information with the last item register for the previous period, you can see which stock transactions were posted in the stock period. It is also possible to reopen stock periods if you need to post in a closed period. When you reopen a stock period, a stock period entry is created.  

## <a name="see-also"></a>See Also

[Design Details: Stock Costing](design-details-inventory-costing.md)  
[Managing Stock Costs](finance-manage-inventory-costs.md)  
[Finance](finance.md)  
[Working with Business Central](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]