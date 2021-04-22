---
title: Planning With or Without Locations | Microsoft Docs
description: Planning with or without location codes on demand lines is important to understand.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b182a66984ea0345e7f33e1292839d1ecfad4bfd
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787559"
---
# <a name="planning-with-or-without-locations"></a><span data-ttu-id="76f8e-103">Planning With or Without Locations</span><span class="sxs-lookup"><span data-stu-id="76f8e-103">Planning With or Without Locations</span></span>
<span data-ttu-id="76f8e-104">Concerning planning with or without location codes on demand lines, the planning system operates in a straight forward way when:</span><span class="sxs-lookup"><span data-stu-id="76f8e-104">Concerning planning with or without location codes on demand lines, the planning system operates in a straight forward way when:</span></span>  

-   <span data-ttu-id="76f8e-105">demand lines always carry location codes and the system fully uses stockkeeping units, including the relevant location setup.</span><span class="sxs-lookup"><span data-stu-id="76f8e-105">demand lines always carry location codes and the system fully uses stockkeeping units, including the relevant location setup.</span></span>  
-   <span data-ttu-id="76f8e-106">demand lines never carry location codes and the system does not use SKUs or any location setup (see last scenario below).</span><span class="sxs-lookup"><span data-stu-id="76f8e-106">demand lines never carry location codes and the system does not use SKUs or any location setup (see last scenario below).</span></span>  

<span data-ttu-id="76f8e-107">However, if demand lines sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.</span><span class="sxs-lookup"><span data-stu-id="76f8e-107">However, if demand lines sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.</span></span>  

## <a name="demand-at-location"></a><span data-ttu-id="76f8e-108">Demand at Location</span><span class="sxs-lookup"><span data-stu-id="76f8e-108">Demand at Location</span></span>  
<span data-ttu-id="76f8e-109">When the planning system detects demand at a location (a line with a location code), it will behave in different ways depending on 3 critical setup values.</span><span class="sxs-lookup"><span data-stu-id="76f8e-109">When the planning system detects demand at a location (a line with a location code), it will behave in different ways depending on 3 critical setup values.</span></span>  

<span data-ttu-id="76f8e-110">During a planning run, the system checks for the 3 setup values in sequence and plans accordingly:</span><span class="sxs-lookup"><span data-stu-id="76f8e-110">During a planning run, the system checks for the 3 setup values in sequence and plans accordingly:</span></span>  

1.  <span data-ttu-id="76f8e-111">Is there a check mark in the **Location Mandatory** field?</span><span class="sxs-lookup"><span data-stu-id="76f8e-111">Is there a check mark in the **Location Mandatory** field?</span></span>  

    <span data-ttu-id="76f8e-112">If yes, then:</span><span class="sxs-lookup"><span data-stu-id="76f8e-112">If yes, then:</span></span>  

2.  <span data-ttu-id="76f8e-113">Does SKU exist for the item?</span><span class="sxs-lookup"><span data-stu-id="76f8e-113">Does SKU exist for the item?</span></span>  

    <span data-ttu-id="76f8e-114">If yes, then:</span><span class="sxs-lookup"><span data-stu-id="76f8e-114">If yes, then:</span></span>  

    <span data-ttu-id="76f8e-115">The item is planned according to planning parameters on the SKU card.</span><span class="sxs-lookup"><span data-stu-id="76f8e-115">The item is planned according to planning parameters on the SKU card.</span></span>  

    <span data-ttu-id="76f8e-116">If no, then:</span><span class="sxs-lookup"><span data-stu-id="76f8e-116">If no, then:</span></span>  

