---
title: Best practices for global planning setup | Microsoft Docs
description: The Planning FastTab in the Manufacturing Setup page contains several fields that define global rules for supply planning.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c19f527f4d9c06aa28212e7519fee67c6dfd042b
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3192234"
---
# <a name="setup-best-practices-global-planning-setup"></a><span data-ttu-id="b5cd2-103">Setup Best Practices: Global Planning Setup</span><span class="sxs-lookup"><span data-stu-id="b5cd2-103">Setup Best Practices: Global Planning Setup</span></span>
<span data-ttu-id="b5cd2-104">The **Planning** FastTab on the **Manufacturing Setup** page contains several fields that define global rules for supply planning.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-104">The **Planning** FastTab on the **Manufacturing Setup** page contains several fields that define global rules for supply planning.</span></span>  

 <span data-ttu-id="b5cd2-105">The following table provides best practices on how to set up selected global planning parameter fields.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-105">The following table provides best practices on how to set up selected global planning parameter fields.</span></span> <span data-ttu-id="b5cd2-106">For more information about a field, choose the link in the **Setup field** column.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-106">For more information about a field, choose the link in the **Setup field** column.</span></span>  

|<span data-ttu-id="b5cd2-107">Setup field</span><span class="sxs-lookup"><span data-stu-id="b5cd2-107">Setup field</span></span>|<span data-ttu-id="b5cd2-108">Best practice</span><span class="sxs-lookup"><span data-stu-id="b5cd2-108">Best practice</span></span>|<span data-ttu-id="b5cd2-109">Comment</span><span class="sxs-lookup"><span data-stu-id="b5cd2-109">Comment</span></span>|  
|-----------------|-------------------|-------------|  
|<span data-ttu-id="b5cd2-110">Use Forecast on Locations</span><span class="sxs-lookup"><span data-stu-id="b5cd2-110">Use Forecast on Locations</span></span>|<span data-ttu-id="b5cd2-111">Select if you have forecasts for specific locations.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-111">Select if you have forecasts for specific locations.</span></span>||  
|<span data-ttu-id="b5cd2-112">Components at Location</span><span class="sxs-lookup"><span data-stu-id="b5cd2-112">Components at Location</span></span>|<span data-ttu-id="b5cd2-113">If items are not defined as SKUs, select the location code of your main warehouse.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-113">If items are not defined as SKUs, select the location code of your main warehouse.</span></span>|<span data-ttu-id="b5cd2-114">This also applies if you only use the requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-114">This also applies if you only use the requisition worksheet.</span></span>|  
|<span data-ttu-id="b5cd2-115">Blank Overflow Level</span><span class="sxs-lookup"><span data-stu-id="b5cd2-115">Blank Overflow Level</span></span>|<span data-ttu-id="b5cd2-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span></span>|<span data-ttu-id="b5cd2-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span></span>|  
|<span data-ttu-id="b5cd2-118">Default Dampener Period</span><span class="sxs-lookup"><span data-stu-id="b5cd2-118">Default Dampener Period</span></span>|<span data-ttu-id="b5cd2-119">Set between 1D and 5D.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-119">Set between 1D and 5D.</span></span><br /><br /> <span data-ttu-id="b5cd2-120">If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-120">If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.</span></span>|<span data-ttu-id="b5cd2-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span></span>|  
|<span data-ttu-id="b5cd2-122">Default Dampener Quantity</span><span class="sxs-lookup"><span data-stu-id="b5cd2-122">Default Dampener Quantity</span></span>|<span data-ttu-id="b5cd2-123">Set between 5 and 20 percent of the item’s lot size.</span><span class="sxs-lookup"><span data-stu-id="b5cd2-123">Set between 5 and 20 percent of the item’s lot size.</span></span>||  

## <a name="see-also"></a><span data-ttu-id="b5cd2-124">See Also</span><span class="sxs-lookup"><span data-stu-id="b5cd2-124">See Also</span></span>  
 <span data-ttu-id="b5cd2-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="b5cd2-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span></span>  
 <span data-ttu-id="b5cd2-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="b5cd2-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
 [<span data-ttu-id="b5cd2-127">Set Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="b5cd2-127">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="b5cd2-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd2-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
