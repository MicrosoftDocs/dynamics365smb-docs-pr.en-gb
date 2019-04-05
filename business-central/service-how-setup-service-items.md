---
title: Set Up for Service Items and Service Item Components | Microsoft Docs
description: Learn about the things you must set up before you can use service items, including default values such as response time, contract discount percent, and service price group.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: e82aa86668da5999117eea636ee29d8fde2cc09e
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "809143"
---
# <a name="set-up-service-items-and-service-item-components"></a><span data-ttu-id="c4705-103">Set Up Service Items and Service Item Components</span><span class="sxs-lookup"><span data-stu-id="c4705-103">Set Up Service Items and Service Item Components</span></span>
<span data-ttu-id="c4705-104">To work with service items, you must set up the following</span><span class="sxs-lookup"><span data-stu-id="c4705-104">To work with service items, you must set up the following</span></span>

* <span data-ttu-id="c4705-105">Service item groups.</span><span class="sxs-lookup"><span data-stu-id="c4705-105">Service item groups.</span></span>
* <span data-ttu-id="c4705-106">Optional</span><span class="sxs-lookup"><span data-stu-id="c4705-106">Optional</span></span>

## <a name="to-set-up-service-item-groups"></a><span data-ttu-id="c4705-107">To set up service item groups</span><span class="sxs-lookup"><span data-stu-id="c4705-107">To set up service item groups</span></span>
<span data-ttu-id="c4705-108">You can set up groups of items that are related in terms of repair and maintenance.</span><span class="sxs-lookup"><span data-stu-id="c4705-108">You can set up groups of items that are related in terms of repair and maintenance.</span></span> <span data-ttu-id="c4705-109">You can define default values for service items in a service item group, such as response time, contract discount percent, and service price group.</span><span class="sxs-lookup"><span data-stu-id="c4705-109">You can define default values for service items in a service item group, such as response time, contract discount percent, and service price group.</span></span> <span data-ttu-id="c4705-110">For items in a service item group, you can select whether you want them to be automatically registered as service items when they are sold.</span><span class="sxs-lookup"><span data-stu-id="c4705-110">For items in a service item group, you can select whether you want them to be automatically registered as service items when they are sold.</span></span>  

<span data-ttu-id="c4705-111">You assign service item groups to items on the **Item** card, and to service items on the **Service Item** card.</span><span class="sxs-lookup"><span data-stu-id="c4705-111">You assign service item groups to items on the **Item** card, and to service items on the **Service Item** card.</span></span>  

1. <span data-ttu-id="c4705-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Item Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c4705-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c4705-113">Create a new service item group.</span><span class="sxs-lookup"><span data-stu-id="c4705-113">Create a new service item group.</span></span>  
3. <span data-ttu-id="c4705-114">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="c4705-114">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="c4705-115">In the **Default Contract Discount %** field, enter the default contract discount percentage that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="c4705-115">In the **Default Contract Discount %** field, enter the default contract discount percentage that you want the service items in the group to have.</span></span>  
5. <span data-ttu-id="c4705-116">In the **Default Serv. Price Group Code** field, enter the default service price group code that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="c4705-116">In the **Default Serv. Price Group Code** field, enter the default service price group code that you want the service items in the group to have.</span></span>  
6. <span data-ttu-id="c4705-117">In the **Default Response Time (Hours)** field, enter the default response time in hours that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="c4705-117">In the **Default Response Time (Hours)** field, enter the default response time in hours that you want the service items in the group to have.</span></span>  
7. <span data-ttu-id="c4705-118">If you want to register the items in the group as service items when they are sold, select the **Create Service Item** field.</span><span class="sxs-lookup"><span data-stu-id="c4705-118">If you want to register the items in the group as service items when they are sold, select the **Create Service Item** field.</span></span>  

## <a name="to-set-up-service-item-components"></a><span data-ttu-id="c4705-119">To set up service item components</span><span class="sxs-lookup"><span data-stu-id="c4705-119">To set up service item components</span></span>
<span data-ttu-id="c4705-120">A service item can consist of several components, which can be replaced with spare parts when the item is serviced.</span><span class="sxs-lookup"><span data-stu-id="c4705-120">A service item can consist of several components, which can be replaced with spare parts when the item is serviced.</span></span> <span data-ttu-id="c4705-121">These components are set up on the **Service Item Component List** page.</span><span class="sxs-lookup"><span data-stu-id="c4705-121">These components are set up on the **Service Item Component List** page.</span></span> <span data-ttu-id="c4705-122">Additionally, if you want to set up components for service items that are BOMs, you can copy the BOM items and create them as service item components.</span><span class="sxs-lookup"><span data-stu-id="c4705-122">Additionally, if you want to set up components for service items that are BOMs, you can copy the BOM items and create them as service item components.</span></span>

