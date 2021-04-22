---
title: Design Details - Item Tracking in the Warehouse | Microsoft Docs
description: Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers. However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fdd76b21254fc40d2d02332f29c2e002900fdc8b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775147"
---
# <a name="design-details-item-tracking-in-the-warehouse"></a><span data-ttu-id="309c0-104">Design Details: Item Tracking in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="309c0-104">Design Details: Item Tracking in the Warehouse</span></span>
<span data-ttu-id="309c0-105">Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers.</span><span class="sxs-lookup"><span data-stu-id="309c0-105">Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers.</span></span>  

<span data-ttu-id="309c0-106">However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.</span><span class="sxs-lookup"><span data-stu-id="309c0-106">However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.</span></span> <span data-ttu-id="309c0-107">Because reservations and item tracking numbers can be handled only at the location level, not at the bin and zone level, the **Item Tracking Lines** page cannot be opened from warehouse activity documents.</span><span class="sxs-lookup"><span data-stu-id="309c0-107">Because reservations and item tracking numbers can be handled only at the location level, not at the bin and zone level, the **Item Tracking Lines** page cannot be opened from warehouse activity documents.</span></span> <span data-ttu-id="309c0-108">The same applies to the **Reservation** page.</span><span class="sxs-lookup"><span data-stu-id="309c0-108">The same applies to the **Reservation** page.</span></span>  

<span data-ttu-id="309c0-109">After a serial or lot number has been added to an item at a warehouse location, it can be moved and reclassified freely within the warehouse by using an independent item tracking structure that is unrelated to the reservation system.</span><span class="sxs-lookup"><span data-stu-id="309c0-109">After a serial or lot number has been added to an item at a warehouse location, it can be moved and reclassified freely within the warehouse by using an independent item tracking structure that is unrelated to the reservation system.</span></span> <span data-ttu-id="309c0-110">**Serial No.** and **Lot No.** fields are accessed directly on warehouse document lines.</span><span class="sxs-lookup"><span data-stu-id="309c0-110">**Serial No.** and **Lot No.** fields are accessed directly on warehouse document lines.</span></span> <span data-ttu-id="309c0-111">When the serial or lot number later partakes in outbound posting, it is synchronised with the reservation system as a part of ordinary bin adjustment.</span><span class="sxs-lookup"><span data-stu-id="309c0-111">When the serial or lot number later partakes in outbound posting, it is synchronized with the reservation system as a part of ordinary bin adjustment.</span></span> <span data-ttu-id="309c0-112">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="309c0-112">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="309c0-113">However, the reservation system does take warehouse activities into consideration when it calculates availability.</span><span class="sxs-lookup"><span data-stu-id="309c0-113">However, the reservation system does take warehouse activities into consideration when it calculates availability.</span></span> <span data-ttu-id="309c0-114">For example, items that are allocated to picks, or registered as picked, cannot be reserved.</span><span class="sxs-lookup"><span data-stu-id="309c0-114">For example, items that are allocated to picks, or registered as picked, cannot be reserved.</span></span> <span data-ttu-id="309c0-115">For more information, see [Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="309c0-115">For more information, see [Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="309c0-116">See Also</span><span class="sxs-lookup"><span data-stu-id="309c0-116">See Also</span></span>  
[<span data-ttu-id="309c0-117">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="309c0-117">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)  
[<span data-ttu-id="309c0-118">Design Details: Integration with Inventory</span><span class="sxs-lookup"><span data-stu-id="309c0-118">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)  
[<span data-ttu-id="309c0-119">Design Details: Warehouse Availability</span><span class="sxs-lookup"><span data-stu-id="309c0-119">Design Details: Warehouse Availability</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="309c0-120">Design Details: Item Tracking Design</span><span class="sxs-lookup"><span data-stu-id="309c0-120">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]