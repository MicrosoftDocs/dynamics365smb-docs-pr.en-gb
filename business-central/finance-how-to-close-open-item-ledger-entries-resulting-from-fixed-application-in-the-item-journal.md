---
title: Close item ledger entries that came from using fixed application
description: Learn how you can create a fixed application between an inbound transaction and the original outbound transaction in the item journal.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 01/14/2020
ms.author: edupont
ms.openlocfilehash: 2cc663d580da4738247b9fcdbe5fc4504c37fa73
ms.sourcegitcommit: 311e86d6abb9b59a5483324d8bb4cd1be7949248
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/15/2021
ms.locfileid: "5013878"
---
# <a name="close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a><span data-ttu-id="39fa0-103">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span><span class="sxs-lookup"><span data-stu-id="39fa0-103">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>

<span data-ttu-id="39fa0-104">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span><span class="sxs-lookup"><span data-stu-id="39fa0-104">You can use the **Applies-from Entry** field on the **Item Journal** page to create a fixed application between an inbound transaction and the original outbound transaction.</span></span> <span data-ttu-id="39fa0-105">For example, to correct the outbound transaction or to process its return.</span><span class="sxs-lookup"><span data-stu-id="39fa0-105">For example, to correct the outbound transaction or to process its return.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="39fa0-106">Fixed applications made in this manner only apply the cost, not the quantity.</span><span class="sxs-lookup"><span data-stu-id="39fa0-106">Fixed applications made in this manner only apply the cost, not the quantity.</span></span> <span data-ttu-id="39fa0-107">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span><span class="sxs-lookup"><span data-stu-id="39fa0-107">Accordingly, the posted positive item ledger entry will not close the applied outbound entry and will itself remain open.</span></span> <span data-ttu-id="39fa0-108">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span><span class="sxs-lookup"><span data-stu-id="39fa0-108">This also applies when you post a fixed application for a positive entry to a negative entry that has not been closed by a regular positive entry, then both the negative and the positive entries will remain open.</span></span>  
>
> <span data-ttu-id="39fa0-109">This also means that you cannot close an inventory period if such an entry exists.</span><span class="sxs-lookup"><span data-stu-id="39fa0-109">This also means that you cannot close an inventory period if such an entry exists.</span></span>  

<span data-ttu-id="39fa0-110">You can change and reapply application entries under certain conditions by using the **Application Worksheet** page.</span><span class="sxs-lookup"><span data-stu-id="39fa0-110">You can change and reapply application entries under certain conditions by using the **Application Worksheet** page.</span></span>  

<span data-ttu-id="39fa0-111">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span><span class="sxs-lookup"><span data-stu-id="39fa0-111">The following procedure shows how to close such entries by performing two corrective postings in the item journal.</span></span>  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a><span data-ttu-id="39fa0-112">To close open item ledger entries that result from a fixed application in the item journal</span><span class="sxs-lookup"><span data-stu-id="39fa0-112">To close open item ledger entries that result from a fixed application in the item journal</span></span>  

1. <span data-ttu-id="39fa0-113">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span><span class="sxs-lookup"><span data-stu-id="39fa0-113">Use the **Applies-from Entry** field to post a positive adjustment with the corresponding quantity.</span></span> <span data-ttu-id="39fa0-114">This closes the original negative entry with a fixed application.</span><span class="sxs-lookup"><span data-stu-id="39fa0-114">This closes the original negative entry with a fixed application.</span></span>  

    <span data-ttu-id="39fa0-115">The **Applies-from Entry** field specifies the number of the outbound item ledger entry whose cost is forwarded to the inbound item ledger entry when you post an inbound transaction of type **Positive Adjmt.** or **Purchase** with the item journal.</span><span class="sxs-lookup"><span data-stu-id="39fa0-115">The **Applies-from Entry** field specifies the number of the outbound item ledger entry whose cost is forwarded to the inbound item ledger entry when you post an inbound transaction of type **Positive Adjmt.** or **Purchase** with the item journal.</span></span>  
2. <span data-ttu-id="39fa0-116">Use the **Applies-to Entry** field to post a negative adjustment.</span><span class="sxs-lookup"><span data-stu-id="39fa0-116">Use the **Applies-to Entry** field to post a negative adjustment.</span></span> <span data-ttu-id="39fa0-117">This closes the original corrective positive entry with a fixed application.</span><span class="sxs-lookup"><span data-stu-id="39fa0-117">This closes the original corrective positive entry with a fixed application.</span></span>  

    <span data-ttu-id="39fa0-118">The **Applies-to Entry** field specifies if the quantity in the item journal line should be applied to an already-posted document.</span><span class="sxs-lookup"><span data-stu-id="39fa0-118">The **Applies-to Entry** field specifies if the quantity in the item journal line should be applied to an already-posted document.</span></span> <span data-ttu-id="39fa0-119">If this is the case, enter the entry number of the item ledger entry to which the item journal line should be applied.</span><span class="sxs-lookup"><span data-stu-id="39fa0-119">If this is the case, enter the entry number of the item ledger entry to which the item journal line should be applied.</span></span>

## <a name="see-also"></a><span data-ttu-id="39fa0-120">See Also</span><span class="sxs-lookup"><span data-stu-id="39fa0-120">See Also</span></span>

[<span data-ttu-id="39fa0-121">Remove and Reapply Item Ledger Entries</span><span class="sxs-lookup"><span data-stu-id="39fa0-121">Remove and Reapply Item Ledger Entries</span></span>](finance-how-to-remove-and-reapply-item-entries.md)  
[<span data-ttu-id="39fa0-122">Process Sales Returns and Cancellations</span><span class="sxs-lookup"><span data-stu-id="39fa0-122">Process Sales Returns and Cancellations</span></span>](sales-how-process-sales-returns-cancellations.md)  
[<span data-ttu-id="39fa0-123">Setting Up Inventory Valuation and Costing</span><span class="sxs-lookup"><span data-stu-id="39fa0-123">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)  
[<span data-ttu-id="39fa0-124">Managing Inventory Costs</span><span class="sxs-lookup"><span data-stu-id="39fa0-124">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="39fa0-125">Design Details: Costing Methods</span><span class="sxs-lookup"><span data-stu-id="39fa0-125">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)
