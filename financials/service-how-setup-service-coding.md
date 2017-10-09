---
title: Set Up Codes for Standard Services | Microsoft Docs
description: Learn how to set up codes for service activities that you often perform.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, service order, repairs, maintenance
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8a31e312fc12d75d4eb75a191b2b82bf9a6ff3c5
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---

# <a name="how-to-set-up-standard-service-codes"></a><span data-ttu-id="3c322-103">How to: Set Up Standard Service Codes</span><span class="sxs-lookup"><span data-stu-id="3c322-103">How to: Set Up Standard Service Codes</span></span>
<span data-ttu-id="3c322-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span><span class="sxs-lookup"><span data-stu-id="3c322-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span></span> <span data-ttu-id="3c322-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span><span class="sxs-lookup"><span data-stu-id="3c322-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span></span> <span data-ttu-id="3c322-106">When you choose the code on a service document, the lines are entered automatically.</span><span class="sxs-lookup"><span data-stu-id="3c322-106">When you choose the code on a service document, the lines are entered automatically.</span></span> <span data-ttu-id="3c322-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standrd text linked to it.</span><span class="sxs-lookup"><span data-stu-id="3c322-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standrd text linked to it.</span></span> <span data-ttu-id="3c322-108">You create service lines of each standard serice code on the **Standard Service Code** card.</span><span class="sxs-lookup"><span data-stu-id="3c322-108">You create service lines of each standard serice code on the **Standard Service Code** card.</span></span> <span data-ttu-id="3c322-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span><span class="sxs-lookup"><span data-stu-id="3c322-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span></span> <span data-ttu-id="3c322-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span><span class="sxs-lookup"><span data-stu-id="3c322-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span></span>  
  
> [!Tip]
>  <span data-ttu-id="3c322-111">You can use the same concept to create lines on sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="3c322-111">You can use the same concept to create lines on sales and purchase documents.</span></span> <span data-ttu-id="3c322-112">For more information, see [How to: Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span><span class="sxs-lookup"><span data-stu-id="3c322-112">For more information, see [How to: Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span></span>    
  
## <a name="to-set-up-a-standard-service-code"></a><span data-ttu-id="3c322-113">To set up a standard service code</span><span class="sxs-lookup"><span data-stu-id="3c322-113">To set up a standard service code</span></span>    
1. <span data-ttu-id="3c322-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Standard Service Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3c322-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Standard Service Codes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c322-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="3c322-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="3c322-116">Fill in the service lines linked to this service code.</span><span class="sxs-lookup"><span data-stu-id="3c322-116">Fill in the service lines linked to this service code.</span></span>  

## <a name="to-assign-a-standard-service-code-to-a-service-item-group"></a><span data-ttu-id="3c322-117">To assign a standard service code to a service item group</span><span class="sxs-lookup"><span data-stu-id="3c322-117">To assign a standard service code to a service item group</span></span>
1. <span data-ttu-id="3c322-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service item Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3c322-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c322-119">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="3c322-119">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="3c322-120">Fill in the service lines linked to this service code.</span><span class="sxs-lookup"><span data-stu-id="3c322-120">Fill in the service lines linked to this service code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3c322-121">See Also</span><span class="sxs-lookup"><span data-stu-id="3c322-121">See Also</span></span>
[<span data-ttu-id="3c322-122">Service Management</span><span class="sxs-lookup"><span data-stu-id="3c322-122">Service Management</span></span>](service-service.md)
