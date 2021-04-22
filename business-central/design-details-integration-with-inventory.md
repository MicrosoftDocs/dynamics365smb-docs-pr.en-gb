---
title: Design Details - Integration with Inventory | Microsoft Docs
description: The Warehouse Management application area and the Inventory application area interact with one another in physical inventory and in inventory or warehouse adjustment.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 95b0010064fc46213d7565e78319f273400fbac7
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779639"
---
# <a name="design-details-integration-with-inventory"></a><span data-ttu-id="8d572-103">Design Details: Integration with Inventory</span><span class="sxs-lookup"><span data-stu-id="8d572-103">Design Details: Integration with Inventory</span></span>
<span data-ttu-id="8d572-104">The Warehouse Management application area and the Inventory application area interact with one another in physical inventory and in inventory or warehouse adjustment.</span><span class="sxs-lookup"><span data-stu-id="8d572-104">The Warehouse Management application area and the Inventory application area interact with one another in physical inventory and in inventory or warehouse adjustment.</span></span>  
  
## <a name="physical-inventory"></a><span data-ttu-id="8d572-105">Physical Inventory</span><span class="sxs-lookup"><span data-stu-id="8d572-105">Physical Inventory</span></span>  
 <span data-ttu-id="8d572-106">The **Whse. Phys. Inventory Journal** page is used with the **Phys. Inventory Journal** page for all advanced warehouse locations.</span><span class="sxs-lookup"><span data-stu-id="8d572-106">The **Whse. Phys. Inventory Journal** page is used with the **Phys. Inventory Journal** page for all advanced warehouse locations.</span></span> <span data-ttu-id="8d572-107">The inventory on bin level is calculated, and a printed list is provided for the warehouse employee.</span><span class="sxs-lookup"><span data-stu-id="8d572-107">The inventory on bin level is calculated, and a printed list is provided for the warehouse employee.</span></span> <span data-ttu-id="8d572-108">The list shows which items in which bins must be counted.</span><span class="sxs-lookup"><span data-stu-id="8d572-108">The list shows which items in which bins must be counted.</span></span>  
  
 <span data-ttu-id="8d572-109">The warehouse employee enters the counted quantity on the **Whse. Phys. Inventory Journal** page and then posts the journal.</span><span class="sxs-lookup"><span data-stu-id="8d572-109">The warehouse employee enters the counted quantity on the **Whse. Phys. Inventory Journal** page and then posts the journal.</span></span>  
  
 <span data-ttu-id="8d572-110">If the counted quantity is greater than the quantity on the journal line, a movement is posted for this difference from the default adjustment bin to the counted bin.</span><span class="sxs-lookup"><span data-stu-id="8d572-110">If the counted quantity is greater than the quantity on the journal line, a movement is posted for this difference from the default adjustment bin to the counted bin.</span></span> <span data-ttu-id="8d572-111">This increases the quantity in the counted bin and decreases the quantity in the default adjustment bin.</span><span class="sxs-lookup"><span data-stu-id="8d572-111">This increases the quantity in the counted bin and decreases the quantity in the default adjustment bin.</span></span>  
  
 <span data-ttu-id="8d572-112">If the quantity counted is less than the quantity on the journal line, a movement for this difference is posted from the counted bin to the default adjustment bin.</span><span class="sxs-lookup"><span data-stu-id="8d572-112">If the quantity counted is less than the quantity on the journal line, a movement for this difference is posted from the counted bin to the default adjustment bin.</span></span> <span data-ttu-id="8d572-113">This decreases the quantity in the counted bin and increases the quantity in the default adjustment bin.</span><span class="sxs-lookup"><span data-stu-id="8d572-113">This decreases the quantity in the counted bin and increases the quantity in the default adjustment bin.</span></span>  
  
 <span data-ttu-id="8d572-114">In advanced warehouse configurations, the value in the **Quantity (Calculated)** field is retrieved from item ledger entries and the value in the **Quantity (Phys. Inventory)** field is retrieved from warehouse entries, excluding the adjustment bin content.</span><span class="sxs-lookup"><span data-stu-id="8d572-114">In advanced warehouse configurations, the value in the **Quantity (Calculated)** field is retrieved from item ledger entries and the value in the **Quantity (Phys. Inventory)** field is retrieved from warehouse entries, excluding the adjustment bin content.</span></span> <span data-ttu-id="8d572-115">The **Quantity** field specifies the difference between the first two fields, which should be equal to the contents of the adjustment bin.</span><span class="sxs-lookup"><span data-stu-id="8d572-115">The **Quantity** field specifies the difference between the first two fields, which should be equal to the contents of the adjustment bin.</span></span>  
  
 <span data-ttu-id="8d572-116">When you post the physical inventory journal, the inventory and the default adjustment bin are updated.</span><span class="sxs-lookup"><span data-stu-id="8d572-116">When you post the physical inventory journal, the inventory and the default adjustment bin are updated.</span></span>  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a><span data-ttu-id="8d572-117">Warehouse Adjustments to the Item Ledger</span><span class="sxs-lookup"><span data-stu-id="8d572-117">Warehouse Adjustments to the Item Ledger</span></span>  
 <span data-ttu-id="8d572-118">You use the **Item Journal** page and the **Calculate Whse. Adjustment** function to adjust inventory on the item ledger in accordance with an adjustment that has been made to the item quantity in a warehouse bin.</span><span class="sxs-lookup"><span data-stu-id="8d572-118">You use the **Item Journal** page and the **Calculate Whse. Adjustment** function to adjust inventory on the item ledger in accordance with an adjustment that has been made to the item quantity in a warehouse bin.</span></span> <span data-ttu-id="8d572-119">To create a link between the inventory and the warehouse, you must define a default adjustment bin per location.</span><span class="sxs-lookup"><span data-stu-id="8d572-119">To create a link between the inventory and the warehouse, you must define a default adjustment bin per location.</span></span>  
  
 <span data-ttu-id="8d572-120">The default adjustment bin registers items in the warehouse when you post an increase for the inventory.</span><span class="sxs-lookup"><span data-stu-id="8d572-120">The default adjustment bin registers items in the warehouse when you post an increase for the inventory.</span></span> <span data-ttu-id="8d572-121">However, if you post a decrease, the quantity on the default bin is also decreased.</span><span class="sxs-lookup"><span data-stu-id="8d572-121">However, if you post a decrease, the quantity on the default bin is also decreased.</span></span> <span data-ttu-id="8d572-122">In both cases, item ledger entries and warehouse entries are created.</span><span class="sxs-lookup"><span data-stu-id="8d572-122">In both cases, item ledger entries and warehouse entries are created.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="8d572-123">The adjustment bin is not included in the availability calculation.</span><span class="sxs-lookup"><span data-stu-id="8d572-123">The adjustment bin is not included in the availability calculation.</span></span>  
  
 <span data-ttu-id="8d572-124">If you want to adjust the bin content, you can use the warehouse item journal, from which you can enter the item number, zone code, bin code, and quantity that you want to adjust.</span><span class="sxs-lookup"><span data-stu-id="8d572-124">If you want to adjust the bin content, you can use the warehouse item journal, from which you can enter the item number, zone code, bin code, and quantity that you want to adjust.</span></span>  
  
 <span data-ttu-id="8d572-125">If you enter a positive quantity and post the line, then the inventory stored in the bin increases, and the quantity of the default adjustment bin decreases correspondingly.</span><span class="sxs-lookup"><span data-stu-id="8d572-125">If you enter a positive quantity and post the line, then the inventory stored in the bin increases, and the quantity of the default adjustment bin decreases correspondingly.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="8d572-126">See Also</span><span class="sxs-lookup"><span data-stu-id="8d572-126">See Also</span></span>  
 <span data-ttu-id="8d572-127">[Design Details: Warehouse Management](design-details-warehouse-management.md) </span><span class="sxs-lookup"><span data-stu-id="8d572-127">[Design Details: Warehouse Management](design-details-warehouse-management.md) </span></span>  
 [<span data-ttu-id="8d572-128">Design Details: Availability in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="8d572-128">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]