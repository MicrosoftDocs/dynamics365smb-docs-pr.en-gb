---
title: How to Update Standard Costs | Microsoft Docs
description: You must periodically update the standard costs of components and roll the new costs up to the parent item.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: feeeae5202cfc5ab0bccf1552ce74f74708445d3
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5391531"
---
# <a name="update-standard-costs"></a><span data-ttu-id="d1e7f-103">Update Standard Costs</span><span class="sxs-lookup"><span data-stu-id="d1e7f-103">Update Standard Costs</span></span>
<span data-ttu-id="d1e7f-104">You must periodically update the standard costs of components and roll the new costs up to the parent item.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-104">You must periodically update the standard costs of components and roll the new costs up to the parent item.</span></span> <span data-ttu-id="d1e7f-105">The process typically consists of the following four steps:</span><span class="sxs-lookup"><span data-stu-id="d1e7f-105">The process typically consists of the following four steps:</span></span>  

1.  <span data-ttu-id="d1e7f-106">Update costs at the component and capacity levels.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-106">Update costs at the component and capacity levels.</span></span> <span data-ttu-id="d1e7f-107">For more information, see the **Suggest Item Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-107">For more information, see the **Suggest Item Standard Cost** batch job.</span></span>  
2.  <span data-ttu-id="d1e7f-108">Consolidate and roll up the component and capacity costs to calculate the total manufacturing or assembly cost of the items.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-108">Consolidate and roll up the component and capacity costs to calculate the total manufacturing or assembly cost of the items.</span></span>  
3.  <span data-ttu-id="d1e7f-109">Implement the standard costs that are entered when you run the previous batch jobs.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-109">Implement the standard costs that are entered when you run the previous batch jobs.</span></span> <span data-ttu-id="d1e7f-110">The standard costs do not take effect until they are implemented.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-110">The standard costs do not take effect until they are implemented.</span></span> <span data-ttu-id="d1e7f-111">For more information, see Implement Standard Cost Changes.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-111">For more information, see Implement Standard Cost Changes.</span></span>  
4.  <span data-ttu-id="d1e7f-112">Implement the changes to update the **Unit Cost** field on the item card and perform inventory revaluation.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-112">Implement the changes to update the **Unit Cost** field on the item card and perform inventory revaluation.</span></span> <span data-ttu-id="d1e7f-113">For more information, see [Revalue Inventory](inventory-how-revalue-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="d1e7f-113">For more information, see [Revalue Inventory](inventory-how-revalue-inventory.md).</span></span>  

<span data-ttu-id="d1e7f-114">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md).</span><span class="sxs-lookup"><span data-stu-id="d1e7f-114">For more information, see [About Calculating Standard Cost](finance-about-calculating-standard-cost.md).</span></span>  
## <a name="to-update-standard-costs"></a><span data-ttu-id="d1e7f-115">To update standard costs</span><span class="sxs-lookup"><span data-stu-id="d1e7f-115">To update standard costs</span></span>  
1.  <span data-ttu-id="d1e7f-116">Run the **Adjust Cost-Item Entries** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-116">Run the **Adjust Cost-Item Entries** batch job.</span></span>  
2.  <span data-ttu-id="d1e7f-117">Run the **Post Inventory Cost to G/L** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-117">Run the **Post Inventory Cost to G/L** batch job.</span></span>  
3.  <span data-ttu-id="d1e7f-118">Open the **Standard Cost Worksheet** and use one or more of the following functions:</span><span class="sxs-lookup"><span data-stu-id="d1e7f-118">Open the **Standard Cost Worksheet** and use one or more of the following functions:</span></span>  

    1.  <span data-ttu-id="d1e7f-119">Run the **Suggest Item Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-119">Run the **Suggest Item Standard Cost** batch job.</span></span>  
    2.  <span data-ttu-id="d1e7f-120">Review the results and make changes as necessary.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-120">Review the results and make changes as necessary.</span></span>  
    3.  <span data-ttu-id="d1e7f-121">Run the **Suggest Capacity Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-121">Run the **Suggest Capacity Standard Cost** batch job.</span></span>  
    4.  <span data-ttu-id="d1e7f-122">Review the results and make changes as necessary.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-122">Review the results and make changes as necessary.</span></span>
    5. <span data-ttu-id="d1e7f-123">Run the **Roll Up Standard Cost** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-123">Run the **Roll Up Standard Cost** batch job.</span></span>
    6.  <span data-ttu-id="d1e7f-124">Review the results and make changes as necessary.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-124">Review the results and make changes as necessary.</span></span>
    7.  <span data-ttu-id="d1e7f-125">Run the **Implement Standard Cost Changes** batch job.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-125">Run the **Implement Standard Cost Changes** batch job.</span></span>  
4.  <span data-ttu-id="d1e7f-126">Review and post the **Revaluation Journal** page, which has been populated with entries from the previous steps in this process.</span><span class="sxs-lookup"><span data-stu-id="d1e7f-126">Review and post the **Revaluation Journal** page, which has been populated with entries from the previous steps in this process.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d1e7f-127">See Also</span><span class="sxs-lookup"><span data-stu-id="d1e7f-127">See Also</span></span>  
 <span data-ttu-id="d1e7f-128">[About Calculating Standard Cost](finance-about-calculating-standard-cost.md) </span><span class="sxs-lookup"><span data-stu-id="d1e7f-128">[About Calculating Standard Cost](finance-about-calculating-standard-cost.md) </span></span>  
 <span data-ttu-id="d1e7f-129">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="d1e7f-129">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="d1e7f-130">[Design Details: Costing Methods](design-details-costing-methods.md) [Finance](finance.md)</span><span class="sxs-lookup"><span data-stu-id="d1e7f-130">[Design Details: Costing Methods](design-details-costing-methods.md) [Finance](finance.md)</span></span>  
 <span data-ttu-id="d1e7f-131">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d1e7f-131">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]