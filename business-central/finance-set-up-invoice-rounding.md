---
title: Set Up Invoice Rounding | Microsoft Docs
description: You can round invoice amounts when you create invoices. Additionally, local regulations or custom may require you to round in a specific way, for example, to an amount divisible by 0.05.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 302552a32e2c6322c156a22095c926dee40b4cf7
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4746598"
---
# <a name="set-up-invoice-rounding"></a><span data-ttu-id="a92df-104">Set Up Invoice Rounding</span><span class="sxs-lookup"><span data-stu-id="a92df-104">Set Up Invoice Rounding</span></span>
<span data-ttu-id="a92df-105">If you need to round invoice amounts when you create invoices, you can use the automatic rounding function.</span><span class="sxs-lookup"><span data-stu-id="a92df-105">If you need to round invoice amounts when you create invoices, you can use the automatic rounding function.</span></span> <span data-ttu-id="a92df-106">When an invoice is rounded, an extra line is added with the rounding amount and posted with the other invoice lines.</span><span class="sxs-lookup"><span data-stu-id="a92df-106">When an invoice is rounded, an extra line is added with the rounding amount and posted with the other invoice lines.</span></span>

> [!NOTE]  
>  <span data-ttu-id="a92df-107">Local regulations or local custom may require the invoice to be rounded in a specific way, for example, to an amount divisible by 0.05.</span><span class="sxs-lookup"><span data-stu-id="a92df-107">Local regulations or local custom may require the invoice to be rounded in a specific way, for example, to an amount divisible by 0.05.</span></span>  

<span data-ttu-id="a92df-108">To use automatic invoice rounding, you must:</span><span class="sxs-lookup"><span data-stu-id="a92df-108">To use automatic invoice rounding, you must:</span></span>  

* <span data-ttu-id="a92df-109">Specify the general ledger accounts to which rounding differences will be posted.</span><span class="sxs-lookup"><span data-stu-id="a92df-109">Specify the general ledger accounts to which rounding differences will be posted.</span></span>  
* <span data-ttu-id="a92df-110">Set up rules for rounding invoices in local currency and in foreign currency.</span><span class="sxs-lookup"><span data-stu-id="a92df-110">Set up rules for rounding invoices in local currency and in foreign currency.</span></span>  
* <span data-ttu-id="a92df-111">Activate the function.</span><span class="sxs-lookup"><span data-stu-id="a92df-111">Activate the function.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a92df-112">In addition to the invoice rounding features, you can round amounts on invoices by the unit-amount rounding feature and the amount rounding feature.</span><span class="sxs-lookup"><span data-stu-id="a92df-112">In addition to the invoice rounding features, you can round amounts on invoices by the unit-amount rounding feature and the amount rounding feature.</span></span>  

## <a name="set-up-general-ledger-accounts-for-invoice-rounding-differences"></a><span data-ttu-id="a92df-113">Set up general ledger accounts for invoice rounding differences</span><span class="sxs-lookup"><span data-stu-id="a92df-113">Set up general ledger accounts for invoice rounding differences</span></span>
<span data-ttu-id="a92df-114">To use the automatic invoice rounding function, you must set up the general ledger account or accounts where rounding differences will be posted.</span><span class="sxs-lookup"><span data-stu-id="a92df-114">To use the automatic invoice rounding function, you must set up the general ledger account or accounts where rounding differences will be posted.</span></span> <span data-ttu-id="a92df-115">Before you can do this, you must set up VAT product posting groups.</span><span class="sxs-lookup"><span data-stu-id="a92df-115">Before you can do this, you must set up VAT product posting groups.</span></span> <span data-ttu-id="a92df-116">For more information, see [Set up VAT](finance-setup-vat.md).</span><span class="sxs-lookup"><span data-stu-id="a92df-116">For more information, see [Set up VAT](finance-setup-vat.md).</span></span>  

### <a name="to-set-up-general-ledger-accounts-for-invoice-rounding-differences"></a><span data-ttu-id="a92df-117">To set up general ledger accounts for invoice rounding differences</span><span class="sxs-lookup"><span data-stu-id="a92df-117">To set up general ledger accounts for invoice rounding differences</span></span>  
1. <span data-ttu-id="a92df-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a92df-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a92df-119">On the **Chart of Accounts** page, set up the account and name it **Invoice Rounding** or something similar.</span><span class="sxs-lookup"><span data-stu-id="a92df-119">On the **Chart of Accounts** page, set up the account and name it **Invoice Rounding** or something similar.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="a92df-120">will use the account name as text for invoices that are rounded.</span><span class="sxs-lookup"><span data-stu-id="a92df-120">will use the account name as text for invoices that are rounded.</span></span>  
3. <span data-ttu-id="a92df-121">Depending on whether you use VAT or sales tax, in the **VAT Prod. Posting Group** or **VAT Prod. Posting Group** fields, choose a posting group for rounded amounts.</span><span class="sxs-lookup"><span data-stu-id="a92df-121">Depending on whether you use VAT or sales tax, in the **Tax Prod. Posting Group** or **VAT Prod. Posting Group** fields, choose a posting group for rounded amounts.</span></span> <span data-ttu-id="a92df-122">You may want to set up a new group code to use for invoice rounding.</span><span class="sxs-lookup"><span data-stu-id="a92df-122">You may want to set up a new group code to use for invoice rounding.</span></span>
4. <span data-ttu-id="a92df-123">Leave the **Gen. Posting Type**, and either the **Tax Bus. Posting Group** or **VAT Bus. Posting Group** fields blank.</span><span class="sxs-lookup"><span data-stu-id="a92df-123">Leave the **Gen. Posting Type**, and either the **Tax Bus. Posting Group** or **VAT Bus. Posting Group** fields blank.</span></span> <!-- Why do we say to leave these blank, when there are a lot of other fields we also leave blank but don't mention? -->  

