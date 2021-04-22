---
title: Design Details - Item Tracking | Microsoft Docs
description: This topic provides an overview of design details for item tracking.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 6e5f20d2f450f3f544cc2f7023160e4e9babdf33
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772811"
---
# <a name="design-details-item-tracking"></a><span data-ttu-id="529e2-103">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="529e2-103">Design Details: Item Tracking</span></span>
<span data-ttu-id="529e2-104">As the flow of goods in today's supply chain becomes more and more complex, the ability to keep track of items is increasingly important to the companies involved.</span><span class="sxs-lookup"><span data-stu-id="529e2-104">As the flow of goods in today's supply chain becomes more and more complex, the ability to keep track of items is increasingly important to the companies involved.</span></span> <span data-ttu-id="529e2-105">Monitoring an item's transaction flow is a legal requirement in the business of medical and chemical supply, but other businesses may want to monitor products with warranties or expiration dates for customer service reasons.</span><span class="sxs-lookup"><span data-stu-id="529e2-105">Monitoring an item's transaction flow is a legal requirement in the business of medical and chemical supply, but other businesses may want to monitor products with warranties or expiration dates for customer service reasons.</span></span>  

<span data-ttu-id="529e2-106">An item tracking system should provide a company with easy handling of serial and lot numbers, considering each unique piece of merchandise: when and where received, where stored, when and where sold.</span><span class="sxs-lookup"><span data-stu-id="529e2-106">An item tracking system should provide a company with easy handling of serial and lot numbers, considering each unique piece of merchandise: when and where received, where stored, when and where sold.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="529e2-107">has gradually expanded its coverage of this business requirement and today provides application-wide functionality and a solid core on which to develop extensions.</span><span class="sxs-lookup"><span data-stu-id="529e2-107">has gradually expanded its coverage of this business requirement and today provides application-wide functionality and a solid core on which to develop extensions.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="529e2-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="529e2-108">In This Section</span></span>  
[<span data-ttu-id="529e2-109">Design Details: Item Tracking Design</span><span class="sxs-lookup"><span data-stu-id="529e2-109">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)  
[<span data-ttu-id="529e2-110">Design Details: Item Tracking Posting Structure</span><span class="sxs-lookup"><span data-stu-id="529e2-110">Design Details: Item Tracking Posting Structure</span></span>](design-details-item-tracking-posting-structure.md)  
[<span data-ttu-id="529e2-111">Design Details: Active versus Historic Item Tracking Entries</span><span class="sxs-lookup"><span data-stu-id="529e2-111">Design Details: Active versus Historic Item Tracking Entries</span></span>](design-details-active-versus-historic-item-tracking-entries.md)  
[<span data-ttu-id="529e2-112">Design Details: Item Tracking Lines Page</span><span class="sxs-lookup"><span data-stu-id="529e2-112">Design Details: Item Tracking Lines Page</span></span>](design-details-item-tracking-lines-window.md)  
[<span data-ttu-id="529e2-113">Design Details: Item Tracking Availability</span><span class="sxs-lookup"><span data-stu-id="529e2-113">Design Details: Item Tracking Availability</span></span>](design-details-item-tracking-availability.md)  
[<span data-ttu-id="529e2-114">Design Details: Item Tracking and Planning</span><span class="sxs-lookup"><span data-stu-id="529e2-114">Design Details: Item Tracking and Planning</span></span>](design-details-item-tracking-and-planning.md)  
[<span data-ttu-id="529e2-115">Design Details: Item Tracking and Reservations</span><span class="sxs-lookup"><span data-stu-id="529e2-115">Design Details: Item Tracking and Reservations</span></span>](design-details-item-tracking-and-reservations.md)  
[<span data-ttu-id="529e2-116">Design Details: Item Tracking in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="529e2-116">Design Details: Item Tracking in the Warehouse</span></span>](design-details-item-tracking-in-the-warehouse.md)

## <a name="see-also"></a><span data-ttu-id="529e2-117">See Also</span><span class="sxs-lookup"><span data-stu-id="529e2-117">See Also</span></span>

[<span data-ttu-id="529e2-118">Work with Serial, Lot, and Package Numbers</span><span class="sxs-lookup"><span data-stu-id="529e2-118">Work with Serial, Lot, and Package Numbers</span></span>](inventory-how-work-item-tracking.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]