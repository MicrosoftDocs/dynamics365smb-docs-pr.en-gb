---
title: Design Details - Planning Assignment Table | Microsoft Docs
description: This topic provides insight into what happens when you change how you plan for an item.
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
ms.openlocfilehash: e7591196c3335f7640d37151054b22dd687b36e8
ms.contentlocale: en-gb
ms.lasthandoff: 12/14/2017

---
# <a name="design-details-planning-assignment-table"></a><span data-ttu-id="5ab86-103">Design Details: Planning Assignment Table</span><span class="sxs-lookup"><span data-stu-id="5ab86-103">Design Details: Planning Assignment Table</span></span>
<span data-ttu-id="5ab86-104">All items should be planned for, however, there is no reason to calculate a plan for an item unless there has been a change in the demand or supply pattern since the last time a plan was calculated.</span><span class="sxs-lookup"><span data-stu-id="5ab86-104">All items should be planned for, however, there is no reason to calculate a plan for an item unless there has been a change in the demand or supply pattern since the last time a plan was calculated.</span></span>  
  
<span data-ttu-id="5ab86-105">If the user has entered a new sales order or changed an existing one, there is reason to recalculate the plan.</span><span class="sxs-lookup"><span data-stu-id="5ab86-105">If the user has entered a new sales order or changed an existing one, there is reason to recalculate the plan.</span></span> <span data-ttu-id="5ab86-106">Other reasons include a change in forecast or the desired safety stock quantity.</span><span class="sxs-lookup"><span data-stu-id="5ab86-106">Other reasons include a change in forecast or the desired safety stock quantity.</span></span> <span data-ttu-id="5ab86-107">Changing a bill of material by adding or removing a component would most likely indicate a change, but for the component item only.</span><span class="sxs-lookup"><span data-stu-id="5ab86-107">Changing a bill of material by adding or removing a component would most likely indicate a change, but for the component item only.</span></span>  
  
<span data-ttu-id="5ab86-108">For multiple locations, the assignment takes place at the level of item per location combination.</span><span class="sxs-lookup"><span data-stu-id="5ab86-108">For multiple locations, the assignment takes place at the level of item per location combination.</span></span> <span data-ttu-id="5ab86-109">If, for example, a sales order has been created at only one location, the program will assign the item at that specific location for planning.</span><span class="sxs-lookup"><span data-stu-id="5ab86-109">If, for example, a sales order has been created at only one location, the program will assign the item at that specific location for planning.</span></span>  
  
<span data-ttu-id="5ab86-110">The reason for selecting items for planning is a matter of system performance.</span><span class="sxs-lookup"><span data-stu-id="5ab86-110">The reason for selecting items for planning is a matter of system performance.</span></span> <span data-ttu-id="5ab86-111">If no change in an item’s demand-supply pattern has occurred, the planning system will not suggest any actions to be taken.</span><span class="sxs-lookup"><span data-stu-id="5ab86-111">If no change in an item’s demand-supply pattern has occurred, the planning system will not suggest any actions to be taken.</span></span> <span data-ttu-id="5ab86-112">Without the planning assignment, the system would have to perform the calculations for all items in order to find out what to plan for, and that would drain system resources.</span><span class="sxs-lookup"><span data-stu-id="5ab86-112">Without the planning assignment, the system would have to perform the calculations for all items in order to find out what to plan for, and that would drain system resources.</span></span>  
  
<span data-ttu-id="5ab86-113">The **Planning Assignment** table monitors demand and supply events and assigns the appropriate items for planning.</span><span class="sxs-lookup"><span data-stu-id="5ab86-113">The **Planning Assignment** table monitors demand and supply events and assigns the appropriate items for planning.</span></span> <span data-ttu-id="5ab86-114">The following events are monitored:</span><span class="sxs-lookup"><span data-stu-id="5ab86-114">The following events are monitored:</span></span>  
  
* <span data-ttu-id="5ab86-115">A new sales order, forecast, component, purchase order, production order, assembly order, or transfer order.</span><span class="sxs-lookup"><span data-stu-id="5ab86-115">A new sales order, forecast, component, purchase order, production order, assembly order, or transfer order.</span></span>  
* <span data-ttu-id="5ab86-116">Change of item, quantity, location, variant, or date on a sales order, forecast, component, purchase order, production order, assembly order, or transfer order.</span><span class="sxs-lookup"><span data-stu-id="5ab86-116">Change of item, quantity, location, variant, or date on a sales order, forecast, component, purchase order, production order, assembly order, or transfer order.</span></span>  
* <span data-ttu-id="5ab86-117">Cancellation of a sales order, forecast, component, purchase order, production order, assembly order, or transfer order.</span><span class="sxs-lookup"><span data-stu-id="5ab86-117">Cancellation of a sales order, forecast, component, purchase order, production order, assembly order, or transfer order.</span></span>  
* <span data-ttu-id="5ab86-118">Consumption of items other than planned.</span><span class="sxs-lookup"><span data-stu-id="5ab86-118">Consumption of items other than planned.</span></span>  
* <span data-ttu-id="5ab86-119">Output of items other than planned.</span><span class="sxs-lookup"><span data-stu-id="5ab86-119">Output of items other than planned.</span></span>  
* <span data-ttu-id="5ab86-120">Unplanned changes in inventory.</span><span class="sxs-lookup"><span data-stu-id="5ab86-120">Unplanned changes in inventory.</span></span>  
  
