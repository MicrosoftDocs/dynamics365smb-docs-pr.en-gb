---
title: Set Up for Service Items and Service Item Components | Microsoft Docs
description: Learn about the things you must set up before you can use service items, including default values such as response time, contract discount percent, and service price group.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 973edb068ee23cb4584aa9f1d76a85fd3cd95809
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5376719"
---
# <a name="set-up-service-items-and-service-item-components"></a><span data-ttu-id="ab693-103">Set Up Service Items and Service Item Components</span><span class="sxs-lookup"><span data-stu-id="ab693-103">Set Up Service Items and Service Item Components</span></span>
<span data-ttu-id="ab693-104">To work with service items, you must set up the following</span><span class="sxs-lookup"><span data-stu-id="ab693-104">To work with service items, you must set up the following</span></span>

* <span data-ttu-id="ab693-105">Service item groups.</span><span class="sxs-lookup"><span data-stu-id="ab693-105">Service item groups.</span></span>
* <span data-ttu-id="ab693-106">Optional</span><span class="sxs-lookup"><span data-stu-id="ab693-106">Optional</span></span>

## <a name="to-set-up-service-item-groups"></a><span data-ttu-id="ab693-107">To set up service item groups</span><span class="sxs-lookup"><span data-stu-id="ab693-107">To set up service item groups</span></span>
<span data-ttu-id="ab693-108">You can set up groups of items that are related in terms of repair and maintenance.</span><span class="sxs-lookup"><span data-stu-id="ab693-108">You can set up groups of items that are related in terms of repair and maintenance.</span></span> <span data-ttu-id="ab693-109">You can define default values for service items in a service item group, such as response time, contract discount percent, and service price group.</span><span class="sxs-lookup"><span data-stu-id="ab693-109">You can define default values for service items in a service item group, such as response time, contract discount percent, and service price group.</span></span> <span data-ttu-id="ab693-110">For items in a service item group, you can select whether you want them to be automatically registered as service items when they are sold.</span><span class="sxs-lookup"><span data-stu-id="ab693-110">For items in a service item group, you can select whether you want them to be automatically registered as service items when they are sold.</span></span>  

<span data-ttu-id="ab693-111">You assign service item groups to items on the **Item** card, and to service items on the **Service Item** card.</span><span class="sxs-lookup"><span data-stu-id="ab693-111">You assign service item groups to items on the **Item** card, and to service items on the **Service Item** card.</span></span>  

1. <span data-ttu-id="ab693-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Item Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab693-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ab693-113">Create a new service item group.</span><span class="sxs-lookup"><span data-stu-id="ab693-113">Create a new service item group.</span></span>  
3. <span data-ttu-id="ab693-114">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="ab693-114">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="ab693-115">In the **Default Contract Discount %** field, enter the default contract discount percentage that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="ab693-115">In the **Default Contract Discount %** field, enter the default contract discount percentage that you want the service items in the group to have.</span></span>  
5. <span data-ttu-id="ab693-116">In the **Default Serv. Price Group Code** field, enter the default service price group code that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="ab693-116">In the **Default Serv. Price Group Code** field, enter the default service price group code that you want the service items in the group to have.</span></span>  
6. <span data-ttu-id="ab693-117">In the **Default Response Time (Hours)** field, enter the default response time in hours that you want the service items in the group to have.</span><span class="sxs-lookup"><span data-stu-id="ab693-117">In the **Default Response Time (Hours)** field, enter the default response time in hours that you want the service items in the group to have.</span></span>  
7. <span data-ttu-id="ab693-118">If you want to register the items in the group as service items when they are sold, select the **Create Service Item** field.</span><span class="sxs-lookup"><span data-stu-id="ab693-118">If you want to register the items in the group as service items when they are sold, select the **Create Service Item** field.</span></span>  

## <a name="to-set-up-service-item-components"></a><span data-ttu-id="ab693-119">To set up service item components</span><span class="sxs-lookup"><span data-stu-id="ab693-119">To set up service item components</span></span>
<span data-ttu-id="ab693-120">A service item can consist of several components, which can be replaced with spare parts when the item is serviced.</span><span class="sxs-lookup"><span data-stu-id="ab693-120">A service item can consist of several components, which can be replaced with spare parts when the item is serviced.</span></span> <span data-ttu-id="ab693-121">These components are set up on the **Service Item Component List** page.</span><span class="sxs-lookup"><span data-stu-id="ab693-121">These components are set up on the **Service Item Component List** page.</span></span> <span data-ttu-id="ab693-122">Additionally, if you want to set up components for service items that are BOMs, you can copy the BOM items and create them as service item components.</span><span class="sxs-lookup"><span data-stu-id="ab693-122">Additionally, if you want to set up components for service items that are BOMs, you can copy the BOM items and create them as service item components.</span></span>

