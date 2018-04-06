---
title: Set Up Pricing and Costs for Services | Microsoft Docs
description: Learn how to set up prices and additional costs for services.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, cost, service order
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 151b63b0f68a6605ae5c935f2331803277766452
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---

# <a name="set-up-pricing-and-additional-costs-for-services"></a><span data-ttu-id="e3b6c-103">Set Up Pricing and Additional Costs for Services</span><span class="sxs-lookup"><span data-stu-id="e3b6c-103">Set Up Pricing and Additional Costs for Services</span></span>
<span data-ttu-id="e3b6c-104">You can use the [!INCLUDE[d365fin](includes/d365fin_md.md)] pricing features to set up and customize your application so that you apply and adjust pricing on service items, repairs, and orders.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-104">You can use the [!INCLUDE[d365fin](includes/d365fin_md.md)] pricing features to set up and customize your application so that you apply and adjust pricing on service items, repairs, and orders.</span></span> <span data-ttu-id="e3b6c-105">These pricing decisions are then easily transmitted to the invoicing process.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-105">These pricing decisions are then easily transmitted to the invoicing process.</span></span>  
  
<span data-ttu-id="e3b6c-106">As your implementation requires, you can set up pricing groups and map them to specific time periods, customers, or currency.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-106">As your implementation requires, you can set up pricing groups and map them to specific time periods, customers, or currency.</span></span> <span data-ttu-id="e3b6c-107">You can set up fixed, minimum, or maximum pricing, depending on the service contracts that you have with customers.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-107">You can set up fixed, minimum, or maximum pricing, depending on the service contracts that you have with customers.</span></span> <span data-ttu-id="e3b6c-108">Finally, as you adjust your prices, you can view and approve the changes before committing them to the ledger.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-108">Finally, as you adjust your prices, you can view and approve the changes before committing them to the ledger.</span></span>  

## <a name="to-set-up-a-service-price-group"></a><span data-ttu-id="e3b6c-109">To set up a service price group</span><span class="sxs-lookup"><span data-stu-id="e3b6c-109">To set up a service price group</span></span>
<span data-ttu-id="e3b6c-110">You can set up groups containing service items that you want to receive the same special service pricing.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-110">You can set up groups containing service items that you want to receive the same special service pricing.</span></span> <span data-ttu-id="e3b6c-111">You assign service price groups to service items on service item lines.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-111">You assign service price groups to service items on service item lines.</span></span> <span data-ttu-id="e3b6c-112">You can also assign service price groups to service item groups.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-112">You can also assign service price groups to service item groups.</span></span>  

1. <span data-ttu-id="e3b6c-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Price Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Price Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e3b6c-114">Create a new service price group.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-114">Create a new service price group.</span></span>  
3. <span data-ttu-id="e3b6c-115">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-115">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="e3b6c-116">Choose the **Setup** action.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-116">Choose the **Setup** action.</span></span>  
2. <span data-ttu-id="e3b6c-117">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

 > [!Tip]
 > <span data-ttu-id="e3b6c-118">The **Adjustment Type** and **Amount** fields work together to specify whether an adjustment concerns a fixed amount, or applies only when the total service price exceeds or is lower than the amount in the **Amount** field.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-118">The **Adjustment Type** and **Amount** fields work together to specify whether an adjustment concerns a fixed amount, or applies only when the total service price exceeds or is lower than the amount in the **Amount** field.</span></span>  

## <a name="to-set-up-a-service-price-adjustment-group"></a><span data-ttu-id="e3b6c-119">To set up a service price adjustment group</span><span class="sxs-lookup"><span data-stu-id="e3b6c-119">To set up a service price adjustment group</span></span>  
<span data-ttu-id="e3b6c-120">You can set up price adjustment groups to adjust service pricing of service items.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-120">You can set up price adjustment groups to adjust service pricing of service items.</span></span> <span data-ttu-id="e3b6c-121">For example, you can set up price adjustment groups that adjust price of freight or spare parts.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-121">For example, you can set up price adjustment groups that adjust price of freight or spare parts.</span></span>  
  
