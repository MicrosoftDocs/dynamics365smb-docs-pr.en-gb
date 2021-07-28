---
title: Batch Post Consumption
description: If the flushing method is Manual, you must post the components manually, using a consumption journal.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 2f31c7f48e88a44eb3f437827b6b24f255180d9a
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6440435"
---
# <a name="batch-post-production-consumption"></a>Batch Post Production Consumption

If the flushing method is **Manual**, you must post the components manually, using a consumption journal.  

>[!NOTE]
> If you have placed a check mark in the **Require Pick** field on the location card to indicate that the location requires stock pick processing, then you do not need to use this batch job. [!INCLUDE[prod_short](includes/prod_short.md)] will handle consumption when you post the stock pick. For more information, see [Pick for Production in Basic Warehouse Configurations](warehouse-how-to-pick-for-production.md#pick-for-production-in-basic-warehouse-configurations).  

You can also set up [!INCLUDE[prod_short](includes/prod_short.md)] to automatically post (*flush*) components when you start or finish works orders. For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a>To post consumption for one or more works order lines

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Consumption Journal**, and then choose the related link.  
2. Fill in the fields with the works order data and the consumption data. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    Use the **Calc. Consumption** action to generate journal lines from works orders based on the actual output (the quantity of finished goods that you have reported) or on the expected output (the quantity of finished goods that you expect to produce).

    > [!NOTE]
    > If you configured the location card to require warehouse pick processing, then only quantities that are already picked through a warehouse activity can be entered in the **Quantity** field in the **Consumption Journal** page, not any calculated quantity. For more information, see [Pick for Production or Assembly in Advanced Warehouse Configurations](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md)

3. Choose the **Post** action to post the consumption. The related stocks are reduced.

## <a name="see-also"></a>See Also

[Manufacturing](production-manage-manufacturing.md)  
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Planning](production-planning.md)  
[Stock](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
