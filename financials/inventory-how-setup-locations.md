---
title: Set Up a Location Card and Define Transfer Routes| Microsoft Docs
description: You create a location card for each place you store inventory items, for example, a warehouse or distribution centre, and set up routes to transfer items between locations.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7d82b1c63bb1da367736f8dd044640b583493af8
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="305b4-103">How to: Set Up Locations</span><span class="sxs-lookup"><span data-stu-id="305b4-103">How to: Set Up Locations</span></span>
<span data-ttu-id="305b4-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span><span class="sxs-lookup"><span data-stu-id="305b4-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="305b4-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span><span class="sxs-lookup"><span data-stu-id="305b4-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="305b4-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="305b4-107">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="305b4-107">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="305b4-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="305b4-109">To create a location card</span><span class="sxs-lookup"><span data-stu-id="305b4-109">To create a location card</span></span>
1. <span data-ttu-id="305b4-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="305b4-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="305b4-111">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="305b4-111">Choose the **New** action.</span></span>
3. <span data-ttu-id="305b4-112">In the **Location Card** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="305b4-112">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="305b4-113">Repeat steps 2 and 3 for every location where you want to keep inventory.</span><span class="sxs-lookup"><span data-stu-id="305b4-113">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="305b4-114">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span><span class="sxs-lookup"><span data-stu-id="305b4-114">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="305b4-115">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-115">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span> 

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="305b4-116">To create a transfer route</span><span class="sxs-lookup"><span data-stu-id="305b4-116">To create a transfer route</span></span>
1. <span data-ttu-id="305b4-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="305b4-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="305b4-118">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span><span class="sxs-lookup"><span data-stu-id="305b4-118">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="305b4-119">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="305b4-119">Choose the **New** action.</span></span>
4. <span data-ttu-id="305b4-120">In the **Location Card** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="305b4-120">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="305b4-121">You can now transfer inventory items between two locations.</span><span class="sxs-lookup"><span data-stu-id="305b4-121">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="305b4-122">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="305b4-122">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="305b4-123">See Also</span><span class="sxs-lookup"><span data-stu-id="305b4-123">See Also</span></span>
[<span data-ttu-id="305b4-124">Manage Inventory</span><span class="sxs-lookup"><span data-stu-id="305b4-124">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="305b4-125">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="305b4-125">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="305b4-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="305b4-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="305b4-127">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="305b4-127">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  
[<span data-ttu-id="305b4-128">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="305b4-128">General Business Functionality</span></span>](ui-across-business-areas.md)

