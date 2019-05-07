---
title: Design Details - The Role of the Time Bucket | Microsoft Docs
description: The purpose of the time bucket is to collect demand events within the time page in order to make a joint supply order.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: 54d4a4aed94b562b82d94d6a5a75a3050c054fc3
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "929652"
---
# <a name="design-details-the-role-of-the-time-bucket"></a><span data-ttu-id="5c6cc-103">Design Details: The Role of the Time Bucket</span><span class="sxs-lookup"><span data-stu-id="5c6cc-103">Design Details: The Role of the Time Bucket</span></span>
<span data-ttu-id="5c6cc-104">The purpose of the time bucket is to collect demand events within the time page in order to make a joint supply order.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-104">The purpose of the time bucket is to collect demand events within the time page in order to make a joint supply order.</span></span>  

 <span data-ttu-id="5c6cc-105">For reordering policies that use a reorder point, you can define a time bucket.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-105">For reordering policies that use a reorder point, you can define a time bucket.</span></span> <span data-ttu-id="5c6cc-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span></span> <span data-ttu-id="5c6cc-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span></span> <span data-ttu-id="5c6cc-108">The time buckets begin on the planning starting date.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-108">The time buckets begin on the planning starting date.</span></span>  

 <span data-ttu-id="5c6cc-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span></span> <span data-ttu-id="5c6cc-110">The user needs to define the frequency (the time bucket).</span><span class="sxs-lookup"><span data-stu-id="5c6cc-110">The user needs to define the frequency (the time bucket).</span></span> <span data-ttu-id="5c6cc-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span></span>  

 <span data-ttu-id="5c6cc-112">![Example of time bucket in planning](media/nav_app_supply_planning_2_reorder_cycle.png "Example of time bucket in planning")</span><span class="sxs-lookup"><span data-stu-id="5c6cc-112">![Example of time bucket in planning](media/nav_app_supply_planning_2_reorder_cycle.png "Example of time bucket in planning")</span></span>  

 <span data-ttu-id="5c6cc-113">The time bucket is generally used to avoid a cascade effect.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-113">The time bucket is generally used to avoid a cascade effect.</span></span> <span data-ttu-id="5c6cc-114">For example, a balanced row of demand and supply where an early demand is cancelled, or a new one is created.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-114">For example, a balanced row of demand and supply where an early demand is canceled, or a new one is created.</span></span> <span data-ttu-id="5c6cc-115">The result would be that every supply order (except the last one) is rescheduled.</span><span class="sxs-lookup"><span data-stu-id="5c6cc-115">The result would be that every supply order (except the last one) is rescheduled.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5c6cc-116">See Also</span><span class="sxs-lookup"><span data-stu-id="5c6cc-116">See Also</span></span>  
 <span data-ttu-id="5c6cc-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="5c6cc-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="5c6cc-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="5c6cc-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="5c6cc-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="5c6cc-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="5c6cc-120">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="5c6cc-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
