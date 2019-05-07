---
title: Set Up Inventory Valuation and Costing | Microsoft Docs
description: The following table describes a sequence of tasks, with links to the topics that describe them.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 184c7651fe8db60b55bd161bb5dc870df1ed01c5
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "919036"
---
# <a name="setting-up-inventory-valuation-and-costing"></a><span data-ttu-id="b59f7-103">Setting Up Inventory Valuation and Costing</span><span class="sxs-lookup"><span data-stu-id="b59f7-103">Setting Up Inventory Valuation and Costing</span></span>
<span data-ttu-id="b59f7-104">To make sure that inventory costs are recorded correctly, you must set up various fields and pages before you begin to make item transactions.</span><span class="sxs-lookup"><span data-stu-id="b59f7-104">To make sure that inventory costs are recorded correctly, you must set up various fields and pages before you begin to make item transactions.</span></span>

<span data-ttu-id="b59f7-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="b59f7-105">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="b59f7-106">**To**</span><span class="sxs-lookup"><span data-stu-id="b59f7-106">**To**</span></span>|<span data-ttu-id="b59f7-107">**See**</span><span class="sxs-lookup"><span data-stu-id="b59f7-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b59f7-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span><span class="sxs-lookup"><span data-stu-id="b59f7-108">Set a costing method for each item to govern how its incoming cost is used to assess inventory value and the cost of goods sold.</span></span>|[<span data-ttu-id="b59f7-109">Register New Items</span><span class="sxs-lookup"><span data-stu-id="b59f7-109">Register New Items</span></span>](inventory-how-register-new-items.md)|  
|<span data-ttu-id="b59f7-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span><span class="sxs-lookup"><span data-stu-id="b59f7-110">Ensure that the cost is automatically posted to the general ledger whenever an inventory transaction is posted.</span></span>|<span data-ttu-id="b59f7-111">**Automatic Cost Posting** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-111">**Automatic Cost Posting** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="b59f7-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span><span class="sxs-lookup"><span data-stu-id="b59f7-112">Ensure that expected costs are posted to the general ledger to see from the interim G/L accounts an estimate of the amounts due and the cost of the traded items before they are actually invoiced.</span></span>|<span data-ttu-id="b59f7-113">**Expected Cost Posting to G/L** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-113">**Expected Cost Posting to G/L** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="b59f7-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span><span class="sxs-lookup"><span data-stu-id="b59f7-114">Set the system up to adjust for any cost changes automatically every time you post inventory transactions.</span></span>|[<span data-ttu-id="b59f7-115">Adjust Item Costs</span><span class="sxs-lookup"><span data-stu-id="b59f7-115">Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|  
|<span data-ttu-id="b59f7-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span><span class="sxs-lookup"><span data-stu-id="b59f7-116">Define if the average cost is to be calculated per item only or per item for each stockkeping unit and for each variant of the item.</span></span>|<span data-ttu-id="b59f7-117">**Average Cost Calc. Type** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-117">**Average Cost Calc. Type** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="b59f7-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span><span class="sxs-lookup"><span data-stu-id="b59f7-118">Select the period of time you would like the program to use for calculating the weighted average cost of items that use the average costing method.</span></span>|<span data-ttu-id="b59f7-119">**Average Cost Period** field on the **Inventory Setup** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-119">**Average Cost Period** field on the **Inventory Setup** page</span></span>|  
|<span data-ttu-id="b59f7-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span><span class="sxs-lookup"><span data-stu-id="b59f7-120">Define inventory periods to control inventory value over time by disallowing transaction posting in closed inventory periods.</span></span>|[<span data-ttu-id="b59f7-121">Work with Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="b59f7-121">Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="b59f7-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="b59f7-122">Ensure that sales returns are applied to the original outbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="b59f7-123">**Exact Cost Reversing Mandatory** field on the **Sales & Receivables** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-123">**Exact Cost Reversing Mandatory** field on the **Sales & Receivables** page</span></span>|  
|<span data-ttu-id="b59f7-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span><span class="sxs-lookup"><span data-stu-id="b59f7-124">Ensure that purchase returns are applied to the original inbound transaction to preserve inventory value.</span></span>|<span data-ttu-id="b59f7-125">**Exact Cost Reversing Mandatory** field on the **´Purchases & Payables** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-125">**Exact Cost Reversing Mandatory** field on the **´Purchases & Payables** page</span></span>|
|<span data-ttu-id="b59f7-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span><span class="sxs-lookup"><span data-stu-id="b59f7-126">Set up the rounding rules to apply when adjusting or suggesting item prices and when adjusting or suggesting standard costs.</span></span>|<span data-ttu-id="b59f7-127">**Rounding Method** page</span><span class="sxs-lookup"><span data-stu-id="b59f7-127">**Rounding Method** page</span></span>|  

## <a name="see-also"></a><span data-ttu-id="b59f7-128">See Also</span><span class="sxs-lookup"><span data-stu-id="b59f7-128">See Also</span></span>  
[<span data-ttu-id="b59f7-129">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="b59f7-129">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="b59f7-130">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="b59f7-130">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="b59f7-131">Finance</span><span class="sxs-lookup"><span data-stu-id="b59f7-131">Finance</span></span>](finance.md)  
