---
title: How to Create Special Orders | Microsoft Docs
description: You can create a special order for a specific catalogue item to be shipped to a specific customer. Your vendor ships the item to your warehouse and you can then ship the item on to your customer either independently or together with other items on another order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f04ac444f807a778cbda03b7062a5c4e23ea8386
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5778429"
---
# <a name="create-special-orders"></a><span data-ttu-id="b31d7-104">Create Special Orders</span><span class="sxs-lookup"><span data-stu-id="b31d7-104">Create Special Orders</span></span>
<span data-ttu-id="b31d7-105">You can create a special order for a specific catalogue item to be shipped to a specific customer.</span><span class="sxs-lookup"><span data-stu-id="b31d7-105">You can create a special order for a specific catalog item to be shipped to a specific customer.</span></span> <span data-ttu-id="b31d7-106">Your vendor ships the item to your warehouse and you can then ship the item on to your customer either independently or together with other items on another order.</span><span class="sxs-lookup"><span data-stu-id="b31d7-106">Your vendor ships the item to your warehouse and you can then ship the item on to your customer either independently or together with other items on another order.</span></span>  

<span data-ttu-id="b31d7-107">Special orders imply that the purchase and sales order are linked to ensure that the specific catalogue item is picked and delivered to the customer.</span><span class="sxs-lookup"><span data-stu-id="b31d7-107">Special orders imply that the purchase and sales order are linked to ensure that the specific catalog item is picked and delivered to the customer.</span></span>  

<span data-ttu-id="b31d7-108">Before you can use this feature, you must first set up the customer, vendor, and item cards necessary for the order.</span><span class="sxs-lookup"><span data-stu-id="b31d7-108">Before you can use this feature, you must first set up the customer, vendor, and item cards necessary for the order.</span></span>  

## <a name="to-create-a-special-order"></a><span data-ttu-id="b31d7-109">To create a special order</span><span class="sxs-lookup"><span data-stu-id="b31d7-109">To create a special order</span></span>  
1.  <span data-ttu-id="b31d7-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Order**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b31d7-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Order**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b31d7-111">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="b31d7-111">Choose the **New** action.</span></span> <span data-ttu-id="b31d7-112">Create and fill in a  sales order for the item.</span><span class="sxs-lookup"><span data-stu-id="b31d7-112">Create and fill in a  sales order for the item.</span></span> <span data-ttu-id="b31d7-113">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="b31d7-113">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
3.  <span data-ttu-id="b31d7-114">On the **Lines** FastTab, fill in the sales line.</span><span class="sxs-lookup"><span data-stu-id="b31d7-114">On the **Lines** FastTab, fill in the sales line.</span></span> <span data-ttu-id="b31d7-115">In the **Purchasing Code** field, select a purchasing code that has the **Special Order** field selected.</span><span class="sxs-lookup"><span data-stu-id="b31d7-115">In the **Purchasing Code** field, select a purchasing code that has the **Special Order** field selected.</span></span>

    <span data-ttu-id="b31d7-116">You must now create a purchase order from a requisition worksheet.</span><span class="sxs-lookup"><span data-stu-id="b31d7-116">You must now create a purchase order from a requisition worksheet.</span></span>  
