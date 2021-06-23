---
title: Design Details - Demand and Supply | Microsoft Docs
description: This topic introduces the concept of demand, which is the common term used for any kind of gross demand, such as a sales order and component need from a works order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 62abcd0e37a9871efd6158a898538b7c18b6b47f
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215335"
---
# <a name="design-details-demand-at-blank-location"></a><span data-ttu-id="72dc8-103">Design Details: Demand at Blank Location</span><span class="sxs-lookup"><span data-stu-id="72dc8-103">Design Details: Demand at Blank Location</span></span>
<span data-ttu-id="72dc8-104">When a user creates a demand event, such as a sales order line, the program allows the user to sometimes specify a location code and other times not, that is, use blank location.</span><span class="sxs-lookup"><span data-stu-id="72dc8-104">When a user creates a demand event, such as a sales order line, the program allows the user to sometimes specify a location code and other times not, that is, use blank location.</span></span>

<span data-ttu-id="72dc8-105">For demand with or without location codes, the planning system operates in a straight forward way when:</span><span class="sxs-lookup"><span data-stu-id="72dc8-105">For demand with or without location codes, the planning system operates in a straight forward way when:</span></span>

- <span data-ttu-id="72dc8-106">Demand lines always carry location codes and the system fully uses SKUs, including the relevant location setup.</span><span class="sxs-lookup"><span data-stu-id="72dc8-106">Demand lines always carry location codes and the system fully uses SKUs, including the relevant location setup.</span></span>
- <span data-ttu-id="72dc8-107">Demand lines never carry location codes, and the system does not use SKUs or any location setup (see the last scenario in the following section).</span><span class="sxs-lookup"><span data-stu-id="72dc8-107">Demand lines never carry location codes, and the system does not use SKUs or any location setup (see the last scenario in the following section).</span></span>

<span data-ttu-id="72dc8-108">However, if demand events sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.</span><span class="sxs-lookup"><span data-stu-id="72dc8-108">However, if demand events sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.</span></span>

## <a name="demand-at-location"></a><span data-ttu-id="72dc8-109">Demand at Location</span><span class="sxs-lookup"><span data-stu-id="72dc8-109">Demand at Location</span></span>
<span data-ttu-id="72dc8-110">When the planning system detects demand at a location, it will behave in different ways depending on three critical setup values.</span><span class="sxs-lookup"><span data-stu-id="72dc8-110">When the planning system detects demand at a location, it will behave in different ways depending on three critical setup values.</span></span> <span data-ttu-id="72dc8-111">During a planning run, the system checks for three setup values in sequence and plans accordingly.</span><span class="sxs-lookup"><span data-stu-id="72dc8-111">During a planning run, the system checks for three setup values in sequence and plans accordingly.</span></span>

1. <span data-ttu-id="72dc8-112">Is there a check mark in the **Location Mandatory** field?</span><span class="sxs-lookup"><span data-stu-id="72dc8-112">Is there a check mark in the **Location Mandatory** field?</span></span>

    <span data-ttu-id="72dc8-113">If yes, then:</span><span class="sxs-lookup"><span data-stu-id="72dc8-113">If yes, then:</span></span>

2. <span data-ttu-id="72dc8-114">Does SKU exist for the item?</span><span class="sxs-lookup"><span data-stu-id="72dc8-114">Does SKU exist for the item?</span></span>

    <span data-ttu-id="72dc8-115">If yes, then:</span><span class="sxs-lookup"><span data-stu-id="72dc8-115">If yes, then:</span></span>

    <span data-ttu-id="72dc8-116">The item is planned according to planning parameters on the SKU card.</span><span class="sxs-lookup"><span data-stu-id="72dc8-116">The item is planned according to planning parameters on the SKU card.</span></span>

    <span data-ttu-id="72dc8-117">If no, then:</span><span class="sxs-lookup"><span data-stu-id="72dc8-117">If no, then:</span></span>