<span data-ttu-id="a92df-124">Now you can assign the invoice rounding account to posting groups on the **Vendor Posting Groups** page.</span><span class="sxs-lookup"><span data-stu-id="a92df-124">Now you can assign the invoice rounding account to posting groups on the **Vendor Posting Groups** page.</span></span>  <!-- Why only the vendor posting groups? -->

## <a name="set-up-rounding-for-foreign-and-local-currencies"></a><span data-ttu-id="a92df-125">Set up rounding for foreign and local currencies</span><span class="sxs-lookup"><span data-stu-id="a92df-125">Set up rounding for foreign and local currencies</span></span>
<span data-ttu-id="a92df-126">Before you can use the automatic invoice rounding function, you must set up rounding rules for foreign and local currencies.</span><span class="sxs-lookup"><span data-stu-id="a92df-126">Before you can use the automatic invoice rounding function, you must set up rounding rules for foreign and local currencies.</span></span>

### <a name="to-set-up-rounding-for-foreign-currencies"></a><span data-ttu-id="a92df-127">To set up rounding for foreign currencies</span><span class="sxs-lookup"><span data-stu-id="a92df-127">To set up rounding for foreign currencies</span></span>  
1. <span data-ttu-id="a92df-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a92df-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a92df-129">On the **Currencies** page, choose the foreign currency to open the **Currency Card**, and then fill in the **Amount Rounding Precision**, **Unit-Amount Rounding Precision**, **Invoice Rounding Precision** and **Invoice Rounding Type** fields.</span><span class="sxs-lookup"><span data-stu-id="a92df-129">On the **Currencies** page, choose the foreign currency to open the **Currency Card**, and then fill in the **Amount Rounding Precision**, **Unit-Amount Rounding Precision**, **Invoice Rounding Precision** and **Invoice Rounding Type** fields.</span></span>

### <a name="to-set-up-rounding-for-your-local-currency"></a><span data-ttu-id="a92df-130">To set up rounding for your local currency</span><span class="sxs-lookup"><span data-stu-id="a92df-130">To set up rounding for your local currency</span></span>
1. <span data-ttu-id="a92df-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a92df-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a92df-132">On the **General Ledger Setup** page, on the **General** FastTab, fill in the **Inv. Rounding Precision** and **Inv. Rounding Type** fields.</span><span class="sxs-lookup"><span data-stu-id="a92df-132">On the **General Ledger Setup** page, on the **General** FastTab, fill in the **Inv. Rounding Precision** and **Inv. Rounding Type** fields.</span></span>  

## <a name="activate-the-invoice-rounding-function"></a><span data-ttu-id="a92df-133">Activate the invoice rounding function</span><span class="sxs-lookup"><span data-stu-id="a92df-133">Activate the invoice rounding function</span></span>  
<span data-ttu-id="a92df-134">To ensure that sales and purchase invoices are rounded automatically, you must activate the invoice rounding function.</span><span class="sxs-lookup"><span data-stu-id="a92df-134">To ensure that sales and purchase invoices are rounded automatically, you must activate the invoice rounding function.</span></span> <span data-ttu-id="a92df-135">You activate invoice rounding separately for sales and purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="a92df-135">You activate invoice rounding separately for sales and purchase invoices.</span></span>

1. <span data-ttu-id="a92df-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup** or **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a92df-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup** or **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a92df-137">On the **General** FastTab, choose the **Invoice Rounding** check box.</span><span class="sxs-lookup"><span data-stu-id="a92df-137">On the **General** FastTab, choose the **Invoice Rounding** check box.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a92df-138">See Also</span><span class="sxs-lookup"><span data-stu-id="a92df-138">See Also</span></span>  
[<span data-ttu-id="a92df-139">Invoice Sales</span><span class="sxs-lookup"><span data-stu-id="a92df-139">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="a92df-140">Record Purchases</span><span class="sxs-lookup"><span data-stu-id="a92df-140">Record Purchases</span></span>](purchasing-how-record-purchases.md)
