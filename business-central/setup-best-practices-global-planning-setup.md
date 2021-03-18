---
title: Best practices for global planning setup | Microsoft Docs
description: The Planning FastTab in the Manufacturing Setup page contains several fields that define global rules for supply planning.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 9dfc1c42d2ce74792209b25b1fb6e48126ed9d5a
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5391106"
---
# <a name="setup-best-practices-global-planning-setup"></a><span data-ttu-id="36acf-103">Setup Best Practices: Global Planning Setup</span><span class="sxs-lookup"><span data-stu-id="36acf-103">Setup Best Practices: Global Planning Setup</span></span>
<span data-ttu-id="36acf-104">The **Planning** FastTab on the **Manufacturing Setup** page contains several fields that define global rules for supply planning.</span><span class="sxs-lookup"><span data-stu-id="36acf-104">The **Planning** FastTab on the **Manufacturing Setup** page contains several fields that define global rules for supply planning.</span></span>  

 <span data-ttu-id="36acf-105">The following table provides best practices on how to set up selected global planning parameter fields.</span><span class="sxs-lookup"><span data-stu-id="36acf-105">The following table provides best practices on how to set up selected global planning parameter fields.</span></span> <span data-ttu-id="36acf-106">For more information about a field, choose the link in the **Setup field** column.</span><span class="sxs-lookup"><span data-stu-id="36acf-106">For more information about a field, choose the link in the **Setup field** column.</span></span>  

|<span data-ttu-id="36acf-107">Setup field</span><span class="sxs-lookup"><span data-stu-id="36acf-107">Setup field</span></span>|<span data-ttu-id="36acf-108">Best practice</span><span class="sxs-lookup"><span data-stu-id="36acf-108">Best practice</span></span>|<span data-ttu-id="36acf-109">Comment</span><span class="sxs-lookup"><span data-stu-id="36acf-109">Comment</span></span>|  
|-----------------|-------------------|-------------|  
|<span data-ttu-id="36acf-110">Use Forecast on Locations</span><span class="sxs-lookup"><span data-stu-id="36acf-110">Use Forecast on Locations</span></span>|<span data-ttu-id="36acf-111">Select if you have forecasts for specific locations.</span><span class="sxs-lookup"><span data-stu-id="36acf-111">Select if you have forecasts for specific locations.</span></span>||  
|<span data-ttu-id="36acf-112">Components at Location</span><span class="sxs-lookup"><span data-stu-id="36acf-112">Components at Location</span></span>|<span data-ttu-id="36acf-113">If items are not defined as SKUs, select the location code of your main warehouse.</span><span class="sxs-lookup"><span data-stu-id="36acf-113">If items are not defined as SKUs, select the location code of your main warehouse.</span></span>|<span data-ttu-id="36acf-114">This also applies if you only use the requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="36acf-114">This also applies if you only use the requisition worksheet.</span></span>|  
|<span data-ttu-id="36acf-115">Blank Overflow Level</span><span class="sxs-lookup"><span data-stu-id="36acf-115">Blank Overflow Level</span></span>|<span data-ttu-id="36acf-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span><span class="sxs-lookup"><span data-stu-id="36acf-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span></span>|<span data-ttu-id="36acf-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span><span class="sxs-lookup"><span data-stu-id="36acf-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span></span>|  
|<span data-ttu-id="36acf-118">Default Dampener Period</span><span class="sxs-lookup"><span data-stu-id="36acf-118">Default Dampener Period</span></span>|<span data-ttu-id="36acf-119">Set between 1D and 5D.</span><span class="sxs-lookup"><span data-stu-id="36acf-119">Set between 1D and 5D.</span></span><br /><br /> <span data-ttu-id="36acf-120">If new to planning in [!INCLUDE[prod_short](includes/prod_short.md)], then set a longer period.</span><span class="sxs-lookup"><span data-stu-id="36acf-120">If new to planning in [!INCLUDE[prod_short](includes/prod_short.md)], then set a longer period.</span></span>|<span data-ttu-id="36acf-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span><span class="sxs-lookup"><span data-stu-id="36acf-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span></span>|  
|<span data-ttu-id="36acf-122">Default Dampener Quantity %</span><span class="sxs-lookup"><span data-stu-id="36acf-122">Default Dampener Quantity %</span></span>|<span data-ttu-id="36acf-123">Set between 5 and 20 percent of the item’s lot size.</span><span class="sxs-lookup"><span data-stu-id="36acf-123">Set between 5 and 20 percent of the item’s lot size.</span></span>||  

## <a name="see-also"></a><span data-ttu-id="36acf-124">See Also</span><span class="sxs-lookup"><span data-stu-id="36acf-124">See Also</span></span>  
 <span data-ttu-id="36acf-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="36acf-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span></span>  
 <span data-ttu-id="36acf-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="36acf-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
 [<span data-ttu-id="36acf-127">Set Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="36acf-127">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="36acf-128">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="36acf-128">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]