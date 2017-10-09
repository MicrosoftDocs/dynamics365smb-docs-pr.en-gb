---
title: How to Calculate Bin Replenishment | Microsoft Docs
description: When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: a683d2f88f8c30d457d44facd21b0068688ad05a
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-calculate-bin-replenishment"></a><span data-ttu-id="22475-103">How to: Calculate Bin Replenishment</span><span class="sxs-lookup"><span data-stu-id="22475-103">How to: Calculate Bin Replenishment</span></span>
<span data-ttu-id="22475-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span><span class="sxs-lookup"><span data-stu-id="22475-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span></span> <span data-ttu-id="22475-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span><span class="sxs-lookup"><span data-stu-id="22475-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span></span> <span data-ttu-id="22475-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span><span class="sxs-lookup"><span data-stu-id="22475-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span></span>  

<span data-ttu-id="22475-107">But inventory does not always arrive in a steady trickle.</span><span class="sxs-lookup"><span data-stu-id="22475-107">But inventory does not always arrive in a steady trickle.</span></span> <span data-ttu-id="22475-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span><span class="sxs-lookup"><span data-stu-id="22475-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span></span> <span data-ttu-id="22475-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span><span class="sxs-lookup"><span data-stu-id="22475-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span></span>  

<span data-ttu-id="22475-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span><span class="sxs-lookup"><span data-stu-id="22475-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span></span>  

<span data-ttu-id="22475-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span><span class="sxs-lookup"><span data-stu-id="22475-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span></span>  

## <a name="to-replenish-pick-bins"></a><span data-ttu-id="22475-112">To replenish pick bins</span><span class="sxs-lookup"><span data-stu-id="22475-112">To replenish pick bins</span></span>  
1.  <span data-ttu-id="22475-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="22475-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="22475-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span><span class="sxs-lookup"><span data-stu-id="22475-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span></span>  
3.  <span data-ttu-id="22475-115">Fill in the batch job request window to limit the scope of the replenishment suggestions that will be calculated.</span><span class="sxs-lookup"><span data-stu-id="22475-115">Fill in the batch job request window to limit the scope of the replenishment suggestions that will be calculated.</span></span> <span data-ttu-id="22475-116">For example, you might be concerned with particular items, zones, or bins.</span><span class="sxs-lookup"><span data-stu-id="22475-116">For example, you might be concerned with particular items, zones, or bins.</span></span>  
4.  <span data-ttu-id="22475-117">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="22475-117">Choose the **OK** button.</span></span> <span data-ttu-id="22475-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span><span class="sxs-lookup"><span data-stu-id="22475-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span></span>  
5.  <span data-ttu-id="22475-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span><span class="sxs-lookup"><span data-stu-id="22475-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span></span> <span data-ttu-id="22475-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span><span class="sxs-lookup"><span data-stu-id="22475-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span></span>  
6.  <span data-ttu-id="22475-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span><span class="sxs-lookup"><span data-stu-id="22475-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span></span>  

<span data-ttu-id="22475-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span><span class="sxs-lookup"><span data-stu-id="22475-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="22475-123">If the following conditions are met for an item:</span><span class="sxs-lookup"><span data-stu-id="22475-123">If the following conditions are met for an item:</span></span>  
>   
>  -   <span data-ttu-id="22475-124">The item has an expiration date, and</span><span class="sxs-lookup"><span data-stu-id="22475-124">The item has an expiration date, and</span></span>  
> -   <span data-ttu-id="22475-125">The **Pick According to FEFO** field on the location card is selected, and</span><span class="sxs-lookup"><span data-stu-id="22475-125">The **Pick According to FEFO** field on the location card is selected, and</span></span>  
> -   <span data-ttu-id="22475-126">You use the **Calculate Bin Replenishment** functionality</span><span class="sxs-lookup"><span data-stu-id="22475-126">You use the **Calculate Bin Replenishment** functionality</span></span>  
>   
>  <span data-ttu-id="22475-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span><span class="sxs-lookup"><span data-stu-id="22475-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span></span>  

## <a name="see-also"></a><span data-ttu-id="22475-128">See Also</span><span class="sxs-lookup"><span data-stu-id="22475-128">See Also</span></span>  
[<span data-ttu-id="22475-129">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="22475-129">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="22475-130">Picking by FEFO</span><span class="sxs-lookup"><span data-stu-id="22475-130">Picking by FEFO</span></span>](warehouse-picking-by-fefo.md)  
[<span data-ttu-id="22475-131">Inventory</span><span class="sxs-lookup"><span data-stu-id="22475-131">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="22475-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="22475-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="22475-133">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="22475-133">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="22475-134">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="22475-134">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="22475-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="22475-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

