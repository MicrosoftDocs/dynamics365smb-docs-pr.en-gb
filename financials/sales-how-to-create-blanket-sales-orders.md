---
title: How to Create Blanket Sales Orders | Microsoft Docs
description: Use blanket orders when a customer has agreed to buy large quantities that are to be delivered in several smaller shipments over a certain period of time.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 89db93227222d79e535f2d18400330aa30566f2f
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="work-with-blanket-sales-orders"></a><span data-ttu-id="dc010-103">Work with Blanket Sales Orders</span><span class="sxs-lookup"><span data-stu-id="dc010-103">Work with Blanket Sales Orders</span></span>
<span data-ttu-id="dc010-104">A blanket sales order represents a framework for a long-term agreement between you and your customer.</span><span class="sxs-lookup"><span data-stu-id="dc010-104">A blanket sales order represents a framework for a long-term agreement between you and your customer.</span></span>

<span data-ttu-id="dc010-105">A blanket order is typically made when a customer has committed to purchasing large quantities that are to be delivered in several smaller shipments over a certain period of time.</span><span class="sxs-lookup"><span data-stu-id="dc010-105">A blanket order is typically made when a customer has committed to purchasing large quantities that are to be delivered in several smaller shipments over a certain period of time.</span></span> <span data-ttu-id="dc010-106">Often blanket orders cover only one item with predetermined delivery dates.</span><span class="sxs-lookup"><span data-stu-id="dc010-106">Often blanket orders cover only one item with predetermined delivery dates.</span></span> <span data-ttu-id="dc010-107">The main reason for using a blanket order rather than a sales order is that quantities entered on a blanket order do not affect item availability and thus can be used as a worksheet for monitoring, forecasting, and planning purposes.</span><span class="sxs-lookup"><span data-stu-id="dc010-107">The main reason for using a blanket order rather than a sales order is that quantities entered on a blanket order do not affect item availability and thus can be used as a worksheet for monitoring, forecasting, and planning purposes.</span></span>

<span data-ttu-id="dc010-108">On the blanket order, each separate shipment can be set up as an order line, which can then be converted into a sales order at the time of shipping.</span><span class="sxs-lookup"><span data-stu-id="dc010-108">On the blanket order, each separate shipment can be set up as an order line, which can then be converted into a sales order at the time of shipping.</span></span>

<span data-ttu-id="dc010-109">An example of when a blanket sales order could be used is if a customer calls and places an order of 1000 units of an item and they want the items to be delivered in 250 units every week over the next month.</span><span class="sxs-lookup"><span data-stu-id="dc010-109">An example of when a blanket sales order could be used is if a customer calls and places an order of 1000 units of an item and they want the items to be delivered in 250 units every week over the next month.</span></span>

> [!NOTE]
> <span data-ttu-id="dc010-110">Blanket purchase orders work in a similar way as blanket sales orders.</span><span class="sxs-lookup"><span data-stu-id="dc010-110">Blanket purchase orders work in a similar way as blanket sales orders.</span></span> <span data-ttu-id="dc010-111">This documentation does not cover blanket purchase orders.</span><span class="sxs-lookup"><span data-stu-id="dc010-111">This documentation does not cover blanket purchase orders.</span></span>

## <a name="to-create-a-blanket-sales-order"></a><span data-ttu-id="dc010-112">To create a blanket sales order</span><span class="sxs-lookup"><span data-stu-id="dc010-112">To create a blanket sales order</span></span>  
1. <span data-ttu-id="dc010-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="dc010-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="dc010-114">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="dc010-114">Choose the **New** action.</span></span>  
3. <span data-ttu-id="dc010-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="dc010-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="dc010-116">Leave the **Order Date** field blank.</span><span class="sxs-lookup"><span data-stu-id="dc010-116">Leave the **Order Date** field blank.</span></span> <span data-ttu-id="dc010-117">When the separate sales orders are created from the blanket order, the order date of the sales order is set to equal the actual work date.</span><span class="sxs-lookup"><span data-stu-id="dc010-117">When the separate sales orders are created from the blanket order, the order date of the sales order is set to equal the actual work date.</span></span>
5. <span data-ttu-id="dc010-118">On the **Lines** FastTab, create separate lines for each shipment.</span><span class="sxs-lookup"><span data-stu-id="dc010-118">On the **Lines** FastTab, create separate lines for each shipment.</span></span> <span data-ttu-id="dc010-119">For instance, if your customer wants 1000 units split out equally between four weeks, you would enter four separate lines of 250 units each.</span><span class="sxs-lookup"><span data-stu-id="dc010-119">For instance, if your customer wants 1000 units split out equally between four weeks, you would enter four separate lines of 250 units each.</span></span>   

