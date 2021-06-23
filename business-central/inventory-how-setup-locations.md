---
title: Set Up a Location Card and Define Transfer Routes
description: You create a location card for each place you store stock items, for example, a warehouse or distribution centre, and set up routes to transfer items between locations.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/01/2021
ms.author: edupont
ms.openlocfilehash: 0319f0c64dd46610aa82705257091bd9478ac14f
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184331"
---
# <a name="set-up-locations"></a><span data-ttu-id="a39d8-103">Set Up Locations</span><span class="sxs-lookup"><span data-stu-id="a39d8-103">Set Up Locations</span></span>

<span data-ttu-id="a39d8-104">If you buy, store, or sell items at more than one place or warehouse, you must set up each location with a location card and define transfer routes.</span><span class="sxs-lookup"><span data-stu-id="a39d8-104">If you buy, store, or sell items at more than one place or warehouse, you must set up each location with a location card and define transfer routes.</span></span> <span data-ttu-id="a39d8-105">[!INCLUDE [prod_short](includes/prod_short.md)] uses locations to help keep track of stock in both simpler cases and the more complex warehouse processes.</span><span class="sxs-lookup"><span data-stu-id="a39d8-105">[!INCLUDE [prod_short](includes/prod_short.md)] uses locations to help keep track of inventory in both simpler cases and the more complex warehouse processes.</span></span>

<span data-ttu-id="a39d8-106">You can then create document lines for a specific location, view availability by location, and transfer stock between locations.</span><span class="sxs-lookup"><span data-stu-id="a39d8-106">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="a39d8-107">For more information, see [Manage Stock](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="a39d8-107">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/videoplayer/embed/RE4aQvq?rel=0]

## <a name="location-cards"></a><span data-ttu-id="a39d8-108">Location cards</span><span class="sxs-lookup"><span data-stu-id="a39d8-108">Location cards</span></span>

<span data-ttu-id="a39d8-109">The location card specifies information about a location, such as a warehouse or distribution centre.</span><span class="sxs-lookup"><span data-stu-id="a39d8-109">The location card specifies information about a location, such as a warehouse or distribution center.</span></span> <span data-ttu-id="a39d8-110">You give each location a name and a code that represents the location.</span><span class="sxs-lookup"><span data-stu-id="a39d8-110">You give each location a name and a code that represents the location.</span></span> <span data-ttu-id="a39d8-111">You can then enter the location code in other parts of the program when you want to record transactions for a given location.</span><span class="sxs-lookup"><span data-stu-id="a39d8-111">You can then enter the location code in other parts of the program when you want to record transactions for a given location.</span></span>  

<span data-ttu-id="a39d8-112">You can enter information about bins and warehouse policies for each location.</span><span class="sxs-lookup"><span data-stu-id="a39d8-112">You can enter information about bins and warehouse policies for each location.</span></span> <span data-ttu-id="a39d8-113">Based on the warehouse policies you select, you can use the options on the **Bins** FastTab to define the bins that will be used as default bins when you are performing transactions.</span><span class="sxs-lookup"><span data-stu-id="a39d8-113">Based on the warehouse policies you select, you can use the options on the **Bins** FastTab to define the bins that will be used as default bins when you are performing transactions.</span></span> <span data-ttu-id="a39d8-114">If you are using directed put-away and pick, you use most of the options on the **Bin Policies** FastTab to define how you would like to use the various advanced warehousing features.</span><span class="sxs-lookup"><span data-stu-id="a39d8-114">If you are using directed put-away and pick, you use most of the options on the **Bin Policies** FastTab to define how you would like to use the various advanced warehousing features.</span></span>  

<span data-ttu-id="a39d8-115">Some option fields are greyed and disabled by other settings in the **Location Card** page to restrict unsupported setup combinations.</span><span class="sxs-lookup"><span data-stu-id="a39d8-115">Some option fields are grayed and disabled by other settings in the **Location Card** page to restrict unsupported setup combinations.</span></span>  