1. <span data-ttu-id="e3b6c-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Price Adjustment Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Price Adjustment Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e3b6c-123">Create a new service price adjustment group.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-123">Create a new service price adjustment group.</span></span>  
3. <span data-ttu-id="e3b6c-124">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-124">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="e3b6c-125">In the **Type** field, enter the type of the entry that you want to adjust.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-125">In the **Type** field, enter the type of the entry that you want to adjust.</span></span>  
  
    * <span data-ttu-id="e3b6c-126">To adjust only one specific entry, enter the number of this entry in the **No.**</span><span class="sxs-lookup"><span data-stu-id="e3b6c-126">To adjust only one specific entry, enter the number of this entry in the **No.**</span></span> <span data-ttu-id="e3b6c-127">field.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-127">field.</span></span> <span data-ttu-id="e3b6c-128">When you leave this field blank, your adjustment group will adjust all entries of the type defined in the **Type** field.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-128">When you leave this field blank, your adjustment group will adjust all entries of the type defined in the **Type** field.</span></span>  
    * <span data-ttu-id="e3b6c-129">To adjust service prices related to only one specific service, fill in the **Work Type** field.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-129">To adjust service prices related to only one specific service, fill in the **Work Type** field.</span></span> <span data-ttu-id="e3b6c-130">When you leave this field blank, it will just be ignored.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-130">When you leave this field blank, it will just be ignored.</span></span>  
  
5. <span data-ttu-id="e3b6c-131">In the **Description** field, enter a short description of the service price adjustment.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-131">In the **Description** field, enter a short description of the service price adjustment.</span></span>  
6. <span data-ttu-id="e3b6c-132">To adjust service prices related to only one specific general product posting group, fill in the **Gen. Prod. Posting Group** field.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-132">To adjust service prices related to only one specific general product posting group, fill in the **Gen. Prod. Posting Group** field.</span></span>

> [!Tip]
> <span data-ttu-id="e3b6c-133">You can choose **Details** to add additional information about the adjustment group.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-133">You can choose **Details** to add additional information about the adjustment group.</span></span> <span data-ttu-id="e3b6c-134">For example, you can specify which item belongs to the service price adjustment group, and whether this is an item, a resource, a resource group, or a service charge.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-134">For example, you can specify which item belongs to the service price adjustment group, and whether this is an item, a resource, a resource group, or a service charge.</span></span>  

## <a name="to-set-up-additional-costs-for-services"></a><span data-ttu-id="e3b6c-135">To set up additional costs for services</span><span class="sxs-lookup"><span data-stu-id="e3b6c-135">To set up additional costs for services</span></span>
<span data-ttu-id="e3b6c-136">When you work with service items and service orders, you may need to register additional costs, such as travel costs to particular service zones or starting fees.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-136">When you work with service items and service orders, you may need to register additional costs, such as travel costs to particular service zones or starting fees.</span></span> <span data-ttu-id="e3b6c-137">When you create a service order, you can insert these costs and a line with the type **Cost** will be added to the order.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-137">When you create a service order, you can insert these costs and a line with the type **Cost** will be added to the order.</span></span> <span data-ttu-id="e3b6c-138">Alternatively, if you want to apply the cost to all service orders, you can set up a default cost.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-138">Alternatively, if you want to apply the cost to all service orders, you can set up a default cost.</span></span> <span data-ttu-id="e3b6c-139">For example, if you always want to apply a starting fee.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-139">For example, if you always want to apply a starting fee.</span></span>
  
### <a name="to-set-up-service-costs"></a><span data-ttu-id="e3b6c-140">To set up service costs</span><span class="sxs-lookup"><span data-stu-id="e3b6c-140">To set up service costs</span></span>
1. <span data-ttu-id="e3b6c-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Costs**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Costs**, and then choose the related link.</span></span> 
2. <span data-ttu-id="e3b6c-142">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-142">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

### <a name="to-specify-a-default-cost-for-service-orders"></a><span data-ttu-id="e3b6c-143">To specify a default cost for service orders</span><span class="sxs-lookup"><span data-stu-id="e3b6c-143">To specify a default cost for service orders</span></span>
1. <span data-ttu-id="e3b6c-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Setup**, and then choose the related link.</span></span> 
2. <span data-ttu-id="e3b6c-145">In the **Service Order Starting Fee** field, choose the appropriate service cost.</span><span class="sxs-lookup"><span data-stu-id="e3b6c-145">In the **Service Order Starting Fee** field, choose the appropriate service cost.</span></span>

## <a name="see-also"></a><span data-ttu-id="e3b6c-146">See Also</span><span class="sxs-lookup"><span data-stu-id="e3b6c-146">See Also</span></span>
[<span data-ttu-id="e3b6c-147">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="e3b6c-147">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="e3b6c-148">Service Management</span><span class="sxs-lookup"><span data-stu-id="e3b6c-148">Service Management</span></span>](service-service.md)  

