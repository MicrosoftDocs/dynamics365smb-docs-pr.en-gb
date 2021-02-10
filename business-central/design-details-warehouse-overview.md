---
title: Design Details - Warehouse Overview | Microsoft Docs
description: To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse. This is managed in the **Warehouse Entry** table. Each transaction is stored in a warehouse register.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 8842bd23f6d2d470599afe9b4382b35cec3d9251
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749550"
---
# <a name="design-details-warehouse-overview"></a><span data-ttu-id="66c69-105">Design Details: Warehouse Overview</span><span class="sxs-lookup"><span data-stu-id="66c69-105">Design Details: Warehouse Overview</span></span>
<span data-ttu-id="66c69-106">To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="66c69-106">To support the physical handling of items on the zone and bin level, all information must be traced for each transaction or movement in the warehouse.</span></span> <span data-ttu-id="66c69-107">This is managed in the **Warehouse Entry** table.</span><span class="sxs-lookup"><span data-stu-id="66c69-107">This is managed in the **Warehouse Entry** table.</span></span> <span data-ttu-id="66c69-108">Each transaction is stored in a warehouse register.</span><span class="sxs-lookup"><span data-stu-id="66c69-108">Each transaction is stored in a warehouse register.</span></span>  

<span data-ttu-id="66c69-109">Warehouse documents and a warehouse journal are used to register item movements in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="66c69-109">Warehouse documents and a warehouse journal are used to register item movements in the warehouse.</span></span> <span data-ttu-id="66c69-110">Every time that an item in the warehouse is moved, received, put away, picked, shipped, or adjusted, warehouse entries are registered to store the physical information about zone, bin, and quantity.</span><span class="sxs-lookup"><span data-stu-id="66c69-110">Every time that an item in the warehouse is moved, received, put away, picked, shipped, or adjusted, warehouse entries are registered to store the physical information about zone, bin, and quantity.</span></span>

