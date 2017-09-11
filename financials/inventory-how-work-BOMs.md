---
title: Work with Bills of Material to Manage Components| Microsoft Docs
description: You create an assembly BOM to specify the components or resources required to put together the item that the assembly BOM represents, and you can view the components of an assembly item.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 05/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: e6aef60ee5b206b0ae978f72b92e6f8778290509
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-work-with-bills-of-material"></a><span data-ttu-id="8bd30-103">How to: Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="8bd30-103">How to: Work with Bills of Material</span></span>
> [!NOTE]  
>   <span data-ttu-id="8bd30-104">The current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] only contains the first part of the Assembly Management feature.</span><span class="sxs-lookup"><span data-stu-id="8bd30-104">The current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] only contains the first part of the Assembly Management feature.</span></span> <span data-ttu-id="8bd30-105">For now, you can only create assembly BOMs and then handle the related parent items as normal inventory items.</span><span class="sxs-lookup"><span data-stu-id="8bd30-105">For now, you can only create assembly BOMs and then handle the related parent items as normal inventory items.</span></span> <span data-ttu-id="8bd30-106">In a future update, you can manage the actual assembly of items from components, either in assemble-to-stock or assemble-to-order flows, and you can sell components as kits.</span><span class="sxs-lookup"><span data-stu-id="8bd30-106">In a future update, you can manage the actual assembly of items from components, either in assemble-to-stock or assemble-to-order flows, and you can sell components as kits.</span></span>

<span data-ttu-id="8bd30-107">You use bills of materials (BOMs) to structure parent items that you sell as kits consisting of the parent's components or that you assemble to order or to stock.</span><span class="sxs-lookup"><span data-stu-id="8bd30-107">You use bills of materials (BOMs) to structure parent items that you sell as kits consisting of the parent's components or that you assemble to order or to stock.</span></span>

<span data-ttu-id="8bd30-108">In [!INCLUDE[d365fin](includes/d365fin_md.md)], a bill of materials is referred to as an "assembly BOM".</span><span class="sxs-lookup"><span data-stu-id="8bd30-108">In [!INCLUDE[d365fin](includes/d365fin_md.md)], a bill of materials is referred to as an "assembly BOM".</span></span> <span data-ttu-id="8bd30-109">Assembly BOMs specify which components are contained in parent items.</span><span class="sxs-lookup"><span data-stu-id="8bd30-109">Assembly BOMs specify which components are contained in parent items.</span></span> <span data-ttu-id="8bd30-110">In this documentation, a parent item is referred to as an "assembly item".</span><span class="sxs-lookup"><span data-stu-id="8bd30-110">In this documentation, a parent item is referred to as an "assembly item".</span></span>

<span data-ttu-id="8bd30-111">Assembly BOMs usually contain items but can also contain one or more resources that are required to put the assembly item together.</span><span class="sxs-lookup"><span data-stu-id="8bd30-111">Assembly BOMs usually contain items but can also contain one or more resources that are required to put the assembly item together.</span></span>

<span data-ttu-id="8bd30-112">Assembly BOMs can have multiple levels, which means that a component on the assembly BOM can be an assembly item itself.</span><span class="sxs-lookup"><span data-stu-id="8bd30-112">Assembly BOMs can have multiple levels, which means that a component on the assembly BOM can be an assembly item itself.</span></span> <span data-ttu-id="8bd30-113">In that case, the **Assembly BOM** field on the assembly BOM line contains **Yes**.</span><span class="sxs-lookup"><span data-stu-id="8bd30-113">In that case, the **Assembly BOM** field on the assembly BOM line contains **Yes**.</span></span>