3.  <span data-ttu-id="76f8e-117">Does the **Components at Location** field contain the demanded location code?</span><span class="sxs-lookup"><span data-stu-id="76f8e-117">Does the **Components at Location** field contain the demanded location code?</span></span>  

    <span data-ttu-id="76f8e-118">If yes, then:</span><span class="sxs-lookup"><span data-stu-id="76f8e-118">If yes, then:</span></span>  

    <span data-ttu-id="76f8e-119">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="76f8e-119">The item is planned according to planning parameters on the item card.</span></span>  

    <span data-ttu-id="76f8e-120">If no, then:</span><span class="sxs-lookup"><span data-stu-id="76f8e-120">If no, then:</span></span>  

    <span data-ttu-id="76f8e-121">The item is planned according to: Reordering Policy =  *Lot-for-Lot*, Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-121">The item is planned according to: Reordering Policy =  *Lot-for-Lot*, Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span> <span data-ttu-id="76f8e-122">(Items using reordering policy  *Order* remain using  *Order* as well as the other settings.)</span><span class="sxs-lookup"><span data-stu-id="76f8e-122">(Items using reordering policy  *Order* remain using  *Order* as well as the other settings.)</span></span>  

> [!NOTE]  
>  <span data-ttu-id="76f8e-123">This minimal alternative only covers the exact demand.</span><span class="sxs-lookup"><span data-stu-id="76f8e-123">This minimal alternative only covers the exact demand.</span></span> <span data-ttu-id="76f8e-124">Any planning parameters defined are ignored.</span><span class="sxs-lookup"><span data-stu-id="76f8e-124">Any planning parameters defined are ignored.</span></span>  

<span data-ttu-id="76f8e-125">See variations in the scenarios below.</span><span class="sxs-lookup"><span data-stu-id="76f8e-125">See variations in the scenarios below.</span></span>  

## <a name="demand-at-blank-location"></a><span data-ttu-id="76f8e-126">Demand at "Blank Location"</span><span class="sxs-lookup"><span data-stu-id="76f8e-126">Demand at "Blank Location"</span></span>  
<span data-ttu-id="76f8e-127">Even if the **Location Mandatory** check box is selected, the system will allow demand lines to be created without a location code – also referred to as *BLANK* location.</span><span class="sxs-lookup"><span data-stu-id="76f8e-127">Even if the **Location Mandatory** check box is selected, the system will allow demand lines to be created without a location code – also referred to as *BLANK* location.</span></span> <span data-ttu-id="76f8e-128">This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.</span><span class="sxs-lookup"><span data-stu-id="76f8e-128">This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.</span></span> <span data-ttu-id="76f8e-129">If the **Location Mandatory** field is not selected but any of the location setup values exist, then that is also considered a deviation and the planning system will react by outputting the "minimal alternative":</span><span class="sxs-lookup"><span data-stu-id="76f8e-129">If the **Location Mandatory** field is not selected but any of the location setup values exist, then that is also considered a deviation and the planning system will react by outputting the "minimal alternative":</span></span>   
<span data-ttu-id="76f8e-130">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains *Order)*, Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-130">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains *Order)*, Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

<span data-ttu-id="76f8e-131">See variations in the setup scenarios below.</span><span class="sxs-lookup"><span data-stu-id="76f8e-131">See variations in the setup scenarios below.</span></span>  

### <a name="setup-1"></a><span data-ttu-id="76f8e-132">Setup 1:</span><span class="sxs-lookup"><span data-stu-id="76f8e-132">Setup 1:</span></span>  

-   <span data-ttu-id="76f8e-133">Location Mandatory = *Yes*</span><span class="sxs-lookup"><span data-stu-id="76f8e-133">Location Mandatory = *Yes*</span></span>  
-   <span data-ttu-id="76f8e-134">SKU is set up for  *RED*</span><span class="sxs-lookup"><span data-stu-id="76f8e-134">SKU is set up for  *RED*</span></span>  
-   <span data-ttu-id="76f8e-135">Component at Location =  *BLUE*</span><span class="sxs-lookup"><span data-stu-id="76f8e-135">Component at Location =  *BLUE*</span></span>  

