---
title: Set Up Inventory Valuation and Costing | Microsoft Docs
description: The following table describes a sequence of tasks, with links to the topics that describe them.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: aa5ee6d9942390a2b4ad0aa8787172b0f7b141d0
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-inventory-valuation-and-costing"></a><span data-ttu-id="3a026-103">Setting Up Inventory Valuation and Costing</span><span class="sxs-lookup"><span data-stu-id="3a026-103">Setting Up Inventory Valuation and Costing</span></span>
<span data-ttu-id="3a026-104">To make sure that inventory costs are recorded correctly, you must set up various fields and windows before you begin to make item transactions.</span><span class="sxs-lookup"><span data-stu-id="3a026-104">To make sure that inventory costs are recorded correctly, you must set up various fields and windows before you begin to make item transactions.</span></span>

<span data-ttu-id="3a026-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="3a026-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="3a026-106">**To**</span><span class="sxs-lookup"><span data-stu-id="3a026-106">**To**</span></span>|<span data-ttu-id="3a026-107">**See**</span><span class="sxs-lookup"><span data-stu-id="3a026-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="3a026-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span><span class="sxs-lookup"><span data-stu-id="3a026-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span></span>|[<span data-ttu-id="3a026-109">How to: Register New Items</span><span class="sxs-lookup"><span data-stu-id="3a026-109">How to: Register New Items</span></span>](inventory-how-register-new-items.md)|  
|<span data-ttu-id="3a026-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span><span class="sxs-lookup"><span data-stu-id="3a026-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span></span>|<span data-ttu-id="3a026-111">**Automatic Cost Posting** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="3a026-111">**Automatic Cost Posting** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="3a026-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span><span class="sxs-lookup"><span data-stu-id="3a026-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span></span>|<span data-ttu-id="3a026-113">**Expected Cost Posting to G/L** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="3a026-113">**Expected Cost Posting to G/L** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="3a026-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span><span class="sxs-lookup"><span data-stu-id="3a026-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span></span>|[<span data-ttu-id="3a026-115">How to: Adjust Item Costs</span><span class="sxs-lookup"><span data-stu-id="3a026-115">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|  
|<span data-ttu-id="3a026-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span><span class="sxs-lookup"><span data-stu-id="3a026-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span></span>|<span data-ttu-id="3a026-117">**Average Cost Calc. Type** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="3a026-117">**Average Cost Calc. Type** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="3a026-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span><span class="sxs-lookup"><span data-stu-id="3a026-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span></span>|<span data-ttu-id="3a026-119">**Average Cost Period** field in the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="3a026-119">**Average Cost Period** field in the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="3a026-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span><span class="sxs-lookup"><span data-stu-id="3a026-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span></span>|[<span data-ttu-id="3a026-121">How to: Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="3a026-121">How to: Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="3a026-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="3a026-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="3a026-123">**Exact Cost Reversing Mandatory** field in the **Sales & Receivables** page</span><span class="sxs-lookup"><span data-stu-id="3a026-123">**Exact Cost Reversing Mandatory** field in the **Sales & Receivables** page</span></span>|  
|<span data-ttu-id="3a026-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="3a026-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="3a026-125">**Exact Cost Reversing Mandatory** field in the **´Purchases & Payables** page</span><span class="sxs-lookup"><span data-stu-id="3a026-125">**Exact Cost Reversing Mandatory** field in the **´Purchases & Payables** page</span></span>|
|<span data-ttu-id="3a026-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span><span class="sxs-lookup"><span data-stu-id="3a026-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span></span>|<span data-ttu-id="3a026-127">**Rounding Method** page</span><span class="sxs-lookup"><span data-stu-id="3a026-127">**Rounding Method** page</span></span>|  

## <a name="see-also"></a><span data-ttu-id="3a026-128">See Also</span><span class="sxs-lookup"><span data-stu-id="3a026-128">See Also</span></span>  
[<span data-ttu-id="3a026-129">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="3a026-129">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="3a026-130">Working with Financials</span><span class="sxs-lookup"><span data-stu-id="3a026-130">Working with Financials</span></span>](ui-work-product.md)  
[<span data-ttu-id="3a026-131">Finance</span><span class="sxs-lookup"><span data-stu-id="3a026-131">Finance</span></span>](finance.md)  

