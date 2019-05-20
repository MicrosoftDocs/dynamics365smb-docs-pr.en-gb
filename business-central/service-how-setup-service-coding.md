---
title: Set Up Codes for Standard Services | Microsoft Docs
description: Learn how to set up codes for service activities that you often perform.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, service order, repairs, maintenance
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: dace0edec8dac567a0a10642450eb15644d8fcaa
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251499"
---
# <a name="set-up-standard-service-codes"></a><span data-ttu-id="3306e-103">Set Up Standard Service Codes</span><span class="sxs-lookup"><span data-stu-id="3306e-103">Set Up Standard Service Codes</span></span>
<span data-ttu-id="3306e-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span><span class="sxs-lookup"><span data-stu-id="3306e-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span></span> <span data-ttu-id="3306e-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span><span class="sxs-lookup"><span data-stu-id="3306e-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span></span> <span data-ttu-id="3306e-106">When you choose the code on a service document, the lines are entered automatically.</span><span class="sxs-lookup"><span data-stu-id="3306e-106">When you choose the code on a service document, the lines are entered automatically.</span></span> <span data-ttu-id="3306e-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standrd text linked to it.</span><span class="sxs-lookup"><span data-stu-id="3306e-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standrd text linked to it.</span></span> <span data-ttu-id="3306e-108">You create service lines of each standard serice code on the **Standard Service Code** card.</span><span class="sxs-lookup"><span data-stu-id="3306e-108">You create service lines of each standard serice code on the **Standard Service Code** card.</span></span> <span data-ttu-id="3306e-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span><span class="sxs-lookup"><span data-stu-id="3306e-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span></span> <span data-ttu-id="3306e-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span><span class="sxs-lookup"><span data-stu-id="3306e-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span></span>  
  
> [!Tip]
>  <span data-ttu-id="3306e-111">You can use the same concept to create lines on sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="3306e-111">You can use the same concept to create lines on sales and purchase documents.</span></span> <span data-ttu-id="3306e-112">For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span><span class="sxs-lookup"><span data-stu-id="3306e-112">For more information, see [Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span></span>    
  
## <a name="to-set-up-a-standard-service-code"></a><span data-ttu-id="3306e-113">To set up a standard service code</span><span class="sxs-lookup"><span data-stu-id="3306e-113">To set up a standard service code</span></span>    
1. <span data-ttu-id="3306e-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Service Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3306e-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Service Codes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3306e-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="3306e-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="3306e-116">Fill in the service lines linked to this service code.</span><span class="sxs-lookup"><span data-stu-id="3306e-116">Fill in the service lines linked to this service code.</span></span>  

## <a name="to-assign-a-standard-service-code-to-a-service-item-group"></a><span data-ttu-id="3306e-117">To assign a standard service code to a service item group</span><span class="sxs-lookup"><span data-stu-id="3306e-117">To assign a standard service code to a service item group</span></span>
1. <span data-ttu-id="3306e-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service item Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3306e-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3306e-119">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="3306e-119">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="3306e-120">Fill in the service lines linked to this service code.</span><span class="sxs-lookup"><span data-stu-id="3306e-120">Fill in the service lines linked to this service code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3306e-121">See Also</span><span class="sxs-lookup"><span data-stu-id="3306e-121">See Also</span></span>
[<span data-ttu-id="3306e-122">Service Management</span><span class="sxs-lookup"><span data-stu-id="3306e-122">Service Management</span></span>](service-service.md)