---
title: How to Assign Default Bins to Items | Microsoft Docs
description: If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 10168f9caafbc0c3245d6d387669592239f0e86b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5393281"
---
# <a name="assign-default-bins-to-items"></a><span data-ttu-id="88d3a-104">Assign Default Bins to Items</span><span class="sxs-lookup"><span data-stu-id="88d3a-104">Assign Default Bins to Items</span></span>
<span data-ttu-id="88d3a-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span><span class="sxs-lookup"><span data-stu-id="88d3a-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="88d3a-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span><span class="sxs-lookup"><span data-stu-id="88d3a-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="88d3a-107">Default bins are defined on the **Bin Content** page.</span><span class="sxs-lookup"><span data-stu-id="88d3a-107">Default bins are defined on the **Bin Content** page.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="88d3a-108">To assign a default bin to an item</span><span class="sxs-lookup"><span data-stu-id="88d3a-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="88d3a-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span><span class="sxs-lookup"><span data-stu-id="88d3a-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="88d3a-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span><span class="sxs-lookup"><span data-stu-id="88d3a-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="88d3a-111">Make sure to select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="88d3a-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="88d3a-112">Choose the **Create Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="88d3a-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="88d3a-113">Default bins are now assigned for your item.</span><span class="sxs-lookup"><span data-stu-id="88d3a-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="88d3a-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span><span class="sxs-lookup"><span data-stu-id="88d3a-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="88d3a-115">To change the default bin for an item</span><span class="sxs-lookup"><span data-stu-id="88d3a-115">To change the default bin for an item</span></span>  
<span data-ttu-id="88d3a-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span><span class="sxs-lookup"><span data-stu-id="88d3a-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="88d3a-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="88d3a-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="88d3a-118">In the **Location Filter** field, select the appropriate location code.</span><span class="sxs-lookup"><span data-stu-id="88d3a-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="88d3a-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="88d3a-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="88d3a-120">Find the bin content line for the bin that you would like as the new default bin.</span><span class="sxs-lookup"><span data-stu-id="88d3a-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="88d3a-121">Select the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="88d3a-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="88d3a-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span><span class="sxs-lookup"><span data-stu-id="88d3a-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="88d3a-123">See Also</span><span class="sxs-lookup"><span data-stu-id="88d3a-123">See Also</span></span>  
[<span data-ttu-id="88d3a-124">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="88d3a-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="88d3a-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="88d3a-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="88d3a-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="88d3a-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="88d3a-127">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="88d3a-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="88d3a-128">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="88d3a-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="88d3a-129">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="88d3a-129">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]