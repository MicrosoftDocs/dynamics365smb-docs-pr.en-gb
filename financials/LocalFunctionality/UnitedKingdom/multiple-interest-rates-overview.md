---
title: Multiple Interest Rates Overview | Microsoft Docs
description: For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period. This is helpful if you charge different interest on payments that are late. The interest calculation is the same for each financial charge, with variation only in the rate of interest for a specific period.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 6d3b5c7a73154b9ce03112524a50ea0ce822c692
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="multiple-interest-rates-overview"></a><span data-ttu-id="8e404-105">Multiple Interest Rates Overview</span><span class="sxs-lookup"><span data-stu-id="8e404-105">Multiple Interest Rates Overview</span></span>
<span data-ttu-id="8e404-106">For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period.</span><span class="sxs-lookup"><span data-stu-id="8e404-106">For each finance charge term code, you can specify multiple interest rates so that you can calculate finance charges with multiple interest rates for a specific period.</span></span> <span data-ttu-id="8e404-107">This is helpful if you charge different interest on payments that are late.</span><span class="sxs-lookup"><span data-stu-id="8e404-107">This is helpful if you charge different interest on payments that are late.</span></span> <span data-ttu-id="8e404-108">The interest calculation is the same for each financial charge, with variation only in the rate of interest for a specific period.</span><span class="sxs-lookup"><span data-stu-id="8e404-108">The interest calculation is the same for each financial charge, with variation only in the rate of interest for a specific period.</span></span>  

## <a name="creating-finance-charges"></a><span data-ttu-id="8e404-109">Creating Finance Charges</span><span class="sxs-lookup"><span data-stu-id="8e404-109">Creating Finance Charges</span></span>  
 <span data-ttu-id="8e404-110">When you create a finance charge memo, the memo lines show the finance charges with different interest rates for each time period.</span><span class="sxs-lookup"><span data-stu-id="8e404-110">When you create a finance charge memo, the memo lines show the finance charges with different interest rates for each time period.</span></span> <span data-ttu-id="8e404-111">For finance charge terms, you can define descriptions for each term, and you can define a description that is used when multiple interest rates are used.</span><span class="sxs-lookup"><span data-stu-id="8e404-111">For finance charge terms, you can define descriptions for each term, and you can define a description that is used when multiple interest rates are used.</span></span>  

 <span data-ttu-id="8e404-112">To use multiple interest rates, you must first define a finance charge term, and you must then add multiple interest rate lines to the terms.</span><span class="sxs-lookup"><span data-stu-id="8e404-112">To use multiple interest rates, you must first define a finance charge term, and you must then add multiple interest rate lines to the terms.</span></span> <span data-ttu-id="8e404-113">For more information, see [How to: Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md).</span><span class="sxs-lookup"><span data-stu-id="8e404-113">For more information, see [How to: Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md).</span></span>  

 <span data-ttu-id="8e404-114">If no multiple interest rates exist, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] will use the interest rate and period that is defined in the **Finance Charge Terms** window for the whole period of calculation.</span><span class="sxs-lookup"><span data-stu-id="8e404-114">If no multiple interest rates exist, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] will use the interest rate and period that is defined in the **Finance Charge Terms** window for the whole period of calculation.</span></span>  

## <a name="delayed-payments"></a><span data-ttu-id="8e404-115">Delayed Payments</span><span class="sxs-lookup"><span data-stu-id="8e404-115">Delayed Payments</span></span>  
 <span data-ttu-id="8e404-116">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span><span class="sxs-lookup"><span data-stu-id="8e404-116">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span></span> <span data-ttu-id="8e404-117">For example, a government specifies the maximum interest to be levied for a consumer.</span><span class="sxs-lookup"><span data-stu-id="8e404-117">For example, a government specifies the maximum interest to be levied for a consumer.</span></span> <span data-ttu-id="8e404-118">This interest rate can be changed twice a year on 01 January and 01 July.</span><span class="sxs-lookup"><span data-stu-id="8e404-118">This interest rate can be changed twice a year on 01 January and 01 July.</span></span> <span data-ttu-id="8e404-119">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span><span class="sxs-lookup"><span data-stu-id="8e404-119">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span></span> <span data-ttu-id="8e404-120">The announced rate is usually four percent more than the normal bank interest.</span><span class="sxs-lookup"><span data-stu-id="8e404-120">The announced rate is usually four percent more than the normal bank interest.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8e404-121">See Also</span><span class="sxs-lookup"><span data-stu-id="8e404-121">See Also</span></span>  
[<span data-ttu-id="8e404-122">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="8e404-122">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  
 <span data-ttu-id="8e404-123">[How to: Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md) </span><span class="sxs-lookup"><span data-stu-id="8e404-123">[How to: Set Up Multiple Interest Rates](how-to-set-up-multiple-interest-rates.md) </span></span>  
 [<span data-ttu-id="8e404-124">How to: Collect Outstanding balances</span><span class="sxs-lookup"><span data-stu-id="8e404-124">How to: Collect Outstanding balances</span></span>](../../receivables-collect-outstanding-balances.md)

