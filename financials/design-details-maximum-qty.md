---
title: Design Details - Maximum Qty. | Microsoft Docs
description: The Maximum Quantity policy is a way to maintain inventory using a reorder point.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 26bed0b8832d5b12ce5d697df8ec6194ac7ae9b2
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-maximum-qty"></a><span data-ttu-id="1a0c6-103">Design Details: Maximum Qty.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-103">Design Details: Maximum Qty.</span></span>
<span data-ttu-id="1a0c6-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span></span>  
  
 <span data-ttu-id="1a0c6-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span></span> <span data-ttu-id="1a0c6-106">The only difference is the quantity of the suggested supply.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-106">The only difference is the quantity of the suggested supply.</span></span> <span data-ttu-id="1a0c6-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span></span>  
  
## <a name="calculated-per-time-bucket"></a><span data-ttu-id="1a0c6-108">Calculated per Time Bucket</span><span class="sxs-lookup"><span data-stu-id="1a0c6-108">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="1a0c6-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span></span> <span data-ttu-id="1a0c6-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span></span> <span data-ttu-id="1a0c6-111">This constitutes the quantity that should be reordered.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-111">This constitutes the quantity that should be reordered.</span></span> <span data-ttu-id="1a0c6-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span></span>  
  
 <span data-ttu-id="1a0c6-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span></span>  
  
## <a name="combines-with-order-modifiers"></a><span data-ttu-id="1a0c6-114">Combines with Order Modifiers</span><span class="sxs-lookup"><span data-stu-id="1a0c6-114">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="1a0c6-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span></span>  
  
## <a name="combines-with-calendars"></a><span data-ttu-id="1a0c6-116">Combines with Calendars</span><span class="sxs-lookup"><span data-stu-id="1a0c6-116">Combines with Calendars</span></span>  
 <span data-ttu-id="1a0c6-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** windows.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** windows.</span></span>  
  
 <span data-ttu-id="1a0c6-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="1a0c6-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="1a0c6-120">For such unbalanced demand, the planning system creates an extra supply.</span><span class="sxs-lookup"><span data-stu-id="1a0c6-120">For such unbalanced demand, the planning system creates an extra supply.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="1a0c6-121">See Also</span><span class="sxs-lookup"><span data-stu-id="1a0c6-121">See Also</span></span>  
 <span data-ttu-id="1a0c6-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="1a0c6-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="1a0c6-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="1a0c6-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="1a0c6-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="1a0c6-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="1a0c6-125">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="1a0c6-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
