---
title: Setup Standard Lines for Recurring Sales and Purchases| Microsoft Docs
description: You can set up sales lines and purchase lines that you frequently make and then insert them on sales and purchase documents to quickly fill the lines with standard information.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, replenishment
ms.date: 10/24/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: f8c8f96e73f6ba119e4345c8ba12c895dd212da3
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="create-recurring-sales-and-purchase-lines"></a><span data-ttu-id="af3c7-103">Create Recurring Sales and Purchase Lines</span><span class="sxs-lookup"><span data-stu-id="af3c7-103">Create Recurring Sales and Purchase Lines</span></span>
<span data-ttu-id="af3c7-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span><span class="sxs-lookup"><span data-stu-id="af3c7-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span></span>  

<span data-ttu-id="af3c7-105">The following procedures show how to work with standard sales lines on a sales invoice.</span><span class="sxs-lookup"><span data-stu-id="af3c7-105">The following procedures show how to work with standard sales lines on a sales invoice.</span></span> <span data-ttu-id="af3c7-106">It works in a similar way for all other sales documents and for all purchase documents.</span><span class="sxs-lookup"><span data-stu-id="af3c7-106">It works in a similar way for all other sales documents and for all purchase documents.</span></span>  

## <a name="to-set-up-standard-sales-lines"></a><span data-ttu-id="af3c7-107">To set up standard sales lines</span><span class="sxs-lookup"><span data-stu-id="af3c7-107">To set up standard sales lines</span></span>  
1. <span data-ttu-id="af3c7-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Sales Lines**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="af3c7-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Sales Lines**, and then choose the related link.</span></span>  
2. <span data-ttu-id="af3c7-109">On the **Standard Sales Lines** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="af3c7-109">On the **Standard Sales Lines** page, choose the **New** action.</span></span>  
3. <span data-ttu-id="af3c7-110">On the **General** FastTab, fill the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="af3c7-110">On the **General** FastTab, fill the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="af3c7-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span><span class="sxs-lookup"><span data-stu-id="af3c7-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span></span>  

> [!NOTE]
> <span data-ttu-id="af3c7-112">You cannot define prices on standard sales lines because prices, discounts, etc. are calculated on the actual sales documents after you insert the standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="af3c7-112">You cannot define prices on standard sales lines because prices, discounts, etc. are calculated on the actual sales documents after you insert the standard sales lines.</span></span>

## <a name="to-assign-standard-sales-lines-to-a-customers"></a><span data-ttu-id="af3c7-113">To assign standard sales lines to a customers</span><span class="sxs-lookup"><span data-stu-id="af3c7-113">To assign standard sales lines to a customers</span></span>
<span data-ttu-id="af3c7-114">Assign one or more standard sales lines to a customer so that they are available to insert on sales documents for that customer.</span><span class="sxs-lookup"><span data-stu-id="af3c7-114">Assign one or more standard sales lines to a customer so that they are available to insert on sales documents for that customer.</span></span>

