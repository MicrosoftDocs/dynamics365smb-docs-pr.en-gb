---
title: How to Set Up Locations to Use Bins | Microsoft Docs
description: Bins represent the basic warehouse structure and are used to make suggestions about the placement of items. When you have created your bins, you can define very specifically the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7fa813b2bbaffe72a0f697101f1c10883cf54f2d
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-locations-to-use-bins"></a><span data-ttu-id="a99fb-104">How to: Set Up Locations to Use Bins</span><span class="sxs-lookup"><span data-stu-id="a99fb-104">How to: Set Up Locations to Use Bins</span></span>
<span data-ttu-id="a99fb-105">Bins represent the basic warehouse structure and are used to make suggestions about the placement of items.</span><span class="sxs-lookup"><span data-stu-id="a99fb-105">Bins represent the basic warehouse structure and are used to make suggestions about the placement of items.</span></span> <span data-ttu-id="a99fb-106">When you have created your bins, you can define very specifically the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.</span><span class="sxs-lookup"><span data-stu-id="a99fb-106">When you have created your bins, you can define very specifically the contents that you want to place in each bin, or the bin can function as a floating bin without specified contents.</span></span>  

<span data-ttu-id="a99fb-107">To use the bin functionality at a location, you first activate the functionality on the **Location** card.</span><span class="sxs-lookup"><span data-stu-id="a99fb-107">To use the bin functionality at a location, you first activate the functionality on the **Location** card.</span></span> <span data-ttu-id="a99fb-108">Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.</span><span class="sxs-lookup"><span data-stu-id="a99fb-108">Then you design the item flow at the location by specifying bin codes in setup fields that represent the different flows.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a99fb-109">Before you can specify bin codes on the location card, the bin codes must be created.</span><span class="sxs-lookup"><span data-stu-id="a99fb-109">Before you can specify bin codes on the location card, the bin codes must be created.</span></span> <span data-ttu-id="a99fb-110">For more information, see [How to: Create Bins](warehouse-how-to-create-individual-bins.md).</span><span class="sxs-lookup"><span data-stu-id="a99fb-110">For more information, see [How to: Create Bins](warehouse-how-to-create-individual-bins.md).</span></span>  

