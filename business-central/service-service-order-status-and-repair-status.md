---
title: Service Order Status and Repair Status
description: The Status field in the Service Order page and the service item repair status, which is represented by the Repair Status Code field in the Service Order page have a certain relationship in Service Management. The service order status reflects the repair status of all the service items in the service order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/15/2020
ms.author: edupont
ms.openlocfilehash: 9bbe3a4263250a7d06bfffa2019114eba72a31ca
ms.sourcegitcommit: 2d2dfb6c3eca1322835f0167dc7dab614346972e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/19/2020
ms.locfileid: "4038625"
---
# <a name="service-order-status-and-repair-status"></a><span data-ttu-id="091a1-104">Service Order Status and Repair Status</span><span class="sxs-lookup"><span data-stu-id="091a1-104">Service Order Status and Repair Status</span></span>

<span data-ttu-id="091a1-105">The **Status** field on the **Service Order** page and the service item repair status, which is represented by the **Repair Status Code** field on the **Service Order** page have a certain relationship in Service Management.</span><span class="sxs-lookup"><span data-stu-id="091a1-105">The **Status** field on the **Service Order** page and the service item repair status, which is represented by the **Repair Status Code** field on the **Service Order** page have a certain relationship in Service Management.</span></span> <span data-ttu-id="091a1-106">The service order status reflects the repair status of all the service items in the service order.</span><span class="sxs-lookup"><span data-stu-id="091a1-106">The service order status reflects the repair status of all the service items in the service order.</span></span>  

> [!NOTE]  
> <span data-ttu-id="091a1-107">These two status field are not related to the **Release Status** field on the service order header, which determines how the warehouse handles service items.</span><span class="sxs-lookup"><span data-stu-id="091a1-107">These two status field are not related to the **Release Status** field on the service order header, which determines how the warehouse handles service items.</span></span>  

<span data-ttu-id="091a1-108">Each time the repair status of a service item is changed in a service order, the status of the order is updated.</span><span class="sxs-lookup"><span data-stu-id="091a1-108">Each time the repair status of a service item is changed in a service order, the status of the order is updated.</span></span> <span data-ttu-id="091a1-109">To display the status that reflects the overall repair status of the individual service items, you must specify the following:</span><span class="sxs-lookup"><span data-stu-id="091a1-109">To display the status that reflects the overall repair status of the individual service items, you must specify the following:</span></span>  

* <span data-ttu-id="091a1-110">The service order status that each repair status is linked to.</span><span class="sxs-lookup"><span data-stu-id="091a1-110">The service order status that each repair status is linked to.</span></span>  
* <span data-ttu-id="091a1-111">The level of priority of each service order status option.</span><span class="sxs-lookup"><span data-stu-id="091a1-111">The level of priority of each service order status option.</span></span>  

<span data-ttu-id="091a1-112">When you convert a service quote to a service order, the repair status of each service item is changed in the order to **Initial** and the service order status is changed to **Pending**.</span><span class="sxs-lookup"><span data-stu-id="091a1-112">When you convert a service quote to a service order, the repair status of each service item is changed in the order to **Initial** and the service order status is changed to **Pending**.</span></span>  

> [!NOTE]
> <span data-ttu-id="091a1-113">Before you can create service orders, you must set up repair statuses and service status priorities.</span><span class="sxs-lookup"><span data-stu-id="091a1-113">Before you can create service orders, you must set up repair statuses and service status priorities.</span></span> <span data-ttu-id="091a1-114">For more information, see [Set Up Statuses for Service Orders and Repairs](service-order-repair-status.md).</span><span class="sxs-lookup"><span data-stu-id="091a1-114">For more information, see [Set Up Statuses for Service Orders and Repairs](service-order-repair-status.md).</span></span>

## <a name="specifying-service-order-status-for-repair-status"></a><span data-ttu-id="091a1-115">Specifying Service Order Status for Repair Status</span><span class="sxs-lookup"><span data-stu-id="091a1-115">Specifying Service Order Status for Repair Status</span></span>

<span data-ttu-id="091a1-116">Each repair status is linked to a particular service order status.</span><span class="sxs-lookup"><span data-stu-id="091a1-116">Each repair status is linked to a particular service order status.</span></span> <span data-ttu-id="091a1-117">The options for the service order status are as follows:</span><span class="sxs-lookup"><span data-stu-id="091a1-117">The options for the service order status are as follows:</span></span>

