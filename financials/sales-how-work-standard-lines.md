---
title: Setup and Use Standard Lines for Recurring Sales and Purchases| Microsoft Docs
description: You can set up sales lines and purchase lines that you frequently make and then insert them on sales and purchase documents to quickly fill the lines with standard information.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade, sell, replenishment
ms.date: 07/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 85d15de13739e944ff8817b402b37ae1c7e1b144
ms.openlocfilehash: 980a0646317c2b5c02c0eadcde9ba984c11580c4
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-create-recurring-sales-and-purchase-lines"></a><span data-ttu-id="51bef-103">How to: Create Recurring Sales and Purchase Lines</span><span class="sxs-lookup"><span data-stu-id="51bef-103">How to: Create Recurring Sales and Purchase Lines</span></span>
<span data-ttu-id="51bef-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span><span class="sxs-lookup"><span data-stu-id="51bef-104">If you often need to create sales and purchase lines with similar information, you can set up standard lines that you can then insert on recurring sales and purchase documents, for example, for recurring replenishment orders.</span></span>  

<span data-ttu-id="51bef-105">The following procedure shows how to work with standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="51bef-105">The following procedure shows how to work with standard sales lines.</span></span> <span data-ttu-id="51bef-106">It works in a similar way for standard purchase lines.</span><span class="sxs-lookup"><span data-stu-id="51bef-106">It works in a similar way for standard purchase lines.</span></span>  

## <a name="to-set-up-standard-sales-lines"></a><span data-ttu-id="51bef-107">To set up standard sales lines</span><span class="sxs-lookup"><span data-stu-id="51bef-107">To set up standard sales lines</span></span>  
1. <span data-ttu-id="51bef-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Standard Sales Codes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="51bef-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Standard Sales Codes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="51bef-109">In the **Standard Sales Lines** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="51bef-109">In the **Standard Sales Lines** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="51bef-110">On the **General** FastTab, fill the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="51bef-110">On the **General** FastTab, fill the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="51bef-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span><span class="sxs-lookup"><span data-stu-id="51bef-111">On the **Lines** FastTab, enter information in the fields to prepare sales lines that reflect the standard lines that you expect to use as recurring lines on sales documents.</span></span>  

## <a name="to-insert-standard-sales-lines-on-a-sales-invoice"></a><span data-ttu-id="51bef-112">To insert standard sales lines on a sales invoice</span><span class="sxs-lookup"><span data-stu-id="51bef-112">To insert standard sales lines on a sales invoice</span></span>
1. <span data-ttu-id="51bef-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="51bef-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="51bef-114">Open the sales invoice that you want to insert one or more standard sales lines on.</span><span class="sxs-lookup"><span data-stu-id="51bef-114">Open the sales invoice that you want to insert one or more standard sales lines on.</span></span>
3. <span data-ttu-id="51bef-115">Choose the **Get Recurring Sales Lines** action.</span><span class="sxs-lookup"><span data-stu-id="51bef-115">Choose the **Get Recurring Sales Lines** action.</span></span>
4. <span data-ttu-id="51bef-116">In the **Recurring Sales Lines** window, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span><span class="sxs-lookup"><span data-stu-id="51bef-116">In the **Recurring Sales Lines** window, choose the lookup button in the **Code** field, and then select a set of standard sales lines.</span></span>
5. <span data-ttu-id="51bef-117">Choose the **OK** button to insert the standard sales lines on the invoice, where you can reuse as is or edit the information.</span><span class="sxs-lookup"><span data-stu-id="51bef-117">Choose the **OK** button to insert the standard sales lines on the invoice, where you can reuse as is or edit the information.</span></span>

## <a name="to-create-multiple-sales-invoices-based-on-standard-sales-lines"></a><span data-ttu-id="51bef-118">To create multiple sales invoices based on standard sales lines</span><span class="sxs-lookup"><span data-stu-id="51bef-118">To create multiple sales invoices based on standard sales lines</span></span>
<span data-ttu-id="51bef-119">You can use the **Create Recurring Sales Inv.**</span><span class="sxs-lookup"><span data-stu-id="51bef-119">You can use the **Create Recurring Sales Inv.**</span></span> <span data-ttu-id="51bef-120">batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales code.</span><span class="sxs-lookup"><span data-stu-id="51bef-120">batch job to create sales invoices according to standard sales lines that are assigned to the customers and with posting dates within the valid-from and valid-to dates that you specify on the standard sales code.</span></span>

<span data-ttu-id="51bef-121">In the **Recurring Sales Lines** window, you can also specify a direct-debit payment method and a direct-debit mandate.</span><span class="sxs-lookup"><span data-stu-id="51bef-121">In the **Recurring Sales Lines** window, you can also specify a direct-debit payment method and a direct-debit mandate.</span></span> <span data-ttu-id="51bef-122">The sales invoices that are created with the **Create Recurring Sales Inv.**</span><span class="sxs-lookup"><span data-stu-id="51bef-122">The sales invoices that are created with the **Create Recurring Sales Inv.**</span></span> <span data-ttu-id="51bef-123">batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span><span class="sxs-lookup"><span data-stu-id="51bef-123">batch job will then include information required to collect payment for the sales invoices with SEPA direct debit.</span></span> <span data-ttu-id="51bef-124">For more information, see Collect Payments with SEPA Direct Debit.</span><span class="sxs-lookup"><span data-stu-id="51bef-124">For more information, see Collect Payments with SEPA Direct Debit.</span></span>

1. <span data-ttu-id="51bef-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="51bef-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Recurring Sales Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="51bef-126">In the **Create Recurring Sales Inv.**</span><span class="sxs-lookup"><span data-stu-id="51bef-126">In the **Create Recurring Sales Inv.**</span></span> <span data-ttu-id="51bef-127">window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="51bef-127">window, fill in the fields as necessary.</span></span>
3. <span data-ttu-id="51bef-128">In the **Code** field, enter the code for standard sales lines assigned to a customer that you want to create sales invoices for.</span><span class="sxs-lookup"><span data-stu-id="51bef-128">In the **Code** field, enter the code for standard sales lines assigned to a customer that you want to create sales invoices for.</span></span>
4. <span data-ttu-id="51bef-129">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="51bef-129">Choose the **OK** button.</span></span>

<span data-ttu-id="51bef-130">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span><span class="sxs-lookup"><span data-stu-id="51bef-130">Sales invoices are created for the customers with the specified standard customer sales code, and any specified direct-debit information, for posting on the specified date.</span></span>

## <a name="see-also"></a><span data-ttu-id="51bef-131">See Also</span><span class="sxs-lookup"><span data-stu-id="51bef-131">See Also</span></span>  
[<span data-ttu-id="51bef-132">Sales</span><span class="sxs-lookup"><span data-stu-id="51bef-132">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="51bef-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="51bef-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

