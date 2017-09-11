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
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 035f4c0e98e3b7ba308319c2017568de832e26c5
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="6ebae-103">How to: Enable Application of Ledger Entries in Different Currencies</span><span class="sxs-lookup"><span data-stu-id="6ebae-103">How to: Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="6ebae-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span><span class="sxs-lookup"><span data-stu-id="6ebae-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="6ebae-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span><span class="sxs-lookup"><span data-stu-id="6ebae-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="6ebae-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="6ebae-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="6ebae-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span><span class="sxs-lookup"><span data-stu-id="6ebae-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

> [!NOTE]  
>   <span data-ttu-id="6ebae-108">This functionality requires that your experience is set to **Suite**.</span><span class="sxs-lookup"><span data-stu-id="6ebae-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="6ebae-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="6ebae-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="6ebae-110">To enable application of vendor ledger entries in different currencies</span><span class="sxs-lookup"><span data-stu-id="6ebae-110">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="6ebae-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6ebae-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="6ebae-112">In the **Appln. between Currencies** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="6ebae-112">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="6ebae-113">Option</span><span class="sxs-lookup"><span data-stu-id="6ebae-113">Option</span></span> | <span data-ttu-id="6ebae-114">Description</span><span class="sxs-lookup"><span data-stu-id="6ebae-114">Description</span></span> |
| --- | --- |
| <span data-ttu-id="6ebae-115">None</span><span class="sxs-lookup"><span data-stu-id="6ebae-115">None</span></span> |<span data-ttu-id="6ebae-116">Application between currencies is not allowed.</span><span class="sxs-lookup"><span data-stu-id="6ebae-116">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="6ebae-117">EMU</span><span class="sxs-lookup"><span data-stu-id="6ebae-117">EMU</span></span> |<span data-ttu-id="6ebae-118">Application between EMU currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="6ebae-118">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="6ebae-119">All</span><span class="sxs-lookup"><span data-stu-id="6ebae-119">All</span></span> |<span data-ttu-id="6ebae-120">Application between all currencies is allowed.</span><span class="sxs-lookup"><span data-stu-id="6ebae-120">Application between all currencies is allowed.</span></span> |

## <a name="see-also"></a><span data-ttu-id="6ebae-121">See Also</span><span class="sxs-lookup"><span data-stu-id="6ebae-121">See Also</span></span>
[<span data-ttu-id="6ebae-122">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="6ebae-122">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="6ebae-123">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="6ebae-123">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="6ebae-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6ebae-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

