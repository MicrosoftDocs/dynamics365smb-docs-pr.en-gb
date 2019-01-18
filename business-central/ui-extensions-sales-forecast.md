---
title: Using the Sales and Inventory Forecast Extension to Manage Inventory | Microsoft Docs
description: This extension helps you predict sales, get a clear overview of expected stock-outs, and even helps you create replenishment requests to vendors.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, budget
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 3ae36c5cb7f1738bded3947c99c197221a621f07
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="the-sales-and-inventory-forecast-extension"></a><span data-ttu-id="260c0-103">The Sales and Inventory Forecast Extension</span><span class="sxs-lookup"><span data-stu-id="260c0-103">The Sales and Inventory Forecast Extension</span></span>
<span data-ttu-id="260c0-104">Inventory management is a trade-off between customer service and managing your cost.</span><span class="sxs-lookup"><span data-stu-id="260c0-104">Inventory management is a trade-off between customer service and managing your cost.</span></span> <span data-ttu-id="260c0-105">On one hand, a low inventory requires less working capital, but, on the other hand, stock-outs potentially lead to missed sales.</span><span class="sxs-lookup"><span data-stu-id="260c0-105">On one hand, a low inventory requires less working capital, but, on the other hand, stock-outs potentially lead to missed sales.</span></span> <span data-ttu-id="260c0-106">The Sales and Inventory Forecast extension predicts potential sales using historical data and gives a clear overview of expected stock-outs.</span><span class="sxs-lookup"><span data-stu-id="260c0-106">The Sales and Inventory Forecast extension predicts potential sales using historical data and gives a clear overview of expected stock-outs.</span></span> <span data-ttu-id="260c0-107">Based on the forecast, the extension helps create replenishment requests to your vendors and saves you time.</span><span class="sxs-lookup"><span data-stu-id="260c0-107">Based on the forecast, the extension helps create replenishment requests to your vendors and saves you time.</span></span>  

## <a name="setting-up-forecasting"></a><span data-ttu-id="260c0-108">Setting up Forecasting</span><span class="sxs-lookup"><span data-stu-id="260c0-108">Setting up Forecasting</span></span>
<span data-ttu-id="260c0-109">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the connection to [Cortana Intelligence](https://www.microsoft.com/en-us/cloud-platform/what-is-cortana-intelligence-suite) is already set up for you.</span><span class="sxs-lookup"><span data-stu-id="260c0-109">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the connection to [Cortana Intelligence](https://www.microsoft.com/en-us/cloud-platform/what-is-cortana-intelligence-suite) is already set up for you.</span></span> <span data-ttu-id="260c0-110">But you can configure the forecast to use a different type of period to report by, such as changing from forecasting by month to forecasting by quarter.</span><span class="sxs-lookup"><span data-stu-id="260c0-110">But you can configure the forecast to use a different type of period to report by, such as changing from forecasting by month to forecasting by quarter.</span></span> <span data-ttu-id="260c0-111">You can also choose the number of periods to calculate the forecast by, depending on how granular you want the forecast to be.</span><span class="sxs-lookup"><span data-stu-id="260c0-111">You can also choose the number of periods to calculate the forecast by, depending on how granular you want the forecast to be.</span></span> <span data-ttu-id="260c0-112">We suggest that you forecast by month and with a 12 month horizon for the forecast.</span><span class="sxs-lookup"><span data-stu-id="260c0-112">We suggest that you forecast by month and with a 12 month horizon for the forecast.</span></span>  

## <a name="using-the-forecasts"></a><span data-ttu-id="260c0-113">Using the Forecasts</span><span class="sxs-lookup"><span data-stu-id="260c0-113">Using the Forecasts</span></span>
<span data-ttu-id="260c0-114">The extension uses Cortana Intelligence to predict future sales based on your sales history to help you avoid inventory shortage.</span><span class="sxs-lookup"><span data-stu-id="260c0-114">The extension uses Cortana Intelligence to predict future sales based on your sales history to help you avoid inventory shortage.</span></span> <span data-ttu-id="260c0-115">For example, when you choose an item on the **Items** page, the chart in the **Item Forecast** pane shows the estimated sales of this item in the coming period.</span><span class="sxs-lookup"><span data-stu-id="260c0-115">For example, when you choose an item on the **Items** page, the chart in the **Item Forecast** pane shows the estimated sales of this item in the coming period.</span></span> <span data-ttu-id="260c0-116">This way you can see if you are likely to run out of stock of the item soon.</span><span class="sxs-lookup"><span data-stu-id="260c0-116">This way you can see if you are likely to run out of stock of the item soon.</span></span>  

<span data-ttu-id="260c0-117">You can also use the extension to suggest when to stock up on inventory.</span><span class="sxs-lookup"><span data-stu-id="260c0-117">You can also use the extension to suggest when to stock up on inventory.</span></span> <span data-ttu-id="260c0-118">For example, if you crate a purchase order for Fabrikam because you want to buy their new desk chair, the Sales and Inventory Forecast extension will suggest that you also restock on the LONDON swivel chair that you usually buy from this vendor.</span><span class="sxs-lookup"><span data-stu-id="260c0-118">For example, if you crate a purchase order for Fabrikam because you want to buy their new desk chair, the Sales and Inventory Forecast extension will suggest that you also restock on the LONDON swivel chair that you usually buy from this vendor.</span></span> <span data-ttu-id="260c0-119">This is because the extension forecasts that you will run out of stock of the LONDON swivel chair in the coming two months, so you might want to order more chairs already now.</span><span class="sxs-lookup"><span data-stu-id="260c0-119">This is because the extension forecasts that you will run out of stock of the LONDON swivel chair in the coming two months, so you might want to order more chairs already now.</span></span>  

## <a name="see-also"></a><span data-ttu-id="260c0-120">See Also</span><span class="sxs-lookup"><span data-stu-id="260c0-120">See Also</span></span>
[<span data-ttu-id="260c0-121">Sales</span><span class="sxs-lookup"><span data-stu-id="260c0-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="260c0-122">Inventory</span><span class="sxs-lookup"><span data-stu-id="260c0-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="260c0-123">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="260c0-123">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  