## <a name="to-create-a-sales-order-from-a-blanket-sales-order"></a><span data-ttu-id="dc010-120">To create a sales order from a blanket sales order</span><span class="sxs-lookup"><span data-stu-id="dc010-120">To create a sales order from a blanket sales order</span></span>  

1.  <span data-ttu-id="dc010-121">To create an order for any of the lines in the blanket assembly order, remove the quantity in the **Qty. to Ship** field on all the lines that you DO NOT wish to ship at this time.</span><span class="sxs-lookup"><span data-stu-id="dc010-121">To create an order for any of the lines in the blanket assembly order, remove the quantity in the **Qty. to Ship** field on all the lines that you DO NOT wish to ship at this time.</span></span>  
2.  <span data-ttu-id="dc010-122">When you are ready to create orders, choose the **Make Order**m action, and then choose **Yes**.</span><span class="sxs-lookup"><span data-stu-id="dc010-122">When you are ready to create orders, choose the **Make Order**m action, and then choose **Yes**.</span></span> <span data-ttu-id="dc010-123">A message appears informing you that the blanket order has been assigned an order number.</span><span class="sxs-lookup"><span data-stu-id="dc010-123">A message appears informing you that the blanket order has been assigned an order number.</span></span> <span data-ttu-id="dc010-124">Note that the blanket order has not been deleted.</span><span class="sxs-lookup"><span data-stu-id="dc010-124">Note that the blanket order has not been deleted.</span></span>  
3.  <span data-ttu-id="dc010-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="dc010-125">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="dc010-126">To see the results of the preceding steps, choose the **Line** action, choose the **Unposted Lines** action, and then choose the **Orders** action.</span><span class="sxs-lookup"><span data-stu-id="dc010-126">To see the results of the preceding steps, choose the **Line** action, choose the **Unposted Lines** action, and then choose the **Orders** action.</span></span>  
5.  <span data-ttu-id="dc010-127">In the **Sales Lines** window, select the appropriate sales order, choose the **Line** action, and then choose the **Show Document** action.</span><span class="sxs-lookup"><span data-stu-id="dc010-127">In the **Sales Lines** window, select the appropriate sales order, choose the **Line** action, and then choose the **Show Document** action.</span></span>  

<span data-ttu-id="dc010-128">The following applies to sales orders after they have been created from blanket sales orders:</span><span class="sxs-lookup"><span data-stu-id="dc010-128">The following applies to sales orders after they have been created from blanket sales orders:</span></span>  