<span data-ttu-id="a39d8-116">Choose the **Zones** or **Bins** action to view information about zones and bins that may be defined for the location.</span><span class="sxs-lookup"><span data-stu-id="a39d8-116">Choose the **Zones** or **Bins** action to view information about zones and bins that may be defined for the location.</span></span>

### <a name="to-create-a-location-card"></a><span data-ttu-id="a39d8-117">To create a location card</span><span class="sxs-lookup"><span data-stu-id="a39d8-117">To create a location card</span></span>

1. <span data-ttu-id="a39d8-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a39d8-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="a39d8-119">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="a39d8-119">Choose the **New** action.</span></span>
3. <span data-ttu-id="a39d8-120">On the **Location Card** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a39d8-120">On the **Location Card** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="a39d8-121">Repeat steps 2 and 3 for every location where you want to keep stock.</span><span class="sxs-lookup"><span data-stu-id="a39d8-121">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="a39d8-122">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span><span class="sxs-lookup"><span data-stu-id="a39d8-122">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="a39d8-123">The fields are not relevant for companies that do not require the more complex warehouse functionality.</span><span class="sxs-lookup"><span data-stu-id="a39d8-123">The fields are not relevant for companies that do not require the more complex warehouse functionality.</span></span> <span data-ttu-id="a39d8-124">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="a39d8-124">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

<span data-ttu-id="a39d8-125">You can change the configuration of a location later, but you cannot edit the setup of locations that have item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="a39d8-125">You can change the configuration of a location later, but you cannot edit the setup of locations that have item ledger entries.</span></span>  

<span data-ttu-id="a39d8-126">Next, if you have multiple locations, you can define transfer routes between locations.</span><span class="sxs-lookup"><span data-stu-id="a39d8-126">Next, if you have multiple locations, you can define transfer routes between locations.</span></span>  

### <a name="to-create-a-transfer-route"></a><span data-ttu-id="a39d8-127">To create a transfer route</span><span class="sxs-lookup"><span data-stu-id="a39d8-127">To create a transfer route</span></span>

1. <span data-ttu-id="a39d8-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Routes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a39d8-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="a39d8-129">Alternatively, from any **Location Card** page, choose the **Transfer Routes** action.</span><span class="sxs-lookup"><span data-stu-id="a39d8-129">Alternatively, from any **Location Card** page, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="a39d8-130">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="a39d8-130">Choose the **New** action.</span></span>
4. <span data-ttu-id="a39d8-131">On the **Location Card** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a39d8-131">On the **Location Card** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="a39d8-132">You can now transfer stock items between two locations.</span><span class="sxs-lookup"><span data-stu-id="a39d8-132">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="a39d8-133">For more information, see [Transfer Stock Between Locations](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="a39d8-133">For more information, see [Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="bins"></a><span data-ttu-id="a39d8-134">Bins</span><span class="sxs-lookup"><span data-stu-id="a39d8-134">Bins</span></span>

<span data-ttu-id="a39d8-135">Bins represent the basic warehouse structure and are used to make suggestions about the placement of items.</span><span class="sxs-lookup"><span data-stu-id="a39d8-135">Bins represent the basic warehouse structure and are used to make suggestions about the placement of items.</span></span> <span data-ttu-id="a39d8-136">When you have created your bins, you can define precisely the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.</span><span class="sxs-lookup"><span data-stu-id="a39d8-136">When you have created your bins, you can define precisely the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.</span></span> <span data-ttu-id="a39d8-137">Bins are predominantly used in basic and advance warehouse operations.</span><span class="sxs-lookup"><span data-stu-id="a39d8-137">Bins are predominantly used in basic and advance warehouse operations.</span></span> <span data-ttu-id="a39d8-138">If you manage stock in a more simple setup, you probably do not need bins.</span><span class="sxs-lookup"><span data-stu-id="a39d8-138">If you manage inventory in a more simple setup, you probably do not need bins.</span></span>

