---
title: Design Details | Microsoft Docs
description: This content contains detailed technical information about complex application features in Business Central.
author: SorenGP
documentationcenter: ''
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: a2280fbeccd51d1c959aa2aa09121d728a18326f
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751862"
---
# <a name="design-details"></a><span data-ttu-id="b4c8d-103">Design Details</span><span class="sxs-lookup"><span data-stu-id="b4c8d-103">Design Details</span></span>
<span data-ttu-id="b4c8d-104">This content contains detailed technical information about complex application features in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b4c8d-104">This content contains detailed technical information about complex application features in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

 <span data-ttu-id="b4c8d-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customise, or set up the features in question.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-105">Design details content is aimed at implementers, developers, and super users who need deeper insight to implement, customize, or set up the features in question.</span></span>  

|<span data-ttu-id="b4c8d-106">**To**</span><span class="sxs-lookup"><span data-stu-id="b4c8d-106">**To**</span></span>|<span data-ttu-id="b4c8d-107">**See**</span><span class="sxs-lookup"><span data-stu-id="b4c8d-107">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b4c8d-108">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-108">Learn how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span>|[<span data-ttu-id="b4c8d-109">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="b4c8d-109">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)|  
|<span data-ttu-id="b4c8d-110">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-110">Understand mechanisms in the costing engine, such as costing method and cost adjustment, and which accounting principles they are designed for.</span></span>|[<span data-ttu-id="b4c8d-111">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="b4c8d-111">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  
|<span data-ttu-id="b4c8d-112">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-112">Learn about central principles behind advanced and basic warehouse features and how they integrate with other supply chain features.</span></span>|[<span data-ttu-id="b4c8d-113">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="b4c8d-113">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)|  
|<span data-ttu-id="b4c8d-114">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-114">Learn about historic and the current design of item tracking functionality and how it integrates with the reservation system to include serial/lot numbers in availability calculations.</span></span>|[<span data-ttu-id="b4c8d-115">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="b4c8d-115">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)|  
|<span data-ttu-id="b4c8d-116">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-116">Learn about the General Journal Posting Line feature, including recent simplifications to the design of codeunit 12.</span></span>|[<span data-ttu-id="b4c8d-117">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="b4c8d-117">Design Details: General Journal Post Line</span></span>](design-details-general-journal-post-line.md)|
|<span data-ttu-id="b4c8d-118">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span><span class="sxs-lookup"><span data-stu-id="b4c8d-118">Learn about the design for storing and posting dimensions, including code examples on how to migrate and upgrade dimension code.</span></span>|[<span data-ttu-id="b4c8d-119">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="b4c8d-119">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)| 

## <a name="see-also"></a><span data-ttu-id="b4c8d-120">See Also</span><span class="sxs-lookup"><span data-stu-id="b4c8d-120">See Also</span></span>  
 <span data-ttu-id="b4c8d-121">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="b4c8d-121">[Planning](production-planning.md) </span></span>  
 <span data-ttu-id="b4c8d-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="b4c8d-122">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 <span data-ttu-id="b4c8d-123">[Warehouse Management](warehouse-manage-warehouse.md) </span><span class="sxs-lookup"><span data-stu-id="b4c8d-123">[Warehouse Management](warehouse-manage-warehouse.md) </span></span>  
 [<span data-ttu-id="b4c8d-124">Setting Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="b4c8d-124">Setting Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="b4c8d-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b4c8d-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>

 ## [!INCLUDE[prod_short](includes/free_trial_md.md)]  
