---
title: Design Details - Stock Periods | Microsoft Docs
description: Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed. This can have adverse effects on accurate reporting, especially within global corporations. The Stock Periods feature can be used to avoid such problems by opening or closing stock periods to limit posting in a set period of time.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 2231fcd34d45ae487bf3344a1efe2e317c75c89a
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215085"
---
# <a name="design-details-inventory-periods"></a><span data-ttu-id="39874-105">Design Details: Stock Periods</span><span class="sxs-lookup"><span data-stu-id="39874-105">Design Details: Inventory Periods</span></span>
<span data-ttu-id="39874-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span><span class="sxs-lookup"><span data-stu-id="39874-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span></span> <span data-ttu-id="39874-107">This can have adverse effects on accurate reporting, especially within global corporations.</span><span class="sxs-lookup"><span data-stu-id="39874-107">This can have adverse effects on accurate reporting, especially within global corporations.</span></span> <span data-ttu-id="39874-108">The Stock Periods feature can be used to avoid such problems by opening or closing stock periods to limit posting in a set period of time.</span><span class="sxs-lookup"><span data-stu-id="39874-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span></span>  

 <span data-ttu-id="39874-109">A stock period is a period of time, defined by an ending date, in which you post stock transactions.</span><span class="sxs-lookup"><span data-stu-id="39874-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span></span> <span data-ttu-id="39874-110">When you close a stock period, no value changes can be posted in the closed period.</span><span class="sxs-lookup"><span data-stu-id="39874-110">When you close an inventory period, no value changes can be posted in the closed period.</span></span> <span data-ttu-id="39874-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span><span class="sxs-lookup"><span data-stu-id="39874-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span></span> <span data-ttu-id="39874-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span><span class="sxs-lookup"><span data-stu-id="39874-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span></span> <span data-ttu-id="39874-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span><span class="sxs-lookup"><span data-stu-id="39874-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span></span>  

 <span data-ttu-id="39874-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before a stock period can close:</span><span class="sxs-lookup"><span data-stu-id="39874-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span></span>  

-   <span data-ttu-id="39874-115">All outbound item ledger entries in the period must be closed (no negative stock).</span><span class="sxs-lookup"><span data-stu-id="39874-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span></span>  
-   <span data-ttu-id="39874-116">All item costs in the period must be adjusted.</span><span class="sxs-lookup"><span data-stu-id="39874-116">All item costs in the period must be adjusted.</span></span>  
-   <span data-ttu-id="39874-117">All released and finished works orders in the period must be cost adjusted.</span><span class="sxs-lookup"><span data-stu-id="39874-117">All released and finished production orders in the period must be cost adjusted.</span></span>  

 <span data-ttu-id="39874-118">When you close a stock period, a stock period entry is created by using the number of the last item register that falls in the stock period.</span><span class="sxs-lookup"><span data-stu-id="39874-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span></span> <span data-ttu-id="39874-119">In addition, the time, date, and user code of the user closing the period are recorded in the stock period entry.</span><span class="sxs-lookup"><span data-stu-id="39874-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span></span> <span data-ttu-id="39874-120">By using this information with the last item register for the previous period, you can see which stock transactions were posted in the stock period.</span><span class="sxs-lookup"><span data-stu-id="39874-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span></span> <span data-ttu-id="39874-121">It is also possible to reopen stock periods if you need to post in a closed period.</span><span class="sxs-lookup"><span data-stu-id="39874-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span></span> <span data-ttu-id="39874-122">When you reopen a stock period, a stock period entry is created.</span><span class="sxs-lookup"><span data-stu-id="39874-122">When you reopen an inventory period, an inventory period entry is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="39874-123">See Also</span><span class="sxs-lookup"><span data-stu-id="39874-123">See Also</span></span>  
 <span data-ttu-id="39874-124">[Design Details: Stock Costing](design-details-inventory-costing.md) [Managing Stock Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span><span class="sxs-lookup"><span data-stu-id="39874-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span></span>  
 [<span data-ttu-id="39874-125">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="39874-125">Working with Business Central</span></span>](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]