3. <span data-ttu-id="72dc8-118">Does the Components at Location field contain the demanded location code?</span><span class="sxs-lookup"><span data-stu-id="72dc8-118">Does the Components at Location field contain the demanded location code?</span></span>

  <span data-ttu-id="72dc8-119">If yes, then:</span><span class="sxs-lookup"><span data-stu-id="72dc8-119">If yes, then:</span></span>

  <span data-ttu-id="72dc8-120">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="72dc8-120">The item is planned according to planning parameters on the item card.</span></span>

  <span data-ttu-id="72dc8-121">If no, then:</span><span class="sxs-lookup"><span data-stu-id="72dc8-121">If no, then:</span></span>

  <span data-ttu-id="72dc8-122">The item is planned according to: Reordering Policy = Lot-for-Lot, Include Stock = Yes, all other planning parameters = Empty, items using Reordering Policy = Order will remain using Order along with the other settings.</span><span class="sxs-lookup"><span data-stu-id="72dc8-122">The item is planned according to: Reordering Policy = Lot-for-Lot, Include Inventory = Yes, all other planning parameters = Empty, items using Reordering Policy = Order will remain using Order along with the other settings.</span></span>

> [!NOTE]
> <span data-ttu-id="72dc8-123">The exceptional planning setup that is output as the last reaction in step 3 above is referred to in the following as the “minimal alternative”.</span><span class="sxs-lookup"><span data-stu-id="72dc8-123">The exceptional planning setup that is output as the last reaction in step 3 above is referred to in the following as the “minimal alternative”.</span></span> <span data-ttu-id="72dc8-124">This planning setup only covers the exact demand, and all other planning parameters are ignored.</span><span class="sxs-lookup"><span data-stu-id="72dc8-124">This planning setup only covers the exact demand, and all other planning parameters are ignored.</span></span>

<span data-ttu-id="72dc8-125">For information about variations of this planning logic, see the Scenarios section below.</span><span class="sxs-lookup"><span data-stu-id="72dc8-125">For information about variations of this planning logic, see the Scenarios section below.</span></span>

## <a name="demand-at-blank-location"></a><span data-ttu-id="72dc8-126">Demand at Blank Location</span><span class="sxs-lookup"><span data-stu-id="72dc8-126">Demand at Blank Location</span></span>
<span data-ttu-id="72dc8-127">Even if the **Location Mandatory** field is selected, the program will allow demand lines to be created without a location code, also referred to as blank location.</span><span class="sxs-lookup"><span data-stu-id="72dc8-127">Even if the **Location Mandatory** field is selected, the program will allow demand lines to be created without a location code, also referred to as blank location.</span></span> <span data-ttu-id="72dc8-128">This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.</span><span class="sxs-lookup"><span data-stu-id="72dc8-128">This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.</span></span>

<span data-ttu-id="72dc8-129">If the **Location Mandatory** field is not selected but any of the location setup values exist, it is also considered a deviation, and the planning system will react by using the “minimal alternative”: The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-129">If the **Location Mandatory** field is not selected but any of the location setup values exist, it is also considered a deviation, and the planning system will react by using the “minimal alternative”: The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

## <a name="scenarios"></a><span data-ttu-id="72dc8-130">Scenarios</span><span class="sxs-lookup"><span data-stu-id="72dc8-130">Scenarios</span></span>
<span data-ttu-id="72dc8-131">The following scenarios describe variations of demand at blank location and how the planning system resolves to the “minimal alternative.”</span><span class="sxs-lookup"><span data-stu-id="72dc8-131">The following scenarios describe variations of demand at blank location and how the planning system resolves to the “minimal alternative.”</span></span>

### <a name="setup-1"></a><span data-ttu-id="72dc8-132">Setup 1:</span><span class="sxs-lookup"><span data-stu-id="72dc8-132">Setup 1:</span></span>
<span data-ttu-id="72dc8-133">Location Mandatory = Yes</span><span class="sxs-lookup"><span data-stu-id="72dc8-133">Location Mandatory = Yes</span></span>