- <span data-ttu-id="dc010-129">After the blanket order is converted into a sales order, the sales order contains all the lines from the blanket order.</span><span class="sxs-lookup"><span data-stu-id="dc010-129">After the blanket order is converted into a sales order, the sales order contains all the lines from the blanket order.</span></span> <span data-ttu-id="dc010-130">The lines where the quantity in the **Qty. to Ship** field was deleted appear, but with blank **Quantity** fields.</span><span class="sxs-lookup"><span data-stu-id="dc010-130">The lines where the quantity in the **Qty. to Ship** field was deleted appear, but with blank **Quantity** fields.</span></span> <span data-ttu-id="dc010-131">You may choose to leave, edit, or delete the lines.</span><span class="sxs-lookup"><span data-stu-id="dc010-131">You may choose to leave, edit, or delete the lines.</span></span>  
- <span data-ttu-id="dc010-132">It is important to remember that the sales order line quantity must not exceed the quantity of the associated blanket order line.</span><span class="sxs-lookup"><span data-stu-id="dc010-132">It is important to remember that the sales order line quantity must not exceed the quantity of the associated blanket order line.</span></span> <span data-ttu-id="dc010-133">Otherwise, posting of the sales order will not be possible.</span><span class="sxs-lookup"><span data-stu-id="dc010-133">Otherwise, posting of the sales order will not be possible.</span></span>  
- <span data-ttu-id="dc010-134">When the sales order is posted as shipped and/or invoiced, the **Quantity Shipped** and **Quantity Invoiced** fields are updated on the related blanket order.</span><span class="sxs-lookup"><span data-stu-id="dc010-134">When the sales order is posted as shipped and/or invoiced, the **Quantity Shipped** and **Quantity Invoiced** fields are updated on the related blanket order.</span></span>  
- <span data-ttu-id="dc010-135">The blanket order number and line number are recorded as properties of the sales lines when created from a blanket order.</span><span class="sxs-lookup"><span data-stu-id="dc010-135">The blanket order number and line number are recorded as properties of the sales lines when created from a blanket order.</span></span>  
- <span data-ttu-id="dc010-136">When sales orders are not created directly from the blanket order but still relate to it, a link between a sales order and a blanket order can be established by entering the associated blanket order number in the **Blanket Order No.**</span><span class="sxs-lookup"><span data-stu-id="dc010-136">When sales orders are not created directly from the blanket order but still relate to it, a link between a sales order and a blanket order can be established by entering the associated blanket order number in the **Blanket Order No.**</span></span> <span data-ttu-id="dc010-137">field on the sales order line.</span><span class="sxs-lookup"><span data-stu-id="dc010-137">field on the sales order line.</span></span>  
- <span data-ttu-id="dc010-138">After the sales order has been created for the total quantity of a blanket order line, no other sales order can be created for the same line.</span><span class="sxs-lookup"><span data-stu-id="dc010-138">After the sales order has been created for the total quantity of a blanket order line, no other sales order can be created for the same line.</span></span> <span data-ttu-id="dc010-139">Users are prevented from entering a quantity in the **Qty. to Ship** field.</span><span class="sxs-lookup"><span data-stu-id="dc010-139">Users are prevented from entering a quantity in the **Qty. to Ship** field.</span></span> <span data-ttu-id="dc010-140">If, however, additional quantities need to be added to a blanket order, the value in the **Quantity** field can be increased and additional orders can then be created.</span><span class="sxs-lookup"><span data-stu-id="dc010-140">If, however, additional quantities need to be added to a blanket order, the value in the **Quantity** field can be increased and additional orders can then be created.</span></span>  
- <span data-ttu-id="dc010-141">The invoiced blanket sales order remains in the system until it is deleted, either by deleting individual blanket orders or by running the **Delete Invoiced Blanket Sales Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="dc010-141">The invoiced blanket sales order remains in the system until it is deleted, either by deleting individual blanket orders or by running the **Delete Invoiced Blanket Sales Orders** batch job.</span></span>  
- <span data-ttu-id="dc010-142">If a customer is also recorded as a contact in the Marketing application area, and if you have specified an interaction template code for blanket sales order in the **Marketing Setup** window, an interaction is recorded in the Interaction Log Entry table when you select **Print** to print the blanket sales order.</span><span class="sxs-lookup"><span data-stu-id="dc010-142">If a customer is also recorded as a contact in the Marketing application area, and if you have specified an interaction template code for blanket sales order in the **Marketing Setup** window, an interaction is recorded in the Interaction Log Entry table when you select **Print** to print the blanket sales order.</span></span>

## <a name="to-view-the-status-of-a-blanket-purchase-order"></a><span data-ttu-id="dc010-143">To view the status of a blanket purchase order</span><span class="sxs-lookup"><span data-stu-id="dc010-143">To view the status of a blanket purchase order</span></span>  
<span data-ttu-id="dc010-144">You can see the status of a blanket sales order in the **Purchase Blanket Order Statistics** window.</span><span class="sxs-lookup"><span data-stu-id="dc010-144">You can see the status of a blanket sales order in the **Purchase Blanket Order Statistics** window.</span></span> <span data-ttu-id="dc010-145">This may be relevant when you start to invoice the order that is created from the blanket purchase order.</span><span class="sxs-lookup"><span data-stu-id="dc010-145">This may be relevant when you start to invoice the order that is created from the blanket purchase order.</span></span>  

