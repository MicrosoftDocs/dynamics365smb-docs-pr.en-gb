---
title: Using the Sales and Inventory Forecast Extension to Manage Inventory | Microsoft Docs
description: This extension helps you predict sales, get a clear overview of expected stock-outs, and even helps you create replenishment requests to vendors.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, budget
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: a0cac0236611c90d3d1fdf1bae9deaaeb235b540
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="sales-and-inventory-forecast-for-dynamics-365-for-financials"></a>Sales and Inventory Forecast for Dynamics 365 for Financials
Inventory management is a trade-off between customer service and managing your cost. On one hand, a low inventory requires less working capital, but, on the other hand, stock-outs potentially lead to missed sales. The Sales and Inventory Forecast extension predicts potential sales using historical data and gives a clear overview of expected stock-outs. Based on the forecast, the extension helps create replenishment requests to your vendors and saves you time.  

## <a name="setting-up-forecasting"></a>Setting up forecasting
In [!INCLUDE[d365fin](includes/d365fin_md.md)], the connection to [Cortana Intelligence](https://www.microsoft.com/en-us/cloud-platform/what-is-cortana-intelligence-suite) is already set up for you. But you can configure the forecast to use a different type of period to report by, such as changing from forecasting by month to forecasting by quarter. You can also choose the number of periods to calculate the forecast by, depending on how granular you want the forecast to be. We suggest that you forecast by month and with a 12 month horizon for the forecast.  

## <a name="using-the-forecasts"></a>Using the forecasts
The extension uses Cortana Intelligence to predict future sales based on your sales history to help you avoid inventory shortage. For example, when you choose an item in the **Items** window, the chart in the **Item Forecast** pane shows the estimated sales of this item in the coming period. This way you can see if you are likely to run out of stock of the item soon.  

You can also use the extension to suggest when to stock up on inventory. For example, if you crate a purchase order for Fabrikam because you want to buy their new desk chair, the Sales and Inventory Forecast extension will suggest that you also restock on the LONDON swivel chair that you usually buy from this vendor. This is because the extension forecasts that you will run out of stock of the LONDON swivel chair in the coming two months, so you might want to order more chairs already now.  

## <a name="see-also"></a>See Also
[Sales](sales-manage-sales.md)  
[Inventory](inventory-manage-inventory.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  