<span data-ttu-id="5ab86-121">For these direct supply-demand displacements, the order tracking and action messaging system maintains the Planning Assignment table and states a planning reason as an action message.</span><span class="sxs-lookup"><span data-stu-id="5ab86-121">For these direct supply-demand displacements, the order tracking and action messaging system maintains the Planning Assignment table and states a planning reason as an action message.</span></span>  
  
<span data-ttu-id="5ab86-122">The following changes in master data can also cause a planning imbalance:</span><span class="sxs-lookup"><span data-stu-id="5ab86-122">The following changes in master data can also cause a planning imbalance:</span></span>  
  
* <span data-ttu-id="5ab86-123">Change of status to Certified in the production BOM header (for all items using that header).</span><span class="sxs-lookup"><span data-stu-id="5ab86-123">Change of status to Certified in the production BOM header (for all items using that header).</span></span>  
* <span data-ttu-id="5ab86-124">Deleted line (child item).</span><span class="sxs-lookup"><span data-stu-id="5ab86-124">Deleted line (child item).</span></span>  
* <span data-ttu-id="5ab86-125">Change of status to Certified in the routing header (for all items using that routing).</span><span class="sxs-lookup"><span data-stu-id="5ab86-125">Change of status to Certified in the routing header (for all items using that routing).</span></span>  
* <span data-ttu-id="5ab86-126">Changes in the following item card fields.</span><span class="sxs-lookup"><span data-stu-id="5ab86-126">Changes in the following item card fields.</span></span>  
* <span data-ttu-id="5ab86-127">Safety Stock Quantity or Safety Lead Time.</span><span class="sxs-lookup"><span data-stu-id="5ab86-127">Safety Stock Quantity or Safety Lead Time.</span></span>  
* <span data-ttu-id="5ab86-128">Lead Time Calculation.</span><span class="sxs-lookup"><span data-stu-id="5ab86-128">Lead Time Calculation.</span></span>  
* <span data-ttu-id="5ab86-129">Reorder Point.</span><span class="sxs-lookup"><span data-stu-id="5ab86-129">Reorder Point.</span></span>  
* <span data-ttu-id="5ab86-130">Production BOM No. (and all children of old BOM reference).</span><span class="sxs-lookup"><span data-stu-id="5ab86-130">Production BOM No. (and all children of old BOM reference).</span></span>  
* <span data-ttu-id="5ab86-131">Routing No.</span><span class="sxs-lookup"><span data-stu-id="5ab86-131">Routing No.</span></span>  
* <span data-ttu-id="5ab86-132">Reordering Policy.</span><span class="sxs-lookup"><span data-stu-id="5ab86-132">Reordering Policy.</span></span>  
  
<span data-ttu-id="5ab86-133">In these cases, a new function, Planning Assignment Management, maintains the table and states the planning reason as Net Change.</span><span class="sxs-lookup"><span data-stu-id="5ab86-133">In these cases, a new function, Planning Assignment Management, maintains the table and states the planning reason as Net Change.</span></span>  
  
<span data-ttu-id="5ab86-134">The following changes do not cause a planning assignment:</span><span class="sxs-lookup"><span data-stu-id="5ab86-134">The following changes do not cause a planning assignment:</span></span>  
  
* <span data-ttu-id="5ab86-135">Calendars</span><span class="sxs-lookup"><span data-stu-id="5ab86-135">Calendars</span></span>  
* <span data-ttu-id="5ab86-136">Other planning parameters on the item card</span><span class="sxs-lookup"><span data-stu-id="5ab86-136">Other planning parameters on the item card</span></span>  
  
<span data-ttu-id="5ab86-137">When calculating an MPS or an MRP, the following restrictions apply:</span><span class="sxs-lookup"><span data-stu-id="5ab86-137">When calculating an MPS or an MRP, the following restrictions apply:</span></span>  
  
* <span data-ttu-id="5ab86-138">MPS: The planning system checks that the item carries a production forecast or a sales order.</span><span class="sxs-lookup"><span data-stu-id="5ab86-138">MPS: The planning system checks that the item carries a production forecast or a sales order.</span></span> <span data-ttu-id="5ab86-139">If not, the item is not included in the plan.</span><span class="sxs-lookup"><span data-stu-id="5ab86-139">If not, the item is not included in the plan.</span></span>  
* <span data-ttu-id="5ab86-140">MRP: If the planning system detects that the item is being replenished by an MPS planning line or MPS supply order, the item will be left out of the planning.</span><span class="sxs-lookup"><span data-stu-id="5ab86-140">MRP: If the planning system detects that the item is being replenished by an MPS planning line or MPS supply order, the item will be left out of the planning.</span></span> <span data-ttu-id="5ab86-141">However, any demand from relevant components is included.</span><span class="sxs-lookup"><span data-stu-id="5ab86-141">However, any demand from relevant components is included.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="5ab86-142">See Also</span><span class="sxs-lookup"><span data-stu-id="5ab86-142">See Also</span></span>  
<span data-ttu-id="5ab86-143">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="5ab86-143">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="5ab86-144">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="5ab86-144">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
<span data-ttu-id="5ab86-145">[Design Details: Transfers in Planning](design-details-transfers-in-planning.md) </span><span class="sxs-lookup"><span data-stu-id="5ab86-145">[Design Details: Transfers in Planning](design-details-transfers-in-planning.md) </span></span>  
[<span data-ttu-id="5ab86-146">Design Details: Planning Parameters</span><span class="sxs-lookup"><span data-stu-id="5ab86-146">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)  

