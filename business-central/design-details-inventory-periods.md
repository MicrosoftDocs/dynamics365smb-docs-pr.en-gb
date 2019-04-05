---
title: Design Details - Inventory Periods | Microsoft Docs
description: Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed. This can have adverse effects on accurate reporting, especially within global corporations. The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 57f0fa4f62a4c8f52eb1e3e6def8907190f3db8e
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "809384"
---
# <a name="design-details-inventory-periods"></a><span data-ttu-id="2beae-105">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="2beae-105">Design Details: Inventory Periods</span></span>
<span data-ttu-id="2beae-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span><span class="sxs-lookup"><span data-stu-id="2beae-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span></span> <span data-ttu-id="2beae-107">This can have adverse effects on accurate reporting, especially within global corporations.</span><span class="sxs-lookup"><span data-stu-id="2beae-107">This can have adverse effects on accurate reporting, especially within global corporations.</span></span> <span data-ttu-id="2beae-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span><span class="sxs-lookup"><span data-stu-id="2beae-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span></span>  

 <span data-ttu-id="2beae-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span><span class="sxs-lookup"><span data-stu-id="2beae-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span></span> <span data-ttu-id="2beae-110">When you close an inventory period, no value changes can be posted in the closed period.</span><span class="sxs-lookup"><span data-stu-id="2beae-110">When you close an inventory period, no value changes can be posted in the closed period.</span></span> <span data-ttu-id="2beae-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span><span class="sxs-lookup"><span data-stu-id="2beae-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span></span> <span data-ttu-id="2beae-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span><span class="sxs-lookup"><span data-stu-id="2beae-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span></span> <span data-ttu-id="2beae-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span><span class="sxs-lookup"><span data-stu-id="2beae-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span></span>  

 <span data-ttu-id="2beae-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span><span class="sxs-lookup"><span data-stu-id="2beae-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span></span>  

-   <span data-ttu-id="2beae-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span><span class="sxs-lookup"><span data-stu-id="2beae-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span></span>  
-   <span data-ttu-id="2beae-116">All item costs in the period must be adjusted.</span><span class="sxs-lookup"><span data-stu-id="2beae-116">All item costs in the period must be adjusted.</span></span>  
-   <span data-ttu-id="2beae-117">All released and finished production orders in the period must be cost adjusted.</span><span class="sxs-lookup"><span data-stu-id="2beae-117">All released and finished production orders in the period must be cost adjusted.</span></span>  

 <span data-ttu-id="2beae-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span><span class="sxs-lookup"><span data-stu-id="2beae-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span></span> <span data-ttu-id="2beae-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span><span class="sxs-lookup"><span data-stu-id="2beae-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span></span> <span data-ttu-id="2beae-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span><span class="sxs-lookup"><span data-stu-id="2beae-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span></span> <span data-ttu-id="2beae-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span><span class="sxs-lookup"><span data-stu-id="2beae-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span></span> <span data-ttu-id="2beae-122">When you reopen an inventory period, an inventory period entry is created.</span><span class="sxs-lookup"><span data-stu-id="2beae-122">When you reopen an inventory period, an inventory period entry is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2beae-123">See Also</span><span class="sxs-lookup"><span data-stu-id="2beae-123">See Also</span></span>  
 <span data-ttu-id="2beae-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span><span class="sxs-lookup"><span data-stu-id="2beae-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span></span>  
 [<span data-ttu-id="2beae-125">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="2beae-125">Working with Business Central</span></span>](ui-work-product.md)