<span data-ttu-id="72dc8-134">SKU is set up for RED</span><span class="sxs-lookup"><span data-stu-id="72dc8-134">SKU is set up for RED</span></span>

<span data-ttu-id="72dc8-135">Components at Location = BLUE</span><span class="sxs-lookup"><span data-stu-id="72dc8-135">Components at Location = BLUE</span></span>

#### <a name="case-11-demand-is-at-red-location"></a><span data-ttu-id="72dc8-136">Case 1.1: Demand is at RED location</span><span class="sxs-lookup"><span data-stu-id="72dc8-136">Case 1.1: Demand is at RED location</span></span>
<span data-ttu-id="72dc8-137">The item is planned according to planning parameters on the SKU card.</span><span class="sxs-lookup"><span data-stu-id="72dc8-137">The item is planned according to planning parameters on the SKU card.</span></span>

#### <a name="case-12-demand-is-at-blue-location"></a><span data-ttu-id="72dc8-138">Case 1.2: Demand is at BLUE location</span><span class="sxs-lookup"><span data-stu-id="72dc8-138">Case 1.2: Demand is at BLUE location</span></span>
<span data-ttu-id="72dc8-139">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-139">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-13-demand-is-at-green-location"></a><span data-ttu-id="72dc8-140">Case 1.3: Demand is at GREEN location</span><span class="sxs-lookup"><span data-stu-id="72dc8-140">Case 1.3: Demand is at GREEN location</span></span>
<span data-ttu-id="72dc8-141">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-141">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-14-demand-is-at-blank-location"></a><span data-ttu-id="72dc8-142">Case 1.4: Demand is at BLANK location</span><span class="sxs-lookup"><span data-stu-id="72dc8-142">Case 1.4: Demand is at BLANK location</span></span>
<span data-ttu-id="72dc8-143">The item is not planned because no location is defined on the demand line.</span><span class="sxs-lookup"><span data-stu-id="72dc8-143">The item is not planned because no location is defined on the demand line.</span></span>

### <a name="setup-2"></a><span data-ttu-id="72dc8-144">Setup 2:</span><span class="sxs-lookup"><span data-stu-id="72dc8-144">Setup 2:</span></span>
<span data-ttu-id="72dc8-145">Location Mandatory = Yes</span><span class="sxs-lookup"><span data-stu-id="72dc8-145">Location Mandatory = Yes</span></span>

<span data-ttu-id="72dc8-146">No SKU exists</span><span class="sxs-lookup"><span data-stu-id="72dc8-146">No SKU exists</span></span>

<span data-ttu-id="72dc8-147">Components at Location = BLUE</span><span class="sxs-lookup"><span data-stu-id="72dc8-147">Components at Location = BLUE</span></span>

#### <a name="case-21-demand-is-at-red-location"></a><span data-ttu-id="72dc8-148">Case 2.1: Demand is at RED location</span><span class="sxs-lookup"><span data-stu-id="72dc8-148">Case 2.1: Demand is at RED location</span></span>
<span data-ttu-id="72dc8-149">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-149">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-22-demand-is-at-blue-location"></a><span data-ttu-id="72dc8-150">Case 2.2: Demand is at BLUE location</span><span class="sxs-lookup"><span data-stu-id="72dc8-150">Case 2.2: Demand is at BLUE location</span></span>
<span data-ttu-id="72dc8-151">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="72dc8-151">The item is planned according to planning parameters on the item card.</span></span>

### <a name="setup-3"></a><span data-ttu-id="72dc8-152">Setup 3:</span><span class="sxs-lookup"><span data-stu-id="72dc8-152">Setup 3:</span></span>
<span data-ttu-id="72dc8-153">Location Mandatory = No</span><span class="sxs-lookup"><span data-stu-id="72dc8-153">Location Mandatory = No</span></span>

<span data-ttu-id="72dc8-154">No SKU exists</span><span class="sxs-lookup"><span data-stu-id="72dc8-154">No SKU exists</span></span>

