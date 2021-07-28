---
title: Define the General Stock Setup
description: Describes how to define the general stock setup so that you can manage your warehouse and stock.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a99de8575891e15712e221f28bbf3f4a46f2f771
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6435629"
---
# <a name="set-up-general-inventory-information"></a>Set Up General Stock Information

You specify your general stock setup on the **Stock Setup** page.

## <a name="to-set-up-general-inventory-information"></a>To set up general stock information

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stock Setup**, and then choose the related link.
2. On the **Stock Setup** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

For detailed information about the costing fields, **Automatic Cost Posting**, **Expected Cost Posting to G/L**, and **Default Costing Method**, see [Reconcile Stock Costs with the General Ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md), [Design Details: Stock Costing](design-details-inventory-costing.md), and [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md). For more information about costing in general, see [Managing Stock Costs](finance-manage-inventory-costs.md).  

If you want to include warehouse handling time in the order promising calculation on the purchase line, you can set it up as a default for the stock, on the **Stock Setup** page, and for your location. For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).  

> [!NOTE]
> The **Automatic Cost Adjustment** toggle is turned on by default to ensure that stock values are always correct in the general ledger, which in turn keeps your sales and profit statistics up to date. Cost changes from inbound entries, such as those for purchases or production output, are assigned to the related outbound entries, such as sales or transfers. This is helpful for new [!INCLUDE[prod_short](includes/prod_short.md)] customers and small businesses with relatively low stock transaction levels. However, as a business grows and stock levels increase, this can slow down system performance. To minimise reduced performance during posting, select a time option to define how far back in time from the work date an inbound transaction can occur to potentially trigger adjustment of related outbound value entries. Alternatively, you can manually adjust costs at regular intervals with the Adjust Cost - Item Entries batch job.

## <a name="see-also"></a>See Also
[Set Up Stock](inventory-setup-inventory.md)  
[Design Details: Costing Methods](design-details-costing-methods.md)    
[Manage Stock](inventory-manage-inventory.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[General Business Functionality](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]