---
title: Set Up Statuses for Service Orders and Repairs | Microsoft Docs
description: You must set up nine repair status options that identify the progress of repair and maintenance of service items in service orders.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/15/2020
ms.author: edupont
ms.openlocfilehash: 4c28fcfbc2cbc7493ba183812383225754fd3dfa
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5389656"
---
# <a name="set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="d9ae6-103">Set Up Statuses for Service Orders and Repairs</span><span class="sxs-lookup"><span data-stu-id="d9ae6-103">Set Up Statuses for Service Orders and Repairs</span></span>

<span data-ttu-id="d9ae6-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="d9ae6-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="d9ae6-106">You can set the priority level for service order status options.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="d9ae6-107">The four priorities are **High**, **Medium High**, **Medium Low**, and **Low**.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-107">The four priorities are **High**, **Medium High**, **Medium Low**, and **Low**.</span></span>  

<span data-ttu-id="d9ae6-108">When you change the repair status of a service item in a service order, the service order status is updated.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="d9ae6-109">The repair status of each service item is linked to the service order status.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="d9ae6-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

<span data-ttu-id="d9ae6-111">Before you can set up a repair status, you must set up service status priorities.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-111">Before you can set up a repair status, you must set up service status priorities.</span></span>

## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="d9ae6-112">To set up service status priorities</span><span class="sxs-lookup"><span data-stu-id="d9ae6-112">To set up service status priorities</span></span>

1. <span data-ttu-id="d9ae6-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d9ae6-114">Select the service order status you want to set a priority for.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-114">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="d9ae6-115">In the **Priority** field, choose the priority you want for this service order status.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-115">In the **Priority** field, choose the priority you want for this service order status.</span></span>  

<span data-ttu-id="d9ae6-116">Repeat steps 2 and 3 until you have set the priority for each of the four status options: **Pending**, **In Process**, **Finished**, and **On Hold**.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-116">Repeat steps 2 and 3 until you have set the priority for each of the four status options: **Pending**, **In Process**, **Finished**, and **On Hold**.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="d9ae6-117">To set up a repair status</span><span class="sxs-lookup"><span data-stu-id="d9ae6-117">To set up a repair status</span></span>

1. <span data-ttu-id="d9ae6-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span></span>
2. <span data-ttu-id="d9ae6-119">Create a new repair status.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-119">Create a new repair status.</span></span>  
3. <span data-ttu-id="d9ae6-120">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-120">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="d9ae6-121">In the **Service Order Status** field, choose the order status to link the repair status to.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-121">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="d9ae6-122">The **Priority** field displays the priority of the service order status you have chosen.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-122">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="d9ae6-123">Choose a repair status.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-123">Choose a repair status.</span></span> <span data-ttu-id="d9ae6-124">You can choose only one.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-124">You can choose only one.</span></span> <span data-ttu-id="d9ae6-125">A repair status cannot be linked more than one repair status option.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-125">A repair status cannot be linked more than one repair status option.</span></span>  
6. <span data-ttu-id="d9ae6-126">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-126">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="d9ae6-127">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-127">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="d9ae6-128">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-128">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>

<span data-ttu-id="d9ae6-129">Repeat these steps for each of the repair status options you want to create.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-129">Repeat these steps for each of the repair status options you want to create.</span></span>

## <a name="see-also"></a><span data-ttu-id="d9ae6-130">See Also</span><span class="sxs-lookup"><span data-stu-id="d9ae6-130">See Also</span></span>

[<span data-ttu-id="d9ae6-131">Service Order Status and Repair Status</span><span class="sxs-lookup"><span data-stu-id="d9ae6-131">Service Order Status and Repair Status</span></span>](service-service-order-status-and-repair-status.md)  
[<span data-ttu-id="d9ae6-132">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="d9ae6-132">Setting Up Service Management</span></span>](service-setup-service.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]