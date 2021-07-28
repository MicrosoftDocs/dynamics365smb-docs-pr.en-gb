---
title: Date Calculation for Purchases
description: The application automatically calculates the date on which you must order an item to have it in stock on a certain date.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/22/2021
ms.author: edupont
ms.openlocfilehash: 6758c631fcddf157894ed06a483b811342a44e0d
ms.sourcegitcommit: e562b45fda20ff88230e086caa6587913eddae26
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/30/2021
ms.locfileid: "6321046"
---
# <a name="date-calculation-for-purchases"></a>Date Calculation for Purchases

[!INCLUDE[prod_short](includes/prod_short.md)] automatically calculates the date on which you must order an item to have it in stock on a certain date. This is the date on which you can expect items ordered on a particular date to be available for picking.  

If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested. Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.  

If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.  

## <a name="calculating-with-a-requested-receipt-date"></a>Calculating with a requested receipt date

If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.  

- requested receipt date - lead time calculation = order date  
- requested receipt date + inbound whse. handling time + safety lead time = expected receipt date  

If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines. You can change this date on any of the lines, or you can remove the date on the line.  

> [!NOTE]
> If your process is based on backward calculation, for example, if you use the requested receipt date to get the order date, we recommend that you use date formulas that have fixed durations, such as "5D" for five days or "1W" for one week. Date formulas without fixed durations, such as "CW" for current week or CM for current month, can result in incorrect date calculations. For more information about date formulas, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).

## <a name="calculating-without-a-requested-delivery-date"></a>Calculating without a requested delivery date

If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header. This is either the date that you entered or the work date. The following dates are then calculated for the purchase order line, with the order date as the starting point.  

- order date + lead time calculation = planned receipt date  
- planned receipt date + inbound whse. handling time + safety lead time = expected receipt date  

If you change the order date on the line, such as when items are not available at your supplier until a later date, then the relevant dates on the line are automatically recalculated.  

If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.  

## <a name="default-values-for-lead-time-calculation"></a>Default values for lead time calculation

[!INCLUDE[prod_short](includes/prod_short.md)] uses the value from the **Lead Time Calculation** field on the purchase order line to calculate the order and the expected receipt dates.  

You can manually specify the value on the line or let the program use values that are defined on the supplier card, item card, stockkeeping unit card, or the item supplier catalogue.
However, the lead time value on the supplier card is used only if a lead time is not specified on the item card, stockkeeping unit card, or the item supplier catalogue for the item. This is also the escalating order of priority for these values. If they are all provided, the lead time from the supplier card has the lowest priority, and the lead time from the item supplier catalogue has the highest priority.  

## <a name="see-also"></a>See Also

[Date Calculation for Sales](sales-date-calculation-for-sales.md)   
[Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]