* <span data-ttu-id="091a1-118">**Pending**</span><span class="sxs-lookup"><span data-stu-id="091a1-118">**Pending**</span></span>
* <span data-ttu-id="091a1-119">**In Process**</span><span class="sxs-lookup"><span data-stu-id="091a1-119">**In Process**</span></span>
* <span data-ttu-id="091a1-120">**On Hold**</span><span class="sxs-lookup"><span data-stu-id="091a1-120">**On Hold**</span></span>
* <span data-ttu-id="091a1-121">**Finished**</span><span class="sxs-lookup"><span data-stu-id="091a1-121">**Finished**</span></span>

<span data-ttu-id="091a1-122">The repair status options are as follows:</span><span class="sxs-lookup"><span data-stu-id="091a1-122">The repair status options are as follows:</span></span>

* <span data-ttu-id="091a1-123">**Initial**</span><span class="sxs-lookup"><span data-stu-id="091a1-123">**Initial**</span></span>
* <span data-ttu-id="091a1-124">**In Process**</span><span class="sxs-lookup"><span data-stu-id="091a1-124">**In Process**</span></span>
* <span data-ttu-id="091a1-125">**Referred**</span><span class="sxs-lookup"><span data-stu-id="091a1-125">**Referred**</span></span>
* <span data-ttu-id="091a1-126">**Partly Serviced**</span><span class="sxs-lookup"><span data-stu-id="091a1-126">**Partly Serviced**</span></span>
* <span data-ttu-id="091a1-127">**Quote Finished**</span><span class="sxs-lookup"><span data-stu-id="091a1-127">**Quote Finished**</span></span>
* <span data-ttu-id="091a1-128">**Waiting for Customer**</span><span class="sxs-lookup"><span data-stu-id="091a1-128">**Waiting for Customer**</span></span>
* <span data-ttu-id="091a1-129">**Spare Part Ordered**</span><span class="sxs-lookup"><span data-stu-id="091a1-129">**Spare Part Ordered**</span></span>
* <span data-ttu-id="091a1-130">**Spare Part Received**</span><span class="sxs-lookup"><span data-stu-id="091a1-130">**Spare Part Received**</span></span>
* <span data-ttu-id="091a1-131">**Finished**</span><span class="sxs-lookup"><span data-stu-id="091a1-131">**Finished**</span></span>  

### <a name="pending"></a><span data-ttu-id="091a1-132">Pending</span><span class="sxs-lookup"><span data-stu-id="091a1-132">Pending</span></span>

<span data-ttu-id="091a1-133">The service order status **Pending** indicates that the service can start or continue at any time.</span><span class="sxs-lookup"><span data-stu-id="091a1-133">The service order status **Pending** indicates that the service can start or continue at any time.</span></span> <span data-ttu-id="091a1-134">Therefore, the repair status options of **Initial**, **Referred**, **Partly Serviced**, and **Spare Part Received** can be linked to this service order status.</span><span class="sxs-lookup"><span data-stu-id="091a1-134">Therefore, the repair status options of **Initial**, **Referred**, **Partly Serviced**, and **Spare Part Received** can be linked to this service order status.</span></span>  

### <a name="in-process"></a><span data-ttu-id="091a1-135">In Process</span><span class="sxs-lookup"><span data-stu-id="091a1-135">In Process</span></span>

<span data-ttu-id="091a1-136">The service order status **In Process** indicates that the service is in process.</span><span class="sxs-lookup"><span data-stu-id="091a1-136">The service order status **In Process** indicates that the service is in process.</span></span> <span data-ttu-id="091a1-137">Therefore, the repair status options **In Process** and **Spare Part Ordered** can both be linked to this service order status.</span><span class="sxs-lookup"><span data-stu-id="091a1-137">Therefore, the repair status options **In Process** and **Spare Part Ordered** can both be linked to this service order status.</span></span> <span data-ttu-id="091a1-138">If you link the **Spare Part Ordered** status to an **In Process** service order status, you must also link the **Spare Part Received** status to this service order status.</span><span class="sxs-lookup"><span data-stu-id="091a1-138">If you link the **Spare Part Ordered** status to an **In Process** service order status, you must also link the **Spare Part Received** status to this service order status.</span></span>  

### <a name="on-hold"></a><span data-ttu-id="091a1-139">On Hold</span><span class="sxs-lookup"><span data-stu-id="091a1-139">On Hold</span></span>

<span data-ttu-id="091a1-140">The service order status **On Hold** indicates that the service is temporarily on hold because you are waiting for a customer response or spare parts before the service can start.</span><span class="sxs-lookup"><span data-stu-id="091a1-140">The service order status **On Hold** indicates that the service is temporarily on hold because you are waiting for a customer response or spare parts before the service can start.</span></span> <span data-ttu-id="091a1-141">Therefore, the repair status options of **Quote Finished**, **Spare Part Ordered**, and **Waiting for Customer** can be linked to this service order status.</span><span class="sxs-lookup"><span data-stu-id="091a1-141">Therefore, the repair status options of **Quote Finished**, **Spare Part Ordered**, and **Waiting for Customer** can be linked to this service order status.</span></span>  