1.  <span data-ttu-id="dc010-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Purchase Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="dc010-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="dc010-147">Select a blanket purchase order, and then choose the **Statistics** action.</span><span class="sxs-lookup"><span data-stu-id="dc010-147">Select a blanket purchase order, and then choose the **Statistics** action.</span></span>  
3.  <span data-ttu-id="dc010-148">In the **Purchase Blanket Order Statistics** window, on the **General** FastTab, you can see summary information about the entire order based on the total quantity in the various **Quantity fields** on the blanket purchase order lines.</span><span class="sxs-lookup"><span data-stu-id="dc010-148">In the **Purchase Blanket Order Statistics** window, on the **General** FastTab, you can see summary information about the entire order based on the total quantity in the various **Quantity fields** on the blanket purchase order lines.</span></span>  

    - <span data-ttu-id="dc010-149">On the **Invoicing** FastTab, you can see summary information based on the total quantity in the **Qty. to Invoice** fields on the purchase blanket order lines.</span><span class="sxs-lookup"><span data-stu-id="dc010-149">On the **Invoicing** FastTab, you can see summary information based on the total quantity in the **Qty. to Invoice** fields on the purchase blanket order lines.</span></span>  
    - <span data-ttu-id="dc010-150">On the **Shipping** FastTab, you can see summary information based on the total quantity in the **Qty. to Receive** fields on the purchase blanket order lines.</span><span class="sxs-lookup"><span data-stu-id="dc010-150">On the **Shipping** FastTab, you can see summary information based on the total quantity in the **Qty. to Receive** fields on the purchase blanket order lines.</span></span>  
    - <span data-ttu-id="dc010-151">On the **Prepayment** FastTab, you can see summary information about any prepaid amounts.</span><span class="sxs-lookup"><span data-stu-id="dc010-151">On the **Prepayment** FastTab, you can see summary information about any prepaid amounts.</span></span>  
    - <span data-ttu-id="dc010-152">On the **Vendor** FastTab, you can see certain basic information about the vendor.</span><span class="sxs-lookup"><span data-stu-id="dc010-152">On the **Vendor** FastTab, you can see certain basic information about the vendor.</span></span>    

## <a name="to-view-unposted-and-posted-blanket-sales-order-lines"></a><span data-ttu-id="dc010-153">To view unposted and posted blanket sales order lines</span><span class="sxs-lookup"><span data-stu-id="dc010-153">To view unposted and posted blanket sales order lines</span></span>   
<span data-ttu-id="dc010-154">The link between the blanket sales order and the originating sales order, and any other sales document, is retained after posting as a list of posted and unposted sales order invoice lines.</span><span class="sxs-lookup"><span data-stu-id="dc010-154">The link between the blanket sales order and the originating sales order, and any other sales document, is retained after posting as a list of posted and unposted sales order invoice lines.</span></span>  