<span data-ttu-id="8bd30-114">Special requirements apply to items on assembly BOMs with regards to availability.</span><span class="sxs-lookup"><span data-stu-id="8bd30-114">Special requirements apply to items on assembly BOMs with regards to availability.</span></span> <span data-ttu-id="8bd30-115">For more information, see the "To see the availability of an item by its use in assembly BOMs" section in [How to: View the Availability of Items](inventory-how-availability-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8bd30-115">For more information, see the "To see the availability of an item by its use in assembly BOMs" section in [How to: View the Availability of Items](inventory-how-availability-overview.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="8bd30-116">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="8bd30-116">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="8bd30-117">For more information, see [Customizing Your Financials Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="8bd30-117">For more information, see [Customizing Your Financials Experience](ui-experiences.md).</span></span>

## <a name="to-create-an-assembly-bom"></a><span data-ttu-id="8bd30-118">To create an assembly BOM</span><span class="sxs-lookup"><span data-stu-id="8bd30-118">To create an assembly BOM</span></span>
<span data-ttu-id="8bd30-119">To define a parent item that consists of other items, and potentially of resources required to put the parent together, you must create an assembly BOM.</span><span class="sxs-lookup"><span data-stu-id="8bd30-119">To define a parent item that consists of other items, and potentially of resources required to put the parent together, you must create an assembly BOM.</span></span>  

<span data-ttu-id="8bd30-120">There are two parts to creating an assembly BOM:</span><span class="sxs-lookup"><span data-stu-id="8bd30-120">There are two parts to creating an assembly BOM:</span></span>
- <span data-ttu-id="8bd30-121">Setting up a new item</span><span class="sxs-lookup"><span data-stu-id="8bd30-121">Setting up a new item</span></span>
- <span data-ttu-id="8bd30-122">Defining the BOM structure of the assembly item.</span><span class="sxs-lookup"><span data-stu-id="8bd30-122">Defining the BOM structure of the assembly item.</span></span>

1. <span data-ttu-id="8bd30-123">Set up a new item.</span><span class="sxs-lookup"><span data-stu-id="8bd30-123">Set up a new item.</span></span> <span data-ttu-id="8bd30-124">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="8bd30-124">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span></span>

    <span data-ttu-id="8bd30-125">Proceed to enter components or resources on the assembly BOM.</span><span class="sxs-lookup"><span data-stu-id="8bd30-125">Proceed to enter components or resources on the assembly BOM.</span></span>  
2. <span data-ttu-id="8bd30-126">In the **Item Card** window for an assembly item, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span><span class="sxs-lookup"><span data-stu-id="8bd30-126">In the **Item Card** window for an assembly item, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
3. <span data-ttu-id="8bd30-127">In the **Assembly BOM** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="8bd30-127">In the **Assembly BOM** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-the-components-of-an-assembly-item-indented-according-to-the-bom-structure"></a><span data-ttu-id="8bd30-128">To view the components of an assembly item indented according to the BOM structure</span><span class="sxs-lookup"><span data-stu-id="8bd30-128">To view the components of an assembly item indented according to the BOM structure</span></span>
<span data-ttu-id="8bd30-129">From the **Assembly BOM** window, you can open a separate window that shows the components and any resources indented according to their BOM position under the assembly item.</span><span class="sxs-lookup"><span data-stu-id="8bd30-129">From the **Assembly BOM** window, you can open a separate window that shows the components and any resources indented according to their BOM position under the assembly item.</span></span>

1. <span data-ttu-id="8bd30-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8bd30-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="8bd30-131">Open the card for an assembly item.</span><span class="sxs-lookup"><span data-stu-id="8bd30-131">Open the card for an assembly item.</span></span> <span data-ttu-id="8bd30-132">(The **Assembly BOM** field in the **Items** window contains **Yes**.)</span><span class="sxs-lookup"><span data-stu-id="8bd30-132">(The **Assembly BOM** field in the **Items** window contains **Yes**.)</span></span>
3. <span data-ttu-id="8bd30-133">In the **Item Card** window, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span><span class="sxs-lookup"><span data-stu-id="8bd30-133">In the **Item Card** window, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
4. <span data-ttu-id="8bd30-134">In the **Assembly BOM** window, choose the **Show BOM** action.</span><span class="sxs-lookup"><span data-stu-id="8bd30-134">In the **Assembly BOM** window, choose the **Show BOM** action.</span></span>

## <a name="to-buy-sell-or-transfer-assembly-items"></a><span data-ttu-id="8bd30-135">To buy, sell, or transfer assembly items</span><span class="sxs-lookup"><span data-stu-id="8bd30-135">To buy, sell, or transfer assembly items</span></span>
<span data-ttu-id="8bd30-136">Because the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] only contains the ability to define and assign assembly BOMs to items, you can handle assembly items on document lines as normal items only.</span><span class="sxs-lookup"><span data-stu-id="8bd30-136">Because the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] only contains the ability to define and assign assembly BOMs to items, you can handle assembly items on document lines as normal items only.</span></span>

<span data-ttu-id="8bd30-137">**Caution**: The inventory quantity of BOM components will not be adjusted if you do so.</span><span class="sxs-lookup"><span data-stu-id="8bd30-137">**Caution**: The inventory quantity of BOM components will not be adjusted if you do so.</span></span>

## <a name="see-also"></a><span data-ttu-id="8bd30-138">See Also</span><span class="sxs-lookup"><span data-stu-id="8bd30-138">See Also</span></span>
[<span data-ttu-id="8bd30-139">How to: Register New Items</span><span class="sxs-lookup"><span data-stu-id="8bd30-139">How to: Register New Items</span></span>](inventory-how-register-new-items.md)  
<span data-ttu-id="8bd30-140">[How to: View the Availability of Items](inventory-how-availability-overview.md)   </span><span class="sxs-lookup"><span data-stu-id="8bd30-140">[How to: View the Availability of Items](inventory-how-availability-overview.md)   </span></span>  
[<span data-ttu-id="8bd30-141">Inventory</span><span class="sxs-lookup"><span data-stu-id="8bd30-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="8bd30-142">[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8bd30-142">[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>