<span data-ttu-id="66c69-111">The **Bin Content** table is used to handle all the different dimensions of the contents of a bin per item, such as unit of measure, maximum quantity, and minimum quantity.</span><span class="sxs-lookup"><span data-stu-id="66c69-111">The **Bin Content** table is used to handle all the different dimensions of the contents of a bin per item, such as unit of measure, maximum quantity, and minimum quantity.</span></span> <span data-ttu-id="66c69-112">The **Bin Content** table also contains flow fields to the warehouse entries, warehouse instructions, and warehouse journal lines, which ensures that the availability of an item per bin and a bin for an item can be calculated quickly.</span><span class="sxs-lookup"><span data-stu-id="66c69-112">The **Bin Content** table also contains flow fields to the warehouse entries, warehouse instructions, and warehouse journal lines, which ensures that the availability of an item per bin and a bin for an item can be calculated quickly.</span></span> <span data-ttu-id="66c69-113">For more information, see [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="66c69-113">For more information, see [Design Details: Availability in the Warehouse](design-details-availability-in-the-warehouse.md).</span></span>  

<span data-ttu-id="66c69-114">When item postings occur outside the warehouse module, a default adjustment bin per location is used to synchronise warehouse entries with inventory entries.</span><span class="sxs-lookup"><span data-stu-id="66c69-114">When item postings occur outside the warehouse module, a default adjustment bin per location is used to synchronize warehouse entries with inventory entries.</span></span> <span data-ttu-id="66c69-115">During physical inventory of the warehouse, any differences between the calculated and counted quantities are recorded in the adjustment bin and then posted as correcting item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="66c69-115">During physical inventory of the warehouse, any differences between the calculated and counted quantities are recorded in the adjustment bin and then posted as correcting item ledger entries.</span></span> <span data-ttu-id="66c69-116">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="66c69-116">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="66c69-117">The following illustration outlines typical warehouse flows.</span><span class="sxs-lookup"><span data-stu-id="66c69-117">The following illustration outlines typical warehouse flows.</span></span>  

<span data-ttu-id="66c69-118">![Overview of warehouse processes](media/design_details_warehouse_management_overview.png "Overview of warehouse processes")</span><span class="sxs-lookup"><span data-stu-id="66c69-118">![Overview of warehouse processes](media/design_details_warehouse_management_overview.png "Overview of warehouse processes")</span></span>  

## <a name="basic-or-advanced-warehousing"></a><span data-ttu-id="66c69-119">Basic or Advanced Warehousing</span><span class="sxs-lookup"><span data-stu-id="66c69-119">Basic or Advanced Warehousing</span></span>  
<span data-ttu-id="66c69-120">Warehouse functionality in [!INCLUDE[prod_short](includes/prod_short.md)] can be implemented in different complexity levels, depending on a company’s processes and order volume.</span><span class="sxs-lookup"><span data-stu-id="66c69-120">Warehouse functionality in [!INCLUDE[prod_short](includes/prod_short.md)] can be implemented in different complexity levels, depending on a company’s processes and order volume.</span></span> <span data-ttu-id="66c69-121">The main difference is that activities are performed order-by-order in basic warehousing when they are consolidated for multiple orders in advanced warehousing.</span><span class="sxs-lookup"><span data-stu-id="66c69-121">The main difference is that activities are performed order-by-order in basic warehousing when they are consolidated for multiple orders in advanced warehousing.</span></span>  

 <span data-ttu-id="66c69-122">To differentiate between the different complexity levels, this documentation refers to two general denominations, Basic and Advanced Warehousing.</span><span class="sxs-lookup"><span data-stu-id="66c69-122">To differentiate between the different complexity levels, this documentation refers to two general denominations, Basic and Advanced Warehousing.</span></span> <span data-ttu-id="66c69-123">This simple differentiation covers several different complexity levels as defined by product granules and location setup, each supported by different UI documents.</span><span class="sxs-lookup"><span data-stu-id="66c69-123">This simple differentiation covers several different complexity levels as defined by product granules and location setup, each supported by different UI documents.</span></span> <span data-ttu-id="66c69-124">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span><span class="sxs-lookup"><span data-stu-id="66c69-124">For more information, see [Design Details: Warehouse Setup](design-details-warehouse-setup.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="66c69-125">The most advanced level of warehousing is referred to as “WMS installations” in this documentation, since this level requires the most advanced granule, Warehouse Management Systems.</span><span class="sxs-lookup"><span data-stu-id="66c69-125">The most advanced level of warehousing is referred to as “WMS installations” in this documentation, since this level requires the most advanced granule, Warehouse Management Systems.</span></span>  

 <span data-ttu-id="66c69-126">The following different UI documents are used in basic and advanced warehousing.</span><span class="sxs-lookup"><span data-stu-id="66c69-126">The following different UI documents are used in basic and advanced warehousing.</span></span>  

## <a name="basic-ui-documents"></a><span data-ttu-id="66c69-127">Basic UI Documents</span><span class="sxs-lookup"><span data-stu-id="66c69-127">Basic UI Documents</span></span>  

-   <span data-ttu-id="66c69-128">**Inventory Put-away**</span><span class="sxs-lookup"><span data-stu-id="66c69-128">**Inventory Put-away**</span></span>  
-   <span data-ttu-id="66c69-129">**Inventory Pick**</span><span class="sxs-lookup"><span data-stu-id="66c69-129">**Inventory Pick**</span></span>  
-   <span data-ttu-id="66c69-130">**Inventory Movement**</span><span class="sxs-lookup"><span data-stu-id="66c69-130">**Inventory Movement**</span></span>  
-   <span data-ttu-id="66c69-131">**Item Journal**</span><span class="sxs-lookup"><span data-stu-id="66c69-131">**Item Journal**</span></span>  
-   <span data-ttu-id="66c69-132">**Item Reclassification Journal**</span><span class="sxs-lookup"><span data-stu-id="66c69-132">**Item Reclassification Journal**</span></span>  
-   <span data-ttu-id="66c69-133">(Various reports)</span><span class="sxs-lookup"><span data-stu-id="66c69-133">(Various reports)</span></span>  

## <a name="advanced-ui-documents"></a><span data-ttu-id="66c69-134">Advanced UI Documents</span><span class="sxs-lookup"><span data-stu-id="66c69-134">Advanced UI Documents</span></span>  

-   <span data-ttu-id="66c69-135">**Warehouse Receipt**</span><span class="sxs-lookup"><span data-stu-id="66c69-135">**Warehouse Receipt**</span></span>  
-   <span data-ttu-id="66c69-136">**Put-away Worksheet**</span><span class="sxs-lookup"><span data-stu-id="66c69-136">**Put-away Worksheet**</span></span>  
-   <span data-ttu-id="66c69-137">**Warehouse Put-away**</span><span class="sxs-lookup"><span data-stu-id="66c69-137">**Warehouse Put-away**</span></span>  
-   <span data-ttu-id="66c69-138">**Pick Worksheet**</span><span class="sxs-lookup"><span data-stu-id="66c69-138">**Pick Worksheet**</span></span>  
-   <span data-ttu-id="66c69-139">**Warehouse Pick**</span><span class="sxs-lookup"><span data-stu-id="66c69-139">**Warehouse Pick**</span></span>  
-   <span data-ttu-id="66c69-140">**Movement Worksheet**</span><span class="sxs-lookup"><span data-stu-id="66c69-140">**Movement Worksheet**</span></span>  
-   <span data-ttu-id="66c69-141">**Warehouse Movement**</span><span class="sxs-lookup"><span data-stu-id="66c69-141">**Warehouse Movement**</span></span>  
-   <span data-ttu-id="66c69-142">**Internal Whse. Pick**</span><span class="sxs-lookup"><span data-stu-id="66c69-142">**Internal Whse. Pick**</span></span>  
-   <span data-ttu-id="66c69-143">**Internal Whse. Put-away**</span><span class="sxs-lookup"><span data-stu-id="66c69-143">**Internal Whse. Put-away**</span></span>  
-   <span data-ttu-id="66c69-144">**Bin Creation Worksheet**</span><span class="sxs-lookup"><span data-stu-id="66c69-144">**Bin Creation Worksheet**</span></span>  
-   <span data-ttu-id="66c69-145">**Bin Content Creation Worksheet**</span><span class="sxs-lookup"><span data-stu-id="66c69-145">**Bin Content Creation Worksheet**</span></span>  
-   <span data-ttu-id="66c69-146">**Whse. Item Journal**</span><span class="sxs-lookup"><span data-stu-id="66c69-146">**Whse. Item Journal**</span></span>  
-   <span data-ttu-id="66c69-147">**Whse. Item Reclass. Journal**</span><span class="sxs-lookup"><span data-stu-id="66c69-147">**Whse. Item Reclass. Journal**</span></span>  
-   <span data-ttu-id="66c69-148">(Various reports)</span><span class="sxs-lookup"><span data-stu-id="66c69-148">(Various reports)</span></span>  

<span data-ttu-id="66c69-149">For more information about each document, see the respective page topics.</span><span class="sxs-lookup"><span data-stu-id="66c69-149">For more information about each document, see the respective page topics.</span></span>  

### <a name="terminology"></a><span data-ttu-id="66c69-150">Terminology</span><span class="sxs-lookup"><span data-stu-id="66c69-150">Terminology</span></span>  
<span data-ttu-id="66c69-151">To align with the financial concepts of purchases and sales, [!INCLUDE[prod_short](includes/prod_short.md)] warehouse documentation refers to the following terms for item flow in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="66c69-151">To align with the financial concepts of purchases and sales, [!INCLUDE[prod_short](includes/prod_short.md)] warehouse documentation refers to the following terms for item flow in the warehouse.</span></span>  

|<span data-ttu-id="66c69-152">Term</span><span class="sxs-lookup"><span data-stu-id="66c69-152">Term</span></span>|<span data-ttu-id="66c69-153">Description</span><span class="sxs-lookup"><span data-stu-id="66c69-153">Description</span></span>|  
|----------|---------------------------------------|  
|<span data-ttu-id="66c69-154">Inbound flow</span><span class="sxs-lookup"><span data-stu-id="66c69-154">Inbound flow</span></span>|<span data-ttu-id="66c69-155">Items moving into the warehouse location, such as purchases and inbound transfers.</span><span class="sxs-lookup"><span data-stu-id="66c69-155">Items moving into the warehouse location, such as purchases and inbound transfers.</span></span>|  
|<span data-ttu-id="66c69-156">Internal flow</span><span class="sxs-lookup"><span data-stu-id="66c69-156">Internal flow</span></span>|<span data-ttu-id="66c69-157">Items moving inside the warehouse location, such as production components and output.</span><span class="sxs-lookup"><span data-stu-id="66c69-157">Items moving inside the warehouse location, such as production components and output.</span></span>|  
|<span data-ttu-id="66c69-158">Outbound flow</span><span class="sxs-lookup"><span data-stu-id="66c69-158">Outbound flow</span></span>|<span data-ttu-id="66c69-159">Items moving out of the warehouse location, such as sales and outbound transfers.</span><span class="sxs-lookup"><span data-stu-id="66c69-159">Items moving out of the warehouse location, such as sales and outbound transfers.</span></span>|  

## <a name="see-also"></a><span data-ttu-id="66c69-160">See Also</span><span class="sxs-lookup"><span data-stu-id="66c69-160">See Also</span></span>  
 [<span data-ttu-id="66c69-161">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="66c69-161">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)