1. <span data-ttu-id="ab693-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab693-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="ab693-124">Open the service item for which you want to set up components.</span><span class="sxs-lookup"><span data-stu-id="ab693-124">Open the service item for which you want to set up components.</span></span>  
3. <span data-ttu-id="ab693-125">Choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="ab693-125">Choose the **Components** action.</span></span> <span data-ttu-id="ab693-126">The **Service Item Component List** page opens.</span><span class="sxs-lookup"><span data-stu-id="ab693-126">The **Service Item Component List** page opens.</span></span>  
4. <span data-ttu-id="ab693-127">Add a new component.</span><span class="sxs-lookup"><span data-stu-id="ab693-127">Add a new component.</span></span>  
5. <span data-ttu-id="ab693-128">In the **Type** field, choose **Service Item** if the component itself is a registered service item.</span><span class="sxs-lookup"><span data-stu-id="ab693-128">In the **Type** field, choose **Service Item** if the component itself is a registered service item.</span></span> <span data-ttu-id="ab693-129">Otherwise, select **Item**.</span><span class="sxs-lookup"><span data-stu-id="ab693-129">Otherwise, select **Item**.</span></span>  
6. <span data-ttu-id="ab693-130">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="ab693-130">In the **No.**</span></span> <span data-ttu-id="ab693-131">field, choose the item or service item that is a component of the service item.</span><span class="sxs-lookup"><span data-stu-id="ab693-131">field, choose the item or service item that is a component of the service item.</span></span>  

## <a name="to-set-up-service-item-components-from-a-bom"></a><span data-ttu-id="ab693-132">To set up service item components from a BOM</span><span class="sxs-lookup"><span data-stu-id="ab693-132">To set up service item components from a BOM</span></span>
1.  <span data-ttu-id="ab693-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab693-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ab693-134">Open the service item for which you want to set up components from a BOM.</span><span class="sxs-lookup"><span data-stu-id="ab693-134">Open the service item for which you want to set up components from a BOM.</span></span>  
3. <span data-ttu-id="ab693-135">Choose the **Components** action.</span><span class="sxs-lookup"><span data-stu-id="ab693-135">Choose the **Components** action.</span></span> <span data-ttu-id="ab693-136">The **Service Item Component List** page opens.</span><span class="sxs-lookup"><span data-stu-id="ab693-136">The **Service Item Component List** page opens.</span></span>  
4. <span data-ttu-id="ab693-137">Choose the **Copy from BOM** action.</span><span class="sxs-lookup"><span data-stu-id="ab693-137">Choose the **Copy from BOM** action.</span></span>  

    <span data-ttu-id="ab693-138">If the item that the service item is linked to is a BOM, the components for all the items in the BOM are created automatically.</span><span class="sxs-lookup"><span data-stu-id="ab693-138">If the item that the service item is linked to is a BOM, the components for all the items in the BOM are created automatically.</span></span>  

## <a name="to-set-up-a-service-shelf"></a><span data-ttu-id="ab693-139">To set up a service shelf</span><span class="sxs-lookup"><span data-stu-id="ab693-139">To set up a service shelf</span></span>
<span data-ttu-id="ab693-140">You can set up service shelves that identify where you store your service items.</span><span class="sxs-lookup"><span data-stu-id="ab693-140">You can set up service shelves that identify where you store your service items.</span></span> <span data-ttu-id="ab693-141">You assign service shelves to service items on the **Service Order** and **Service Item Worksheet** pages.</span><span class="sxs-lookup"><span data-stu-id="ab693-141">You assign service shelves to service items on the **Service Order** and **Service Item Worksheet** pages.</span></span>  

1. <span data-ttu-id="ab693-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Shelves**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab693-142">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Shelves**, and then choose the related link.</span></span>
2. <span data-ttu-id="ab693-143">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ab693-143">Fill in the fields as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="ab693-144">See Also</span><span class="sxs-lookup"><span data-stu-id="ab693-144">See Also</span></span>
<span data-ttu-id="ab693-145">[Set Up Codes for Standard Services](service-how-setup-service-coding.md) </span><span class="sxs-lookup"><span data-stu-id="ab693-145">[Set Up Codes for Standard Services](service-how-setup-service-coding.md) </span></span>  
[<span data-ttu-id="ab693-146">Set Up Troubleshooting</span><span class="sxs-lookup"><span data-stu-id="ab693-146">Set Up Troubleshooting</span></span>](service-how-setup-troubleshooting.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]