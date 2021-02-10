---
title: How to Create Prepayment Invoices | Microsoft Docs
description: Learn how to handle situations where you require prepayment, or your vendor does.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5f227cc73531111ae15f69d6fba5ac541e28560c
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4746873"
---
# <a name="create-prepayment-invoices"></a><span data-ttu-id="4376a-103">Create Prepayment Invoices</span><span class="sxs-lookup"><span data-stu-id="4376a-103">Create Prepayment Invoices</span></span>

<span data-ttu-id="4376a-104">If you require your customers to submit payment before you ship an order to them, you can use the prepayment functionality.</span><span class="sxs-lookup"><span data-stu-id="4376a-104">If you require your customers to submit payment before you ship an order to them, you can use the prepayment functionality.</span></span> <span data-ttu-id="4376a-105">The same applies if your vendor requires you to submit payment before they ship an order to you.</span><span class="sxs-lookup"><span data-stu-id="4376a-105">The same applies if your vendor requires you to submit payment before they ship an order to you.</span></span>  

<span data-ttu-id="4376a-106">You can start the prepayment process when you create a sales or purchase order.</span><span class="sxs-lookup"><span data-stu-id="4376a-106">You can start the prepayment process when you create a sales or purchase order.</span></span> <span data-ttu-id="4376a-107">If you have a default prepayment percentage for this customer or vendor, that will be included automatically in the resulting prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="4376a-107">If you have a default prepayment percentage for this customer or vendor, that will be included automatically in the resulting prepayment invoice.</span></span> <span data-ttu-id="4376a-108">You can also specify a prepayment percentage to the entire document.</span><span class="sxs-lookup"><span data-stu-id="4376a-108">You can also specify a prepayment percentage to the entire document.</span></span>

<span data-ttu-id="4376a-109">After you create a sales or purchase order, you can create a prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="4376a-109">After you create a sales or purchase order, you can create a prepayment invoice.</span></span> <span data-ttu-id="4376a-110">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span><span class="sxs-lookup"><span data-stu-id="4376a-110">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span></span> <span data-ttu-id="4376a-111">For example, you can specify a total amount for the entire order.</span><span class="sxs-lookup"><span data-stu-id="4376a-111">For example, you can specify a total amount for the entire order.</span></span>  

<span data-ttu-id="4376a-112">The following procedure describes how to invoice a prepayment for a sales order.</span><span class="sxs-lookup"><span data-stu-id="4376a-112">The following procedure describes how to invoice a prepayment for a sales order.</span></span> <span data-ttu-id="4376a-113">The steps are similar for purchase orders.</span><span class="sxs-lookup"><span data-stu-id="4376a-113">The steps are similar for purchase orders.</span></span>  

## <a name="to-create-a-prepayment-invoice"></a><span data-ttu-id="4376a-114">To create a prepayment invoice</span><span class="sxs-lookup"><span data-stu-id="4376a-114">To create a prepayment invoice</span></span>

1. <span data-ttu-id="4376a-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4376a-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="4376a-116">Create a new sales order for the relevant customer.</span><span class="sxs-lookup"><span data-stu-id="4376a-116">Create a new sales order for the relevant customer.</span></span> <span data-ttu-id="4376a-117">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="4376a-117">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>  

    <span data-ttu-id="4376a-118">On the **Prepayment** FastTab, the **Prepayment %** field specifies the percentage to use to calculate the prepayment amount.</span><span class="sxs-lookup"><span data-stu-id="4376a-118">On the **Prepayment** FastTab, the **Prepayment %** field specifies the percentage to use to calculate the prepayment amount.</span></span> <span data-ttu-id="4376a-119">If there is a default prepayment percentage on the customer card, the field is filled in automatically.</span><span class="sxs-lookup"><span data-stu-id="4376a-119">If there is a default prepayment percentage on the customer card, the field is filled in automatically.</span></span> <span data-ttu-id="4376a-120">You can change the percentage.</span><span class="sxs-lookup"><span data-stu-id="4376a-120">You can change the percentage.</span></span> <!--This percentage is applied to lines where the item on that line does not already specify a prepayment percentage. The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.-->  

    <span data-ttu-id="4376a-121">Choose the **Compress Prepayment** field if you want to create lines on the prepayment invoice that combine lines from the sales order if:</span><span class="sxs-lookup"><span data-stu-id="4376a-121">Choose the **Compress Prepayment** field if you want to create lines on the prepayment invoice that combine lines from the sales order if:</span></span>  

    - <span data-ttu-id="4376a-122">They have the same general ledger account for prepayments as determined by the general posting setup.</span><span class="sxs-lookup"><span data-stu-id="4376a-122">They have the same general ledger account for prepayments as determined by the general posting setup.</span></span>  
    - <span data-ttu-id="4376a-123">They have the same dimensions.</span><span class="sxs-lookup"><span data-stu-id="4376a-123">They have the same dimensions.</span></span>  

    <span data-ttu-id="4376a-124">If you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage, then do not choose the **Compress Prepayment** field.</span><span class="sxs-lookup"><span data-stu-id="4376a-124">If you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage, then do not choose the **Compress Prepayment** field.</span></span>  

    <span data-ttu-id="4376a-125">The due date for the prepayment is calculated automatically based on the value of the **Prepmt. Payment Terms Code**.</span><span class="sxs-lookup"><span data-stu-id="4376a-125">The due date for the prepayment is calculated automatically based on the value of the **Prepmt. Payment Terms Code**.</span></span>

