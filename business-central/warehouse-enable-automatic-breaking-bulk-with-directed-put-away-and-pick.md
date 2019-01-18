---
title: Automatic Breaking Bulk with Directed Put-away and Pick | Microsoft Docs
description: For locations that use directed put-away and pick, you can break a larger unit of measure into smaller units of measure, when it creates warehouse instructions that fulfil the needs of source documents, production orders, or internal picks and put-aways.
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
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: c328df334d1bb1be33ced814677c3ef3ea634799
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="enable-automatic-breaking-bulk-with-directed-put-away-and-pick"></a><span data-ttu-id="371ad-103">Enable Automatic Breaking Bulk with Directed Put-away and Pick</span><span class="sxs-lookup"><span data-stu-id="371ad-103">Enable Automatic Breaking Bulk with Directed Put-away and Pick</span></span>
<span data-ttu-id="371ad-104">For locations that use directed put-away and pick, [!INCLUDE[d365fin](includes/d365fin_md.md)] can, in various situations, automatically breakbulk, that is, break a larger unit of measure into smaller units of measure, when it creates warehouse instructions that fulfil the needs of source documents, production orders, or internal picks and put-aways.</span><span class="sxs-lookup"><span data-stu-id="371ad-104">For locations that use directed put-away and pick, [!INCLUDE[d365fin](includes/d365fin_md.md)] can, in various situations, automatically breakbulk, that is, break a larger unit of measure into smaller units of measure, when it creates warehouse instructions that fulfill the needs of source documents, production orders, or internal picks and put-aways.</span></span> <span data-ttu-id="371ad-105">To breakbulk sometimes also means gathering smaller units of measure, if necessary, to meet outbound requests by breaking the larger unit of measure on the source document or production order into the smaller units of measure that are available in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="371ad-105">To breakbulk sometimes also means gathering smaller units of measure, if necessary, to meet outbound requests by breaking the larger unit of measure on the source document or production order into the smaller units of measure that are available in the warehouse.</span></span>   

## <a name="breakbulking-in-picks"></a><span data-ttu-id="371ad-106">Breakbulking in Picks</span><span class="sxs-lookup"><span data-stu-id="371ad-106">Breakbulking in Picks</span></span>  
<span data-ttu-id="371ad-107">If you want to store items in several different units of measure and allow them to be automatically combined as needed in the picking process, select the **Allow Breakbulk** field on the location card.</span><span class="sxs-lookup"><span data-stu-id="371ad-107">If you want to store items in several different units of measure and allow them to be automatically combined as needed in the picking process, select the **Allow Breakbulk** field on the location card.</span></span>  

<span data-ttu-id="371ad-108">To fulfill a task, the program automatically looks for an item in the same unit of measure.</span><span class="sxs-lookup"><span data-stu-id="371ad-108">To fulfill a task, the program automatically looks for an item in the same unit of measure.</span></span> <span data-ttu-id="371ad-109">But if it cannot find this form of the item, and this field is selected, the program will suggest that you break a larger unit of measure into the unit of measure that is needed.</span><span class="sxs-lookup"><span data-stu-id="371ad-109">But if it cannot find this form of the item, and this field is selected, the program will suggest that you break a larger unit of measure into the unit of measure that is needed.</span></span>  

<span data-ttu-id="371ad-110">If the system can only find smaller units of measure, it will suggest that you gather items to fulfil the quantity on the shipment or production order.</span><span class="sxs-lookup"><span data-stu-id="371ad-110">If the system can only find smaller units of measure, it will suggest that you gather items to fulfill the quantity on the shipment or production order.</span></span> <span data-ttu-id="371ad-111">In effect, it breaks the larger unit of measure on the source document into smaller units for picking.</span><span class="sxs-lookup"><span data-stu-id="371ad-111">In effect, it breaks the larger unit of measure on the source document into smaller units for picking.</span></span>  