1. <span data-ttu-id="c4705-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c4705-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="c4705-124">Open the service item for which you want to set up components.</span><span class="sxs-lookup"><span data-stu-id="c4705-124">Open the service item for which you want to set up components.</span></span>  
3. <span data-ttu-id="c4705-125">Choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="c4705-125">Choose the **Components** action.</span></span> <span data-ttu-id="c4705-126">The **Service Item Component List** page opens.</span><span class="sxs-lookup"><span data-stu-id="c4705-126">The **Service Item Component List** page opens.</span></span>  
4. <span data-ttu-id="c4705-127">Add a new component.</span><span class="sxs-lookup"><span data-stu-id="c4705-127">Add a new component.</span></span>  
5. <span data-ttu-id="c4705-128">In the **Type** field, choose **Service Item** if the component itself is a registered service item.</span><span class="sxs-lookup"><span data-stu-id="c4705-128">In the **Type** field, choose **Service Item** if the component itself is a registered service item.</span></span> <span data-ttu-id="c4705-129">Otherwise, select **Item**.</span><span class="sxs-lookup"><span data-stu-id="c4705-129">Otherwise, select **Item**.</span></span>  
6. <span data-ttu-id="c4705-130">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="c4705-130">In the **No.**</span></span> <span data-ttu-id="c4705-131">field, choose the item or service item that is a component of the service item.</span><span class="sxs-lookup"><span data-stu-id="c4705-131">field, choose the item or service item that is a component of the service item.</span></span>  

## <a name="to-set-up-service-item-components-from-a-bom"></a><span data-ttu-id="c4705-132">To set up service item components from a BOM</span><span class="sxs-lookup"><span data-stu-id="c4705-132">To set up service item components from a BOM</span></span>
1.  <span data-ttu-id="c4705-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c4705-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c4705-134">Open the service item for which you want to set up components from a BOM.</span><span class="sxs-lookup"><span data-stu-id="c4705-134">Open the service item for which you want to set up components from a BOM.</span></span>  
3. <span data-ttu-id="c4705-135">Choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="c4705-135">Choose the **Components** action.</span></span> <span data-ttu-id="c4705-136">The **Service Item Component List** page opens.</span><span class="sxs-lookup"><span data-stu-id="c4705-136">The **Service Item Component List** page opens.</span></span>  
4. <span data-ttu-id="c4705-137">Choose the **Copy from BOM** action.</span><span class="sxs-lookup"><span data-stu-id="c4705-137">Choose the **Copy from BOM** action.</span></span>  

    <span data-ttu-id="c4705-138">If the item that the service item is linked to is a BOM, the components for all the items in the BOM are created automatically.</span><span class="sxs-lookup"><span data-stu-id="c4705-138">If the item that the service item is linked to is a BOM, the components for all the items in the BOM are created automatically.</span></span>  

## <a name="to-set-up-a-service-shelf"></a><span data-ttu-id="c4705-139">To set up a service shelf</span><span class="sxs-lookup"><span data-stu-id="c4705-139">To set up a service shelf</span></span>
<span data-ttu-id="c4705-140">You can set up service shelves that identify where you store your service items.</span><span class="sxs-lookup"><span data-stu-id="c4705-140">You can set up service shelves that identify where you store your service items.</span></span> <span data-ttu-id="c4705-141">You assign service shelves to service items on the **Service Order** and **Service Item Worksheet** pages.</span><span class="sxs-lookup"><span data-stu-id="c4705-141">You assign service shelves to service items on the **Service Order** and **Service Item Worksheet** pages.</span></span>  

1. <span data-ttu-id="c4705-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Shelves**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c4705-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Shelves**, and then choose the related link.</span></span>
2. <span data-ttu-id="c4705-143">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="c4705-143">Fill in the fields as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="c4705-144">See Also</span><span class="sxs-lookup"><span data-stu-id="c4705-144">See Also</span></span>
<span data-ttu-id="c4705-145">[Set Up Codes for Standard Services](service-how-setup-service-coding.md) </span><span class="sxs-lookup"><span data-stu-id="c4705-145">[Set Up Codes for Standard Services](service-how-setup-service-coding.md) </span></span>  
[<span data-ttu-id="c4705-146">Set Up Troubleshooting</span><span class="sxs-lookup"><span data-stu-id="c4705-146">Set Up Troubleshooting</span></span>](service-how-setup-troubleshooting.md)
