---
title: Apply Entries in Different Currencies| Microsoft Docs
description: You can apply ledger entries in multiple currencies, for example, if you sell in one currency and receive payment in another.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 6379aea58ab7943b117e5b19b22f71193290c2cb
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="b970b-103">How to: Enable Application of Ledger Entries in Different Currencies</span><span class="sxs-lookup"><span data-stu-id="b970b-103">How to: Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="b970b-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span><span class="sxs-lookup"><span data-stu-id="b970b-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="b970b-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="b970b-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="b970b-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="b970b-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="b970b-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="b970b-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

> [!NOTE]  
>   <span data-ttu-id="b970b-108">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="b970b-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="b970b-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="b970b-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="b970b-110">To enable application of vendor ledger entries in different currencies</span><span class="sxs-lookup"><span data-stu-id="b970b-110">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="b970b-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b970b-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="b970b-112">In the **Appln. between Currencies** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="b970b-112">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="b970b-113">Option</span><span class="sxs-lookup"><span data-stu-id="b970b-113">Option</span></span> | <span data-ttu-id="b970b-114">Description</span><span class="sxs-lookup"><span data-stu-id="b970b-114">Description</span></span> |
| --- | --- |
| <span data-ttu-id="b970b-115">None</span><span class="sxs-lookup"><span data-stu-id="b970b-115">None</span></span> |<span data-ttu-id="b970b-116">Application between currencies is not allowed.</span><span class="sxs-lookup"><span data-stu-id="b970b-116">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="b970b-117">EMU</span><span class="sxs-lookup"><span data-stu-id="b970b-117">EMU</span></span> |<span data-ttu-id="b970b-118">Application between EMU currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="b970b-118">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="b970b-119">All</span><span class="sxs-lookup"><span data-stu-id="b970b-119">All</span></span> |<span data-ttu-id="b970b-120">Application between all currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="b970b-120">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="b970b-121">To set up G/L accounts for currency application rounding differences</span><span class="sxs-lookup"><span data-stu-id="b970b-121">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="b970b-122">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="b970b-122">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="b970b-123">You must set up the general ledger accounts before you complete the task.</span><span class="sxs-lookup"><span data-stu-id="b970b-123">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="b970b-124">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="b970b-124">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span> 
  
1. <span data-ttu-id="b970b-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b970b-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b970b-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="b970b-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="b970b-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b970b-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="b970b-128">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="b970b-128">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b970b-129">See Also</span><span class="sxs-lookup"><span data-stu-id="b970b-129">See Also</span></span>
[<span data-ttu-id="b970b-130">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="b970b-130">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="b970b-131">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="b970b-131">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="b970b-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b970b-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