## <a name="breakbulking-in-put-aways"></a><span data-ttu-id="371ad-112">Breakbulking in Put-aways</span><span class="sxs-lookup"><span data-stu-id="371ad-112">Breakbulking in Put-aways</span></span>  
<span data-ttu-id="371ad-113">In the warehouse put-away, the program automatically suggests Place action lines in the put-away unit of measure, for example, pieces, even though the items arrive in a different unit of measure.</span><span class="sxs-lookup"><span data-stu-id="371ad-113">In the warehouse put-away, the program automatically suggests Place action lines in the put-away unit of measure, for example, pieces, even though the items arrive in a different unit of measure.</span></span>  

## <a name="breakbulking-in-movements"></a><span data-ttu-id="371ad-114">Breakbulking in Movements</span><span class="sxs-lookup"><span data-stu-id="371ad-114">Breakbulking in Movements</span></span>  
<span data-ttu-id="371ad-115">The programme also breakbulks automatically in replenishment movements, if the **Allow Breakbulk** field is selected on the **Option** FastTab on the **Calculate Bin Replenishment** page.</span><span class="sxs-lookup"><span data-stu-id="371ad-115">The program also breakbulks automatically in replenishment movements, if the **Allow Breakbulk** field is selected on the **Option** FastTab on the **Calculate Bin Replenishment** page.</span></span>  

<span data-ttu-id="371ad-116">You can view the results of the conversion process from one unit of measure to another as intermediate breakbulk lines in the put-away, pick, or movement instructions.</span><span class="sxs-lookup"><span data-stu-id="371ad-116">You can view the results of the conversion process from one unit of measure to another as intermediate breakbulk lines in the put-away, pick, or movement instructions.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="371ad-117">If you select the **Set Breakbulk Filter** field on the warehouse instruction header, the program will hide the breakbulk lines whenever the larger unit of measure is going to be completely used.</span><span class="sxs-lookup"><span data-stu-id="371ad-117">If you select the **Set Breakbulk Filter** field on the warehouse instruction header, the program will hide the breakbulk lines whenever the larger unit of measure is going to be completely used.</span></span> <span data-ttu-id="371ad-118">For example, if a pallet is 12 pieces and you are going to use all 12 pieces, the pick will then direct you to take 1 pallet and place 12 pieces.</span><span class="sxs-lookup"><span data-stu-id="371ad-118">For example, if a pallet is 12 pieces and you are going to use all 12 pieces, the pick will then direct you to take 1 pallet and place 12 pieces.</span></span> <span data-ttu-id="371ad-119">However, if you have to pick only 9 pieces, then the breakbulk lines will not be hidden, even if you have selected the **Breakbulk Filter** field, because you have to place the remaining three pieces somewhere in the warehouse.</span><span class="sxs-lookup"><span data-stu-id="371ad-119">However, if you have to pick only 9 pieces, then the breakbulk lines will not be hidden, even if you have selected the **Breakbulk Filter** field, because you have to place the remaining three pieces somewhere in the warehouse.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="371ad-120">If you want your units of measure to perform optimally in the warehouse, also in connection with the breakbulk functionality, you should wherever possible try to:</span><span class="sxs-lookup"><span data-stu-id="371ad-120">If you want your units of measure to perform optimally in the warehouse, also in connection with the breakbulk functionality, you should wherever possible try to:</span></span>  
>   
> - <span data-ttu-id="371ad-121">Set up the base unit of measure for an item as the smallest unit of measure that you expect to handle in your warehouse processes.</span><span class="sxs-lookup"><span data-stu-id="371ad-121">Set up the base unit of measure for an item as the smallest unit of measure that you expect to handle in your warehouse processes.</span></span>  
> - <span data-ttu-id="371ad-122">Set up your alternative units of measure for the item as multiples of the base unit of measure.</span><span class="sxs-lookup"><span data-stu-id="371ad-122">Set up your alternative units of measure for the item as multiples of the base unit of measure.</span></span>  

## <a name="see-also"></a><span data-ttu-id="371ad-123">See Also</span><span class="sxs-lookup"><span data-stu-id="371ad-123">See Also</span></span>  
[<span data-ttu-id="371ad-124">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="371ad-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="371ad-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="371ad-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="371ad-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="371ad-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="371ad-127">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="371ad-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="371ad-128">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="371ad-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="371ad-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="371ad-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

