---
title: Use Item Cross-References| Microsoft Docs
description: If you set up a cross-reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.** field.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 2c676af23e5a6e988ab5d89d07118b9ff1cce86b
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3777968"
---
# <a name="use-item-cross-references"></a><span data-ttu-id="2a551-104">Use Item Cross References</span><span class="sxs-lookup"><span data-stu-id="2a551-104">Use Item Cross References</span></span>
<span data-ttu-id="2a551-105">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="2a551-105">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span></span> <span data-ttu-id="2a551-106">field.</span><span class="sxs-lookup"><span data-stu-id="2a551-106">field.</span></span> <span data-ttu-id="2a551-107">The same functionality applies for customer item numbers on sales documents.</span><span class="sxs-lookup"><span data-stu-id="2a551-107">The same functionality applies for customer item numbers on sales documents.</span></span>

<span data-ttu-id="2a551-108">The following procedures describe how to use item cross references on the purchase side.</span><span class="sxs-lookup"><span data-stu-id="2a551-108">The following procedures describe how to use item cross references on the purchase side.</span></span> <span data-ttu-id="2a551-109">The steps are similar for the sales side.</span><span class="sxs-lookup"><span data-stu-id="2a551-109">The steps are similar for the sales side.</span></span>

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a><span data-ttu-id="2a551-110">To set up an item cross reference to a vendor's item description</span><span class="sxs-lookup"><span data-stu-id="2a551-110">To set up an item cross reference to a vendor's item description</span></span>

1. <span data-ttu-id="2a551-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2a551-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="2a551-112">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span><span class="sxs-lookup"><span data-stu-id="2a551-112">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span></span>
3. <span data-ttu-id="2a551-113">Choose the **Cross References** action.</span><span class="sxs-lookup"><span data-stu-id="2a551-113">Choose the **Cross References** action.</span></span>

     <span data-ttu-id="2a551-114">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Navigate**, **Item**.</span><span class="sxs-lookup"><span data-stu-id="2a551-114">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Navigate**, **Item**.</span></span>
  
4. <span data-ttu-id="2a551-115">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="2a551-115">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="2a551-116">.</span><span class="sxs-lookup"><span data-stu-id="2a551-116">.</span></span>

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a><span data-ttu-id="2a551-117">To enter a vendor's item description on a purchase order</span><span class="sxs-lookup"><span data-stu-id="2a551-117">To enter a vendor's item description on a purchase order</span></span>

1. <span data-ttu-id="2a551-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2a551-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="2a551-119">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="2a551-119">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span></span>
3. <span data-ttu-id="2a551-120">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="2a551-120">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span></span>
4. <span data-ttu-id="2a551-121">In the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="2a551-121">In the **Cross-Reference No.**</span></span> <span data-ttu-id="2a551-122">field, select the item cross reference that you have created, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="2a551-122">field, select the item cross reference that you have created, and then choose the **OK** button.</span></span>

<span data-ttu-id="2a551-123">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span><span class="sxs-lookup"><span data-stu-id="2a551-123">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="2a551-124">See Also</span><span class="sxs-lookup"><span data-stu-id="2a551-124">See Also</span></span>
[<span data-ttu-id="2a551-125">Register New Items</span><span class="sxs-lookup"><span data-stu-id="2a551-125">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="2a551-126">Inventory</span><span class="sxs-lookup"><span data-stu-id="2a551-126">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="2a551-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2a551-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
