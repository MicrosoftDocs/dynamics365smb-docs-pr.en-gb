---
title: Use Item Cross-References
description: Set up references between the descriptions that you and your vendor use for an item so you can insert the vendor's item description on purchase documents.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item reference, cross reference, inventory
ms.date: 01/12/2021
ms.author: edupont
ms.openlocfilehash: 7d670f6553a1bd70dcc3d97f90436f36c6627c56
ms.sourcegitcommit: 311e86d6abb9b59a5483324d8bb4cd1be7949248
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/15/2021
ms.locfileid: "5013799"
---
# <a name="use-item-cross-references"></a><span data-ttu-id="21b76-103">Use Item Cross References</span><span class="sxs-lookup"><span data-stu-id="21b76-103">Use Item Cross References</span></span>
<span data-ttu-id="21b76-104">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="21b76-104">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span></span> <span data-ttu-id="21b76-105">field.</span><span class="sxs-lookup"><span data-stu-id="21b76-105">field.</span></span> <span data-ttu-id="21b76-106">The same functionality applies for customer item numbers on sales documents.</span><span class="sxs-lookup"><span data-stu-id="21b76-106">The same functionality applies for customer item numbers on sales documents.</span></span>

<span data-ttu-id="21b76-107">The following procedures describe how to use item cross references on the purchase side.</span><span class="sxs-lookup"><span data-stu-id="21b76-107">The following procedures describe how to use item cross references on the purchase side.</span></span> <span data-ttu-id="21b76-108">The steps are similar for the sales side.</span><span class="sxs-lookup"><span data-stu-id="21b76-108">The steps are similar for the sales side.</span></span>

> [!NOTE]
> <span data-ttu-id="21b76-109">It's becoming more common for item identifiers such as GTINs or GUIDs to contain 30 or more characters, which is more than the current feature for item cross references can handle.</span><span class="sxs-lookup"><span data-stu-id="21b76-109">It's becoming more common for item identifiers such as GTINs or GUIDs to contain 30 or more characters, which is more than the current feature for item cross references can handle.</span></span> <span data-ttu-id="21b76-110">If you need to use references that contain more than 30 characters, your administrator can turn on the **Write longer item references** feature on the [Feature Management](https://businesscentral.dynamics.com/?page=2610) page (link requires that you have a [!INCLUDE[prod_short](includes/prod_short.md)] tenant).</span><span class="sxs-lookup"><span data-stu-id="21b76-110">If you need to use references that contain more than 30 characters, your administrator can turn on the **Write longer item references** feature on the [Feature Management](https://businesscentral.dynamics.com/?page=2610) page (link requires that you have a [!INCLUDE[prod_short](includes/prod_short.md)] tenant).</span></span> <span data-ttu-id="21b76-111">How you use references doesn't change, but the names of things like pages and buttons will.</span><span class="sxs-lookup"><span data-stu-id="21b76-111">How you use references doesn't change, but the names of things like pages and buttons will.</span></span> <span data-ttu-id="21b76-112">For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.</span><span class="sxs-lookup"><span data-stu-id="21b76-112">For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.</span></span>

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a><span data-ttu-id="21b76-113">To set up an item cross reference to a vendor's item description</span><span class="sxs-lookup"><span data-stu-id="21b76-113">To set up an item cross reference to a vendor's item description</span></span>

1. <span data-ttu-id="21b76-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="21b76-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="21b76-115">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span><span class="sxs-lookup"><span data-stu-id="21b76-115">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span></span>
3. <span data-ttu-id="21b76-116">Choose the **Cross References** action.</span><span class="sxs-lookup"><span data-stu-id="21b76-116">Choose the **Cross References** action.</span></span>

     <span data-ttu-id="21b76-117">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Related** > **Item**.</span><span class="sxs-lookup"><span data-stu-id="21b76-117">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Related** > **Item**.</span></span>
  
4. <span data-ttu-id="21b76-118">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="21b76-118">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="21b76-119">.</span><span class="sxs-lookup"><span data-stu-id="21b76-119">.</span></span>

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a><span data-ttu-id="21b76-120">To enter a vendor's item description on a purchase order</span><span class="sxs-lookup"><span data-stu-id="21b76-120">To enter a vendor's item description on a purchase order</span></span>

1. <span data-ttu-id="21b76-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="21b76-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="21b76-122">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="21b76-122">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span></span>
3. <span data-ttu-id="21b76-123">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span><span class="sxs-lookup"><span data-stu-id="21b76-123">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span></span>
4. <span data-ttu-id="21b76-124">In the **Cross-Reference No.**</span><span class="sxs-lookup"><span data-stu-id="21b76-124">In the **Cross-Reference No.**</span></span> <span data-ttu-id="21b76-125">field, select the item cross reference that you have created, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="21b76-125">field, select the item cross reference that you have created, and then choose the **OK** button.</span></span>

<span data-ttu-id="21b76-126">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span><span class="sxs-lookup"><span data-stu-id="21b76-126">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="21b76-127">See Also</span><span class="sxs-lookup"><span data-stu-id="21b76-127">See Also</span></span>
[<span data-ttu-id="21b76-128">Register New Items</span><span class="sxs-lookup"><span data-stu-id="21b76-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="21b76-129">Inventory</span><span class="sxs-lookup"><span data-stu-id="21b76-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="21b76-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="21b76-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