4. <span data-ttu-id="b31d7-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requisition Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b31d7-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requisition Worksheet**, and then choose the related link.</span></span>  
5. <span data-ttu-id="b31d7-118">Choose the **Special Order** action, and then choose the **Get Sales Orders** action.</span><span class="sxs-lookup"><span data-stu-id="b31d7-118">Choose the **Special Order** action, and then choose the **Get Sales Orders** action.</span></span>  
6.  <span data-ttu-id="b31d7-119">On the **Get Sales Orders** page, show results where the **Document No.** is the sales order number.</span><span class="sxs-lookup"><span data-stu-id="b31d7-119">On the **Get Sales Orders** page, show results where the **Document No.** is the sales order number.</span></span> <span data-ttu-id="b31d7-120">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b31d7-120">Choose the **OK** button.</span></span> <span data-ttu-id="b31d7-121">A requisition worksheet line is created for the item.</span><span class="sxs-lookup"><span data-stu-id="b31d7-121">A requisition worksheet line is created for the item.</span></span>  
7.  <span data-ttu-id="b31d7-122">On the requisition worksheet line, in the **Action Message** field, select **New**.</span><span class="sxs-lookup"><span data-stu-id="b31d7-122">On the requisition worksheet line, in the **Action Message** field, select **New**.</span></span>  
8.  <span data-ttu-id="b31d7-123">On the **Req. Worksheet** page, choose the **Carry Out Action Message** action.</span><span class="sxs-lookup"><span data-stu-id="b31d7-123">On the **Req. Worksheet** page, choose the **Carry Out Action Message** action.</span></span> <span data-ttu-id="b31d7-124">The **Carry Out Action Msg. - Req.** page opens.</span><span class="sxs-lookup"><span data-stu-id="b31d7-124">The **Carry Out Action Msg. - Req.** page opens.</span></span> <span data-ttu-id="b31d7-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b31d7-125">Choose the **OK** button.</span></span>  

    <span data-ttu-id="b31d7-126">A message appears telling you that the purchase orders have been created.</span><span class="sxs-lookup"><span data-stu-id="b31d7-126">A message appears telling you that the purchase orders have been created.</span></span> <span data-ttu-id="b31d7-127">Choost the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="b31d7-127">Choost the **OK** button.</span></span>  

<span data-ttu-id="b31d7-128">A purchase order created as a special order for a sales order is respected by the planning system as it balances demand and supply.</span><span class="sxs-lookup"><span data-stu-id="b31d7-128">A purchase order created as a special order for a sales order is respected by the planning system as it balances demand and supply.</span></span> <span data-ttu-id="b31d7-129">That is, the purchase order (supply) remains linked to the sales order (demand), even if that purchase order could supply another earlier demand.</span><span class="sxs-lookup"><span data-stu-id="b31d7-129">That is, the purchase order (supply) remains linked to the sales order (demand), even if that purchase order could supply another earlier demand.</span></span> <span data-ttu-id="b31d7-130">For more information, see [Design Details: Reordering Policies](design-details-reservation-order-tracking-and-action-messaging.md).</span><span class="sxs-lookup"><span data-stu-id="b31d7-130">For more information, see [Design Details: Reordering Policies](design-details-reservation-order-tracking-and-action-messaging.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="b31d7-131">You cannot use the special order functionality if the item is already reserved.</span><span class="sxs-lookup"><span data-stu-id="b31d7-131">You cannot use the special order functionality if the item is already reserved.</span></span> <span data-ttu-id="b31d7-132">Therefore, for items that are sold on special orders, make sure the **Reserve** field on the item card is not set to **Always**.</span><span class="sxs-lookup"><span data-stu-id="b31d7-132">Therefore, for items that are sold on special orders, make sure the **Reserve** field on the item card is not set to **Always**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b31d7-133">See Also</span><span class="sxs-lookup"><span data-stu-id="b31d7-133">See Also</span></span>  
[<span data-ttu-id="b31d7-134">Work with Catalogue Items</span><span class="sxs-lookup"><span data-stu-id="b31d7-134">Work with Catalog Items</span></span>](inventory-how-work-nonstock-items.md)  
[<span data-ttu-id="b31d7-135">Sales</span><span class="sxs-lookup"><span data-stu-id="b31d7-135">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="b31d7-136">[Make Drop Shipments](sales-how-drop-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="b31d7-136">[Make Drop Shipments](sales-how-drop-shipment.md) </span></span>  
[<span data-ttu-id="b31d7-137">Design Details: Reordering Policies</span><span class="sxs-lookup"><span data-stu-id="b31d7-137">Design Details: Reordering Policies</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="b31d7-138">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b31d7-138">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]