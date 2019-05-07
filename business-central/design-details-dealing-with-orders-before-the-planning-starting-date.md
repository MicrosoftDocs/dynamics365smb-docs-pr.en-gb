---
title: Design Details - Dealing with Orders Before the Planning Starting Date | Microsoft Docs
description: This topic describes the rules that planning applies to orders in the frozen zone.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: planning, frozen, design serial, lot
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: design-details-balancing-demand-and-supply
ms.openlocfilehash: 32c523eda09620bd74df53f09bc103a44fbb367a
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "919781"
---
# <a name="design-details-dealing-with-orders-before-the-planning-starting-date"></a><span data-ttu-id="9c778-103">Design Details: Dealing with Orders Before the Planning Starting Date</span><span class="sxs-lookup"><span data-stu-id="9c778-103">Design Details: Dealing with Orders Before the Planning Starting Date</span></span>
<span data-ttu-id="9c778-104">To avoid that a supply plan shows impossible and therefore useless suggestions, the planning system regards the period up until the planning starting date a frozen zone where nothing is planned for.</span><span class="sxs-lookup"><span data-stu-id="9c778-104">To avoid that a supply plan shows impossible and therefore useless suggestions, the planning system regards the period up until the planning starting date a frozen zone where nothing is planned for.</span></span> <span data-ttu-id="9c778-105">The following rule applies to the frozen zone:</span><span class="sxs-lookup"><span data-stu-id="9c778-105">The following rule applies to the frozen zone:</span></span>  

<span data-ttu-id="9c778-106">All supply and demand before the starting date of the planning period will be considered a part of inventory or shipped.</span><span class="sxs-lookup"><span data-stu-id="9c778-106">All supply and demand before the starting date of the planning period will be considered a part of inventory or shipped.</span></span>  

<span data-ttu-id="9c778-107">Accordingly, the planning system will not, with a few exceptions, suggest any changes to supply orders in the frozen zone, and no order tracking links are created or maintained for that period.</span><span class="sxs-lookup"><span data-stu-id="9c778-107">Accordingly, the planning system will not, with a few exceptions, suggest any changes to supply orders in the frozen zone, and no order tracking links are created or maintained for that period.</span></span>  

<span data-ttu-id="9c778-108">The exceptions to this rule are as follows:</span><span class="sxs-lookup"><span data-stu-id="9c778-108">The exceptions to this rule are as follows:</span></span>  

* <span data-ttu-id="9c778-109">If the projected available inventory, including the sum of supply and demand in the frozen zone, is below zero.</span><span class="sxs-lookup"><span data-stu-id="9c778-109">If the projected available inventory, including the sum of supply and demand in the frozen zone, is below zero.</span></span>  
* <span data-ttu-id="9c778-110">If serial/lot numbers are required on the backdated order(s).</span><span class="sxs-lookup"><span data-stu-id="9c778-110">If serial/lot numbers are required on the backdated order(s).</span></span>  
* <span data-ttu-id="9c778-111">If the supply-demand set is linked by an order-to-order policy.</span><span class="sxs-lookup"><span data-stu-id="9c778-111">If the supply-demand set is linked by an order-to-order policy.</span></span>  

<span data-ttu-id="9c778-112">If the initial available inventory is below zero, the planning system suggests an emergency supply order on the day before the planning period to cover the missing quantity.</span><span class="sxs-lookup"><span data-stu-id="9c778-112">If the initial available inventory is below zero, the planning system suggests an emergency supply order on the day before the planning period to cover the missing quantity.</span></span> <span data-ttu-id="9c778-113">Consequently, the projected and available inventory will always be at least zero when planning for the future period begins.</span><span class="sxs-lookup"><span data-stu-id="9c778-113">Consequently, the projected and available inventory will always be at least zero when planning for the future period begins.</span></span> <span data-ttu-id="9c778-114">The planning line for this supply order will display an Emergency warning icon and additional information is provided upon lookup.</span><span class="sxs-lookup"><span data-stu-id="9c778-114">The planning line for this supply order will display an Emergency warning icon and additional information is provided upon lookup.</span></span>  

## <a name="seriallot-numbers-and-order-to-order-links-are-exempt-from-the-frozen-zone"></a><span data-ttu-id="9c778-115">Serial/Lot Numbers and Order-to-Order Links are Exempt from the Frozen Zone</span><span class="sxs-lookup"><span data-stu-id="9c778-115">Serial/Lot Numbers and Order-to-Order Links are Exempt from the Frozen Zone</span></span>  
<span data-ttu-id="9c778-116">If serial/lot numbers are required or an order-to-order link exists, the planning system will disregard the frozen zone and incorporate such quantities that are back-dated from the starting date and potentially suggest corrective actions if demand and supply is not synchronised.</span><span class="sxs-lookup"><span data-stu-id="9c778-116">If serial/lot numbers are required or an order-to-order link exists, the planning system will disregard the frozen zone and incorporate such quantities that are back-dated from the starting date and potentially suggest corrective actions if demand and supply is not synchronized.</span></span> <span data-ttu-id="9c778-117">The business reason for this principle is that such specific demand-supply sets must match to ensure that this specific demand is fulfilled.</span><span class="sxs-lookup"><span data-stu-id="9c778-117">The business reason for this principle is that such specific demand-supply sets must match to ensure that this specific demand is fulfilled.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9c778-118">See Also</span><span class="sxs-lookup"><span data-stu-id="9c778-118">See Also</span></span>  
<span data-ttu-id="9c778-119">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="9c778-119">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="9c778-120">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="9c778-120">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="9c778-121">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="9c778-121">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
