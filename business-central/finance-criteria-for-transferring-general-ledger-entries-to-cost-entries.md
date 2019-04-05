---
title: Criteria for Transferring General Ledger Entries to Cost Entries | Microsoft Docs
description: It is important to understand the criteria for transferring general ledger entries to cost entries. During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: 6e5fcfedbb899633f61c05b0b8b5ec8125112d65
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "808709"
---
# <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="80f4d-104">Criteria for Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="80f4d-104">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="80f4d-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span><span class="sxs-lookup"><span data-stu-id="80f4d-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span></span> <span data-ttu-id="80f4d-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span><span class="sxs-lookup"><span data-stu-id="80f4d-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span></span>  

<span data-ttu-id="80f4d-107">General ledger entries are transferred if:</span><span class="sxs-lookup"><span data-stu-id="80f4d-107">General ledger entries are transferred if:</span></span>  

-   <span data-ttu-id="80f4d-108">The entries have dimension values corresponding to either a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="80f4d-108">The entries have dimension values corresponding to either a cost center or a cost object.</span></span>  
-   <span data-ttu-id="80f4d-109">The entries have dimension values that correspond to a cost centre and a cost object.</span><span class="sxs-lookup"><span data-stu-id="80f4d-109">The entries have dimension values that correspond to a cost center and a cost object.</span></span> <span data-ttu-id="80f4d-110">For these entries, the cost centre takes precedence.</span><span class="sxs-lookup"><span data-stu-id="80f4d-110">For these entries, the cost center takes precedence.</span></span> <span data-ttu-id="80f4d-111">This helps avoid a situation where a cost type appears in both a cost object and a cost centre and is therefore counted twice in the statistics.</span><span class="sxs-lookup"><span data-stu-id="80f4d-111">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span></span>  
-   <span data-ttu-id="80f4d-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span><span class="sxs-lookup"><span data-stu-id="80f4d-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span></span>  
-   <span data-ttu-id="80f4d-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span><span class="sxs-lookup"><span data-stu-id="80f4d-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span></span>  

<span data-ttu-id="80f4d-114">General ledger entries are not transferred if:</span><span class="sxs-lookup"><span data-stu-id="80f4d-114">General ledger entries are not transferred if:</span></span>  

-   <span data-ttu-id="80f4d-115">The entries have dimension values that do not correspond to a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="80f4d-115">The entries have dimension values that do not correspond to a cost center or a cost object.</span></span>  
-   <span data-ttu-id="80f4d-116">The entries have an amount of zero.</span><span class="sxs-lookup"><span data-stu-id="80f4d-116">The entries have an amount of zero.</span></span>  
-   <span data-ttu-id="80f4d-117">The entries have a general ledger account that has been deleted.</span><span class="sxs-lookup"><span data-stu-id="80f4d-117">The entries have a general ledger account that has been deleted.</span></span>  
-   <span data-ttu-id="80f4d-118">The entries have a general ledger account that is not of the type **Income Statement**.</span><span class="sxs-lookup"><span data-stu-id="80f4d-118">The entries have a general ledger account that is not of the type **Income Statement**.</span></span>  
-   <span data-ttu-id="80f4d-119">The entries have a general ledger account that is not assigned a cost type.</span><span class="sxs-lookup"><span data-stu-id="80f4d-119">The entries have a general ledger account that is not assigned a cost type.</span></span>  
-   <span data-ttu-id="80f4d-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span><span class="sxs-lookup"><span data-stu-id="80f4d-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span></span>  
-   <span data-ttu-id="80f4d-121">The entries have been posted with a closing date.</span><span class="sxs-lookup"><span data-stu-id="80f4d-121">The entries have been posted with a closing date.</span></span> <span data-ttu-id="80f4d-122">These are typically entries that set back the balance of the income statement at the end of the year.</span><span class="sxs-lookup"><span data-stu-id="80f4d-122">These are typically entries that set back the balance of the income statement at the end of the year.</span></span>  

## <a name="see-also"></a><span data-ttu-id="80f4d-123">See Also</span><span class="sxs-lookup"><span data-stu-id="80f4d-123">See Also</span></span>  
[<span data-ttu-id="80f4d-124">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="80f4d-124">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
 <span data-ttu-id="80f4d-125">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="80f4d-125">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="80f4d-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="80f4d-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="80f4d-127">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="80f4d-127">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
 <span data-ttu-id="80f4d-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="80f4d-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
