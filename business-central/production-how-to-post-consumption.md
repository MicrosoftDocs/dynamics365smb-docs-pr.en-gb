---
title: How to Batch Post Consumption | Microsoft Docs
description: If the flushing method is **Manual**, you must post the components manually, using a consumption journal.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: ad21fa7f0a18b3549bdab19c07e0065d5fb684dd
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4759174"
---
# <a name="batch-post-production-consumption"></a>Batch Post Production Consumption
If the flushing method is **Manual**, you must post the components manually, using a consumption journal.

You can also set the system up to automatically post (*flush*) components when you start or finish production orders. For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a>To post consumption for one or more production order lines  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Consumption Journal**, and then choose the related link.  
2.  Fill in the fields with the production order data and the consumption data. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse. For more information, see [Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).  
3.  Choose the **Post** action to post the consumption. The related item ledger entries are reduced.

## <a name="see-also"></a>See Also  
[Manufacturing](production-manage-manufacturing.md)    
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Planning](production-planning.md)      
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]