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
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: ca9f31b737fbd81bd1abba2a942301d0c9c919a6
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1244052"
---
# <a name="use-item-cross-references"></a><span data-ttu-id="40ecc-104">Use Item Cross References</span><span class="sxs-lookup"><span data-stu-id="40ecc-104">Use Item Cross References</span></span>
<span data-ttu-id="40ecc-105">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="40ecc-105">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span></span> <span data-ttu-id="40ecc-106">field.</span><span class="sxs-lookup"><span data-stu-id="40ecc-106">field.</span></span> <span data-ttu-id="40ecc-107">The same functionality applies for customer item numbers on sales documents.</span><span class="sxs-lookup"><span data-stu-id="40ecc-107">The same functionality applies for customer item numbers on sales documents.</span></span>

<span data-ttu-id="40ecc-108">The following procedures describe how to use item cross references on the purchase side.</span><span class="sxs-lookup"><span data-stu-id="40ecc-108">The following procedures describe how to use item cross references on the purchase side.</span></span> <span data-ttu-id="40ecc-109">The steps are similar for the sales side.</span><span class="sxs-lookup"><span data-stu-id="40ecc-109">The steps are similar for the sales side.</span></span>

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a><span data-ttu-id="40ecc-110">To set up an item cross reference to a vendor's item description</span><span class="sxs-lookup"><span data-stu-id="40ecc-110">To set up an item cross reference to a vendor's item description</span></span>
1. <span data-ttu-id="40ecc-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="40ecc-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="40ecc-112">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span><span class="sxs-lookup"><span data-stu-id="40ecc-112">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span></span>
3. <span data-ttu-id="40ecc-113">Choose the **Cross References** action.</span><span class="sxs-lookup"><span data-stu-id="40ecc-113">Choose the **Cross References** action.</span></span>
4. <span data-ttu-id="40ecc-114">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="40ecc-114">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="40ecc-115">.</span><span class="sxs-lookup"><span data-stu-id="40ecc-115">.</span></span>

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a><span data-ttu-id="40ecc-116">To enter a vendor's item description on a purchase order</span><span class="sxs-lookup"><span data-stu-id="40ecc-116">To enter a vendor's item description on a purchase order</span></span>
1. <span data-ttu-id="40ecc-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="40ecc-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="40ecc-118">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="40ecc-118">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span></span>
3. <span data-ttu-id="40ecc-119">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="40ecc-119">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span></span>
4. <span data-ttu-id="40ecc-120">In the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="40ecc-120">In the **Cross-Reference No.**</span></span> <span data-ttu-id="40ecc-121">field, select the item cross reference that you have created, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="40ecc-121">field, select the item cross reference that you have created, and then choose the **OK** button.</span></span>

<span data-ttu-id="40ecc-122">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span><span class="sxs-lookup"><span data-stu-id="40ecc-122">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="40ecc-123">See Also</span><span class="sxs-lookup"><span data-stu-id="40ecc-123">See Also</span></span>
[<span data-ttu-id="40ecc-124">Register New Items</span><span class="sxs-lookup"><span data-stu-id="40ecc-124">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="40ecc-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="40ecc-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="40ecc-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="40ecc-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
