---
title: Design Details - Item Tracking Availability | Microsoft Docs
description: This topic discusses how to make sure that the people who process orders can rely on the availability of serial or lot numbers.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: fcdfc219f94462048474acdef259f671e1c8a402
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="design-details-item-tracking-availability"></a><span data-ttu-id="99eea-103">Design Details: Item Tracking Availability</span><span class="sxs-lookup"><span data-stu-id="99eea-103">Design Details: Item Tracking Availability</span></span>
<span data-ttu-id="99eea-104">The **Item Tracking Lines** and **Item Tracking Summary** pages provide dynamic availability information for serial or lot numbers.</span><span class="sxs-lookup"><span data-stu-id="99eea-104">The **Item Tracking Lines** and **Item Tracking Summary** pages provide dynamic availability information for serial or lot numbers.</span></span> <span data-ttu-id="99eea-105">The purpose of this is to increase transparency for users on outbound documents, such as sales orders, by showing them which serial numbers or how many units of a lot number are currently assigned on other open documents.</span><span class="sxs-lookup"><span data-stu-id="99eea-105">The purpose of this is to increase transparency for users on outbound documents, such as sales orders, by showing them which serial numbers or how many units of a lot number are currently assigned on other open documents.</span></span> <span data-ttu-id="99eea-106">This reduces uncertainty that is caused by double allocation and instills confidence in order processors that the item tracking numbers and dates that they are promising on unposted sales orders can be fulfilled.</span><span class="sxs-lookup"><span data-stu-id="99eea-106">This reduces uncertainty that is caused by double allocation and instills confidence in order processors that the item tracking numbers and dates that they are promising on unposted sales orders can be fulfilled.</span></span> <span data-ttu-id="99eea-107">For more information, see [Design Details: Item Tracking Lines Page](design-details-item-tracking-lines-window.md).</span><span class="sxs-lookup"><span data-stu-id="99eea-107">For more information, see [Design Details: Item Tracking Lines Page](design-details-item-tracking-lines-window.md).</span></span>  

<span data-ttu-id="99eea-108">When you open the **Item Tracking Lines** page, availability data is retrieved from the **Item Ledger Entry** table and the **Reservation Entry** table, with no date filter.</span><span class="sxs-lookup"><span data-stu-id="99eea-108">When you open the **Item Tracking Lines** page, availability data is retrieved from the **Item Ledger Entry** table and the **Reservation Entry** table, with no date filter.</span></span> <span data-ttu-id="99eea-109">When you choose the **Serial No.** field or the **Lot No.** field, the **Item Tracking Summary** page opens and shows a summary of the item tracking information in the **Reservation Entry** table.</span><span class="sxs-lookup"><span data-stu-id="99eea-109">When you choose the **Serial No.** field or the **Lot No.** field, the **Item Tracking Summary** page opens and shows a summary of the item tracking information in the **Reservation Entry** table.</span></span> <span data-ttu-id="99eea-110">The summary contains the following information about each serial or lot number on the item tracking line:</span><span class="sxs-lookup"><span data-stu-id="99eea-110">The summary contains the following information about each serial or lot number on the item tracking line:</span></span>  

