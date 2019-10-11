---
title: Apply Entries in Different Currencies| Microsoft Docs
description: You can apply ledger entries in multiple currencies, for example, if you sell in one currency and receive payment in another.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 56e225ba1de59f596bc9fd54f924d1ca783d3599
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302238"
---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="18e0f-103">Enable Application of Ledger Entries in Different Currencies</span><span class="sxs-lookup"><span data-stu-id="18e0f-103">Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="18e0f-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span><span class="sxs-lookup"><span data-stu-id="18e0f-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="18e0f-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="18e0f-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="18e0f-106">The following procedure describes how to set this up for vendor ledger entries on the **Purchases & Payables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="18e0f-106">The following procedure describes how to set this up for vendor ledger entries on the **Purchases & Payables Setup** page.</span></span> <span data-ttu-id="18e0f-107">The setup is similar for customer ledger entries on the **Sales & Receivables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="18e0f-107">The setup is similar for customer ledger entries on the **Sales & Receivables Setup** page.</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="18e0f-108">To enable application of vendor ledger entries in different currencies</span><span class="sxs-lookup"><span data-stu-id="18e0f-108">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="18e0f-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18e0f-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="18e0f-110">In the **Appln. between Currencies** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="18e0f-110">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="18e0f-111">Option</span><span class="sxs-lookup"><span data-stu-id="18e0f-111">Option</span></span> | <span data-ttu-id="18e0f-112">Description</span><span class="sxs-lookup"><span data-stu-id="18e0f-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="18e0f-113">None</span><span class="sxs-lookup"><span data-stu-id="18e0f-113">None</span></span> |<span data-ttu-id="18e0f-114">Application between currencies is not allowed.</span><span class="sxs-lookup"><span data-stu-id="18e0f-114">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="18e0f-115">EMU</span><span class="sxs-lookup"><span data-stu-id="18e0f-115">EMU</span></span> |<span data-ttu-id="18e0f-116">Application between EMU currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="18e0f-116">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="18e0f-117">All</span><span class="sxs-lookup"><span data-stu-id="18e0f-117">All</span></span> |<span data-ttu-id="18e0f-118">Application between all currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="18e0f-118">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="18e0f-119">To set up G/L accounts for currency application rounding differences</span><span class="sxs-lookup"><span data-stu-id="18e0f-119">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="18e0f-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="18e0f-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="18e0f-121">You must set up the general ledger accounts before you complete the task.</span><span class="sxs-lookup"><span data-stu-id="18e0f-121">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="18e0f-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="18e0f-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>

1. <span data-ttu-id="18e0f-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18e0f-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18e0f-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="18e0f-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="18e0f-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18e0f-125">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="18e0f-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span><span class="sxs-lookup"><span data-stu-id="18e0f-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="18e0f-127">See Also</span><span class="sxs-lookup"><span data-stu-id="18e0f-127">See Also</span></span>
[<span data-ttu-id="18e0f-128">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="18e0f-128">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="18e0f-129">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="18e0f-129">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="18e0f-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="18e0f-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