1. <span data-ttu-id="dc010-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon enter **Blanket Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="dc010-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon enter **Blanket Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="dc010-156">Open the blanket sales order you want to view.</span><span class="sxs-lookup"><span data-stu-id="dc010-156">Open the blanket sales order you want to view.</span></span>
3. <span data-ttu-id="dc010-157">To view unposted entries, select the line in question, choose the **Line** action, and then choose the **Unposted Lines** action.</span><span class="sxs-lookup"><span data-stu-id="dc010-157">To view unposted entries, select the line in question, choose the **Line** action, and then choose the **Unposted Lines** action.</span></span> <span data-ttu-id="dc010-158">Choose one of the following options.</span><span class="sxs-lookup"><span data-stu-id="dc010-158">Choose one of the following options.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="dc010-159">Option</span><span class="sxs-lookup"><span data-stu-id="dc010-159">Option</span></span></th>
    <th><span data-ttu-id="dc010-160">Description</span><span class="sxs-lookup"><span data-stu-id="dc010-160">Description</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-161">**Orders**</span><span class="sxs-lookup"><span data-stu-id="dc010-161">**Orders**</span></span></td>
    <td><span data-ttu-id="dc010-162">Specifies open orders associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-162">Specifies open orders associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-163">**Invoices**</span><span class="sxs-lookup"><span data-stu-id="dc010-163">**Invoices**</span></span></td>
    <td><span data-ttu-id="dc010-164">Specifies open invoices that have been associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-164">Specifies open invoices that have been associated with the selected line.</span></span> <span data-ttu-id="dc010-165">Open invoices are manually associated with a blanket order by entering the blanket order number on the sales invoice line.</span><span class="sxs-lookup"><span data-stu-id="dc010-165">Open invoices are manually associated with a blanket order by entering the blanket order number on the sales invoice line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-166">**Return Orders**</span><span class="sxs-lookup"><span data-stu-id="dc010-166">**Return Orders**</span></span></td>
    <td><span data-ttu-id="dc010-167">Specifies open return orders that have been associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-167">Specifies open return orders that have been associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-168">**Credit Memos**</span><span class="sxs-lookup"><span data-stu-id="dc010-168">**Credit Memos**</span></span></td>
    <td><span data-ttu-id="dc010-169">Specifies open credit memos that have been associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-169">Specifies open credit memos that have been associated with the selected line.</span></span></td>
    </tr>
    </table><span data-ttu-id="dc010-170">
4. To view posted entries, select the line in question, choose the **Line** action, and then choose the **Posted Lines** action.</span><span class="sxs-lookup"><span data-stu-id="dc010-170">
4. To view posted entries, select the line in question, choose the **Line** action, and then choose the **Posted Lines** action.</span></span> <span data-ttu-id="dc010-171">Choose one of the following options.</span><span class="sxs-lookup"><span data-stu-id="dc010-171">Choose one of the following options.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="dc010-172">Option</span><span class="sxs-lookup"><span data-stu-id="dc010-172">Option</span></span></th>
    <th><span data-ttu-id="dc010-173">Description</span><span class="sxs-lookup"><span data-stu-id="dc010-173">Description</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-174">**Shipments**</span><span class="sxs-lookup"><span data-stu-id="dc010-174">**Shipments**</span></span></td>
    <td><span data-ttu-id="dc010-175">Posted shipments associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-175">Posted shipments associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-176">**Invoices**</span><span class="sxs-lookup"><span data-stu-id="dc010-176">**Invoices**</span></span></td>
    <td><span data-ttu-id="dc010-177">Posted invoices associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-177">Posted invoices associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-178">**Return Receipts**</span><span class="sxs-lookup"><span data-stu-id="dc010-178">**Return Receipts**</span></span></td>
    <td><span data-ttu-id="dc010-179">Posted return receipts that have been associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-179">Posted return receipts that have been associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="dc010-180">**Credit Memos**</span><span class="sxs-lookup"><span data-stu-id="dc010-180">**Credit Memos**</span></span></td>
    <td><span data-ttu-id="dc010-181">Posted credit memos that have been associated with the selected line.</span><span class="sxs-lookup"><span data-stu-id="dc010-181">Posted credit memos that have been associated with the selected line.</span></span></td>
    </tr>
    </table><span data-ttu-id="dc010-182">
5. In the **Sales Lines** window, choose the **Show Document** action to view the entry.</span><span class="sxs-lookup"><span data-stu-id="dc010-182">
5. In the **Sales Lines** window, choose the **Show Document** action to view the entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="dc010-183">See Also</span><span class="sxs-lookup"><span data-stu-id="dc010-183">See Also</span></span>
[<span data-ttu-id="dc010-184">Sales</span><span class="sxs-lookup"><span data-stu-id="dc010-184">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="dc010-185">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="dc010-185">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="dc010-186">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dc010-186">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