<span data-ttu-id="a39d8-139">To use the bin functionality at a location, you first activate the functionality on the **Location** card by selecting the **Bins Mandatory** field on the **Warehouse** FastTab.</span><span class="sxs-lookup"><span data-stu-id="a39d8-139">To use the bin functionality at a location, you first activate the functionality on the **Location** card by selecting the **Bins Mandatory** field on the **Warehouse** FastTab.</span></span> <span data-ttu-id="a39d8-140">Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.</span><span class="sxs-lookup"><span data-stu-id="a39d8-140">Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.</span></span>

> [!NOTE]
> <span data-ttu-id="a39d8-141">Before you can specify bin codes on the location card, the bin codes must be created.</span><span class="sxs-lookup"><span data-stu-id="a39d8-141">Before you can specify bin codes on the location card, the bin codes must be created.</span></span>

<span data-ttu-id="a39d8-142">For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md) and [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).</span><span class="sxs-lookup"><span data-stu-id="a39d8-142">For more information, see [Create Bins](warehouse-how-to-create-individual-bins.md) and [Set Up Bin Types](warehouse-how-to-set-up-bin-types.md).</span></span>  

## <a name="zones"></a><span data-ttu-id="a39d8-143">Zones</span><span class="sxs-lookup"><span data-stu-id="a39d8-143">Zones</span></span>

<span data-ttu-id="a39d8-144">If you want to structure your bins under zones, you can do that in the **Zones** page.</span><span class="sxs-lookup"><span data-stu-id="a39d8-144">If you want to structure your bins under zones, you can do that in the **Zones** page.</span></span>

<span data-ttu-id="a39d8-145">[!INCLUDE [prod_short](includes/prod_short.md)] copies the fields that you set for any particular zone to the bins within it.</span><span class="sxs-lookup"><span data-stu-id="a39d8-145">[!INCLUDE [prod_short](includes/prod_short.md)] copies the fields that you set for any particular zone to the bins within it.</span></span> <span data-ttu-id="a39d8-146">This way, you can assign a zone to a bin or a bin template (bin creation filter), and several other fields are then filled in automatically.</span><span class="sxs-lookup"><span data-stu-id="a39d8-146">This way, you can assign a zone to a bin or a bin template (bin creation filter), and several other fields are then filled in automatically.</span></span>

<span data-ttu-id="a39d8-147">However, you can choose to set up just one zone and to organise your warehouse according to bins alone.</span><span class="sxs-lookup"><span data-stu-id="a39d8-147">However, you can choose to set up just one zone and to organize your warehouse according to bins alone.</span></span> <span data-ttu-id="a39d8-148">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="a39d8-148">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a39d8-149">See Also</span><span class="sxs-lookup"><span data-stu-id="a39d8-149">See Also</span></span>

[<span data-ttu-id="a39d8-150">Manage Stock</span><span class="sxs-lookup"><span data-stu-id="a39d8-150">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="a39d8-151">Transfer Stock Between Locations</span><span class="sxs-lookup"><span data-stu-id="a39d8-151">Transfer Inventory Between Locations</span></span>](inventory-how-transfer-between-locations.md)  
[<span data-ttu-id="a39d8-152">Create Bins</span><span class="sxs-lookup"><span data-stu-id="a39d8-152">Create Bins</span></span>](warehouse-how-to-create-individual-bins.md)  
[<span data-ttu-id="a39d8-153">Set Up Bin Types</span><span class="sxs-lookup"><span data-stu-id="a39d8-153">Set Up Bin Types</span></span>](warehouse-how-to-set-up-bin-types.md)  
[<span data-ttu-id="a39d8-154">Setting Up Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="a39d8-154">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
<span data-ttu-id="a39d8-155">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a39d8-155">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="a39d8-156">Change Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="a39d8-156">Change Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="a39d8-157">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="a39d8-157">General Business Functionality</span></span>](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]