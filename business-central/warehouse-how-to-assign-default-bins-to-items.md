---
title: How to Assign Default Bins to Items | Microsoft Docs
description: If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier. When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 8c8cca84e7ace9eb25f3e1366a5beefa954edbc4
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911903"
---
# <a name="assign-default-bins-to-items"></a><span data-ttu-id="06f85-104">Assign Default Bins to Items</span><span class="sxs-lookup"><span data-stu-id="06f85-104">Assign Default Bins to Items</span></span>
<span data-ttu-id="06f85-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span><span class="sxs-lookup"><span data-stu-id="06f85-105">If you are using bins at a location, assigning default bins to your items can make the process of shipping, receiving, and moving your items much easier.</span></span> <span data-ttu-id="06f85-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span><span class="sxs-lookup"><span data-stu-id="06f85-106">When a default bin is assigned to an item, this bin is suggested every time you initiate a transaction for this item.</span></span> <span data-ttu-id="06f85-107">Default bins are defined on the **Bin Content** page.</span><span class="sxs-lookup"><span data-stu-id="06f85-107">Default bins are defined on the **Bin Content** page.</span></span>  

## <a name="to-assign-a-default-bin-to-an-item"></a><span data-ttu-id="06f85-108">To assign a default bin to an item</span><span class="sxs-lookup"><span data-stu-id="06f85-108">To assign a default bin to an item</span></span>
1.  <span data-ttu-id="06f85-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet** , and choose the related link.</span><span class="sxs-lookup"><span data-stu-id="06f85-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Content Creation Worksheet** , and choose the related link.</span></span>  
2.  <span data-ttu-id="06f85-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span><span class="sxs-lookup"><span data-stu-id="06f85-110">Fill in the bin code and item information for each bin that you would like to set up as a default for an item.</span></span> <span data-ttu-id="06f85-111">Make sure to select the **Default** field.</span><span class="sxs-lookup"><span data-stu-id="06f85-111">Make sure to select the **Default** field.</span></span>  
3.  <span data-ttu-id="06f85-112">Choose the **Create Bin Content** action.</span><span class="sxs-lookup"><span data-stu-id="06f85-112">Choose the **Create Bin Content** action.</span></span> <span data-ttu-id="06f85-113">Default bins are now assigned for your item.</span><span class="sxs-lookup"><span data-stu-id="06f85-113">Default bins are now assigned for your item.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="06f85-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span><span class="sxs-lookup"><span data-stu-id="06f85-114">When an item is put away, if the item does not have a default bin assigned, the bin where the item is put away is assigned as the default.</span></span>  

## <a name="to-change-the-default-bin-for-an-item"></a><span data-ttu-id="06f85-115">To change the default bin for an item</span><span class="sxs-lookup"><span data-stu-id="06f85-115">To change the default bin for an item</span></span>  
<span data-ttu-id="06f85-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span><span class="sxs-lookup"><span data-stu-id="06f85-116">You may need to change the default bin assignment for an item or assign a default bin to a new item.</span></span>    
1.  <span data-ttu-id="06f85-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="06f85-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bin Contents** , and then choose the related link.</span></span>  
2.  <span data-ttu-id="06f85-118">In the **Location Filter** field, select the appropriate location code.</span><span class="sxs-lookup"><span data-stu-id="06f85-118">In the **Location Filter** field, select the appropriate location code.</span></span>  
3.  <span data-ttu-id="06f85-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="06f85-119">Find the current default bin content entry for the item and clear the **Default Bin** check box.</span></span>  
4.  <span data-ttu-id="06f85-120">Find the bin content line for the bin that you would like as the new default bin.</span><span class="sxs-lookup"><span data-stu-id="06f85-120">Find the bin content line for the bin that you would like as the new default bin.</span></span> <span data-ttu-id="06f85-121">Select the **Default Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="06f85-121">Select the **Default Bin** check box.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="06f85-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span><span class="sxs-lookup"><span data-stu-id="06f85-122">When an item is put away for the first time, and the item does not have a default bin assigned, the system will assign the bin where the item is put away as the default bin for the item.</span></span>  

## <a name="see-also"></a><span data-ttu-id="06f85-123">See Also</span><span class="sxs-lookup"><span data-stu-id="06f85-123">See Also</span></span>  
[<span data-ttu-id="06f85-124">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="06f85-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="06f85-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="06f85-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="06f85-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="06f85-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="06f85-127">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="06f85-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="06f85-128">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="06f85-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="06f85-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="06f85-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
