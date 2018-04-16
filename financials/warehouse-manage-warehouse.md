---
title: Warehouse Activities | Microsoft Docs
description: After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: 7540467cdb958f82a64ca0097b365b09b2d1e947
ms.contentlocale: en-gb
ms.lasthandoff: 04/16/2018

---
# <a name="warehouse-management"></a><span data-ttu-id="b8cf6-103">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b8cf6-103">Warehouse Management</span></span>
<span data-ttu-id="b8cf6-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.</span></span>

<span data-ttu-id="b8cf6-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span></span> <span data-ttu-id="b8cf6-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span></span> <span data-ttu-id="b8cf6-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="b8cf6-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>  

<span data-ttu-id="b8cf6-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span></span> <span data-ttu-id="b8cf6-109">In simpler installations, the flow is less formalised and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-109">In simpler installations, the flow is less formalized and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span></span> <span data-ttu-id="b8cf6-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b8cf6-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span></span>

<span data-ttu-id="b8cf6-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span></span> <span data-ttu-id="b8cf6-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="b8cf6-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

 <span data-ttu-id="b8cf6-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="b8cf6-114">**To**</span><span class="sxs-lookup"><span data-stu-id="b8cf6-114">**To**</span></span>|<span data-ttu-id="b8cf6-115">**See**</span><span class="sxs-lookup"><span data-stu-id="b8cf6-115">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b8cf6-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span></span>|[<span data-ttu-id="b8cf6-117">Receive Items</span><span class="sxs-lookup"><span data-stu-id="b8cf6-117">Receive Items</span></span>](warehouse-how-receive-items.md)|
|<span data-ttu-id="b8cf6-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span></span>|[<span data-ttu-id="b8cf6-119">Cross-Dock Items</span><span class="sxs-lookup"><span data-stu-id="b8cf6-119">Cross-Dock Items</span></span>](warehouse-how-to-cross-dock-items.md)|    
|<span data-ttu-id="b8cf6-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span></span>|[<span data-ttu-id="b8cf6-121">Putting Items Away</span><span class="sxs-lookup"><span data-stu-id="b8cf6-121">Putting Items Away</span></span>](warehouse-put-away-items.md)|
|<span data-ttu-id="b8cf6-122">Move items between bins in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-122">Move items between bins in the warehouse.</span></span>|[<span data-ttu-id="b8cf6-123">Moving Items</span><span class="sxs-lookup"><span data-stu-id="b8cf6-123">Moving Items</span></span>](warehouse-move-items.md)|
|<span data-ttu-id="b8cf6-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span></span>|[<span data-ttu-id="b8cf6-125">Picking Items</span><span class="sxs-lookup"><span data-stu-id="b8cf6-125">Picking Items</span></span>](warehouse-pick-items.md)|
|<span data-ttu-id="b8cf6-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span><span class="sxs-lookup"><span data-stu-id="b8cf6-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span></span>|[<span data-ttu-id="b8cf6-127">Ship Items</span><span class="sxs-lookup"><span data-stu-id="b8cf6-127">Ship Items</span></span>](warehouse-how-ship-items.md)|  

## <a name="see-also"></a><span data-ttu-id="b8cf6-128">See Also</span><span class="sxs-lookup"><span data-stu-id="b8cf6-128">See Also</span></span>  
[<span data-ttu-id="b8cf6-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="b8cf6-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="b8cf6-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="b8cf6-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="b8cf6-131">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="b8cf6-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="b8cf6-132">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b8cf6-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b8cf6-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b8cf6-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE [d365fin](includes/free_trial_md.md)]  
## [!INCLUDE [d365fin](includes/training_link_md.md)]

