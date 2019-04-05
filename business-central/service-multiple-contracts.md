---
title: Multiple Contracts | Microsoft Docs
description: Depending on your service level agreements with a customer, you may have to handle a service item under more than one service contract.
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
ms.openlocfilehash: 58e92211695ea3a8d8c4137c699794f935c1bc69
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "808558"
---
# <a name="multiple-contracts"></a><span data-ttu-id="2dd79-103">Multiple Contracts</span><span class="sxs-lookup"><span data-stu-id="2dd79-103">Multiple Contracts</span></span>
<span data-ttu-id="2dd79-104">Depending on your service level agreements with a customer, you may have to handle a service item under more than one service contract.</span><span class="sxs-lookup"><span data-stu-id="2dd79-104">Depending on your service level agreements with a customer, you may have to handle a service item under more than one service contract.</span></span>  
  
<span data-ttu-id="2dd79-105">By handling a service item under multiple contracts, you can do the following:</span><span class="sxs-lookup"><span data-stu-id="2dd79-105">By handling a service item under multiple contracts, you can do the following:</span></span>  
  
* <span data-ttu-id="2dd79-106">Issue different contracts for the same service item.</span><span class="sxs-lookup"><span data-stu-id="2dd79-106">Issue different contracts for the same service item.</span></span>  
* <span data-ttu-id="2dd79-107">Service parts separately.</span><span class="sxs-lookup"><span data-stu-id="2dd79-107">Service parts separately.</span></span>  
* <span data-ttu-id="2dd79-108">Consider different skills that are required to service different aspects of a service item, such as mechanical components and software.</span><span class="sxs-lookup"><span data-stu-id="2dd79-108">Consider different skills that are required to service different aspects of a service item, such as mechanical components and software.</span></span>  
* <span data-ttu-id="2dd79-109">Specify different response times and frequencies in servicing different parts of a service item.</span><span class="sxs-lookup"><span data-stu-id="2dd79-109">Specify different response times and frequencies in servicing different parts of a service item.</span></span>  
* <span data-ttu-id="2dd79-110">Address different kinds of activities to be performed on a service item when the service item requires different types of service in different time periods.</span><span class="sxs-lookup"><span data-stu-id="2dd79-110">Address different kinds of activities to be performed on a service item when the service item requires different types of service in different time periods.</span></span>  
* <span data-ttu-id="2dd79-111">Select and assign an appropriate contract number to a service item line when you are creating a service order.</span><span class="sxs-lookup"><span data-stu-id="2dd79-111">Select and assign an appropriate contract number to a service item line when you are creating a service order.</span></span>  
* <span data-ttu-id="2dd79-112">Handle relevant financial information about service items and service level agreements.</span><span class="sxs-lookup"><span data-stu-id="2dd79-112">Handle relevant financial information about service items and service level agreements.</span></span>  
  
<span data-ttu-id="2dd79-113">You can consider the following examples of using the multiple contracts functionality.</span><span class="sxs-lookup"><span data-stu-id="2dd79-113">You can consider the following examples of using the multiple contracts functionality.</span></span>  
  
## <a name="creating-multiple-contracts-per-service-item"></a><span data-ttu-id="2dd79-114">Creating Multiple Contracts per Service Item</span><span class="sxs-lookup"><span data-stu-id="2dd79-114">Creating Multiple Contracts per Service Item</span></span>  
<span data-ttu-id="2dd79-115">You can manually create a service contract or contract quote for service items already registered in non-cancelled contracts owned by the same customer.</span><span class="sxs-lookup"><span data-stu-id="2dd79-115">You can manually create a service contract or contract quote for service items already registered in non-canceled contracts owned by the same customer.</span></span> <span data-ttu-id="2dd79-116">To do this, follow the standard procedure of creating service contracts and service contract quotes.</span><span class="sxs-lookup"><span data-stu-id="2dd79-116">To do this, follow the standard procedure of creating service contracts and service contract quotes.</span></span> <span data-ttu-id="2dd79-117">For more information, see [Work with Service Contracts and Service Contract Quotes](service-how-to-create-service-contracts-and-service-contract-quotes.md).</span><span class="sxs-lookup"><span data-stu-id="2dd79-117">For more information, see [Work with Service Contracts and Service Contract Quotes](service-how-to-create-service-contracts-and-service-contract-quotes.md).</span></span>  
  
<span data-ttu-id="2dd79-118">When you add a service item on a contract line that is registered in other service contracts or contract quotes, a warning message is displayed stating that the service item already belongs to one or more service contracts or contract quotes.</span><span class="sxs-lookup"><span data-stu-id="2dd79-118">When you add a service item on a contract line that is registered in other service contracts or contract quotes, a warning message is displayed stating that the service item already belongs to one or more service contracts or contract quotes.</span></span> <span data-ttu-id="2dd79-119">If you confirm this message, all relevant service item information is copied to a newly created contract line.</span><span class="sxs-lookup"><span data-stu-id="2dd79-119">If you confirm this message, all relevant service item information is copied to a newly created contract line.</span></span>  
  
## <a name="copying-documents"></a><span data-ttu-id="2dd79-120">Copying Documents</span><span class="sxs-lookup"><span data-stu-id="2dd79-120">Copying Documents</span></span>  
<span data-ttu-id="2dd79-121">You can automatically create a service contract or contract quote for service items that are already registered in other service contracts or contract quotes by using the **Copy Document** action.</span><span class="sxs-lookup"><span data-stu-id="2dd79-121">You can automatically create a service contract or contract quote for service items that are already registered in other service contracts or contract quotes by using the **Copy Document** action.</span></span>  
  
## <a name="creating-service-orders-for-multiple-contracts"></a><span data-ttu-id="2dd79-122">Creating Service Orders for Multiple Contracts</span><span class="sxs-lookup"><span data-stu-id="2dd79-122">Creating Service Orders for Multiple Contracts</span></span>  
<span data-ttu-id="2dd79-123">You can manually create a service order for a service item that is registered in multiple active contracts.</span><span class="sxs-lookup"><span data-stu-id="2dd79-123">You can manually create a service order for a service item that is registered in multiple active contracts.</span></span> <span data-ttu-id="2dd79-124">A service contract is active when it is signed and not expired.</span><span class="sxs-lookup"><span data-stu-id="2dd79-124">A service contract is active when it is signed and not expired.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2dd79-125">See Also</span><span class="sxs-lookup"><span data-stu-id="2dd79-125">See Also</span></span>  
[<span data-ttu-id="2dd79-126">Fulfilling Service Contracts</span><span class="sxs-lookup"><span data-stu-id="2dd79-126">Fulfilling Service Contracts</span></span>](service-fulfill-service-contracts.md)  
[<span data-ttu-id="2dd79-127">Create Service Orders</span><span class="sxs-lookup"><span data-stu-id="2dd79-127">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