#### <a name="case-11-demand-is-at--red-location"></a><span data-ttu-id="76f8e-136">Case 1.1: Demand is at  *RED* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-136">Case 1.1: Demand is at  *RED* location</span></span>  

<span data-ttu-id="76f8e-137">The item is planned according to planning parameters on the SKU card (including possible transfer).</span><span class="sxs-lookup"><span data-stu-id="76f8e-137">The item is planned according to planning parameters on the SKU card (including possible transfer).</span></span>  

#### <a name="case-12-demand-is-at--blue-location"></a><span data-ttu-id="76f8e-138">Case 1.2: Demand is at  *BLUE* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-138">Case 1.2: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="76f8e-139">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="76f8e-139">The item is planned according to planning parameters on the item card.</span></span>  

#### <a name="case-13-demand-is-at--green-location"></a><span data-ttu-id="76f8e-140">Case 1.3: Demand is at  *GREEN* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-140">Case 1.3: Demand is at  *GREEN* location</span></span>  

<span data-ttu-id="76f8e-141">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-141">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-14-demand-is-at--blank-location"></a><span data-ttu-id="76f8e-142">Case 1.4: Demand is at  *BLANK* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-142">Case 1.4: Demand is at  *BLANK* location</span></span>  

<span data-ttu-id="76f8e-143">The item is not planned because no location is defined on the demand line.</span><span class="sxs-lookup"><span data-stu-id="76f8e-143">The item is not planned because no location is defined on the demand line.</span></span>  

### <a name="setup-2"></a><span data-ttu-id="76f8e-144">Setup 2:</span><span class="sxs-lookup"><span data-stu-id="76f8e-144">Setup 2:</span></span>  

-   <span data-ttu-id="76f8e-145">Location Mandatory = *Yes*</span><span class="sxs-lookup"><span data-stu-id="76f8e-145">Location Mandatory = *Yes*</span></span>  
-   <span data-ttu-id="76f8e-146">No SKU exists</span><span class="sxs-lookup"><span data-stu-id="76f8e-146">No SKU exists</span></span>  
-   <span data-ttu-id="76f8e-147">Component at Location =  *BLUE*</span><span class="sxs-lookup"><span data-stu-id="76f8e-147">Component at Location =  *BLUE*</span></span>  

#### <a name="case-21-demand-is-at--red-location"></a><span data-ttu-id="76f8e-148">Case 2.1: Demand is at  *RED* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-148">Case 2.1: Demand is at  *RED* location</span></span>  

<span data-ttu-id="76f8e-149">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-149">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-22-demand-is-at--blue-location"></a><span data-ttu-id="76f8e-150">Case 2.2: Demand is at  *BLUE* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-150">Case 2.2: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="76f8e-151">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="76f8e-151">The item is planned according to planning parameters on the item card.</span></span>  

### <a name="setup-3"></a><span data-ttu-id="76f8e-152">Setup 3:</span><span class="sxs-lookup"><span data-stu-id="76f8e-152">Setup 3:</span></span>  

-   <span data-ttu-id="76f8e-153">Location Mandatory = *No*</span><span class="sxs-lookup"><span data-stu-id="76f8e-153">Location Mandatory = *No*</span></span>  
-   <span data-ttu-id="76f8e-154">No SKU exists</span><span class="sxs-lookup"><span data-stu-id="76f8e-154">No SKU exists</span></span>  
-   <span data-ttu-id="76f8e-155">Component at Location =  *BLUE*</span><span class="sxs-lookup"><span data-stu-id="76f8e-155">Component at Location =  *BLUE*</span></span>  

#### <a name="case-31-demand-is-at--red-location"></a><span data-ttu-id="76f8e-156">Case 3.1: Demand is at  *RED* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-156">Case 3.1: Demand is at  *RED* location</span></span>  