<span data-ttu-id="72dc8-155">Components at Location = BLUE</span><span class="sxs-lookup"><span data-stu-id="72dc8-155">Components at Location = BLUE</span></span>

#### <a name="case-31-demand-is-at-red-location"></a><span data-ttu-id="72dc8-156">Case 3.1: Demand is at RED location</span><span class="sxs-lookup"><span data-stu-id="72dc8-156">Case 3.1: Demand is at RED location</span></span>
<span data-ttu-id="72dc8-157">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-157">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-32-demand-is-at-blue-location"></a><span data-ttu-id="72dc8-158">Case 3.2: Demand is at BLUE location</span><span class="sxs-lookup"><span data-stu-id="72dc8-158">Case 3.2: Demand is at BLUE location</span></span>
<span data-ttu-id="72dc8-159">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="72dc8-159">The item is planned according to planning parameters on the item card.</span></span>

#### <a name="case-33-demand-is-at-blank-location"></a><span data-ttu-id="72dc8-160">Case 3.3: Demand is at BLANK location</span><span class="sxs-lookup"><span data-stu-id="72dc8-160">Case 3.3: Demand is at BLANK location</span></span>
<span data-ttu-id="72dc8-161">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-161">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

### <a name="setup-4"></a><span data-ttu-id="72dc8-162">Setup 4:</span><span class="sxs-lookup"><span data-stu-id="72dc8-162">Setup 4:</span></span>
<span data-ttu-id="72dc8-163">Location Mandatory = No</span><span class="sxs-lookup"><span data-stu-id="72dc8-163">Location Mandatory = No</span></span>

<span data-ttu-id="72dc8-164">No SKU exists</span><span class="sxs-lookup"><span data-stu-id="72dc8-164">No SKU exists</span></span>

<span data-ttu-id="72dc8-165">Components at Location = BLANK</span><span class="sxs-lookup"><span data-stu-id="72dc8-165">Components at Location = BLANK</span></span>

#### <a name="case-41-demand-is-at-blue-location"></a><span data-ttu-id="72dc8-166">Case 4.1: Demand is at BLUE location</span><span class="sxs-lookup"><span data-stu-id="72dc8-166">Case 4.1: Demand is at BLUE location</span></span>
<span data-ttu-id="72dc8-167">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Stock = Yes, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="72dc8-167">The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.</span></span>

#### <a name="case-42-demand-is-at-blank-location"></a><span data-ttu-id="72dc8-168">Case 4.2: Demand is at BLANK location</span><span class="sxs-lookup"><span data-stu-id="72dc8-168">Case 4.2: Demand is at BLANK location</span></span>
<span data-ttu-id="72dc8-169">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="72dc8-169">The item is planned according to planning parameters on the item card.</span></span>

<span data-ttu-id="72dc8-170">As illustrated in the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations.</span><span class="sxs-lookup"><span data-stu-id="72dc8-170">As illustrated in the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations.</span></span> <span data-ttu-id="72dc8-171">Similarly, the only way to get stable planning results for demand at locations is to use SKUs.</span><span class="sxs-lookup"><span data-stu-id="72dc8-171">Similarly, the only way to get stable planning results for demand at locations is to use SKUs.</span></span> <span data-ttu-id="72dc8-172">Therefore, if companies often plan for demand at locations, they are strongly advised to use the Stockkeeping Units granule.</span><span class="sxs-lookup"><span data-stu-id="72dc8-172">Therefore, if companies often plan for demand at locations, they are strongly advised to use the Stockkeeping Units granule.</span></span>

## <a name="see-also"></a><span data-ttu-id="72dc8-173">See Also</span><span class="sxs-lookup"><span data-stu-id="72dc8-173">See Also</span></span>  
<span data-ttu-id="72dc8-174">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="72dc8-174">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="72dc8-175">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="72dc8-175">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="72dc8-176">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="72dc8-176">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]