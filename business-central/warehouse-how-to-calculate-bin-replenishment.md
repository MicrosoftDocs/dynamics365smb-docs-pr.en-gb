---
title: How to Calculate Bin Replenishment | Microsoft Docs
description: When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: ac684ffdb7bc6e9ddefa218e27babb7c9c5bb3ea
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="calculate-bin-replenishment"></a><span data-ttu-id="14622-103">Calculate Bin Replenishment</span><span class="sxs-lookup"><span data-stu-id="14622-103">Calculate Bin Replenishment</span></span>
<span data-ttu-id="14622-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span><span class="sxs-lookup"><span data-stu-id="14622-104">When the location is set up to use directed put-away and pick, priorities of the put-away template for the location are taken into account when putting receipts away.</span></span> <span data-ttu-id="14622-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span><span class="sxs-lookup"><span data-stu-id="14622-105">Priorities include the minimum and maximum quantities of bin content that have been fixed for a particular bin, and the bin rankings.</span></span> <span data-ttu-id="14622-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span><span class="sxs-lookup"><span data-stu-id="14622-106">Therefore, if items are arriving at a steady pace, the most-used pick bins will be filled up as they are emptied.</span></span>  

<span data-ttu-id="14622-107">But inventory does not always arrive in a steady trickle.</span><span class="sxs-lookup"><span data-stu-id="14622-107">But inventory does not always arrive in a steady trickle.</span></span> <span data-ttu-id="14622-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span><span class="sxs-lookup"><span data-stu-id="14622-108">Sometimes, items are purchased in large quantities so that the company can obtain a rebate, or your production unit might produce a lot of one item to achieve a low unit cost.</span></span> <span data-ttu-id="14622-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span><span class="sxs-lookup"><span data-stu-id="14622-109">Then items will not be received in the warehouse again for some time, and the warehouse needs to periodically move items to pick bins from bulk storage areas.</span></span>  

<span data-ttu-id="14622-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span><span class="sxs-lookup"><span data-stu-id="14622-110">It could also be that the warehouse is expecting new stock to arrive soon and wants to empty the bulk storage area of items before the new merchandise arrives.</span></span>  

<span data-ttu-id="14622-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span><span class="sxs-lookup"><span data-stu-id="14622-111">Finally, if you have defined your bulk storage bins with a bin type action **Put Away** only, that is, the bin type does not have the **Pick** action selected, you must always keep your pick bins replenished, since Put Away-type bins are not suggested for a pick of inventory.</span></span>  

## <a name="to-replenish-pick-bins"></a><span data-ttu-id="14622-112">To replenish pick bins</span><span class="sxs-lookup"><span data-stu-id="14622-112">To replenish pick bins</span></span>  
1.  <span data-ttu-id="14622-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="14622-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="14622-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span><span class="sxs-lookup"><span data-stu-id="14622-114">Choose the **Calculate Bin Replenishment** action to open the report request page.</span></span>  
3.  <span data-ttu-id="14622-115">Fill in the batch job request window to limit the scope of the replenishment suggestions that will be calculated.</span><span class="sxs-lookup"><span data-stu-id="14622-115">Fill in the batch job request window to limit the scope of the replenishment suggestions that will be calculated.</span></span> <span data-ttu-id="14622-116">For example, you might be concerned with particular items, zones, or bins.</span><span class="sxs-lookup"><span data-stu-id="14622-116">For example, you might be concerned with particular items, zones, or bins.</span></span>  
4.  <span data-ttu-id="14622-117">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="14622-117">Choose the **OK** button.</span></span> <span data-ttu-id="14622-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span><span class="sxs-lookup"><span data-stu-id="14622-118">Lines are created for the replenishment movements that need to be performed according to the rules that have been set up for the bins and bin contents, that is, items in bins.</span></span>  
5.  <span data-ttu-id="14622-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span><span class="sxs-lookup"><span data-stu-id="14622-119">If you want to perform all the suggested replenishments, choose the **Create Movement** action.</span></span> <span data-ttu-id="14622-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span><span class="sxs-lookup"><span data-stu-id="14622-120">Employees can now find instructions in the **Movements** menu item, carry them out and register them.</span></span>  
6.  <span data-ttu-id="14622-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span><span class="sxs-lookup"><span data-stu-id="14622-121">If you only want some of the suggestions to be performed, delete the lines that are less important and then create a movement.</span></span>  

<span data-ttu-id="14622-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span><span class="sxs-lookup"><span data-stu-id="14622-122">The next time you calculate bin replenishment, the suggestions that you have deleted will be recreated, if they are still valid at that time.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="14622-123">If the following conditions are met for an item:</span><span class="sxs-lookup"><span data-stu-id="14622-123">If the following conditions are met for an item:</span></span>  
>   
>  -   <span data-ttu-id="14622-124">The item has an expiration date, and</span><span class="sxs-lookup"><span data-stu-id="14622-124">The item has an expiration date, and</span></span>  
> -   <span data-ttu-id="14622-125">The **Pick According to FEFO** field on the location card is selected, and</span><span class="sxs-lookup"><span data-stu-id="14622-125">The **Pick According to FEFO** field on the location card is selected, and</span></span>  
> -   <span data-ttu-id="14622-126">You use the **Calculate Bin Replenishment** functionality</span><span class="sxs-lookup"><span data-stu-id="14622-126">You use the **Calculate Bin Replenishment** functionality</span></span>  
>   
>  <span data-ttu-id="14622-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span><span class="sxs-lookup"><span data-stu-id="14622-127">then the **From Zone** and **From Bin** fields will be blank because the algorithm to calculate from where to move the items is triggered only when you activate the **Create Movement** function.</span></span>  

## <a name="see-also"></a><span data-ttu-id="14622-128">See Also</span><span class="sxs-lookup"><span data-stu-id="14622-128">See Also</span></span>  
[<span data-ttu-id="14622-129">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="14622-129">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="14622-130">Picking by FEFO</span><span class="sxs-lookup"><span data-stu-id="14622-130">Picking by FEFO</span></span>](warehouse-picking-by-fefo.md)  
[<span data-ttu-id="14622-131">Inventory</span><span class="sxs-lookup"><span data-stu-id="14622-131">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="14622-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="14622-132">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="14622-133">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="14622-133">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="14622-134">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="14622-134">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="14622-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="14622-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