<span data-ttu-id="76f8e-157">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-157">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-32-demand-is-at--blue-location"></a><span data-ttu-id="76f8e-158">Case 3.2: Demand is at  *BLUE* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-158">Case 3.2: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="76f8e-159">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="76f8e-159">The item is planned according to planning parameters on the item card.</span></span>  

#### <a name="case-33-demand-is-at--blank-location"></a><span data-ttu-id="76f8e-160">Case 3.3: Demand is at  *BLANK* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-160">Case 3.3: Demand is at  *BLANK* location</span></span>  

<span data-ttu-id="76f8e-161">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-161">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

### <a name="setup-4"></a><span data-ttu-id="76f8e-162">Setup 4:</span><span class="sxs-lookup"><span data-stu-id="76f8e-162">Setup 4:</span></span>  

-   <span data-ttu-id="76f8e-163">Location Mandatory = *No*</span><span class="sxs-lookup"><span data-stu-id="76f8e-163">Location Mandatory = *No*</span></span>  
-   <span data-ttu-id="76f8e-164">No SKU exists</span><span class="sxs-lookup"><span data-stu-id="76f8e-164">No SKU exists</span></span>  
-   <span data-ttu-id="76f8e-165">Component at Location =  *BLANK*</span><span class="sxs-lookup"><span data-stu-id="76f8e-165">Component at Location =  *BLANK*</span></span>  

#### <a name="case-41-demand-is-at--blue-location"></a><span data-ttu-id="76f8e-166">Case 4.1: Demand is at  *BLUE* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-166">Case 4.1: Demand is at  *BLUE* location</span></span>  

<span data-ttu-id="76f8e-167">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span><span class="sxs-lookup"><span data-stu-id="76f8e-167">The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.</span></span>  

#### <a name="case-42-demand-is-at--blank-location"></a><span data-ttu-id="76f8e-168">Case 4.2: Demand is at  *BLANK* location</span><span class="sxs-lookup"><span data-stu-id="76f8e-168">Case 4.2: Demand is at  *BLANK* location</span></span>  

<span data-ttu-id="76f8e-169">The item is planned according to planning parameters on the item card.</span><span class="sxs-lookup"><span data-stu-id="76f8e-169">The item is planned according to planning parameters on the item card.</span></span>  

<span data-ttu-id="76f8e-170">As you can see from the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations.</span><span class="sxs-lookup"><span data-stu-id="76f8e-170">As you can see from the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations.</span></span> <span data-ttu-id="76f8e-171">Similarly, the only way to get stable planning results for demand at locations is to use stockkeeping units.</span><span class="sxs-lookup"><span data-stu-id="76f8e-171">Similarly, the only way to get stable planning results for demand at locations is to use stockkeeping units.</span></span>  

<span data-ttu-id="76f8e-172">Therefore, if you often plan for demand at locations, it is strongly advised to use the Stockkeeping Units feature.</span><span class="sxs-lookup"><span data-stu-id="76f8e-172">Therefore, if you often plan for demand at locations, it is strongly advised to use the Stockkeeping Units feature.</span></span>  

## <a name="see-also"></a><span data-ttu-id="76f8e-173">See Also</span><span class="sxs-lookup"><span data-stu-id="76f8e-173">See Also</span></span>
<span data-ttu-id="76f8e-174">[Planning](production-planning.md)  </span><span class="sxs-lookup"><span data-stu-id="76f8e-174">[Planning](production-planning.md)  </span></span>  
[<span data-ttu-id="76f8e-175">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="76f8e-175">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="76f8e-176">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="76f8e-176">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="76f8e-177">Inventory</span><span class="sxs-lookup"><span data-stu-id="76f8e-177">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="76f8e-178">Purchasing</span><span class="sxs-lookup"><span data-stu-id="76f8e-178">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="76f8e-179">[Design Details: Supply Planning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="76f8e-179">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="76f8e-180">Setup Best Practices: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="76f8e-180">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="76f8e-181">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="76f8e-181">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]