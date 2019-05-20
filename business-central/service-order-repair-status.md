---
title: Set Up Statuses for Service Orders and Repairs | Microsoft Docs
description: You must set up nine repair status options that identify the progress of repair and maintenance of service items in service orders.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 64afbccba0573445902efdaf3c3919dacdb40e8c
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1250579"
---
# <a name="set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="86e82-103">Set Up Statuses for Service Orders and Repairs</span><span class="sxs-lookup"><span data-stu-id="86e82-103">Set Up Statuses for Service Orders and Repairs</span></span>
<span data-ttu-id="86e82-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span><span class="sxs-lookup"><span data-stu-id="86e82-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="86e82-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span><span class="sxs-lookup"><span data-stu-id="86e82-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="86e82-106">You can set the priority level for service order status options.</span><span class="sxs-lookup"><span data-stu-id="86e82-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="86e82-107">There four priorities are High, Medium High, Medium Low, and Low.</span><span class="sxs-lookup"><span data-stu-id="86e82-107">There four priorities are High, Medium High, Medium Low, and Low.</span></span>  

<span data-ttu-id="86e82-108">When you change the repair status of a service item in a service order, the service order status is updated.</span><span class="sxs-lookup"><span data-stu-id="86e82-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="86e82-109">The repair status of each service item is linked to the service order status.</span><span class="sxs-lookup"><span data-stu-id="86e82-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="86e82-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span><span class="sxs-lookup"><span data-stu-id="86e82-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="86e82-111">To set up a repair status</span><span class="sxs-lookup"><span data-stu-id="86e82-111">To set up a repair status</span></span>  
1. <span data-ttu-id="86e82-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="86e82-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Repair Status**, and then choose the related link.</span></span>
2. <span data-ttu-id="86e82-113">Create a new repair status.</span><span class="sxs-lookup"><span data-stu-id="86e82-113">Create a new repair status.</span></span>  
3. <span data-ttu-id="86e82-114">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="86e82-114">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="86e82-115">In the **Service Order Status** field, choose the order status to link the repair status to.</span><span class="sxs-lookup"><span data-stu-id="86e82-115">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="86e82-116">The **Priority** field displays the priority of the service order status you have chosen.</span><span class="sxs-lookup"><span data-stu-id="86e82-116">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="86e82-117">Choose a repair status.</span><span class="sxs-lookup"><span data-stu-id="86e82-117">Choose a repair status.</span></span> <span data-ttu-id="86e82-118">You can choose only one.</span><span class="sxs-lookup"><span data-stu-id="86e82-118">You can choose only one.</span></span>  
6. <span data-ttu-id="86e82-119">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span><span class="sxs-lookup"><span data-stu-id="86e82-119">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="86e82-120">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span><span class="sxs-lookup"><span data-stu-id="86e82-120">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="86e82-121">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span><span class="sxs-lookup"><span data-stu-id="86e82-121">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>
  
## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="86e82-122">To set up service status priorities</span><span class="sxs-lookup"><span data-stu-id="86e82-122">To set up service status priorities</span></span>  
1. <span data-ttu-id="86e82-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="86e82-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="86e82-124">Select the service order status you want to set a priority for.</span><span class="sxs-lookup"><span data-stu-id="86e82-124">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="86e82-125">In the **Priority** field, choose the priority you want for this service order status.</span><span class="sxs-lookup"><span data-stu-id="86e82-125">In the **Priority** field, choose the priority you want for this service order status.</span></span> <span data-ttu-id="86e82-126">Repeat this step for each status.</span><span class="sxs-lookup"><span data-stu-id="86e82-126">Repeat this step for each status.</span></span>  

## <a name="see-also"></a><span data-ttu-id="86e82-127">See Also</span><span class="sxs-lookup"><span data-stu-id="86e82-127">See Also</span></span>  
[<span data-ttu-id="86e82-128">Service Order Status and Repair Status</span><span class="sxs-lookup"><span data-stu-id="86e82-128">Service Order Status and Repair Status</span></span>](service-service-order-status-and-repair-status.md)  
[<span data-ttu-id="86e82-129">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="86e82-129">Setting Up Service Management</span></span>](service-setup-service.md)  
