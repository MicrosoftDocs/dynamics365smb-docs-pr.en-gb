---
title: How to Assign Default Bins to Items | Microsoft Docs
description: If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.
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
ms.openlocfilehash: 0eb6dc74d9ac050c692c003799c3142bdbdaeeaa
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "927909"
---
# <a name="assign-default-bins-to-items"></a><span data-ttu-id="2128b-104">Assign Default Bins to Items</span><span class="sxs-lookup"><span data-stu-id="2128b-104">Assign Default Bins to Items</span></span>
<span data-ttu-id="2128b-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span><span class="sxs-lookup"><span data-stu-id="2128b-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="2128b-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span><span class="sxs-lookup"><span data-stu-id="2128b-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="2128b-107">Default bins are defined on the **Bin Content** page.</span><span class="sxs-lookup"><span data-stu-id="2128b-107">Default bins are defined on the **Bin Content** page.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="2128b-108">To assign a default bin to an item</span><span class="sxs-lookup"><span data-stu-id="2128b-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="2128b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2128b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet**, and choose the related link.</span></span>  
2.  <span data-ttu-id="2128b-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span><span class="sxs-lookup"><span data-stu-id="2128b-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="2128b-111">Make sure to select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="2128b-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="2128b-112">Choose the **Create Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="2128b-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="2128b-113">Default bins are now assigned for your item.</span><span class="sxs-lookup"><span data-stu-id="2128b-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2128b-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span><span class="sxs-lookup"><span data-stu-id="2128b-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="2128b-115">To change the default bin for an item</span><span class="sxs-lookup"><span data-stu-id="2128b-115">To change the default bin for an item</span></span>  
<span data-ttu-id="2128b-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span><span class="sxs-lookup"><span data-stu-id="2128b-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="2128b-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2128b-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2128b-118">In the **Location Filter** field, select the appropriate location code.</span><span class="sxs-lookup"><span data-stu-id="2128b-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="2128b-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="2128b-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="2128b-120">Find the bin content line for the bin that you would like as the new default bin.</span><span class="sxs-lookup"><span data-stu-id="2128b-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="2128b-121">Select the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="2128b-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="2128b-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span><span class="sxs-lookup"><span data-stu-id="2128b-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2128b-123">See Also</span><span class="sxs-lookup"><span data-stu-id="2128b-123">See Also</span></span>  
[<span data-ttu-id="2128b-124">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="2128b-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="2128b-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="2128b-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="2128b-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="2128b-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="2128b-127">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="2128b-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="2128b-128">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="2128b-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="2128b-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2128b-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
