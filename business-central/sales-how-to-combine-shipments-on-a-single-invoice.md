---
title: How to Combine Shipments on a Single Invoice | Microsoft Docs
description: If you want to invoice more than one shipment at a time, you can use the combined shipments feature.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: d100ec6888fbd2e8fa55ce0facef8645a079dc76
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="combine-shipments-on-a-single-invoice"></a><span data-ttu-id="4c14d-103">Combine Shipments on a Single Invoice</span><span class="sxs-lookup"><span data-stu-id="4c14d-103">Combine Shipments on a Single Invoice</span></span>
<span data-ttu-id="4c14d-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span><span class="sxs-lookup"><span data-stu-id="4c14d-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span></span>  

 <span data-ttu-id="4c14d-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span><span class="sxs-lookup"><span data-stu-id="4c14d-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span></span> <span data-ttu-id="4c14d-106">In other words, you must have filled in two or more sales orders and posted them as shipped, but not invoiced.</span><span class="sxs-lookup"><span data-stu-id="4c14d-106">In other words, you must have filled in two or more sales orders and posted them as shipped, but not invoiced.</span></span> <span data-ttu-id="4c14d-107">To combine shipments, the **Combine Shipments** check box must be selected on the **Shipping** FastTab of the **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="4c14d-107">To combine shipments, the **Combine Shipments** check box must be selected on the **Shipping** FastTab of the **Customer** card.</span></span>  

## <a name="to-manually-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="4c14d-108">To manually combine shipments on a single invoice</span><span class="sxs-lookup"><span data-stu-id="4c14d-108">To manually combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="4c14d-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c14d-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="4c14d-110">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="4c14d-110">Choose the **New** action.</span></span> <span data-ttu-id="4c14d-111">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="4c14d-111">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>
3. <span data-ttu-id="4c14d-112">In the **Sell-to Customer No.**</span><span class="sxs-lookup"><span data-stu-id="4c14d-112">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="4c14d-113">field, enter the customer who will receive the invoice for the shipped items.</span><span class="sxs-lookup"><span data-stu-id="4c14d-113">field, enter the customer who will receive the invoice for the shipped items.</span></span>  
4. <span data-ttu-id="4c14d-114">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span><span class="sxs-lookup"><span data-stu-id="4c14d-114">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span></span>  
5. <span data-ttu-id="4c14d-115">Select the shipment line that you want to include in the invoice:</span><span class="sxs-lookup"><span data-stu-id="4c14d-115">Select the shipment line that you want to include in the invoice:</span></span>  

    - <span data-ttu-id="4c14d-116">To insert all lines, select all lines and choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4c14d-116">To insert all lines, select all lines and choose the **OK** button.</span></span>  
    - <span data-ttu-id="4c14d-117">To insert specific lines, select the lines and choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4c14d-117">To insert specific lines, select the lines and choose the **OK** button.</span></span> <span data-ttu-id="4c14d-118">You can use the Ctrl key to select multiple nonsequential lines.</span><span class="sxs-lookup"><span data-stu-id="4c14d-118">You can use the Ctrl key to select multiple nonsequential lines.</span></span>  

    <span data-ttu-id="4c14d-119">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span><span class="sxs-lookup"><span data-stu-id="4c14d-119">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span></span>  
7. <span data-ttu-id="4c14d-120">To post the invoice, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="4c14d-120">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-automatically-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="4c14d-121">To automatically combine shipments on a single invoice</span><span class="sxs-lookup"><span data-stu-id="4c14d-121">To automatically combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="4c14d-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Combine Shipments**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4c14d-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Combine Shipments**, and then choose the related link.</span></span> <span data-ttu-id="4c14d-123">The batch job request window opens.</span><span class="sxs-lookup"><span data-stu-id="4c14d-123">The batch job request window opens.</span></span>  
2. <span data-ttu-id="4c14d-124">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="4c14d-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="4c14d-125">Select the **Post Invoices** check box.</span><span class="sxs-lookup"><span data-stu-id="4c14d-125">Select the **Post Invoices** check box.</span></span>  
4.  <span data-ttu-id="4c14d-126">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4c14d-126">Choose the **OK** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="4c14d-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span><span class="sxs-lookup"><span data-stu-id="4c14d-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span></span>  

## <a name="to-remove-open-sales-orders-after-combined-shipment-posting"></a><span data-ttu-id="4c14d-128">To remove open sales orders after combined shipment posting</span><span class="sxs-lookup"><span data-stu-id="4c14d-128">To remove open sales orders after combined shipment posting</span></span> 
<span data-ttu-id="4c14d-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span><span class="sxs-lookup"><span data-stu-id="4c14d-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span></span> <span data-ttu-id="4c14d-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span><span class="sxs-lookup"><span data-stu-id="4c14d-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span></span>  

<span data-ttu-id="4c14d-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span><span class="sxs-lookup"><span data-stu-id="4c14d-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span></span>   

1. <span data-ttu-id="4c14d-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span><span class="sxs-lookup"><span data-stu-id="4c14d-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span></span>  
2. <span data-ttu-id="4c14d-133">Specify in the **No.**</span><span class="sxs-lookup"><span data-stu-id="4c14d-133">Specify in the **No.**</span></span> <span data-ttu-id="4c14d-134">filter field which sales orders to delete.</span><span class="sxs-lookup"><span data-stu-id="4c14d-134">filter field which sales orders to delete.</span></span>  
3. <span data-ttu-id="4c14d-135">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="4c14d-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="4c14d-136">Alternatively, delete individual sales orders manually.</span><span class="sxs-lookup"><span data-stu-id="4c14d-136">Alternatively, delete individual sales orders manually.</span></span>  

<span data-ttu-id="4c14d-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span><span class="sxs-lookup"><span data-stu-id="4c14d-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="4c14d-138">See Also</span><span class="sxs-lookup"><span data-stu-id="4c14d-138">See Also</span></span>  
[<span data-ttu-id="4c14d-139">Sales</span><span class="sxs-lookup"><span data-stu-id="4c14d-139">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="4c14d-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4c14d-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

