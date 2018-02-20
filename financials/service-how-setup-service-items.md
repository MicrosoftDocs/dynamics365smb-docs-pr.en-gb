---
title: Overview of Setups for Service Items and Service Item Components | Microsoft Docs
description: Learn about the things you must set up before you can use service items, including default values such as response time, contract discount percent, and service price group.
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 068d141ee8490cc34e8b2092b7dcfda36139660d
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="set-up-service-items-and-service-item-components"></a><span data-ttu-id="8a61c-103">Set Up Service Items and Service Item Components</span><span class="sxs-lookup"><span data-stu-id="8a61c-103">Set Up Service Items and Service Item Components</span></span>
<span data-ttu-id="8a61c-104">To work with service items, you must set up the following</span><span class="sxs-lookup"><span data-stu-id="8a61c-104">To work with service items, you must set up the following</span></span>

* <span data-ttu-id="8a61c-105">Service item groups.</span><span class="sxs-lookup"><span data-stu-id="8a61c-105">Service item groups.</span></span> 
* <span data-ttu-id="8a61c-106">Optional</span><span class="sxs-lookup"><span data-stu-id="8a61c-106">Optional</span></span>

## <a name="to-set-up-service-item-groups"></a><span data-ttu-id="8a61c-107">To set up service item groups</span><span class="sxs-lookup"><span data-stu-id="8a61c-107">To set up service item groups</span></span>
<span data-ttu-id="8a61c-108">You can set up groups of items that are related in terms of repair and maintenance.</span><span class="sxs-lookup"><span data-stu-id="8a61c-108">You can set up groups of items that are related in terms of repair and maintenance.</span></span> <span data-ttu-id="8a61c-109">You can define default values for service items in a service item group, such as response time, contract discount percent, and service price group.</span><span class="sxs-lookup"><span data-stu-id="8a61c-109">You can define default values for service items in a service item group, such as response time, contract discount percent, and service price group.</span></span> <span data-ttu-id="8a61c-110">For items in a service item group, you can select whether you want them to be automatically registered as service items when they are sold.</span><span class="sxs-lookup"><span data-stu-id="8a61c-110">For items in a service item group, you can select whether you want them to be automatically registered as service items when they are sold.</span></span>  
  
<span data-ttu-id="8a61c-111">You assign service item groups to items on the **Item** card, and to service items on the **Service Item** card.</span><span class="sxs-lookup"><span data-stu-id="8a61c-111">You assign service item groups to items on the **Item** card, and to service items on the **Service Item** card.</span></span>  
  
1. <span data-ttu-id="8a61c-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Item Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8a61c-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8a61c-113">Create a new service item group.</span><span class="sxs-lookup"><span data-stu-id="8a61c-113">Create a new service item group.</span></span>  
3. <span data-ttu-id="8a61c-114">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="8a61c-114">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="8a61c-115">In the **Default Contract Discount %** field, enter the default contract discount percentage that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="8a61c-115">In the **Default Contract Discount %** field, enter the default contract discount percentage that you want the service items in the group to have.</span></span>  
5. <span data-ttu-id="8a61c-116">In the **Default Serv. Price Group Code** field, enter the default service price group code that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="8a61c-116">In the **Default Serv. Price Group Code** field, enter the default service price group code that you want the service items in the group to have.</span></span>  
6. <span data-ttu-id="8a61c-117">In the **Default Response Time (Hours)** field, enter the default response time in hours that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="8a61c-117">In the **Default Response Time (Hours)** field, enter the default response time in hours that you want the service items in the group to have.</span></span>  
7. <span data-ttu-id="8a61c-118">If you want to register the items in the group as service items when they are sold, select the **Create Service Item** field.</span><span class="sxs-lookup"><span data-stu-id="8a61c-118">If you want to register the items in the group as service items when they are sold, select the **Create Service Item** field.</span></span>  

## <a name="to-set-up-service-item-components"></a><span data-ttu-id="8a61c-119">To set up service item components</span><span class="sxs-lookup"><span data-stu-id="8a61c-119">To set up service item components</span></span>
<span data-ttu-id="8a61c-120">A service item can consist of several components, which can be replaced with spare parts when the item is serviced.</span><span class="sxs-lookup"><span data-stu-id="8a61c-120">A service item can consist of several components, which can be replaced with spare parts when the item is serviced.</span></span> <span data-ttu-id="8a61c-121">These components are set up on the **Service Item Component List** page.</span><span class="sxs-lookup"><span data-stu-id="8a61c-121">These components are set up on the **Service Item Component List** page.</span></span> <span data-ttu-id="8a61c-122">Additionally, if you want to set up components for service items that are BOMs, you can copy the BOM items and create them as service item components.</span><span class="sxs-lookup"><span data-stu-id="8a61c-122">Additionally, if you want to set up components for service items that are BOMs, you can copy the BOM items and create them as service item components.</span></span> 
  
