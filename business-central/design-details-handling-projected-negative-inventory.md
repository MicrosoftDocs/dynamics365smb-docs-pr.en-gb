---
title: Design Details - Handling Projected Negative Inventory | Microsoft Docs
description: The reorder point expresses the anticipated demand during the lead time of the item. When the reorder point is passed, it is time to order more. But the projected inventory must be large enough to cover the demand until the new order is received. Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.
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
ms.openlocfilehash: cfedced3a1e7ccf94294ebd36f4fb5311fd1933e
ms.contentlocale: en-gb
ms.lasthandoff: 11/20/2018

---
# <a name="design-details-handling-projected-negative-inventory"></a><span data-ttu-id="b1318-106">Design Details: Handling Projected Negative Inventory</span><span class="sxs-lookup"><span data-stu-id="b1318-106">Design Details: Handling Projected Negative Inventory</span></span>
<span data-ttu-id="b1318-107">The reorder point expresses the anticipated demand during the lead time of the item.</span><span class="sxs-lookup"><span data-stu-id="b1318-107">The reorder point expresses the anticipated demand during the lead time of the item.</span></span> <span data-ttu-id="b1318-108">When the reorder point is passed, it is time to order more.</span><span class="sxs-lookup"><span data-stu-id="b1318-108">When the reorder point is passed, it is time to order more.</span></span> <span data-ttu-id="b1318-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span><span class="sxs-lookup"><span data-stu-id="b1318-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span></span> <span data-ttu-id="b1318-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span><span class="sxs-lookup"><span data-stu-id="b1318-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span></span>  

 <span data-ttu-id="b1318-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span><span class="sxs-lookup"><span data-stu-id="b1318-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span></span> <span data-ttu-id="b1318-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span><span class="sxs-lookup"><span data-stu-id="b1318-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span></span> <span data-ttu-id="b1318-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span><span class="sxs-lookup"><span data-stu-id="b1318-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span></span> <span data-ttu-id="b1318-114">Instead, it will reflect the exact deficiency.</span><span class="sxs-lookup"><span data-stu-id="b1318-114">Instead, it will reflect the exact deficiency.</span></span>  

 <span data-ttu-id="b1318-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span><span class="sxs-lookup"><span data-stu-id="b1318-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span></span>  

 <span data-ttu-id="b1318-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span><span class="sxs-lookup"><span data-stu-id="b1318-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span></span>  

 <span data-ttu-id="b1318-117">![Emergency planning suggestion to avoid negative inventory](media/nav_app_supply_planning_2_negative_inventory.png "Emergency planning suggestion to avoid negative inventory")</span><span class="sxs-lookup"><span data-stu-id="b1318-117">![Emergency planning suggestion to avoid negative inventory](media/nav_app_supply_planning_2_negative_inventory.png "Emergency planning suggestion to avoid negative inventory")</span></span>  

1.  <span data-ttu-id="b1318-118">Supply **A**, initial projected inventory, is below reorder point.</span><span class="sxs-lookup"><span data-stu-id="b1318-118">Supply **A**, initial projected inventory, is below reorder point.</span></span>  
2.  <span data-ttu-id="b1318-119">A new forward-scheduled supply is created (**C**).</span><span class="sxs-lookup"><span data-stu-id="b1318-119">A new forward-scheduled supply is created (**C**).</span></span>  

     <span data-ttu-id="b1318-120">(Quantity = Maximum Inventory – Projected Inventory Level)</span><span class="sxs-lookup"><span data-stu-id="b1318-120">(Quantity = Maximum Inventory – Projected Inventory Level)</span></span>  
3.  <span data-ttu-id="b1318-121">Supply **A** is closed by demand **B**, which is not fully covered.</span><span class="sxs-lookup"><span data-stu-id="b1318-121">Supply **A** is closed by demand **B**, which is not fully covered.</span></span>  

     <span data-ttu-id="b1318-122">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span><span class="sxs-lookup"><span data-stu-id="b1318-122">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span></span>  
4.  <span data-ttu-id="b1318-123">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span><span class="sxs-lookup"><span data-stu-id="b1318-123">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span></span>  
5.  <span data-ttu-id="b1318-124">Demand **B** is closed (creating a reminder to the projected inventory).</span><span class="sxs-lookup"><span data-stu-id="b1318-124">Demand **B** is closed (creating a reminder to the projected inventory).</span></span>  
6.  <span data-ttu-id="b1318-125">The new supply **D** is closed.</span><span class="sxs-lookup"><span data-stu-id="b1318-125">The new supply **D** is closed.</span></span>  
7.  <span data-ttu-id="b1318-126">Projected Inventory is checked; reorder point has not been crossed.</span><span class="sxs-lookup"><span data-stu-id="b1318-126">Projected Inventory is checked; reorder point has not been crossed.</span></span>  
8.  <span data-ttu-id="b1318-127">Supply **C** is closed (no more demand exists).</span><span class="sxs-lookup"><span data-stu-id="b1318-127">Supply **C** is closed (no more demand exists).</span></span>  
9. <span data-ttu-id="b1318-128">Final check: No outstanding inventory level reminders exist.</span><span class="sxs-lookup"><span data-stu-id="b1318-128">Final check: No outstanding inventory level reminders exist.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="b1318-129">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span><span class="sxs-lookup"><span data-stu-id="b1318-129">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span></span>  

 <span data-ttu-id="b1318-130">This concludes the description of central principles relating to inventory planning based on reordering policies.</span><span class="sxs-lookup"><span data-stu-id="b1318-130">This concludes the description of central principles relating to inventory planning based on reordering policies.</span></span> <span data-ttu-id="b1318-131">The following section describes the characteristics of the four supported reordering policies.</span><span class="sxs-lookup"><span data-stu-id="b1318-131">The following section describes the characteristics of the four supported reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b1318-132">See Also</span><span class="sxs-lookup"><span data-stu-id="b1318-132">See Also</span></span>  
 <span data-ttu-id="b1318-133">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="b1318-133">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="b1318-134">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="b1318-134">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="b1318-135">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="b1318-135">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="b1318-136">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="b1318-136">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

