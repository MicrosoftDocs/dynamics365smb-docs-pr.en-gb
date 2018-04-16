---
title: Execute Production | Microsoft Docs
description: When demand is planned for and the materials have been issued according to production BOMs, then the actual production operations can start and be executed in the sequence defined by the production order routing.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: aeef0cf47c6f83278313ccdb44aa94d4f1017b43
ms.contentlocale: en-gb
ms.lasthandoff: 04/16/2018

---
# <a name="manufacturing"></a><span data-ttu-id="aaf09-103">Manufacturing</span><span class="sxs-lookup"><span data-stu-id="aaf09-103">Manufacturing</span></span>
<span data-ttu-id="aaf09-104">When demand is planned for and the materials have been issued according to production BOMs, then the actual production operations can start and be executed in the sequence defined by the production order routing.</span><span class="sxs-lookup"><span data-stu-id="aaf09-104">When demand is planned for and the materials have been issued according to production BOMs, then the actual production operations can start and be executed in the sequence defined by the production order routing.</span></span>  

<span data-ttu-id="aaf09-105">An important part of executing production, from a system point of view, is to post production output to the database to report progress and to update inventory with the finished items.</span><span class="sxs-lookup"><span data-stu-id="aaf09-105">An important part of executing production, from a system point of view, is to post production output to the database to report progress and to update inventory with the finished items.</span></span> <span data-ttu-id="aaf09-106">Output posting can be done manually, by filling and posting journal lines after production operations.</span><span class="sxs-lookup"><span data-stu-id="aaf09-106">Output posting can be done manually, by filling and posting journal lines after production operations.</span></span> <span data-ttu-id="aaf09-107">Or, it can be done automatically with the use of backward flushing.</span><span class="sxs-lookup"><span data-stu-id="aaf09-107">Or, it can be done automatically with the use of backward flushing.</span></span> <span data-ttu-id="aaf09-108">In that case material consumption is automatically posted along with output when the production order changes to finished.</span><span class="sxs-lookup"><span data-stu-id="aaf09-108">In that case material consumption is automatically posted along with output when the production order changes to finished.</span></span>  

<span data-ttu-id="aaf09-109">As an alternative to the batch journal for output posting for multiple production orders, you can use the **Production Journal** window to post consumption and/or output for one production order line.</span><span class="sxs-lookup"><span data-stu-id="aaf09-109">As an alternative to the batch journal for output posting for multiple production orders, you can use the **Production Journal** window to post consumption and/or output for one production order line.</span></span>

<span data-ttu-id="aaf09-110">Before you can begin to produce items, you must make various setup, such as work centres, routings, and production BOMs.</span><span class="sxs-lookup"><span data-stu-id="aaf09-110">Before you can begin to produce items, you must make various setup, such as work centers, routings, and production BOMs.</span></span> <span data-ttu-id="aaf09-111">For more information, see [Setting Up Manufacturing](production-configure-production-processes.md).</span><span class="sxs-lookup"><span data-stu-id="aaf09-111">For more information, see [Setting Up Manufacturing](production-configure-production-processes.md).</span></span>

