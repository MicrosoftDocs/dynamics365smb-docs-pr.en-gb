---
title: Create Works Order Headers
description: You can create a works order manually, and the first step is to create a works order header.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 9325, 99000815, 99000829, 9900083
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 814770db81744306120445a509325cff8502041d
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2022
ms.locfileid: "8516855"
---
# <a name="create-production-order-headers"></a>Create Works Order Headers

You can create a works order manually, and the first step is to create a works order header.

Works orders are typically created automatically by a planning function to fulfil a known demand. For more information, see [Planning](production-planning.md).  

In the following procedure, a firm planned works order is created. You can also create works orders with a different status.  

## <a name="to-create-a-production-order-header"></a>To create a works order header

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.  
2. Choose the **New** action.  
3. In the **No.** field, insert the next number in the series.  
4. In the **Source Type** field, select the source of the works order.

Here you can select to produce for a family of items. For more information, see [Work With Production Families](production-how-work-family.md).
5. In the **Source No.** field, select the item number, family, or sales header for which the works order is to be generated.  
6. Fill in the **Quantity** and **Due Date** fields according to your specifications.  

When production requirements change, such as components or operations, you can quickly replan the works order. For more information, see [Replan or Refresh Works Orders Directly](production-how-to-replan-refresh-production-orders.md).  

## <a name="see-also"></a>See Also

[Manufacturing](production-manage-manufacturing.md)
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Planning](production-planning.md)  
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]