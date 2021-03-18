---
title: How to Set Up Stockkeeping Units | Microsoft Docs
description: You can use stockkeeping units to record information about your items for a specific location or a specific variant code.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 4136cdb7dd89e2998a3fe0e8107dd82b3ab40619
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5393056"
---
# <a name="set-up-stockkeeping-units"></a><span data-ttu-id="886a3-103">Set Up Stockkeeping Units</span><span class="sxs-lookup"><span data-stu-id="886a3-103">Set Up Stockkeeping Units</span></span>
<span data-ttu-id="886a3-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span><span class="sxs-lookup"><span data-stu-id="886a3-104">You can use stockkeeping units to record information about your items for a specific location or a specific variant code.</span></span>  

 <span data-ttu-id="886a3-105">Stockkeeping units are a supplement to item cards.</span><span class="sxs-lookup"><span data-stu-id="886a3-105">Stockkeeping units are a supplement to item cards.</span></span> <span data-ttu-id="886a3-106">They do not replace them, although they are related to them.</span><span class="sxs-lookup"><span data-stu-id="886a3-106">They do not replace them, although they are related to them.</span></span> <span data-ttu-id="886a3-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution centre, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span><span class="sxs-lookup"><span data-stu-id="886a3-107">Stockkeeping units allow you to differentiate information about an item for a specific location, such as a warehouse or distribution center, or a specific variant, such as different shelf numbers and different replenishment information, for the same item.</span></span>  

## <a name="to-set-up-a-stockkeeping-unit"></a><span data-ttu-id="886a3-108">To set up a stockkeeping unit</span><span class="sxs-lookup"><span data-stu-id="886a3-108">To set up a stockkeeping unit</span></span>  

1.  <span data-ttu-id="886a3-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="886a3-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stockkeeping Units**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="886a3-110">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="886a3-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="886a3-111">Fill in the fields on the card.</span><span class="sxs-lookup"><span data-stu-id="886a3-111">Fill in the fields on the card.</span></span> <span data-ttu-id="886a3-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span><span class="sxs-lookup"><span data-stu-id="886a3-112">The following fields are required: **Item No.**, **Location Code**, and/or **Variant Code**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="886a3-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span><span class="sxs-lookup"><span data-stu-id="886a3-113">When you have set up the first stockkeeping unit for an item, the **Stockkeeping Unit Exists** check box on the **Item** card is selected.</span></span>  

<span data-ttu-id="886a3-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span><span class="sxs-lookup"><span data-stu-id="886a3-114">To create several stockkeeping units for an item, use the **Create Stockkeeping Unit** batch job.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="886a3-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span><span class="sxs-lookup"><span data-stu-id="886a3-115">The information on the **Stockkeeping Unit** card has priority over the **Item** card.</span></span>

> [!Warning]
> <span data-ttu-id="886a3-116">If the SKU is supplied through production, then the **Standard Cost** field is not used when invoicing and adjusting the actual cost of the produced item.</span><span class="sxs-lookup"><span data-stu-id="886a3-116">If the SKU is supplied through production, then the **Standard Cost** field is not used when invoicing and adjusting the actual cost of the produced item.</span></span> <span data-ttu-id="886a3-117">Instead, the **Standard Cost** field on the underlying item card is used, and any variances are calculated against the cost shares of that item.</span><span class="sxs-lookup"><span data-stu-id="886a3-117">Instead, the **Standard Cost** field on the underlying item card is used, and any variances are calculated against the cost shares of that item.</span></span><br /><br />
> <span data-ttu-id="886a3-118">Because production BOMs and routing cannot be assigned to SKUs, then the unit cost roll-up and the related calculation of cost shares are also not available on SKUs.</span><span class="sxs-lookup"><span data-stu-id="886a3-118">Because production BOMs and routing cannot be assigned to SKUs, then the unit cost roll-up and the related calculation of cost shares are also not available on SKUs.</span></span> <span data-ttu-id="886a3-119">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md)</span><span class="sxs-lookup"><span data-stu-id="886a3-119">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md)</span></span>

## <a name="see-also"></a><span data-ttu-id="886a3-120">See Also</span><span class="sxs-lookup"><span data-stu-id="886a3-120">See Also</span></span>  
[<span data-ttu-id="886a3-121">Register New Items</span><span class="sxs-lookup"><span data-stu-id="886a3-121">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="886a3-122">Setting Up Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="886a3-122">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="886a3-123">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="886a3-123">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="886a3-124">Inventory</span><span class="sxs-lookup"><span data-stu-id="886a3-124">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="886a3-125">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="886a3-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="886a3-126">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="886a3-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="886a3-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="886a3-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]