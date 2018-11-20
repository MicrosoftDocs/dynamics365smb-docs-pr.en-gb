---
title: Design Details - Lot-for-Lot | Microsoft Docs
description: Learn how to use the lot-for-lot policy to settle order quantity based on demand.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.translationtype: HT
ms.sourcegitcommit: 67400e424305cc705db5c1bd52a8e4de17ecc5a9
ms.openlocfilehash: 7bc65fdb33b94b313b7d2b5b046156ca1d0788a2
ms.contentlocale: en-gb
ms.lasthandoff: 11/20/2018

---
# <a name="design-details-lot-for-lot"></a><span data-ttu-id="22870-103">Design Details: Lot-for-Lot</span><span class="sxs-lookup"><span data-stu-id="22870-103">Design Details: Lot-for-Lot</span></span>
<span data-ttu-id="22870-104">The lot-for-lot policy is the most flexible because the system only reacts on actual demand, plus it acts on anticipated demand from forecast and blanket orders and then settles the order quantity based on the demand.</span><span class="sxs-lookup"><span data-stu-id="22870-104">The lot-for-lot policy is the most flexible because the system only reacts on actual demand, plus it acts on anticipated demand from forecast and blanket orders and then settles the order quantity based on the demand.</span></span> <span data-ttu-id="22870-105">The lot-for-lot policy is aimed at A- and B-items where inventory can be accepted but should be avoided.</span><span class="sxs-lookup"><span data-stu-id="22870-105">The lot-for-lot policy is aimed at A- and B-items where inventory can be accepted but should be avoided.</span></span>  

<span data-ttu-id="22870-106">In some ways, the lot-for-lot policy looks like the Order policy, but it has a generic approach to items; it can accept quantities in inventory, and it bundles demand and corresponding supply in time buckets defined by the user.</span><span class="sxs-lookup"><span data-stu-id="22870-106">In some ways, the lot-for-lot policy looks like the Order policy, but it has a generic approach to items; it can accept quantities in inventory, and it bundles demand and corresponding supply in time buckets defined by the user.</span></span>  

<span data-ttu-id="22870-107">The time bucket is defined in the **Time Bucket** field.</span><span class="sxs-lookup"><span data-stu-id="22870-107">The time bucket is defined in the **Time Bucket** field.</span></span> <span data-ttu-id="22870-108">The system works with a minimum time bucket of one day, since this is the smallest time unit of measure on demand and supply events in the system (although, in practice, the time unit of measure on production orders and component needs can be seconds).</span><span class="sxs-lookup"><span data-stu-id="22870-108">The system works with a minimum time bucket of one day, since this is the smallest time unit of measure on demand and supply events in the system (although, in practice, the time unit of measure on production orders and component needs can be seconds).</span></span>  

<span data-ttu-id="22870-109">The time bucket also sets limits on when an existing supply order should be rescheduled to meet a given demand.</span><span class="sxs-lookup"><span data-stu-id="22870-109">The time bucket also sets limits on when an existing supply order should be rescheduled to meet a given demand.</span></span> <span data-ttu-id="22870-110">If the supply lies within the time bucket, it will be rescheduled in or out to meet the demand.</span><span class="sxs-lookup"><span data-stu-id="22870-110">If the supply lies within the time bucket, it will be rescheduled in or out to meet the demand.</span></span> <span data-ttu-id="22870-111">Otherwise, if it lies earlier, it will cause unnecessary build-up of inventory and should be cancelled.</span><span class="sxs-lookup"><span data-stu-id="22870-111">Otherwise, if it lies earlier, it will cause unnecessary build-up of inventory and should be canceled.</span></span> <span data-ttu-id="22870-112">If it lies later, a new supply order will be created instead.</span><span class="sxs-lookup"><span data-stu-id="22870-112">If it lies later, a new supply order will be created instead.</span></span>  

<span data-ttu-id="22870-113">With this policy, it is also possible to define a safety stock in order to compensate for possible fluctuations in supply, or to meet sudden demand.</span><span class="sxs-lookup"><span data-stu-id="22870-113">With this policy, it is also possible to define a safety stock in order to compensate for possible fluctuations in supply, or to meet sudden demand.</span></span>  

<span data-ttu-id="22870-114">Because the supply order quantity is based on the actual demand it can make sense to use the order modifiers: round the order quantity up to meet a specified order multiple (or purchase unit of measure), increase the order to a specified minimum order quantity, or decrease the quantity to the specified maximum quantity (and thus create two or more supplies to reach the total needed quantity).</span><span class="sxs-lookup"><span data-stu-id="22870-114">Because the supply order quantity is based on the actual demand it can make sense to use the order modifiers: round the order quantity up to meet a specified order multiple (or purchase unit of measure), increase the order to a specified minimum order quantity, or decrease the quantity to the specified maximum quantity (and thus create two or more supplies to reach the total needed quantity).</span></span>  

## <a name="see-also"></a><span data-ttu-id="22870-115">See Also</span><span class="sxs-lookup"><span data-stu-id="22870-115">See Also</span></span>  
<span data-ttu-id="22870-116">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="22870-116">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="22870-117">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="22870-117">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="22870-118">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="22870-118">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="22870-119">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="22870-119">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