### <a name="finished"></a><span data-ttu-id="091a1-142">Finished</span><span class="sxs-lookup"><span data-stu-id="091a1-142">Finished</span></span>

<span data-ttu-id="091a1-143">The service order status **Finished** indicates that the service has been completed.</span><span class="sxs-lookup"><span data-stu-id="091a1-143">The service order status **Finished** indicates that the service has been completed.</span></span> <span data-ttu-id="091a1-144">Therefore, the **Finished** repair status is linked to this status.</span><span class="sxs-lookup"><span data-stu-id="091a1-144">Therefore, the **Finished** repair status is linked to this status.</span></span>  

## <a name="assigning-priority-to-service-order-status"></a><span data-ttu-id="091a1-145">Assigning Priority to Service Order Status</span><span class="sxs-lookup"><span data-stu-id="091a1-145">Assigning Priority to Service Order Status</span></span>

<span data-ttu-id="091a1-146">When a repair status of a service item is changed, the service order status options linked to the different repair status options of all the service items in the order are identified.</span><span class="sxs-lookup"><span data-stu-id="091a1-146">When a repair status of a service item is changed, the service order status options linked to the different repair status options of all the service items in the order are identified.</span></span> <span data-ttu-id="091a1-147">If the service items are linked to two or more service order status options, the service order status option with the highest priority is selected.</span><span class="sxs-lookup"><span data-stu-id="091a1-147">If the service items are linked to two or more service order status options, the service order status option with the highest priority is selected.</span></span>  

<span data-ttu-id="091a1-148">You must decide which service order status contains the most important information about the status of the service order and assign that status the highest priority, and so on.</span><span class="sxs-lookup"><span data-stu-id="091a1-148">You must decide which service order status contains the most important information about the status of the service order and assign that status the highest priority, and so on.</span></span>  

<span data-ttu-id="091a1-149">Then, when you create a new service order and you add service items to it, the **Priority** field on the service order header is updated based on the priorities on the service items.</span><span class="sxs-lookup"><span data-stu-id="091a1-149">Then, when you create a new service order and you add service items to it, the **Priority** field on the service order header is updated based on the priorities on the service items.</span></span>  

### <a name="example"></a><span data-ttu-id="091a1-150">Example</span><span class="sxs-lookup"><span data-stu-id="091a1-150">Example</span></span>

<span data-ttu-id="091a1-151">A typical priority level assignment could be as follows:</span><span class="sxs-lookup"><span data-stu-id="091a1-151">A typical priority level assignment could be as follows:</span></span>  

* <span data-ttu-id="091a1-152">In Process - High</span><span class="sxs-lookup"><span data-stu-id="091a1-152">In Process - High</span></span>  
* <span data-ttu-id="091a1-153">Pending - Medium high</span><span class="sxs-lookup"><span data-stu-id="091a1-153">Pending - Medium high</span></span>  
* <span data-ttu-id="091a1-154">On Hold - Medium low</span><span class="sxs-lookup"><span data-stu-id="091a1-154">On Hold - Medium low</span></span>  
* <span data-ttu-id="091a1-155">Finished - Low</span><span class="sxs-lookup"><span data-stu-id="091a1-155">Finished - Low</span></span>  

<span data-ttu-id="091a1-156">For example, if one service item has the repair status **Initial**, linked to the service order status **Pending**, another has the repair status **In Process**, linked to the service order status **In Process**, and a third has the repair status **Spare Part Ordered**, linked to the service order status **On Hold**, the resulting service order status will be **In Process** because this has the highest priority.</span><span class="sxs-lookup"><span data-stu-id="091a1-156">For example, if one service item has the repair status **Initial**, linked to the service order status **Pending**, another has the repair status **In Process**, linked to the service order status **In Process**, and a third has the repair status **Spare Part Ordered**, linked to the service order status **On Hold**, the resulting service order status will be **In Process** because this has the highest priority.</span></span>  

## <a name="see-also"></a><span data-ttu-id="091a1-157">See Also</span><span class="sxs-lookup"><span data-stu-id="091a1-157">See Also</span></span>

[<span data-ttu-id="091a1-158">Set Up Statuses for Service Orders and Repairs</span><span class="sxs-lookup"><span data-stu-id="091a1-158">Set Up Statuses for Service Orders and Repairs</span></span>](service-order-repair-status.md)  
[<span data-ttu-id="091a1-159">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="091a1-159">Setting Up Service Management</span></span>](service-setup-service.md)  
