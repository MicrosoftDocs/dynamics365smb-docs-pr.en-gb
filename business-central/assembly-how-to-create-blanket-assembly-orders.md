---
title: How to Create Blanket Assembly Orders | Microsoft Docs
description: If the **Replenishment System** field on the item card contains **Assembly**, then the default method of supplying the item is to assemble it from defined components and potentially by a defined resource.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: kit, kitting
ms.date: 12/20/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 5801fcc1284edfe1b8578518c084455c336d5a40
ms.openlocfilehash: 8796ccf6ce73ded327fad35573a2268e249fb7a7
ms.contentlocale: en-gb
ms.lasthandoff: 12/27/2018

---
# <a name="create-blanket-assembly-orders"></a><span data-ttu-id="6ca11-103">Create Blanket Assembly Orders</span><span class="sxs-lookup"><span data-stu-id="6ca11-103">Create Blanket Assembly Orders</span></span>
<span data-ttu-id="6ca11-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span><span class="sxs-lookup"><span data-stu-id="6ca11-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="6ca11-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="6ca11-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

 <span data-ttu-id="6ca11-106">As with any other type of item, you can also create blanket sales orders for customized assembly items before periodically making the actual sales orders according to the blanket order agreement.</span><span class="sxs-lookup"><span data-stu-id="6ca11-106">As with any other type of item, you can also create blanket sales orders for customized assembly items before periodically making the actual sales orders according to the blanket order agreement.</span></span> <span data-ttu-id="6ca11-107">This process involves several extra steps when you compare it to creating a regular blanket sales order, and it uses a variation of a linked assembly order, which is a blanket assembly order.</span><span class="sxs-lookup"><span data-stu-id="6ca11-107">This process involves several extra steps when you compare it to creating a regular blanket sales order, and it uses a variation of a linked assembly order, which is a blanket assembly order.</span></span>

> [!NOTE]  
>  <span data-ttu-id="6ca11-108">Like all blanket orders, quantities on assembly blanket orders are only forecasts and are not operational until they are converted to actual assembly orders.</span><span class="sxs-lookup"><span data-stu-id="6ca11-108">Like all blanket orders, quantities on assembly blanket orders are only forecasts and are not operational until they are converted to actual assembly orders.</span></span> <span data-ttu-id="6ca11-109">Therefore, order functionality, such as availability calculation, reservation, and item tracking, is not active on blanket assembly orders.</span><span class="sxs-lookup"><span data-stu-id="6ca11-109">Therefore, order functionality, such as availability calculation, reservation, and item tracking, is not active on blanket assembly orders.</span></span>  

## <a name="to-create-a-blanket-assembly-order-for-an-assemble-to-order-item"></a><span data-ttu-id="6ca11-110">To create a blanket assembly order for an assemble\-to\-order item</span><span class="sxs-lookup"><span data-stu-id="6ca11-110">To create a blanket assembly order for an assemble\-to\-order item</span></span>  
1. <span data-ttu-id="6ca11-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Blanket Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6ca11-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Blanket Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6ca11-112">Create a new blanket sales order with one line for an assembly item.</span><span class="sxs-lookup"><span data-stu-id="6ca11-112">Create a new blanket sales order with one line for an assembly item.</span></span> <span data-ttu-id="6ca11-113">For more information, see [Create Blanket Sales Orders](sales-how-to-create-blanket-sales-orders.md).</span><span class="sxs-lookup"><span data-stu-id="6ca11-113">For more information, see [Create Blanket Sales Orders](sales-how-to-create-blanket-sales-orders.md).</span></span>  
3. <span data-ttu-id="6ca11-114">In the **Qty. to Assemble to Order** field on the blanket assembly order line, enter the full quantity.</span><span class="sxs-lookup"><span data-stu-id="6ca11-114">In the **Qty. to Assemble to Order** field on the blanket assembly order line, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="6ca11-115">You should not create blanket order agreements for a partial quantity.</span><span class="sxs-lookup"><span data-stu-id="6ca11-115">You should not create blanket order agreements for a partial quantity.</span></span> <span data-ttu-id="6ca11-116">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the blanket sales order line.</span><span class="sxs-lookup"><span data-stu-id="6ca11-116">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the blanket sales order line.</span></span>  

4. <span data-ttu-id="6ca11-117">Choose the **Assemble to Order** action, and then choose the **Assemble-to-Order Lines** action.</span><span class="sxs-lookup"><span data-stu-id="6ca11-117">Choose the **Assemble to Order** action, and then choose the **Assemble-to-Order Lines** action.</span></span> <span data-ttu-id="6ca11-118">Alternatively, choose the **Qty. to Assemble to Order)** field on the line.</span><span class="sxs-lookup"><span data-stu-id="6ca11-118">Alternatively, choose the **Qty. to Assemble to Order)** field on the line.</span></span>  
5. <span data-ttu-id="6ca11-119">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the blanket order agreement that you have made with the customer.</span><span class="sxs-lookup"><span data-stu-id="6ca11-119">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the blanket order agreement that you have made with the customer.</span></span> <span data-ttu-id="6ca11-120">If you want to view more information, choose the **Show Document** action to open the complete blanket assembly order.</span><span class="sxs-lookup"><span data-stu-id="6ca11-120">If you want to view more information, choose the **Show Document** action to open the complete blanket assembly order.</span></span> <span data-ttu-id="6ca11-121">You cannot change the contents of most fields, and you cannot post.</span><span class="sxs-lookup"><span data-stu-id="6ca11-121">You cannot change the contents of most fields, and you cannot post.</span></span>  
6. <span data-ttu-id="6ca11-122">When you have adjusted the assembly order lines according to the blanket order agreement, close the **Assemble-to-Order Lines** page to return to the **Blanket Sales Order** page.</span><span class="sxs-lookup"><span data-stu-id="6ca11-122">When you have adjusted the assembly order lines according to the blanket order agreement, close the **Assemble-to-Order Lines** page to return to the **Blanket Sales Order** page.</span></span>  
7. <span data-ttu-id="6ca11-123">When the customer requests to create a sales order based on the agreed blanket sales order, create a sales order for the agreed assembly item or items.</span><span class="sxs-lookup"><span data-stu-id="6ca11-123">When the customer requests to create a sales order based on the agreed blanket sales order, create a sales order for the agreed assembly item or items.</span></span> <span data-ttu-id="6ca11-124">For more information, see [Create Blanket Sales Orders](sales-how-to-create-blanket-sales-orders.md).</span><span class="sxs-lookup"><span data-stu-id="6ca11-124">For more information, see [Create Blanket Sales Orders](sales-how-to-create-blanket-sales-orders.md).</span></span>

<span data-ttu-id="6ca11-125">The linked blanket assembly order and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span><span class="sxs-lookup"><span data-stu-id="6ca11-125">The linked blanket assembly order and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6ca11-126">See Also</span><span class="sxs-lookup"><span data-stu-id="6ca11-126">See Also</span></span>
[<span data-ttu-id="6ca11-127">Create Blanket Sales Orders</span><span class="sxs-lookup"><span data-stu-id="6ca11-127">Create Blanket Sales Orders</span></span>](sales-how-to-create-blanket-sales-orders.md)  
[<span data-ttu-id="6ca11-128">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="6ca11-128">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="6ca11-129">Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="6ca11-129">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="6ca11-130">Inventory</span><span class="sxs-lookup"><span data-stu-id="6ca11-130">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="6ca11-131">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="6ca11-131">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="6ca11-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6ca11-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