1. <span data-ttu-id="af3c7-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="af3c7-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="af3c7-116">Open the card for a relevant customer.</span><span class="sxs-lookup"><span data-stu-id="af3c7-116">Open the card for a relevant customer.</span></span>
3. <span data-ttu-id="af3c7-117">Choose the **Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="af3c7-117">Choose the **Recurring Sales Lines** action.</span></span>
4. <span data-ttu-id="af3c7-118">On the **Recurring Sales Lines** page, select codes for the recurring sales lines that you want to be able to insert on sales documents for the customer.</span><span class="sxs-lookup"><span data-stu-id="af3c7-118">On the **Recurring Sales Lines** page, select codes for the recurring sales lines that you want to be able to insert on sales documents for the customer.</span></span>
5. <span data-ttu-id="af3c7-119">Fill in the additional fields to define when, how, and where the recurring sales lines are to be used.</span><span class="sxs-lookup"><span data-stu-id="af3c7-119">Fill in the additional fields to define when, how, and where the recurring sales lines are to be used.</span></span> [!INCLUDE [tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-insert-recurring-sales-lines-on-a-sales-invoice"></a><span data-ttu-id="af3c7-120">To insert recurring sales lines on a sales invoice</span><span class="sxs-lookup"><span data-stu-id="af3c7-120">To insert recurring sales lines on a sales invoice</span></span>
<span data-ttu-id="af3c7-121">If recurring sales lines exist for the customer, you can insert them on all types of sales documents, such as a sales invoice.</span><span class="sxs-lookup"><span data-stu-id="af3c7-121">If recurring sales lines exist for the customer, you can insert them on all types of sales documents, such as a sales invoice.</span></span> <span data-ttu-id="af3c7-122">If you have activated the notification in question, you will be informed if recurring sales lines exist.</span><span class="sxs-lookup"><span data-stu-id="af3c7-122">If you have activated the notification in question, you will be informed if recurring sales lines exist.</span></span>
1. <span data-ttu-id="af3c7-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="af3c7-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="af3c7-124">Open the sales invoice that you want to insert one or more standard sales lines on.</span><span class="sxs-lookup"><span data-stu-id="af3c7-124">Open the sales invoice that you want to insert one or more standard sales lines on.</span></span>
3. <span data-ttu-id="af3c7-125">Choose the **Get Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="af3c7-125">Choose the **Get Recurring Sales Lines** action.</span></span>
4. <span data-ttu-id="af3c7-126">On the **Recurring Sales Lines** page, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="af3c7-126">On the **Recurring Sales Lines** page, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span></span>

    > [!NOTE]
    > <span data-ttu-id="af3c7-127">To use the recurring sales lines set together with the **Create Recurring Sales Invoices** batch job, you must also fill in the **Valid From Date** and **Valid To Date** fields on the **Recurring Sales Lines** page.</span><span class="sxs-lookup"><span data-stu-id="af3c7-127">To use the recurring sales lines set together with the **Create Recurring Sales Invoices** batch job, you must also fill in the **Valid From Date** and **Valid To Date** fields on the **Recurring Sales Lines** page.</span></span> <span data-ttu-id="af3c7-128">For more information, see the "To create multiple sales invoices based on standard sales lines" section.</span><span class="sxs-lookup"><span data-stu-id="af3c7-128">For more information, see the "To create multiple sales invoices based on standard sales lines" section.</span></span>

5. <span data-ttu-id="af3c7-129">Choose the **OK** button to insert the standard sales lines on the invoice where you can reuse them as is or edit the information.</span><span class="sxs-lookup"><span data-stu-id="af3c7-129">Choose the **OK** button to insert the standard sales lines on the invoice where you can reuse them as is or edit the information.</span></span>

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a><span data-ttu-id="af3c7-130">To create multiple sales invoices based on standard sales lines</span><span class="sxs-lookup"><span data-stu-id="af3c7-130">To create multiple sales invoices based on standard sales lines</span></span>
<span data-ttu-id="af3c7-131">You can use the **Create Recurring Sales Invoices** batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="af3c7-131">You can use the **Create Recurring Sales Invoices** batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales lines.</span></span>

> [!NOTE]
> <span data-ttu-id="af3c7-132">On the **Recurring Sales Lines** page, you can also specify a direct-debit payment method and a direct-debit mandate.</span><span class="sxs-lookup"><span data-stu-id="af3c7-132">On the **Recurring Sales Lines** page, you can also specify a direct-debit payment method and a direct-debit mandate.</span></span> <span data-ttu-id="af3c7-133">The sales invoices that are created with the **Create Recurring Sales Inv.** batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span><span class="sxs-lookup"><span data-stu-id="af3c7-133">The sales invoices that are created with the **Create Recurring Sales Inv.** batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span></span> <span data-ttu-id="af3c7-134">For more information, see [Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md).</span><span class="sxs-lookup"><span data-stu-id="af3c7-134">For more information, see [Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md).</span></span>

1. <span data-ttu-id="af3c7-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="af3c7-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="af3c7-136">On the **Create Recurring Sales Invoices** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="af3c7-136">On the **Create Recurring Sales Invoices** page, fill in the fields as necessary.</span></span>
3. <span data-ttu-id="af3c7-137">In the **Code** filter field, enter the code for standard sales lines that are assigned to a customer that you want to create sales invoices for.</span><span class="sxs-lookup"><span data-stu-id="af3c7-137">In the **Code** filter field, enter the code for standard sales lines that are assigned to a customer that you want to create sales invoices for.</span></span>
4. <span data-ttu-id="af3c7-138">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="af3c7-138">Choose the **OK** button.</span></span>

<span data-ttu-id="af3c7-139">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span><span class="sxs-lookup"><span data-stu-id="af3c7-139">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span></span>

## <a name="see-also"></a><span data-ttu-id="af3c7-140">See Also</span><span class="sxs-lookup"><span data-stu-id="af3c7-140">See Also</span></span>  
[<span data-ttu-id="af3c7-141">Sales</span><span class="sxs-lookup"><span data-stu-id="af3c7-141">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="af3c7-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="af3c7-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

