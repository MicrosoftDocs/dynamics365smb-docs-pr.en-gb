---
title: How to Use the Manufacturing Batch Unit of Measure | Microsoft Docs
description: If an item is stocked in one unit of measure but produced in another, then the production order must be use a manufacturing batch unit of measure to calculate the correct quantity of components. An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9abad1ccc89ef8d47d1d3fe19077814b03668db6
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787684"
---
# <a name="work-with-manufacturing-batch-units-of-measure"></a><span data-ttu-id="e16c4-104">Work with Manufacturing Batch Units of Measure</span><span class="sxs-lookup"><span data-stu-id="e16c4-104">Work with Manufacturing Batch Units of Measure</span></span>
<span data-ttu-id="e16c4-105">If an item is stocked in one unit of measure but produced in another, a production order is created that uses a manufacturing batch unit of measure to calculate the correct quantity of the components during the **Refresh Production Order** batch job.</span><span class="sxs-lookup"><span data-stu-id="e16c4-105">If an item is stocked in one unit of measure but produced in another, a production order is created that uses a manufacturing batch unit of measure to calculate the correct quantity of the components during the **Refresh Production Order** batch job.</span></span> <span data-ttu-id="e16c4-106">An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.</span><span class="sxs-lookup"><span data-stu-id="e16c4-106">An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.</span></span>  

## <a name="to-create-a-production-bom-using-a-batch-unit-of-measure"></a><span data-ttu-id="e16c4-107">To create a production BOM using a batch unit of measure</span><span class="sxs-lookup"><span data-stu-id="e16c4-107">To create a production BOM using a batch unit of measure</span></span>  
1.  <span data-ttu-id="e16c4-108">The manufacturing batch unit of measure is set up as an alternative unit of measure on the **Item Units of Measure** page on the item to be produced.</span><span class="sxs-lookup"><span data-stu-id="e16c4-108">The manufacturing batch unit of measure is set up as an alternative unit of measure on the **Item Units of Measure** page on the item to be produced.</span></span> <span data-ttu-id="e16c4-109">The batch unit of measure will not replace the base unit of measure on the item.</span><span class="sxs-lookup"><span data-stu-id="e16c4-109">The batch unit of measure will not replace the base unit of measure on the item.</span></span>  
2.  <span data-ttu-id="e16c4-110">Create a production BOM for the item set up with the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-110">Create a production BOM for the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="e16c4-111">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="e16c4-111">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span></span>  
3.  <span data-ttu-id="e16c4-112">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-112">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure.</span></span>  
4.  <span data-ttu-id="e16c4-113">For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-113">For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measure.</span></span>  
5.  <span data-ttu-id="e16c4-114">Open the **Item Card** for the related item.</span><span class="sxs-lookup"><span data-stu-id="e16c4-114">Open the **Item Card** for the related item.</span></span>  

    <span data-ttu-id="e16c4-115">On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.</span><span class="sxs-lookup"><span data-stu-id="e16c4-115">On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.</span></span>  
6.  <span data-ttu-id="e16c4-116">Create a production order header using the item set up with the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-116">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="e16c4-117">For more information, see [Create Production Orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="e16c4-117">For more information, see [Create Production Orders](production-how-to-create-production-orders.md).</span></span>  
7.  <span data-ttu-id="e16c4-118">Choose the **Refresh** action, and then choose  the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e16c4-118">Choose the **Refresh** action, and then choose  the **OK** button.</span></span>  

<span data-ttu-id="e16c4-119">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span><span class="sxs-lookup"><span data-stu-id="e16c4-119">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="e16c4-120">The application calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-120">The application calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measure.</span></span>  

## <a name="to-calculate-a-manufacturing-batch-unit-of-measure-on-a-production-order"></a><span data-ttu-id="e16c4-121">To calculate a manufacturing batch unit of measure on a production order</span><span class="sxs-lookup"><span data-stu-id="e16c4-121">To calculate a manufacturing batch unit of measure on a production order</span></span>  
1.  <span data-ttu-id="e16c4-122">Create a production order header using the item set up with the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-122">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span>  
2.  <span data-ttu-id="e16c4-123">In the **Item No.** field in the Production Order line, type the same item number used in the header.</span><span class="sxs-lookup"><span data-stu-id="e16c4-123">In the **Item No.** field in the Production Order line, type the same item number used in the header.</span></span>  
3.  <span data-ttu-id="e16c4-124">In the **Quantity** field, enter the same quantity used in the header.</span><span class="sxs-lookup"><span data-stu-id="e16c4-124">In the **Quantity** field, enter the same quantity used in the header.</span></span>  
4.  <span data-ttu-id="e16c4-125">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure code.</span><span class="sxs-lookup"><span data-stu-id="e16c4-125">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure code.</span></span>  
5.  <span data-ttu-id="e16c4-126">Choose the **Refresh** action.</span><span class="sxs-lookup"><span data-stu-id="e16c4-126">Choose the **Refresh** action.</span></span>
6.  <span data-ttu-id="e16c4-127">On the **Calculate** FastTab, clear the **Lines** check box.</span><span class="sxs-lookup"><span data-stu-id="e16c4-127">On the **Calculate** FastTab, clear the **Lines** check box.</span></span>  
7.  <span data-ttu-id="e16c4-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="e16c4-128">Choose the **OK** button.</span></span>  
8.  <span data-ttu-id="e16c4-129">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span><span class="sxs-lookup"><span data-stu-id="e16c4-129">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="e16c4-130">The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measure.</span><span class="sxs-lookup"><span data-stu-id="e16c4-130">The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measure.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e16c4-131">See Also</span><span class="sxs-lookup"><span data-stu-id="e16c4-131">See Also</span></span>  
[<span data-ttu-id="e16c4-132">Create Routings</span><span class="sxs-lookup"><span data-stu-id="e16c4-132">Create Routings</span></span>](production-how-to-create-routings.md)  
<span data-ttu-id="e16c4-133">[Create Production BOMs](production-how-to-create-production-boms.md)   </span><span class="sxs-lookup"><span data-stu-id="e16c4-133">[Create Production BOMs](production-how-to-create-production-boms.md)   </span></span>  
[<span data-ttu-id="e16c4-134">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="e16c4-134">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="e16c4-135">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="e16c4-135">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="e16c4-136">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="e16c4-136">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="e16c4-137">Inventory</span><span class="sxs-lookup"><span data-stu-id="e16c4-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="e16c4-138">Purchasing</span><span class="sxs-lookup"><span data-stu-id="e16c4-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="e16c4-139">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e16c4-139">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]