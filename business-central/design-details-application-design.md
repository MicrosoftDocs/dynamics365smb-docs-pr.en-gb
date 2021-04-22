---
title: Design Details | Microsoft Docs
description: This content contains detailed technical information about complex application features in Business Central.
author: SorenGP
documentationcenter: ''
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f669944766894e57a772e229a436953953f3892c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785196"
---
# <a name="design-details"></a><span data-ttu-id="4f295-103">Design Details</span><span class="sxs-lookup"><span data-stu-id="4f295-103">Design Details</span></span>
<span data-ttu-id="4f295-104">This content contains detailed technical information about complex application features in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="4f295-104">This content contains detailed technical information about complex application features in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

 <span data-ttu-id="4f295-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customise, or set up the features in question.</span><span class="sxs-lookup"><span data-stu-id="4f295-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customize, or set up the features in question.</span></span>  

|<span data-ttu-id="4f295-106">**To**</span><span class="sxs-lookup"><span data-stu-id="4f295-106">**To**</span></span>|<span data-ttu-id="4f295-107">**See**</span><span class="sxs-lookup"><span data-stu-id="4f295-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="4f295-108">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span><span class="sxs-lookup"><span data-stu-id="4f295-108">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span>|[<span data-ttu-id="4f295-109">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="4f295-109">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)|  
|<span data-ttu-id="4f295-110">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span><span class="sxs-lookup"><span data-stu-id="4f295-110">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span></span>|[<span data-ttu-id="4f295-111">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="4f295-111">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  
|<span data-ttu-id="4f295-112">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span><span class="sxs-lookup"><span data-stu-id="4f295-112">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span></span>|[<span data-ttu-id="4f295-113">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="4f295-113">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)|  
|<span data-ttu-id="4f295-114">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span><span class="sxs-lookup"><span data-stu-id="4f295-114">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span></span>|[<span data-ttu-id="4f295-115">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="4f295-115">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)|  
|<span data-ttu-id="4f295-116">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span><span class="sxs-lookup"><span data-stu-id="4f295-116">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span></span>|[<span data-ttu-id="4f295-117">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="4f295-117">Design Details: General Journal Post Line</span></span>](design-details-general-journal-post-line.md)|
|<span data-ttu-id="4f295-118">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span><span class="sxs-lookup"><span data-stu-id="4f295-118">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span></span>|[<span data-ttu-id="4f295-119">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="4f295-119">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries-overview.md)|

## <a name="see-also"></a><span data-ttu-id="4f295-120">See Also</span><span class="sxs-lookup"><span data-stu-id="4f295-120">See Also</span></span>

[<span data-ttu-id="4f295-121">Planning</span><span class="sxs-lookup"><span data-stu-id="4f295-121">Planning</span></span>](production-planning.md)  
[<span data-ttu-id="4f295-122">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="4f295-122">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="4f295-123">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="4f295-123">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="4f295-124">Setting Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="4f295-124">Setting Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
<span data-ttu-id="4f295-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4f295-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  
