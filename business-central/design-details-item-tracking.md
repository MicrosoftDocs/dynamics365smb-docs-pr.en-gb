---
title: Design Details - Item Tracking | Microsoft Docs
description: This topic provides an overview of design details for item tracking.
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
ms.openlocfilehash: 344c3162ce7f84aa61f9e572f3245d9515cbd81b
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "925214"
---
# <a name="design-details-item-tracking"></a><span data-ttu-id="31f4b-103">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="31f4b-103">Design Details: Item Tracking</span></span>
<span data-ttu-id="31f4b-104">As the flow of goods in today’s supply chain becomes more and more complex, the ability to keep track of items is increasingly important to the companies involved.</span><span class="sxs-lookup"><span data-stu-id="31f4b-104">As the flow of goods in today’s supply chain becomes more and more complex, the ability to keep track of items is increasingly important to the companies involved.</span></span> <span data-ttu-id="31f4b-105">Monitoring an item’s transaction flow is a legal requirement in the business of medical and chemical supply, but other businesses may want to monitor products with warranties or expiration dates for customer service reasons.</span><span class="sxs-lookup"><span data-stu-id="31f4b-105">Monitoring an item’s transaction flow is a legal requirement in the business of medical and chemical supply, but other businesses may want to monitor products with warranties or expiration dates for customer service reasons.</span></span>  

<span data-ttu-id="31f4b-106">An item tracking system should provide a company with easy handling of serial and lot numbers, considering each unique piece of merchandise: when and where received, where stored, when and where sold.</span><span class="sxs-lookup"><span data-stu-id="31f4b-106">An item tracking system should provide a company with easy handling of serial and lot numbers, considering each unique piece of merchandise: when and where received, where stored, when and where sold.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="31f4b-107">has gradually expanded its coverage of this business requirement and today provides application-wide functionality and a solid core on which to develop extensions.</span><span class="sxs-lookup"><span data-stu-id="31f4b-107">has gradually expanded its coverage of this business requirement and today provides application-wide functionality and a solid core on which to develop extensions.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="31f4b-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="31f4b-108">In This Section</span></span>  
[<span data-ttu-id="31f4b-109">Design Details: Item Tracking Design</span><span class="sxs-lookup"><span data-stu-id="31f4b-109">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)  
[<span data-ttu-id="31f4b-110">Design Details: Item Tracking Posting Structure</span><span class="sxs-lookup"><span data-stu-id="31f4b-110">Design Details: Item Tracking Posting Structure</span></span>](design-details-item-tracking-posting-structure.md)  
[<span data-ttu-id="31f4b-111">Design Details: Active versus Historic Item Tracking Entries</span><span class="sxs-lookup"><span data-stu-id="31f4b-111">Design Details: Active versus Historic Item Tracking Entries</span></span>](design-details-active-versus-historic-item-tracking-entries.md)  
[<span data-ttu-id="31f4b-112">Design Details: Item Tracking Lines Page</span><span class="sxs-lookup"><span data-stu-id="31f4b-112">Design Details: Item Tracking Lines Page</span></span>](design-details-item-tracking-lines-window.md)  
[<span data-ttu-id="31f4b-113">Design Details: Item Tracking Availability</span><span class="sxs-lookup"><span data-stu-id="31f4b-113">Design Details: Item Tracking Availability</span></span>](design-details-item-tracking-availability.md)  
[<span data-ttu-id="31f4b-114">Design Details: Item Tracking and Planning</span><span class="sxs-lookup"><span data-stu-id="31f4b-114">Design Details: Item Tracking and Planning</span></span>](design-details-item-tracking-and-planning.md)  
[<span data-ttu-id="31f4b-115">Design Details: Item Tracking and Reservations</span><span class="sxs-lookup"><span data-stu-id="31f4b-115">Design Details: Item Tracking and Reservations</span></span>](design-details-item-tracking-and-reservations.md)  
[<span data-ttu-id="31f4b-116">Design Details: Item Tracking in the Warehouse</span><span class="sxs-lookup"><span data-stu-id="31f4b-116">Design Details: Item Tracking in the Warehouse</span></span>](design-details-item-tracking-in-the-warehouse.md)