3. <span data-ttu-id="4376a-126">Fill in the sales lines.</span><span class="sxs-lookup"><span data-stu-id="4376a-126">Fill in the sales lines.</span></span>  

    <span data-ttu-id="4376a-127">If you have specified a default prepayment percentage either for the customer or on the **Prepayment** FastTab on this document, this value is copied to each line.</span><span class="sxs-lookup"><span data-stu-id="4376a-127">If you have specified a default prepayment percentage either for the customer or on the **Prepayment** FastTab on this document, this value is copied to each line.</span></span> <span data-ttu-id="4376a-128">You can change the contents of the **Prepayment %** field on the line.</span><span class="sxs-lookup"><span data-stu-id="4376a-128">You can change the contents of the **Prepayment %** field on the line.</span></span>  

4. <span data-ttu-id="4376a-129">To view the total prepayment amount, choose the **Statistics** action.</span><span class="sxs-lookup"><span data-stu-id="4376a-129">To view the total prepayment amount, choose the **Statistics** action.</span></span>

    <span data-ttu-id="4376a-130">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span><span class="sxs-lookup"><span data-stu-id="4376a-130">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field on the **Sales Order Statistics** page.</span></span>  

    <span data-ttu-id="4376a-131">If the **Prices Including VAT** field is selected, the **Prepayment Amount Incl. VAT** field is editable.</span><span class="sxs-lookup"><span data-stu-id="4376a-131">If the **Prices Including VAT** field is selected, the **Prepayment Amount Incl. VAT** field is editable.</span></span>  

    <span data-ttu-id="4376a-132">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span><span class="sxs-lookup"><span data-stu-id="4376a-132">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span></span>  

5. <span data-ttu-id="4376a-133">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span><span class="sxs-lookup"><span data-stu-id="4376a-133">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span></span>  
6. <span data-ttu-id="4376a-134">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="4376a-134">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span></span>  

    <span data-ttu-id="4376a-135">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span><span class="sxs-lookup"><span data-stu-id="4376a-135">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span></span>  

<span data-ttu-id="4376a-136">You can issue additional prepayment invoices for the order.</span><span class="sxs-lookup"><span data-stu-id="4376a-136">You can issue additional prepayment invoices for the order.</span></span> <span data-ttu-id="4376a-137">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span><span class="sxs-lookup"><span data-stu-id="4376a-137">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span></span> <span data-ttu-id="4376a-138">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span><span class="sxs-lookup"><span data-stu-id="4376a-138">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span></span>  

> [!NOTE]  
> <span data-ttu-id="4376a-139">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span><span class="sxs-lookup"><span data-stu-id="4376a-139">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span></span> <span data-ttu-id="4376a-140">This is prevented in the North American version of [!INCLUDE[prod_short](includes/prod_short.md)] because the calculation of sales tax will otherwise be incorrect.</span><span class="sxs-lookup"><span data-stu-id="4376a-140">This is prevented in the North American version of [!INCLUDE[prod_short](includes/prod_short.md)] because the calculation of sales tax will otherwise be incorrect.</span></span>  

 <span data-ttu-id="4376a-141">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span><span class="sxs-lookup"><span data-stu-id="4376a-141">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4376a-142">See Also</span><span class="sxs-lookup"><span data-stu-id="4376a-142">See Also</span></span>

[<span data-ttu-id="4376a-143">Invoicing Prepayments</span><span class="sxs-lookup"><span data-stu-id="4376a-143">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="4376a-144">Walkthrough: Setting Up and Invoicing Sales Prepayments</span><span class="sxs-lookup"><span data-stu-id="4376a-144">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="4376a-145">Finance</span><span class="sxs-lookup"><span data-stu-id="4376a-145">Finance</span></span>](finance.md)  
<span data-ttu-id="4376a-146">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4376a-146">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
