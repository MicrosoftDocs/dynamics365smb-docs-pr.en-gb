---
title: Design Details - Demand and Supply | Microsoft Docs
description: Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order. In addition, application allows more technical types of demand, such as negative inventory and purchase returns.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: design-details-balancing-demand-and-supply
ms.openlocfilehash: 8ef7211aa812b1faf784ecf36f1873a6e2dcc6fc
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2303638"
---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="3b6c0-104">Design Details: Demand and Supply</span><span class="sxs-lookup"><span data-stu-id="3b6c0-104">Design Details: Demand and Supply</span></span>
<span data-ttu-id="3b6c0-105">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-105">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="3b6c0-106">In addition, application allows more technical types of demand, such as negative inventory and purchase returns.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-106">In addition, application allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  

 <span data-ttu-id="3b6c0-107">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-107">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="3b6c0-108">In addition, a sales return may also represent supply.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-108">In addition, a sales return may also represent supply.</span></span>  

 <span data-ttu-id="3b6c0-109">To sort out the many sources of demand and supply, the planning system organises them on two time lines called inventory profiles.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-109">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="3b6c0-110">One profile holds demand events, and the other holds the corresponding supply events.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-110">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="3b6c0-111">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-111">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  

 <span data-ttu-id="3b6c0-112">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-112">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  

 <span data-ttu-id="3b6c0-113">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span><span class="sxs-lookup"><span data-stu-id="3b6c0-113">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="3b6c0-114">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="3b6c0-114">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="3b6c0-115">See Also</span><span class="sxs-lookup"><span data-stu-id="3b6c0-115">See Also</span></span>  
 <span data-ttu-id="3b6c0-116">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="3b6c0-116">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="3b6c0-117">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="3b6c0-117">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="3b6c0-118">Design Details: Supply Planning</span><span class="sxs-lookup"><span data-stu-id="3b6c0-118">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
