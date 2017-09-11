---
title: Create a Purchase Invoice from a Sales Invoice to Buy Items for a Sale | Microsoft Docs
description: From a sales invoice, to purchase products, you can create a purchase invoice for a vendor or supplier.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 05/16/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 2d7eb238395a0b1060668996fbbc3e13d9dd8a94
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-purchase-items-for-a-sale"></a><span data-ttu-id="a99d2-103">How to: Purchase Items for a Sale</span><span class="sxs-lookup"><span data-stu-id="a99d2-103">How to: Purchase Items for a Sale</span></span>
<span data-ttu-id="a99d2-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span><span class="sxs-lookup"><span data-stu-id="a99d2-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span></span> <span data-ttu-id="a99d2-105">You can use two different functions depending on the document type.</span><span class="sxs-lookup"><span data-stu-id="a99d2-105">You can use two different functions depending on the document type.</span></span>
|<span data-ttu-id="a99d2-106">Function</span><span class="sxs-lookup"><span data-stu-id="a99d2-106">Function</span></span>|<span data-ttu-id="a99d2-107">Description</span><span class="sxs-lookup"><span data-stu-id="a99d2-107">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="a99d2-108">**Create Purchase Orders**</span><span class="sxs-lookup"><span data-stu-id="a99d2-108">**Create Purchase Orders**</span></span>|<span data-ttu-id="a99d2-109">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span><span class="sxs-lookup"><span data-stu-id="a99d2-109">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span></span> <span data-ttu-id="a99d2-110">You can edit the purchase quantity before you create the purchase orders.</span><span class="sxs-lookup"><span data-stu-id="a99d2-110">You can edit the purchase quantity before you create the purchase orders.</span></span> <span data-ttu-id="a99d2-111">Only unavailable sales quantities are suggested.</span><span class="sxs-lookup"><span data-stu-id="a99d2-111">Only unavailable sales quantities are suggested.</span></span>
|<span data-ttu-id="a99d2-112">**Create Purchase Invoice**</span><span class="sxs-lookup"><span data-stu-id="a99d2-112">**Create Purchase Invoice**</span></span>|<span data-ttu-id="a99d2-113">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span><span class="sxs-lookup"><span data-stu-id="a99d2-113">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span></span> <span data-ttu-id="a99d2-114">The full sales quantity is suggested.</span><span class="sxs-lookup"><span data-stu-id="a99d2-114">The full sales quantity is suggested.</span></span>|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a><span data-ttu-id="a99d2-115">To create one or more purchase orders from a sales order</span><span class="sxs-lookup"><span data-stu-id="a99d2-115">To create one or more purchase orders from a sales order</span></span>
<span data-ttu-id="a99d2-116">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span><span class="sxs-lookup"><span data-stu-id="a99d2-116">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span></span> 

> [!NOTE]  
>   <span data-ttu-id="a99d2-117">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="a99d2-117">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="a99d2-118">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="a99d2-118">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

1. <span data-ttu-id="a99d2-119">On the Home page, choose the **Ongoing Sales Orders** tile.</span><span class="sxs-lookup"><span data-stu-id="a99d2-119">On the Home page, choose the **Ongoing Sales Orders** tile.</span></span>
2. <span data-ttu-id="a99d2-120">Open a sales order that you want to purchase items for.</span><span class="sxs-lookup"><span data-stu-id="a99d2-120">Open a sales order that you want to purchase items for.</span></span>
3. <span data-ttu-id="a99d2-121">Choose the **Create Purchase Orders** action.</span><span class="sxs-lookup"><span data-stu-id="a99d2-121">Choose the **Create Purchase Orders** action.</span></span>

    <span data-ttu-id="a99d2-122">The **Create Purchase Orders** window opens showing a line for each different item on the sales order.</span><span class="sxs-lookup"><span data-stu-id="a99d2-122">The **Create Purchase Orders** window opens showing a line for each different item on the sales order.</span></span> <span data-ttu-id="a99d2-123">Lines for both fully available sales quantities and unavailable sales quantities (greyed) are shown by default.</span><span class="sxs-lookup"><span data-stu-id="a99d2-123">Lines for both fully available sales quantities and unavailable sales quantities (grayed) are shown by default.</span></span> <span data-ttu-id="a99d2-124">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span><span class="sxs-lookup"><span data-stu-id="a99d2-124">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span></span>

    <span data-ttu-id="a99d2-125">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span><span class="sxs-lookup"><span data-stu-id="a99d2-125">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span></span>
