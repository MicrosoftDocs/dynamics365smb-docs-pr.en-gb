---
title: Design Details - Handling Projected Negative Inventory | Microsoft Docs
description: The reorder point expresses the anticipated demand during the lead time of the item. When the reorder point is passed, it is time to order more. But the projected inventory must be large enough to cover the demand until the new order is received. Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.
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
ms.openlocfilehash: 3436e2a00858a1dbfcbb0a44cb9db32bd7665593
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-handling-projected-negative-inventory"></a><span data-ttu-id="150e9-106">Design Details: Handling Projected Negative Inventory</span><span class="sxs-lookup"><span data-stu-id="150e9-106">Design Details: Handling Projected Negative Inventory</span></span>
<span data-ttu-id="150e9-107">The reorder point expresses the anticipated demand during the lead time of the item.</span><span class="sxs-lookup"><span data-stu-id="150e9-107">The reorder point expresses the anticipated demand during the lead time of the item.</span></span> <span data-ttu-id="150e9-108">When the reorder point is passed, it is time to order more.</span><span class="sxs-lookup"><span data-stu-id="150e9-108">When the reorder point is passed, it is time to order more.</span></span> <span data-ttu-id="150e9-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span><span class="sxs-lookup"><span data-stu-id="150e9-109">But the projected inventory must be large enough to cover the demand until the new order is received.</span></span> <span data-ttu-id="150e9-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span><span class="sxs-lookup"><span data-stu-id="150e9-110">Meanwhile, the safety stock should take care of fluctuations in demand up to a targeted service level.</span></span>  

 <span data-ttu-id="150e9-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span><span class="sxs-lookup"><span data-stu-id="150e9-111">Consequently, the planning system considers it an emergency if a future demand cannot be served from the projected inventory, or expressed in another way, that the projected inventory goes negative.</span></span> <span data-ttu-id="150e9-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span><span class="sxs-lookup"><span data-stu-id="150e9-112">The system deals with such an exception by suggesting a new supply order to meet the part of the demand that cannot be met by inventory or other supply.</span></span> <span data-ttu-id="150e9-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span><span class="sxs-lookup"><span data-stu-id="150e9-113">The order size of the new supply order will not take the maximum inventory or the reorder quantity into consideration, nor will it take into consideration the order modifiers Maximum Order Quantity, Minimum Order Quantity, and Order Multiple.</span></span> <span data-ttu-id="150e9-114">Instead, it will reflect the exact deficiency.</span><span class="sxs-lookup"><span data-stu-id="150e9-114">Instead, it will reflect the exact deficiency.</span></span>  

 <span data-ttu-id="150e9-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span><span class="sxs-lookup"><span data-stu-id="150e9-115">The planning line for this type of supply order will display an Emergency warning icon, and additional information will be provided upon lookup to inform the user of the situation.</span></span>  

 <span data-ttu-id="150e9-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span><span class="sxs-lookup"><span data-stu-id="150e9-116">In the following illustration, supply D represents an emergency order to adjust for negative inventory.</span></span>  

 ![](media/nav_app_supply_planning_2_negative_inventory.png "NAV_APP_supply_planning_2_negative_inventory")  

1.  <span data-ttu-id="150e9-117">Supply **A**, initial projected inventory, is below reorder point.</span><span class="sxs-lookup"><span data-stu-id="150e9-117">Supply **A**, initial projected inventory, is below reorder point.</span></span>  

2.  <span data-ttu-id="150e9-118">A new forward-scheduled supply is created (**C**).</span><span class="sxs-lookup"><span data-stu-id="150e9-118">A new forward-scheduled supply is created (**C**).</span></span>  

     <span data-ttu-id="150e9-119">(Quantity = Maximum Inventory – Projected Inventory Level)</span><span class="sxs-lookup"><span data-stu-id="150e9-119">(Quantity = Maximum Inventory – Projected Inventory Level)</span></span>  

3.  <span data-ttu-id="150e9-120">Supply **A** is closed by demand **B**, which is not fully covered.</span><span class="sxs-lookup"><span data-stu-id="150e9-120">Supply **A** is closed by demand **B**, which is not fully covered.</span></span>  

     <span data-ttu-id="150e9-121">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span><span class="sxs-lookup"><span data-stu-id="150e9-121">(Demand **B** could try to schedule Supply C in but that will not happen according to the time-bucket concept.)</span></span>  

4.  <span data-ttu-id="150e9-122">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span><span class="sxs-lookup"><span data-stu-id="150e9-122">New supply (**D**) is created to cover the remaining quantity on Demand **B**.</span></span>  

5.  <span data-ttu-id="150e9-123">Demand **B** is closed (creating a reminder to the projected inventory).</span><span class="sxs-lookup"><span data-stu-id="150e9-123">Demand **B** is closed (creating a reminder to the projected inventory).</span></span>  

6.  <span data-ttu-id="150e9-124">The new supply **D** is closed.</span><span class="sxs-lookup"><span data-stu-id="150e9-124">The new supply **D** is closed.</span></span>  

7.  <span data-ttu-id="150e9-125">Projected Inventory is checked; reorder point has not been crossed.</span><span class="sxs-lookup"><span data-stu-id="150e9-125">Projected Inventory is checked; reorder point has not been crossed.</span></span>  

8.  <span data-ttu-id="150e9-126">Supply **C** is closed (no more demand exists).</span><span class="sxs-lookup"><span data-stu-id="150e9-126">Supply **C** is closed (no more demand exists).</span></span>  

9. <span data-ttu-id="150e9-127">Final check: No outstanding inventory level reminders exist.</span><span class="sxs-lookup"><span data-stu-id="150e9-127">Final check: No outstanding inventory level reminders exist.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="150e9-128">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span><span class="sxs-lookup"><span data-stu-id="150e9-128">Step 4 reflects how the system reacts in versions earlier than Microsoft Dynamics NAV 2009 SP1.</span></span>  

 <span data-ttu-id="150e9-129">This concludes the description of central principles relating to inventory planning based on reordering policies.</span><span class="sxs-lookup"><span data-stu-id="150e9-129">This concludes the description of central principles relating to inventory planning based on reordering policies.</span></span> <span data-ttu-id="150e9-130">The following section describes the characteristics of the four supported reordering policies.</span><span class="sxs-lookup"><span data-stu-id="150e9-130">The following section describes the characteristics of the four supported reordering policies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="150e9-131">See Also</span><span class="sxs-lookup"><span data-stu-id="150e9-131">See Also</span></span>  
 <span data-ttu-id="150e9-132">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="150e9-132">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="150e9-133">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="150e9-133">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="150e9-134">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="150e9-134">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="150e9-135">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="150e9-135">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

