---
title: Use the Suggest Vendor Payments Batch Job| Microsoft Docs
description: You can specify vendor payment settings to get suggestions or proposals for payments that are due soon or where a discount is available.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3bf91f092f911f5544ecb5d442ce3c61bae0be43
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775122"
---
# <a name="suggest-vendor-payments"></a><span data-ttu-id="efeba-103">Suggest Vendor Payments</span><span class="sxs-lookup"><span data-stu-id="efeba-103">Suggest Vendor Payments</span></span>
<span data-ttu-id="efeba-104">On the **Payment Journal** page, you can use the **Suggest Vendor Payments** batch job to suggest payment lines.</span><span class="sxs-lookup"><span data-stu-id="efeba-104">On the **Payment Journal** page, you can use the **Suggest Vendor Payments** batch job to suggest payment lines.</span></span> <span data-ttu-id="efeba-105">Lines for payments that are due soon or payments where a payment discount is available are suggested based on your settings.</span><span class="sxs-lookup"><span data-stu-id="efeba-105">Lines for payments that are due soon or payments where a payment discount is available are suggested based on your settings.</span></span>

<span data-ttu-id="efeba-106">To benefit fully from payment suggestions, you must first prioritise your vendors.</span><span class="sxs-lookup"><span data-stu-id="efeba-106">To benefit fully from payment suggestions, you must first prioritize your vendors.</span></span> <span data-ttu-id="efeba-107">For more information, see [Prioritise Vendors](purchasing-how-prioritize-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="efeba-107">For more information, see [Prioritize Vendors](purchasing-how-prioritize-vendors.md).</span></span>  

> [!NOTE]  
> <span data-ttu-id="efeba-108">Vendor ledger entries that are **On Hold** are not included in the batch job.</span><span class="sxs-lookup"><span data-stu-id="efeba-108">Vendor ledger entries that are **On Hold** are not included in the batch job.</span></span>  

> [!IMPORTANT]  
>   <span data-ttu-id="efeba-109">If you want to take advantage of payment discounts, and have entered an available amount, the amount will be used for:</span><span class="sxs-lookup"><span data-stu-id="efeba-109">If you want to take advantage of payment discounts, and have entered an available amount, the amount will be used for:</span></span>  
    * <span data-ttu-id="efeba-110">Prioritised overdue vendor entries first in order of priority.</span><span class="sxs-lookup"><span data-stu-id="efeba-110">Prioritized overdue vendor entries first in order of priority.</span></span>   
    * <span data-ttu-id="efeba-111">Overdue vendor entries that are not prioritised.</span><span class="sxs-lookup"><span data-stu-id="efeba-111">Overdue vendor entries that are not prioritized.</span></span>  
    * <span data-ttu-id="efeba-112">Open vendor entries that qualify for payment discounts, arranged by vendor number.</span><span class="sxs-lookup"><span data-stu-id="efeba-112">Open vendor entries that qualify for payment discounts, arranged by vendor number.</span></span>  

## <a name="to-use-the-suggest-vendor-payments-function"></a><span data-ttu-id="efeba-113">To use the Suggest Vendor Payments function</span><span class="sxs-lookup"><span data-stu-id="efeba-113">To use the Suggest Vendor Payments function</span></span>
1. <span data-ttu-id="efeba-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="efeba-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="efeba-115">Open the relevant journal, and then choose the **Suggest Vendor Payments** action.</span><span class="sxs-lookup"><span data-stu-id="efeba-115">Open the relevant journal, and then choose the **Suggest Vendor Payments** action.</span></span>  
3. <span data-ttu-id="efeba-116">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="efeba-116">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="efeba-117">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="efeba-117">Choose the **OK** button.</span></span>  

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a><span data-ttu-id="efeba-118">To insert the due date as posting date on payment journal lines</span><span class="sxs-lookup"><span data-stu-id="efeba-118">To insert the due date as posting date on payment journal lines</span></span>
<span data-ttu-id="efeba-119">When you use the **Suggest Vendor Payments** batch job to create payment lines for your vendors, you can fill two special fields to make sure that the generated lines use the due date to calculate the posting date.</span><span class="sxs-lookup"><span data-stu-id="efeba-119">When you use the **Suggest Vendor Payments** batch job to create payment lines for your vendors, you can fill two special fields to make sure that the generated lines use the due date to calculate the posting date.</span></span> <span data-ttu-id="efeba-120">These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.</span><span class="sxs-lookup"><span data-stu-id="efeba-120">These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.</span></span>  

> [!IMPORTANT]  
>   <span data-ttu-id="efeba-121">You cannot use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarise per Vendor** field.</span><span class="sxs-lookup"><span data-stu-id="efeba-121">You cannot use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarize per Vendor** field.</span></span> <span data-ttu-id="efeba-122">If the posting date is based on the due date, some payment discounts may not calculate correctly because the posting date is after the payment discount date.</span><span class="sxs-lookup"><span data-stu-id="efeba-122">If the posting date is based on the due date, some payment discounts may not calculate correctly because the posting date is after the payment discount date.</span></span>  

<span data-ttu-id="efeba-123">Also, if the calculated posting date is in the past, then the posting date is moved up to the work date, and a warning is displayed.</span><span class="sxs-lookup"><span data-stu-id="efeba-123">Also, if the calculated posting date is in the past, then the posting date is moved up to the work date, and a warning is displayed.</span></span>  

<span data-ttu-id="efeba-124">Alternatively, you can manually create payment lines using the due date to calculate the posting date.</span><span class="sxs-lookup"><span data-stu-id="efeba-124">Alternatively, you can manually create payment lines using the due date to calculate the posting date.</span></span> <span data-ttu-id="efeba-125">After you apply vendor ledger entries, you can use the **Calculate Posting Date** action to update the posting date on the journal line with the due date of the related purchase invoice.</span><span class="sxs-lookup"><span data-stu-id="efeba-125">After you apply vendor ledger entries, you can use the **Calculate Posting Date** action to update the posting date on the journal line with the due date of the related purchase invoice.</span></span> <span data-ttu-id="efeba-126">For more information, see [Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="efeba-126">For more information, see [Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).</span></span>  

> [!NOTE]  
>   <span data-ttu-id="efeba-127">If the purchase invoice is overdue, the posting date is set to the work date, and the font on the line becomes red.</span><span class="sxs-lookup"><span data-stu-id="efeba-127">If the purchase invoice is overdue, the posting date is set to the work date, and the font on the line becomes red.</span></span>  

## <a name="see-also"></a><span data-ttu-id="efeba-128">See Also</span><span class="sxs-lookup"><span data-stu-id="efeba-128">See Also</span></span>
[<span data-ttu-id="efeba-129">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="efeba-129">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="efeba-130">Making Payments</span><span class="sxs-lookup"><span data-stu-id="efeba-130">Making Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="efeba-131">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="efeba-131">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="efeba-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="efeba-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]