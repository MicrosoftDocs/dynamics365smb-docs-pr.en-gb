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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: df4f093ded0a55d45c40be15c5888035d6e3b2df
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="create-recurring-sales-and-purchase-lines"></a><span data-ttu-id="894d2-103">Create Recurring Sales and Purchase Lines</span><span class="sxs-lookup"><span data-stu-id="894d2-103">Create Recurring Sales and Purchase Lines</span></span>
<span data-ttu-id="894d2-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span><span class="sxs-lookup"><span data-stu-id="894d2-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span></span>  

<span data-ttu-id="894d2-105">The following procedure shows how to work with standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="894d2-105">The following procedure shows how to work with standard sales lines.</span></span> <span data-ttu-id="894d2-106">It works in a similar way for standard purchase lines.</span><span class="sxs-lookup"><span data-stu-id="894d2-106">It works in a similar way for standard purchase lines.</span></span>  

## <a name="to-set-up-standard-sales-lines"></a><span data-ttu-id="894d2-107">To set up standard sales lines</span><span class="sxs-lookup"><span data-stu-id="894d2-107">To set up standard sales lines</span></span>  
1. <span data-ttu-id="894d2-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Sales Lines**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="894d2-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Standard Sales Lines**, and then choose the related link.</span></span>  
2. <span data-ttu-id="894d2-109">In the **Standard Sales Lines** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="894d2-109">In the **Standard Sales Lines** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="894d2-110">On the **General** FastTab, fill the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="894d2-110">On the **General** FastTab, fill the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="894d2-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span><span class="sxs-lookup"><span data-stu-id="894d2-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span></span>  

## <a name="to-insert-standard-sales-lines-on-a-sales-invoice"></a><span data-ttu-id="894d2-112">To insert standard sales lines on a sales invoice</span><span class="sxs-lookup"><span data-stu-id="894d2-112">To insert standard sales lines on a sales invoice</span></span>
1. <span data-ttu-id="894d2-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="894d2-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="894d2-114">Open the sales invoice that you want to insert one or more standard sales lines on.</span><span class="sxs-lookup"><span data-stu-id="894d2-114">Open the sales invoice that you want to insert one or more standard sales lines on.</span></span>
3. <span data-ttu-id="894d2-115">Choose the **Get Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="894d2-115">Choose the **Get Recurring Sales Lines** action.</span></span>
4. <span data-ttu-id="894d2-116">In the **Recurring Sales Lines** window, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="894d2-116">In the **Recurring Sales Lines** window, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span></span>

    > [!NOTE]
    > <span data-ttu-id="894d2-117">To use the recurring sales lines set together with the **Create Recurring Sales Invoices** batch job, you must also fill in the **Valid From Date** and **Valid To Date** fields in the **Recurring Sales Lines** window.</span><span class="sxs-lookup"><span data-stu-id="894d2-117">To use the recurring sales lines set together with the **Create Recurring Sales Invoices** batch job, you must also fill in the **Valid From Date** and **Valid To Date** fields in the **Recurring Sales Lines** window.</span></span> <span data-ttu-id="894d2-118">For more information, see the "To create multiple sales invoices based on standard sales lines" section.</span><span class="sxs-lookup"><span data-stu-id="894d2-118">For more information, see the "To create multiple sales invoices based on standard sales lines" section.</span></span>

5. <span data-ttu-id="894d2-119">Choose the **OK** button to insert the standard sales lines on the invoice where you can reuse them as is or edit the information.</span><span class="sxs-lookup"><span data-stu-id="894d2-119">Choose the **OK** button to insert the standard sales lines on the invoice where you can reuse them as is or edit the information.</span></span>

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a><span data-ttu-id="894d2-120">To create multiple sales invoices based on standard sales lines</span><span class="sxs-lookup"><span data-stu-id="894d2-120">To create multiple sales invoices based on standard sales lines</span></span>
<span data-ttu-id="894d2-121">You can use the **Create Recurring Sales Invoices** batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="894d2-121">You can use the **Create Recurring Sales Invoices** batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales lines.</span></span>

> [!NOTE]
> <span data-ttu-id="894d2-122">In the **Recurring Sales Lines** window, you can also specify a direct-debit payment method and a direct-debit mandate.</span><span class="sxs-lookup"><span data-stu-id="894d2-122">In the **Recurring Sales Lines** window, you can also specify a direct-debit payment method and a direct-debit mandate.</span></span> <span data-ttu-id="894d2-123">The sales invoices that are created with the **Create Recurring Sales Inv.** batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span><span class="sxs-lookup"><span data-stu-id="894d2-123">The sales invoices that are created with the **Create Recurring Sales Inv.** batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span></span> <span data-ttu-id="894d2-124">For more information, see [Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md).</span><span class="sxs-lookup"><span data-stu-id="894d2-124">For more information, see [Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md).</span></span>

1. <span data-ttu-id="894d2-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="894d2-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="894d2-126">In the **Create Recurring Sales Invoices** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="894d2-126">In the **Create Recurring Sales Invoices** window, fill in the fields as necessary.</span></span>
3. <span data-ttu-id="894d2-127">In the **Code** filter field, enter the code for standard sales lines that are assigned to a customer that you want to create sales invoices for.</span><span class="sxs-lookup"><span data-stu-id="894d2-127">In the **Code** filter field, enter the code for standard sales lines that are assigned to a customer that you want to create sales invoices for.</span></span>
4. <span data-ttu-id="894d2-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="894d2-128">Choose the **OK** button.</span></span>

<span data-ttu-id="894d2-129">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span><span class="sxs-lookup"><span data-stu-id="894d2-129">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span></span>

## <a name="see-also"></a><span data-ttu-id="894d2-130">See Also</span><span class="sxs-lookup"><span data-stu-id="894d2-130">See Also</span></span>  
[<span data-ttu-id="894d2-131">Sales</span><span class="sxs-lookup"><span data-stu-id="894d2-131">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="894d2-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="894d2-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