1. <span data-ttu-id="8a61c-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8a61c-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items**, and then choose the related link.</span></span> 
2. <span data-ttu-id="8a61c-124">Open the service item for which you want to set up components.</span><span class="sxs-lookup"><span data-stu-id="8a61c-124">Open the service item for which you want to set up components.</span></span>  
3. <span data-ttu-id="8a61c-125">Choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="8a61c-125">Choose the **Components** action.</span></span> <span data-ttu-id="8a61c-126">The **Service Item Component List** window opens.</span><span class="sxs-lookup"><span data-stu-id="8a61c-126">The **Service Item Component List** window opens.</span></span>  
4. <span data-ttu-id="8a61c-127">Add a new component.</span><span class="sxs-lookup"><span data-stu-id="8a61c-127">Add a new component.</span></span>  
5. <span data-ttu-id="8a61c-128">In the **Type** field, choose **Service Item** if the component itself is a registered service item.</span><span class="sxs-lookup"><span data-stu-id="8a61c-128">In the **Type** field, choose **Service Item** if the component itself is a registered service item.</span></span> <span data-ttu-id="8a61c-129">Otherwise, select **Item**.</span><span class="sxs-lookup"><span data-stu-id="8a61c-129">Otherwise, select **Item**.</span></span>  
6. <span data-ttu-id="8a61c-130">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="8a61c-130">In the **No.**</span></span> <span data-ttu-id="8a61c-131">field, choose the item or service item that is a component of the service item.</span><span class="sxs-lookup"><span data-stu-id="8a61c-131">field, choose the item or service item that is a component of the service item.</span></span>  

## <a name="to-set-up-service-item-components-from-a-bom"></a><span data-ttu-id="8a61c-132">To set up service item components from a BOM</span><span class="sxs-lookup"><span data-stu-id="8a61c-132">To set up service item components from a BOM</span></span>
1.  <span data-ttu-id="8a61c-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8a61c-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8a61c-134">Open the service item for which you want to set up components from a BOM.</span><span class="sxs-lookup"><span data-stu-id="8a61c-134">Open the service item for which you want to set up components from a BOM.</span></span>  
3. <span data-ttu-id="8a61c-135">Choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="8a61c-135">Choose the **Components** action.</span></span> <span data-ttu-id="8a61c-136">The **Service Item Component List** window opens.</span><span class="sxs-lookup"><span data-stu-id="8a61c-136">The **Service Item Component List** window opens.</span></span>  
4. <span data-ttu-id="8a61c-137">Choose the **Copy from BOM** action.</span><span class="sxs-lookup"><span data-stu-id="8a61c-137">Choose the **Copy from BOM** action.</span></span>  
  
    <span data-ttu-id="8a61c-138">If the item that the service item is linked to is a BOM, the components for all the items in the BOM are created automatically.</span><span class="sxs-lookup"><span data-stu-id="8a61c-138">If the item that the service item is linked to is a BOM, the components for all the items in the BOM are created automatically.</span></span>  

## <a name="to-set-up-a-service-shelf"></a><span data-ttu-id="8a61c-139">To set up a service shelf</span><span class="sxs-lookup"><span data-stu-id="8a61c-139">To set up a service shelf</span></span>
<span data-ttu-id="8a61c-140">You can set up service shelves that identify where you store your service items.</span><span class="sxs-lookup"><span data-stu-id="8a61c-140">You can set up service shelves that identify where you store your service items.</span></span> <span data-ttu-id="8a61c-141">You assign service shelves to service items on the **Service Order** and **Service Item Worksheet** pages.</span><span class="sxs-lookup"><span data-stu-id="8a61c-141">You assign service shelves to service items on the **Service Order** and **Service Item Worksheet** pages.</span></span>  
  
1. <span data-ttu-id="8a61c-142">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Shelves**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8a61c-142">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Shelves**, and then choose the related link.</span></span>
2. <span data-ttu-id="8a61c-143">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="8a61c-143">Fill in the fields as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="8a61c-144">See Also</span><span class="sxs-lookup"><span data-stu-id="8a61c-144">See Also</span></span>
<span data-ttu-id="8a61c-145">[Set Up Codes for Standard Services](service-how-setup-service-coding.md) </span><span class="sxs-lookup"><span data-stu-id="8a61c-145">[Set Up Codes for Standard Services](service-how-setup-service-coding.md) </span></span>  
[<span data-ttu-id="8a61c-146">Set Up Troubleshooting</span><span class="sxs-lookup"><span data-stu-id="8a61c-146">Set Up Troubleshooting</span></span>](service-how-setup-troubleshooting.md)