|<span data-ttu-id="99eea-111">Field</span><span class="sxs-lookup"><span data-stu-id="99eea-111">Field</span></span>|<span data-ttu-id="99eea-112">Description</span><span class="sxs-lookup"><span data-stu-id="99eea-112">Description</span></span>|  
|---------------------------------|---------------------------------------|  
|<span data-ttu-id="99eea-113">**Total Quantity**</span><span class="sxs-lookup"><span data-stu-id="99eea-113">**Total Quantity**</span></span>|<span data-ttu-id="99eea-114">The total quantity of the serial or lot number that is currently in inventory.</span><span class="sxs-lookup"><span data-stu-id="99eea-114">The total quantity of the serial or lot number that is currently in inventory.</span></span>|  
|<span data-ttu-id="99eea-115">**Total Requested Quantity**</span><span class="sxs-lookup"><span data-stu-id="99eea-115">**Total Requested Quantity**</span></span>|<span data-ttu-id="99eea-116">The total quantity of the serial or lot number that is currently requested in all documents.</span><span class="sxs-lookup"><span data-stu-id="99eea-116">The total quantity of the serial or lot number that is currently requested in all documents.</span></span>|  
|<span data-ttu-id="99eea-117">**Current Pending Quantity**</span><span class="sxs-lookup"><span data-stu-id="99eea-117">**Current Pending Quantity**</span></span>|<span data-ttu-id="99eea-118">The quantity that is entered in the current instance of the **Item Tracking Lines** page but is not yet committed to the database.</span><span class="sxs-lookup"><span data-stu-id="99eea-118">The quantity that is entered in the current instance of the **Item Tracking Lines** page but is not yet committed to the database.</span></span>|  
|<span data-ttu-id="99eea-119">**Total Available Quantity**</span><span class="sxs-lookup"><span data-stu-id="99eea-119">**Total Available Quantity**</span></span>|<span data-ttu-id="99eea-120">The quantity of the serial or lot number that is available for the user to request.</span><span class="sxs-lookup"><span data-stu-id="99eea-120">The quantity of the serial or lot number that is available for the user to request.</span></span><br /><br /> <span data-ttu-id="99eea-121">This quantity is calculated from other fields on the page as follows:</span><span class="sxs-lookup"><span data-stu-id="99eea-121">This quantity is calculated from other fields on the page as follows:</span></span><br /><br /> <span data-ttu-id="99eea-122">total quantity – (total requested quantity + current pending quantity).</span><span class="sxs-lookup"><span data-stu-id="99eea-122">total quantity – (total requested quantity + current pending quantity).</span></span>|  

> [!NOTE]  
>  <span data-ttu-id="99eea-123">You can also see the information in the preceding table by using the **Select Entries** function on the **Item Tracking Lines** page.</span><span class="sxs-lookup"><span data-stu-id="99eea-123">You can also see the information in the preceding table by using the **Select Entries** function on the **Item Tracking Lines** page.</span></span>  

<span data-ttu-id="99eea-124">To preserve database performance, availability data is only retrieved once from the database when you open the **Item Tracking Lines** page and use the **Refresh Availability** function on the page.</span><span class="sxs-lookup"><span data-stu-id="99eea-124">To preserve database performance, availability data is only retrieved once from the database when you open the **Item Tracking Lines** page and use the **Refresh Availability** function on the page.</span></span>  

## <a name="calculation-formula"></a><span data-ttu-id="99eea-125">Calculation Formula</span><span class="sxs-lookup"><span data-stu-id="99eea-125">Calculation Formula</span></span>  
<span data-ttu-id="99eea-126">As described in the preceding table, the availability of a given serial or lot number is calculated as follows:</span><span class="sxs-lookup"><span data-stu-id="99eea-126">As described in the preceding table, the availability of a given serial or lot number is calculated as follows:</span></span>  

* <span data-ttu-id="99eea-127">total available quantity = quantity in inventory – (all demands + quantity not yet committed to the database)</span><span class="sxs-lookup"><span data-stu-id="99eea-127">total available quantity = quantity in inventory – (all demands + quantity not yet committed to the database)</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="99eea-128">This formula implies that the serial or lot number availability calculation considers only inventory and ignores projected receipts.</span><span class="sxs-lookup"><span data-stu-id="99eea-128">This formula implies that the serial or lot number availability calculation considers only inventory and ignores projected receipts.</span></span> <span data-ttu-id="99eea-129">Accordingly, supply that is not yet posted to inventory does not affect item tracking availability, as opposed to regular item availability where projected receipts are included.</span><span class="sxs-lookup"><span data-stu-id="99eea-129">Accordingly, supply that is not yet posted to inventory does not affect item tracking availability, as opposed to regular item availability where projected receipts are included.</span></span>  

## <a name="see-also"></a><span data-ttu-id="99eea-130">See Also</span><span class="sxs-lookup"><span data-stu-id="99eea-130">See Also</span></span>  
[<span data-ttu-id="99eea-131">Design Details: Item Tracking</span><span class="sxs-lookup"><span data-stu-id="99eea-131">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)

