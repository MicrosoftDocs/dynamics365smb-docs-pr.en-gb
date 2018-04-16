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
ms.date: 01/25/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: 52ac51bc028b09f9dd38c1114312f1d613951cad
ms.contentlocale: en-gb
ms.lasthandoff: 04/16/2018

---
# <a name="purchase-items-for-a-sale"></a><span data-ttu-id="a8378-103">Purchase Items for a Sale</span><span class="sxs-lookup"><span data-stu-id="a8378-103">Purchase Items for a Sale</span></span>
<span data-ttu-id="a8378-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span><span class="sxs-lookup"><span data-stu-id="a8378-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span></span> <span data-ttu-id="a8378-105">You can use two different functions depending on the document type.</span><span class="sxs-lookup"><span data-stu-id="a8378-105">You can use two different functions depending on the document type.</span></span>

|<span data-ttu-id="a8378-106">Function</span><span class="sxs-lookup"><span data-stu-id="a8378-106">Function</span></span>|<span data-ttu-id="a8378-107">Description</span><span class="sxs-lookup"><span data-stu-id="a8378-107">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="a8378-108">**Create Purchase Orders**</span><span class="sxs-lookup"><span data-stu-id="a8378-108">**Create Purchase Orders**</span></span>|<span data-ttu-id="a8378-109">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span><span class="sxs-lookup"><span data-stu-id="a8378-109">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span></span> <span data-ttu-id="a8378-110">You can edit the purchase quantity before you create the purchase orders.</span><span class="sxs-lookup"><span data-stu-id="a8378-110">You can edit the purchase quantity before you create the purchase orders.</span></span> <span data-ttu-id="a8378-111">Only unavailable sales quantities are suggested.</span><span class="sxs-lookup"><span data-stu-id="a8378-111">Only unavailable sales quantities are suggested.</span></span>
|<span data-ttu-id="a8378-112">**Create Purchase Invoice**</span><span class="sxs-lookup"><span data-stu-id="a8378-112">**Create Purchase Invoice**</span></span>|<span data-ttu-id="a8378-113">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span><span class="sxs-lookup"><span data-stu-id="a8378-113">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span></span> <span data-ttu-id="a8378-114">The full sales quantity is suggested.</span><span class="sxs-lookup"><span data-stu-id="a8378-114">The full sales quantity is suggested.</span></span>|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a><span data-ttu-id="a8378-115">To create one or more purchase orders from a sales order</span><span class="sxs-lookup"><span data-stu-id="a8378-115">To create one or more purchase orders from a sales order</span></span>
<span data-ttu-id="a8378-116">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span><span class="sxs-lookup"><span data-stu-id="a8378-116">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span></span>

1. <span data-ttu-id="a8378-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a8378-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="a8378-118">Open a sales order that you want to purchase items for.</span><span class="sxs-lookup"><span data-stu-id="a8378-118">Open a sales order that you want to purchase items for.</span></span>
3. <span data-ttu-id="a8378-119">Choose the **Create Purchase Orders** action.</span><span class="sxs-lookup"><span data-stu-id="a8378-119">Choose the **Create Purchase Orders** action.</span></span>

    <span data-ttu-id="a8378-120">The **Create Purchase Orders** window opens showing a line for each different item on the sales order.</span><span class="sxs-lookup"><span data-stu-id="a8378-120">The **Create Purchase Orders** window opens showing a line for each different item on the sales order.</span></span> <span data-ttu-id="a8378-121">Lines for both fully available sales quantities and unavailable sales quantities (greyed) are shown by default.</span><span class="sxs-lookup"><span data-stu-id="a8378-121">Lines for both fully available sales quantities and unavailable sales quantities (grayed) are shown by default.</span></span> <span data-ttu-id="a8378-122">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span><span class="sxs-lookup"><span data-stu-id="a8378-122">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span></span>

    <span data-ttu-id="a8378-123">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span><span class="sxs-lookup"><span data-stu-id="a8378-123">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span></span>
4. <span data-ttu-id="a8378-124">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span><span class="sxs-lookup"><span data-stu-id="a8378-124">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span></span>

    > [!NOTE]  
   >   <span data-ttu-id="a8378-125">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span><span class="sxs-lookup"><span data-stu-id="a8378-125">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span></span>
5. <span data-ttu-id="a8378-126">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a8378-126">Choose the **OK** button.</span></span>

    <span data-ttu-id="a8378-127">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made in the **Create Purchase Orders** window.</span><span class="sxs-lookup"><span data-stu-id="a8378-127">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made in the **Create Purchase Orders** window.</span></span>
6. <span data-ttu-id="a8378-128">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="a8378-128">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span></span> <span data-ttu-id="a8378-129">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="a8378-129">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a><span data-ttu-id="a8378-130">To create a purchase invoice from a sales order or sales invoice</span><span class="sxs-lookup"><span data-stu-id="a8378-130">To create a purchase invoice from a sales order or sales invoice</span></span>
<span data-ttu-id="a8378-131">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span><span class="sxs-lookup"><span data-stu-id="a8378-131">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span></span>

> [!NOTE]  
>   <span data-ttu-id="a8378-132">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span><span class="sxs-lookup"><span data-stu-id="a8378-132">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span></span> <span data-ttu-id="a8378-133">To change the purchase quantity, you must edit the purchase invoice after it is created.</span><span class="sxs-lookup"><span data-stu-id="a8378-133">To change the purchase quantity, you must edit the purchase invoice after it is created.</span></span>  

1. <span data-ttu-id="a8378-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a8378-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="a8378-135">Open a sales invoice that you want to purchase items for.</span><span class="sxs-lookup"><span data-stu-id="a8378-135">Open a sales invoice that you want to purchase items for.</span></span>
3. <span data-ttu-id="a8378-136">Select one or more sales invoice lines that you want to use on the purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="a8378-136">Select one or more sales invoice lines that you want to use on the purchase invoice.</span></span> <span data-ttu-id="a8378-137">To use all the sales invoice lines, select either all of them or do not select any lines.</span><span class="sxs-lookup"><span data-stu-id="a8378-137">To use all the sales invoice lines, select either all of them or do not select any lines.</span></span>
4. <span data-ttu-id="a8378-138">Choose the **Create Purchase Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="a8378-138">Choose the **Create Purchase Invoice** action.</span></span>
5. <span data-ttu-id="a8378-139">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a8378-139">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span></span>  
6. <span data-ttu-id="a8378-140">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a8378-140">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span></span>

    <span data-ttu-id="a8378-141">A purchase invoice is created that contains one, more, or all the lines on the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="a8378-141">A purchase invoice is created that contains one, more, or all the lines on the sales invoice.</span></span>
7. <span data-ttu-id="a8378-142">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span><span class="sxs-lookup"><span data-stu-id="a8378-142">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span></span> <span data-ttu-id="a8378-143">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="a8378-143">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="a8378-144">See Also</span><span class="sxs-lookup"><span data-stu-id="a8378-144">See Also</span></span>
[<span data-ttu-id="a8378-145">Purchasing</span><span class="sxs-lookup"><span data-stu-id="a8378-145">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="a8378-146">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="a8378-146">Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="a8378-147">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="a8378-147">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="a8378-148">Register New Vendors</span><span class="sxs-lookup"><span data-stu-id="a8378-148">Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
<span data-ttu-id="a8378-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a8378-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