## <a name="to-set-up-a-location-to-use-bins"></a><span data-ttu-id="a99fb-111">To set up a location to use bins</span><span class="sxs-lookup"><span data-stu-id="a99fb-111">To set up a location to use bins</span></span>  
1.  <span data-ttu-id="a99fb-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a99fb-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a99fb-113">Select the location where you want to use bins.</span><span class="sxs-lookup"><span data-stu-id="a99fb-113">Select the location where you want to use bins.</span></span>  
3.  <span data-ttu-id="a99fb-114">Choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="a99fb-114">Choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="a99fb-115">On the **Warehouse** FastTab, select the **Bin Mandatory** check box.</span><span class="sxs-lookup"><span data-stu-id="a99fb-115">On the **Warehouse** FastTab, select the **Bin Mandatory** check box.</span></span>  
5.  <span data-ttu-id="a99fb-116">If you are not using directed put-away and pick for the location, fill in the **Default Bin Selection** field with the method the system should use when assigning a default bin to an item.</span><span class="sxs-lookup"><span data-stu-id="a99fb-116">If you are not using directed put-away and pick for the location, fill in the **Default Bin Selection** field with the method the system should use when assigning a default bin to an item.</span></span>  
6.  <span data-ttu-id="a99fb-117">Open the card for the location that you want to set up bins for.</span><span class="sxs-lookup"><span data-stu-id="a99fb-117">Open the card for the location that you want to set up bins for.</span></span>
7.  <span data-ttu-id="a99fb-118">On the **Bins** FastTab, select the bins that you want to use as the default for receipts, shipments, inbound, outbound, and open shop floor bins.</span><span class="sxs-lookup"><span data-stu-id="a99fb-118">On the **Bins** FastTab, select the bins that you want to use as the default for receipts, shipments, inbound, outbound, and open shop floor bins.</span></span>  
8.  <span data-ttu-id="a99fb-119">The bin codes you fill in here will appear automatically on the headers and on the lines of various warehouse documents.</span><span class="sxs-lookup"><span data-stu-id="a99fb-119">The bin codes you fill in here will appear automatically on the headers and on the lines of various warehouse documents.</span></span> <span data-ttu-id="a99fb-120">The default bins define all starting or ending placements of items in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="a99fb-120">The default bins define all starting or ending placements of items in the warehouse.</span></span>  
9.  <span data-ttu-id="a99fb-121">If you are using directed put-away and pick, select a bin for your warehouse adjustments.</span><span class="sxs-lookup"><span data-stu-id="a99fb-121">If you are using directed put-away and pick, select a bin for your warehouse adjustments.</span></span> <span data-ttu-id="a99fb-122">The bin code in the **Adjustment Bin Code** field defines the virtual bin in which to record discrepancies in inventory when you register either observed differences registered in the warehouse item journal, or differences calculated when you register a warehouse physical inventory.</span><span class="sxs-lookup"><span data-stu-id="a99fb-122">The bin code in the **Adjustment Bin Code** field defines the virtual bin in which to record discrepancies in inventory when you register either observed differences registered in the warehouse item journal, or differences calculated when you register a warehouse physical inventory.</span></span>  
10. <span data-ttu-id="a99fb-123">Fill in the fields on the **Bin Policies** FastTab if they are relevant to your warehouse.</span><span class="sxs-lookup"><span data-stu-id="a99fb-123">Fill in the fields on the **Bin Policies** FastTab if they are relevant to your warehouse.</span></span> <span data-ttu-id="a99fb-124">The most important fields are **Bin Capacity Policy**, **Allow Breakbulk**, and **Put-away Template Code** fields.</span><span class="sxs-lookup"><span data-stu-id="a99fb-124">The most important fields are **Bin Capacity Policy**, **Allow Breakbulk**, and **Put-away Template Code** fields.</span></span>  
11. <span data-ttu-id="a99fb-125">On the **Warehouse** FastTab, fill in the **Outbound Whse. Handling Time**, **Inbound Whse. Handling Time**, and the **Base Calendar Code** fields.</span><span class="sxs-lookup"><span data-stu-id="a99fb-125">On the **Warehouse** FastTab, fill in the **Outbound Whse. Handling Time**, **Inbound Whse. Handling Time**, and the **Base Calendar Code** fields.</span></span> <span data-ttu-id="a99fb-126">For more information, see [How to: Set Up Base Calendars](across-how-to-assign-base-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="a99fb-126">For more information, see [How to: Set Up Base Calendars](across-how-to-assign-base-calendars.md).</span></span>

## <a name="filling-the-consumption-bin"></a><span data-ttu-id="a99fb-127">Filling the Consumption Bin</span><span class="sxs-lookup"><span data-stu-id="a99fb-127">Filling the Consumption Bin</span></span>
<span data-ttu-id="a99fb-128">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span><span class="sxs-lookup"><span data-stu-id="a99fb-128">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span></span>

<span data-ttu-id="a99fb-129">![Bin flow chart](media/binflow.png "BinFlow")</span><span class="sxs-lookup"><span data-stu-id="a99fb-129">![Bin flow chart](media/binflow.png "BinFlow")</span></span>  

## <a name="see-also"></a><span data-ttu-id="a99fb-130">See Also</span><span class="sxs-lookup"><span data-stu-id="a99fb-130">See Also</span></span>
[<span data-ttu-id="a99fb-131">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="a99fb-131">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="a99fb-132">Inventory</span><span class="sxs-lookup"><span data-stu-id="a99fb-132">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="a99fb-133">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="a99fb-133">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="a99fb-134">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="a99fb-134">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="a99fb-135">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="a99fb-135">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="a99fb-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a99fb-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