<span data-ttu-id="aaf09-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="aaf09-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="aaf09-113">**To**</span><span class="sxs-lookup"><span data-stu-id="aaf09-113">**To**</span></span>|<span data-ttu-id="aaf09-114">**See**</span><span class="sxs-lookup"><span data-stu-id="aaf09-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="aaf09-115">Understand how production orders work.</span><span class="sxs-lookup"><span data-stu-id="aaf09-115">Understand how production orders work.</span></span>|[<span data-ttu-id="aaf09-116">About Production Orders</span><span class="sxs-lookup"><span data-stu-id="aaf09-116">About Production Orders</span></span>](production-about-production-orders.md)|
|<span data-ttu-id="aaf09-117">Create production orders manually.</span><span class="sxs-lookup"><span data-stu-id="aaf09-117">Create production orders manually.</span></span>|[<span data-ttu-id="aaf09-118">Create Production Orders</span><span class="sxs-lookup"><span data-stu-id="aaf09-118">Create Production Orders</span></span>](production-how-to-create-production-orders.md)|
|<span data-ttu-id="aaf09-119">Outsource all or selected operations in a production order to a subcontractor.</span><span class="sxs-lookup"><span data-stu-id="aaf09-119">Outsource all or selected operations in a production order to a subcontractor.</span></span>|[<span data-ttu-id="aaf09-120">Subcontract Manufacturing</span><span class="sxs-lookup"><span data-stu-id="aaf09-120">Subcontract Manufacturing</span></span>](production-how-to-subcontract-manufacturing.md)|
|<span data-ttu-id="aaf09-121">Record and post production output along with material and time consumption for a single released production order line.</span><span class="sxs-lookup"><span data-stu-id="aaf09-121">Record and post production output along with material and time consumption for a single released production order line.</span></span>|[<span data-ttu-id="aaf09-122">Post Consumption and Output for One Released Production Order Line</span><span class="sxs-lookup"><span data-stu-id="aaf09-122">Post Consumption and Output for One Released Production Order Line</span></span>](production-how-to-register-consumption-and-output.md)|  
|<span data-ttu-id="aaf09-123">Batch post the quantity of components used per operation in a journal that can processes multiple planned production orders.</span><span class="sxs-lookup"><span data-stu-id="aaf09-123">Batch post the quantity of components used per operation in a journal that can processes multiple planned production orders.</span></span>|[<span data-ttu-id="aaf09-124">Batch Post Consumption</span><span class="sxs-lookup"><span data-stu-id="aaf09-124">Batch Post Consumption</span></span>](production-how-to-post-consumption.md)|
|<span data-ttu-id="aaf09-125">Post the quantity of finished items and the time spent per operation in a journal that can processes multiple released production orders.</span><span class="sxs-lookup"><span data-stu-id="aaf09-125">Post the quantity of finished items and the time spent per operation in a journal that can processes multiple released production orders.</span></span>|[<span data-ttu-id="aaf09-126">Batch Post Output and Run Times</span><span class="sxs-lookup"><span data-stu-id="aaf09-126">Batch Post Output and Run Times</span></span>](production-how-to-post-output-quantity.md)|  
|<span data-ttu-id="aaf09-127">Post the number of items produced in each finished operation which do not qualify as finished output, but as scrapped material.</span><span class="sxs-lookup"><span data-stu-id="aaf09-127">Post the number of items produced in each finished operation which do not qualify as finished output, but as scrapped material.</span></span>|[<span data-ttu-id="aaf09-128">Post Scrap</span><span class="sxs-lookup"><span data-stu-id="aaf09-128">Post Scrap</span></span>](production-how-to-post-scrap.md)|
|<span data-ttu-id="aaf09-129">View the shop floor load as a result of planned and released production orders.</span><span class="sxs-lookup"><span data-stu-id="aaf09-129">View the shop floor load as a result of planned and released production orders.</span></span>|[<span data-ttu-id="aaf09-130">View the Load in Work and Machine Centres</span><span class="sxs-lookup"><span data-stu-id="aaf09-130">View the Load in Work and Machine Centers</span></span>](production-how-to-view-the-load-on-work-centers.md)|      
|<span data-ttu-id="aaf09-131">Use the **Capacity Journal** window to post consumed capacities that are not assigned to a production order, such as maintenance work.</span><span class="sxs-lookup"><span data-stu-id="aaf09-131">Use the **Capacity Journal** window to post consumed capacities that are not assigned to a production order, such as maintenance work.</span></span>|[<span data-ttu-id="aaf09-132">Post Capacities</span><span class="sxs-lookup"><span data-stu-id="aaf09-132">Post Capacities</span></span>](production-how-to-post-capacities.md)|  
|<span data-ttu-id="aaf09-133">Calculate and adjust the cost of finished production items and consumed components for financial reconciliation.</span><span class="sxs-lookup"><span data-stu-id="aaf09-133">Calculate and adjust the cost of finished production items and consumed components for financial reconciliation.</span></span>|[<span data-ttu-id="aaf09-134">About Finished Production Order Costs</span><span class="sxs-lookup"><span data-stu-id="aaf09-134">About Finished Production Order Costs</span></span>](finance-about-finished-production-order-costs.md)|  

## <a name="see-also"></a><span data-ttu-id="aaf09-135">See Also</span><span class="sxs-lookup"><span data-stu-id="aaf09-135">See Also</span></span>  
[<span data-ttu-id="aaf09-136">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="aaf09-136">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="aaf09-137">[Planning](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="aaf09-137">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="aaf09-138">Inventory</span><span class="sxs-lookup"><span data-stu-id="aaf09-138">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="aaf09-139">Purchasing</span><span class="sxs-lookup"><span data-stu-id="aaf09-139">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="aaf09-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="aaf09-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

## [!INCLUDE [d365fin](includes/free_trial_md.md)]  
## [!INCLUDE [d365fin](includes/training_link_md.md)]

