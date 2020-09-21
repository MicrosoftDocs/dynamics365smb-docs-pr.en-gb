---
title: Organise Items in Categories| Microsoft Docs
description: To help you search for and find items, you can assign item attributes and organise items in categories.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: category, search, attribute, facet
ms.date: 06/22/2020
ms.author: edupont
ms.openlocfilehash: 9d474f4e4b8381795405e11b1c3513cbf8a7ed90
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3777598"
---
# <a name="categorize-items"></a><span data-ttu-id="0c138-103">Categorise Items</span><span class="sxs-lookup"><span data-stu-id="0c138-103">Categorize Items</span></span>

<span data-ttu-id="0c138-104">To maintain an overview of your items and to help you sort and find items, it is useful to organise your items in item categories.</span><span class="sxs-lookup"><span data-stu-id="0c138-104">To maintain an overview of your items and to help you sort and find items, it is useful to organize your items in item categories.</span></span>

<span data-ttu-id="0c138-105">To find items by characteristics, you can assign item attributes to items and also to item categories.</span><span class="sxs-lookup"><span data-stu-id="0c138-105">To find items by characteristics, you can assign item attributes to items and also to item categories.</span></span> <span data-ttu-id="0c138-106">For more information, see [Work with Item Attributes](inventory-how-work-item-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="0c138-106">For more information, see [Work with Item Attributes](inventory-how-work-item-attributes.md).</span></span>
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4j4mo?rel=0]

## <a name="to-create-an-item-category"></a><span data-ttu-id="0c138-107">To create an item category</span><span class="sxs-lookup"><span data-stu-id="0c138-107">To create an item category</span></span>
1. <span data-ttu-id="0c138-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Categories**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c138-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Categories**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c138-109">On the **Item Categories** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="0c138-109">On the **Item Categories** page, choose the **New** action.</span></span>
3. <span data-ttu-id="0c138-110">On the **Item Category Card** page, on the **General** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c138-110">On the **Item Category Card** page, on the **General** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="0c138-111">On the **Attributes** FastTab, specify any item attributes for the item category.</span><span class="sxs-lookup"><span data-stu-id="0c138-111">On the **Attributes** FastTab, specify any item attributes for the item category.</span></span> <span data-ttu-id="0c138-112">For more information, see [To assign item attributes to item categories](inventory-how-work-item-attributes.md#to-assign-item-attributes-to-item-categories).</span><span class="sxs-lookup"><span data-stu-id="0c138-112">For more information, see [To assign item attributes to item categories](inventory-how-work-item-attributes.md#to-assign-item-attributes-to-item-categories).</span></span>

> [!NOTE]  
> <span data-ttu-id="0c138-113">If the item category has a parent item category, as indicated by the **Parent Category** field, then any item attributes that are assigned to that parent item category are prefilled on the **Attributes** FastTab.</span><span class="sxs-lookup"><span data-stu-id="0c138-113">If the item category has a parent item category, as indicated by the **Parent Category** field, then any item attributes that are assigned to that parent item category are prefilled on the **Attributes** FastTab.</span></span>

> [!NOTE]  
> <span data-ttu-id="0c138-114">Item attributes that you assign to an item category will automatically apply to the item that the item category is assigned to.</span><span class="sxs-lookup"><span data-stu-id="0c138-114">Item attributes that you assign to an item category will automatically apply to the item that the item category is assigned to.</span></span>

## <a name="to-assign-an-item-category-to-an-item"></a><span data-ttu-id="0c138-115">To assign an item category to an item</span><span class="sxs-lookup"><span data-stu-id="0c138-115">To assign an item category to an item</span></span>

1. <span data-ttu-id="0c138-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c138-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c138-117">Open the card for the item that you want to assign to an item category.</span><span class="sxs-lookup"><span data-stu-id="0c138-117">Open the card for the item that you want to assign to an item category.</span></span>
3. <span data-ttu-id="0c138-118">Choose the lookup button in the **Item Category Code** field and select an existing item category.</span><span class="sxs-lookup"><span data-stu-id="0c138-118">Choose the lookup button in the **Item Category Code** field and select an existing item category.</span></span> <span data-ttu-id="0c138-119">Alternatively, choose the **New** action to first create a new item category as explained in [To create an item category](inventory-how-categorize-items.md#to-create-an-item-category).</span><span class="sxs-lookup"><span data-stu-id="0c138-119">Alternatively, choose the **New** action to first create a new item category as explained in [To create an item category](inventory-how-categorize-items.md#to-create-an-item-category).</span></span>

## <a name="categories-attributes-and-variants"></a><span data-ttu-id="0c138-120">Categories, attributes, and variants</span><span class="sxs-lookup"><span data-stu-id="0c138-120">Categories, attributes, and variants</span></span>

[!INCLUDE[inventory_variant](includes/inventory_variant.md)]

## <a name="see-also"></a><span data-ttu-id="0c138-121">See Also</span><span class="sxs-lookup"><span data-stu-id="0c138-121">See Also</span></span>

[<span data-ttu-id="0c138-122">Work with Item Attributes</span><span class="sxs-lookup"><span data-stu-id="0c138-122">Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)  
[<span data-ttu-id="0c138-123">Register New Items</span><span class="sxs-lookup"><span data-stu-id="0c138-123">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="0c138-124">Inventory</span><span class="sxs-lookup"><span data-stu-id="0c138-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="0c138-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0c138-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
