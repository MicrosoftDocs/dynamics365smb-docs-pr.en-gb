---
title: How to Enable Picking by FEFO | Microsoft Docs
description: First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: f3355fb6ff46e7fa59d5b76aec8e88e675de31f8
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3195976"
---
# <a name="enable-picking-items-by-fefo"></a><span data-ttu-id="5d691-103">Enable Picking Items by FEFO</span><span class="sxs-lookup"><span data-stu-id="5d691-103">Enable Picking Items by FEFO</span></span>
<span data-ttu-id="5d691-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span><span class="sxs-lookup"><span data-stu-id="5d691-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span></span>  

 <span data-ttu-id="5d691-105">This functionality only works when the following criteria are met:</span><span class="sxs-lookup"><span data-stu-id="5d691-105">This functionality only works when the following criteria are met:</span></span>  

-   <span data-ttu-id="5d691-106">The item must have a serial/lot number.</span><span class="sxs-lookup"><span data-stu-id="5d691-106">The item must have a serial/lot number.</span></span>  
-   <span data-ttu-id="5d691-107">On the item’s item tracking code setup, the **SN Specific Tracking** field or the **Lot Specific Tracking** field must be selected.</span><span class="sxs-lookup"><span data-stu-id="5d691-107">On the item’s item tracking code setup, the **SN Specific Tracking** field or the **Lot Specific Tracking** field must be selected.</span></span>  
-   <span data-ttu-id="5d691-108">The item must be posted to inventory with an expiration date.</span><span class="sxs-lookup"><span data-stu-id="5d691-108">The item must be posted to inventory with an expiration date.</span></span>  
-   <span data-ttu-id="5d691-109">On the location card, the **Require Pick** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="5d691-109">On the location card, the **Require Pick** check box must be selected.</span></span>  
-   <span data-ttu-id="5d691-110">On the location card, the **Pick According to FEFO** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="5d691-110">On the location card, the **Pick According to FEFO** check box must be selected.</span></span>  
-   <span data-ttu-id="5d691-111">On the location card, the **Bin Mandatory** check box must be selected.</span><span class="sxs-lookup"><span data-stu-id="5d691-111">On the location card, the **Bin Mandatory** check box must be selected.</span></span>  

 <span data-ttu-id="5d691-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span><span class="sxs-lookup"><span data-stu-id="5d691-112">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span></span>  

> [!NOTE]  
> <span data-ttu-id="5d691-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="5d691-113">If some serial/lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span></span>
<br /><br />
<span data-ttu-id="5d691-114">If two serial/lot-numbered items have the same expiration date, then application selects the item with the lowest serial or lot number.</span><span class="sxs-lookup"><span data-stu-id="5d691-114">If two serial/lot-numbered items have the same expiration date, then application selects the item with the lowest serial or lot number.</span></span>
<br /><br />
<span data-ttu-id="5d691-115">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="5d691-115">When picking serial/lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span></span>  
<br /><br />
<span data-ttu-id="5d691-116">To enable movements according to FEFO, either on the **Inventory Movement** page or the **Movement Worksheet** page, you must leave the **From Bin** field empty.</span><span class="sxs-lookup"><span data-stu-id="5d691-116">To enable movements according to FEFO, either on the **Inventory Movement** page or the **Movement Worksheet** page, you must leave the **From Bin** field empty.</span></span>  
<br /><br />
<span data-ttu-id="5d691-117">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span><span class="sxs-lookup"><span data-stu-id="5d691-117">If the **Strict Expiration Posting** field is selected, then only items that are not expired will be included in the pick.</span></span> <span data-ttu-id="5d691-118">This applies even if you are not using Pick according to FEFO.</span><span class="sxs-lookup"><span data-stu-id="5d691-118">This applies even if you are not using Pick according to FEFO.</span></span>

## <a name="see-also"></a><span data-ttu-id="5d691-119">See Also</span><span class="sxs-lookup"><span data-stu-id="5d691-119">See Also</span></span>  
<span data-ttu-id="5d691-120">[Picking Items](warehouse-pick-items.md) </span><span class="sxs-lookup"><span data-stu-id="5d691-120">[Picking Items](warehouse-pick-items.md) </span></span>  
<span data-ttu-id="5d691-121">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="5d691-121">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
<span data-ttu-id="5d691-122">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="5d691-122">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
[<span data-ttu-id="5d691-123">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="5d691-123">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
[<span data-ttu-id="5d691-124">Inventory</span><span class="sxs-lookup"><span data-stu-id="5d691-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="5d691-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5d691-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