4. <span data-ttu-id="a99d2-126">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span><span class="sxs-lookup"><span data-stu-id="a99d2-126">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="a99d2-127">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span><span class="sxs-lookup"><span data-stu-id="a99d2-127">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span></span>
5. <span data-ttu-id="a99d2-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a99d2-128">Choose the **OK** button.</span></span> 
    
    <span data-ttu-id="a99d2-129">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made in the **Create Purchase Orders** window.</span><span class="sxs-lookup"><span data-stu-id="a99d2-129">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made in the **Create Purchase Orders** window.</span></span>
7. <span data-ttu-id="a99d2-130">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="a99d2-130">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span></span> <span data-ttu-id="a99d2-131">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="a99d2-131">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a><span data-ttu-id="a99d2-132">To create a purchase invoice from a sales order or sales invoice</span><span class="sxs-lookup"><span data-stu-id="a99d2-132">To create a purchase invoice from a sales order or sales invoice</span></span>
<span data-ttu-id="a99d2-133">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span><span class="sxs-lookup"><span data-stu-id="a99d2-133">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span></span> 

> [!NOTE]  
>   <span data-ttu-id="a99d2-134">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span><span class="sxs-lookup"><span data-stu-id="a99d2-134">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span></span> <span data-ttu-id="a99d2-135">To change the purchase quantity, you must edit the purchase invoice after it is created.</span><span class="sxs-lookup"><span data-stu-id="a99d2-135">To change the purchase quantity, you must edit the purchase invoice after it is created.</span></span>  

1. <span data-ttu-id="a99d2-136">On the Home page, choose the **Ongoing Sales Invoices** tile.</span><span class="sxs-lookup"><span data-stu-id="a99d2-136">On the Home page, choose the **Ongoing Sales Invoices** tile.</span></span>
2. <span data-ttu-id="a99d2-137">Open a sales invoice that you want to purchase items for.</span><span class="sxs-lookup"><span data-stu-id="a99d2-137">Open a sales invoice that you want to purchase items for.</span></span>
3. <span data-ttu-id="a99d2-138">Select one or more sales invoice lines that you want to use on the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="a99d2-138">Select one or more sales invoice lines that you want to use on the purchase invoice.</span></span> <span data-ttu-id="a99d2-139">To use all the sales invoice lines, select either all of them or do not select any lines.</span><span class="sxs-lookup"><span data-stu-id="a99d2-139">To use all the sales invoice lines, select either all of them or do not select any lines.</span></span>
4. <span data-ttu-id="a99d2-140">Choose the **Create Purchase Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="a99d2-140">Choose the **Create Purchase Invoice** action.</span></span>
5. <span data-ttu-id="a99d2-141">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a99d2-141">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span></span>  
6. <span data-ttu-id="a99d2-142">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a99d2-142">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span></span>

    <span data-ttu-id="a99d2-143">A purchase invoice is created that contains one, more, or all the lines on the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="a99d2-143">A purchase invoice is created that contains one, more, or all the lines on the sales invoice.</span></span>
7. <span data-ttu-id="a99d2-144">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span><span class="sxs-lookup"><span data-stu-id="a99d2-144">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span></span> <span data-ttu-id="a99d2-145">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="a99d2-145">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="a99d2-146">See Also</span><span class="sxs-lookup"><span data-stu-id="a99d2-146">See Also</span></span>
[<span data-ttu-id="a99d2-147">Purchasing</span><span class="sxs-lookup"><span data-stu-id="a99d2-147">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="a99d2-148">How to: Record Purchases</span><span class="sxs-lookup"><span data-stu-id="a99d2-148">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="a99d2-149">How to: Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="a99d2-149">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="a99d2-150">How to: Register New Vendors</span><span class="sxs-lookup"><span data-stu-id="a99d2-150">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
<span data-ttu-id="a99d2-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a99d2-151">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

