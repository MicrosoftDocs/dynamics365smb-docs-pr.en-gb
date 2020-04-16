---
title: Link a Sales Order to a Purchase Order for Direct Shipment | Microsoft Docs
description: Describes how to create a sales order linked to a purchase order to enable shipment directly from the vendor to the customer.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c61f55701ecb07862f42d3cce242756001529588
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3193690"
---
# <a name="make-drop-shipments"></a><span data-ttu-id="eb069-103">Make Drop Shipments</span><span class="sxs-lookup"><span data-stu-id="eb069-103">Make Drop Shipments</span></span>
<span data-ttu-id="eb069-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span><span class="sxs-lookup"><span data-stu-id="eb069-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="eb069-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span><span class="sxs-lookup"><span data-stu-id="eb069-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Ship-to** field, **Customer Address**, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM?rel=0]

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="eb069-106">To create a sales order for drop shipment</span><span class="sxs-lookup"><span data-stu-id="eb069-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="eb069-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span><span class="sxs-lookup"><span data-stu-id="eb069-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="eb069-108">Create a sales order for an item.</span><span class="sxs-lookup"><span data-stu-id="eb069-108">Create a sales order for an item.</span></span> <span data-ttu-id="eb069-109">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="eb069-109">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="eb069-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span><span class="sxs-lookup"><span data-stu-id="eb069-110">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="eb069-111">Use the **Choose Columns** function if the field is not visible.</span><span class="sxs-lookup"><span data-stu-id="eb069-111">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="eb069-112">For more information, see [Personalise Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="eb069-112">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="eb069-113">To create the purchase order for drop shipment</span><span class="sxs-lookup"><span data-stu-id="eb069-113">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="eb069-114">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span><span class="sxs-lookup"><span data-stu-id="eb069-114">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="eb069-115">Create a purchase order.</span><span class="sxs-lookup"><span data-stu-id="eb069-115">Create a purchase order.</span></span> <span data-ttu-id="eb069-116">Do not fill any fields on the lines.</span><span class="sxs-lookup"><span data-stu-id="eb069-116">Do not fill any fields on the lines.</span></span> <span data-ttu-id="eb069-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="eb069-117">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="eb069-118">In the **Ship-to** field, select **Customer Address**.</span><span class="sxs-lookup"><span data-stu-id="eb069-118">In the **Ship-to** field, select **Customer Address**.</span></span>
3. <span data-ttu-id="eb069-119">In the **Customer** field, select the customer that you are selling to.</span><span class="sxs-lookup"><span data-stu-id="eb069-119">In the **Customer** field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="eb069-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span><span class="sxs-lookup"><span data-stu-id="eb069-120">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="eb069-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span><span class="sxs-lookup"><span data-stu-id="eb069-121">On the **Sales List** page, select the sales order that you prepared in [To create a sales order for drop shipment](sales-how-drop-shipment.md#to-create-a-sales-order-for-drop-shipment).</span></span>
5. <span data-ttu-id="eb069-122">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="eb069-122">Choose the **OK** button.</span></span>

<span data-ttu-id="eb069-123">The line information from the sales order is inserted on the purchase order line(s).</span><span class="sxs-lookup"><span data-stu-id="eb069-123">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="eb069-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span><span class="sxs-lookup"><span data-stu-id="eb069-124">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="eb069-125">To view the linked purchase order from the sales order</span><span class="sxs-lookup"><span data-stu-id="eb069-125">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="eb069-126">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span><span class="sxs-lookup"><span data-stu-id="eb069-126">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="eb069-127">To post a drop shipment</span><span class="sxs-lookup"><span data-stu-id="eb069-127">To post a drop shipment</span></span>
<span data-ttu-id="eb069-128">After the vendor ships the items, you can post the sales order as shipped.</span><span class="sxs-lookup"><span data-stu-id="eb069-128">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="eb069-129">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span><span class="sxs-lookup"><span data-stu-id="eb069-129">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="eb069-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="eb069-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="eb069-131">Open the sales order that you created in [To create a sales order for drop shipment]().</span><span class="sxs-lookup"><span data-stu-id="eb069-131">Open the sales order that you created in [To create a sales order for drop shipment]().</span></span>
3. <span data-ttu-id="eb069-132">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span><span class="sxs-lookup"><span data-stu-id="eb069-132">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="eb069-133">Choose the **Post** or **Post and Send** action.</span><span class="sxs-lookup"><span data-stu-id="eb069-133">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="eb069-134">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span><span class="sxs-lookup"><span data-stu-id="eb069-134">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="eb069-135">See Also</span><span class="sxs-lookup"><span data-stu-id="eb069-135">See Also</span></span>
[<span data-ttu-id="eb069-136">Create Special Orders</span><span class="sxs-lookup"><span data-stu-id="eb069-136">Create Special Orders</span></span>](sales-how-to-create-special-orders.md)  
[<span data-ttu-id="eb069-137">Purchase Items for a Sale</span><span class="sxs-lookup"><span data-stu-id="eb069-137">Purchase Items for a Sale</span></span>](purchasing-how-purchase-products-sale.md)  
[<span data-ttu-id="eb069-138">Sell Products</span><span class="sxs-lookup"><span data-stu-id="eb069-138">Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="eb069-139">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="eb069-139">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="eb069-140">Sales</span><span class="sxs-lookup"><span data-stu-id="eb069-140">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="eb069-141">Inventory</span><span class="sxs-lookup"><span data-stu-id="eb069-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="eb069-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eb069-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
