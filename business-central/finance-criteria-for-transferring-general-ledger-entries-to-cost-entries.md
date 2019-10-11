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
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: fe7a7d0c3d7a56f129a1ae94d1e7f015eb145bda
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302459"
---
# <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="d34b6-104">Criteria for Transferring General Ledger Entries to Cost Entries</span><span class="sxs-lookup"><span data-stu-id="d34b6-104">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="d34b6-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span><span class="sxs-lookup"><span data-stu-id="d34b6-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span></span> <span data-ttu-id="d34b6-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span><span class="sxs-lookup"><span data-stu-id="d34b6-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span></span>  

<span data-ttu-id="d34b6-107">General ledger entries are transferred if:</span><span class="sxs-lookup"><span data-stu-id="d34b6-107">General ledger entries are transferred if:</span></span>  

-   <span data-ttu-id="d34b6-108">The entries have dimension values corresponding to either a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="d34b6-108">The entries have dimension values corresponding to either a cost center or a cost object.</span></span>  
-   <span data-ttu-id="d34b6-109">The entries have dimension values that correspond to a cost centre and a cost object.</span><span class="sxs-lookup"><span data-stu-id="d34b6-109">The entries have dimension values that correspond to a cost center and a cost object.</span></span> <span data-ttu-id="d34b6-110">For these entries, the cost centre takes precedence.</span><span class="sxs-lookup"><span data-stu-id="d34b6-110">For these entries, the cost center takes precedence.</span></span> <span data-ttu-id="d34b6-111">This helps avoid a situation where a cost type appears in both a cost object and a cost centre and is therefore counted twice in the statistics.</span><span class="sxs-lookup"><span data-stu-id="d34b6-111">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span></span>  
-   <span data-ttu-id="d34b6-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span><span class="sxs-lookup"><span data-stu-id="d34b6-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span></span>  
-   <span data-ttu-id="d34b6-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span><span class="sxs-lookup"><span data-stu-id="d34b6-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span></span>  

<span data-ttu-id="d34b6-114">General ledger entries are not transferred if:</span><span class="sxs-lookup"><span data-stu-id="d34b6-114">General ledger entries are not transferred if:</span></span>  

-   <span data-ttu-id="d34b6-115">The entries have dimension values that do not correspond to a cost centre or a cost object.</span><span class="sxs-lookup"><span data-stu-id="d34b6-115">The entries have dimension values that do not correspond to a cost center or a cost object.</span></span>  
-   <span data-ttu-id="d34b6-116">The entries have an amount of zero.</span><span class="sxs-lookup"><span data-stu-id="d34b6-116">The entries have an amount of zero.</span></span>  
-   <span data-ttu-id="d34b6-117">The entries have a general ledger account that has been deleted.</span><span class="sxs-lookup"><span data-stu-id="d34b6-117">The entries have a general ledger account that has been deleted.</span></span>  
-   <span data-ttu-id="d34b6-118">The entries have a general ledger account that is not of the type **Income Statement**.</span><span class="sxs-lookup"><span data-stu-id="d34b6-118">The entries have a general ledger account that is not of the type **Income Statement**.</span></span>  
-   <span data-ttu-id="d34b6-119">The entries have a general ledger account that is not assigned a cost type.</span><span class="sxs-lookup"><span data-stu-id="d34b6-119">The entries have a general ledger account that is not assigned a cost type.</span></span>  
-   <span data-ttu-id="d34b6-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span><span class="sxs-lookup"><span data-stu-id="d34b6-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span></span>  
-   <span data-ttu-id="d34b6-121">The entries have been posted with a closing date.</span><span class="sxs-lookup"><span data-stu-id="d34b6-121">The entries have been posted with a closing date.</span></span> <span data-ttu-id="d34b6-122">These are typically entries that set back the balance of the income statement at the end of the year.</span><span class="sxs-lookup"><span data-stu-id="d34b6-122">These are typically entries that set back the balance of the income statement at the end of the year.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d34b6-123">See Also</span><span class="sxs-lookup"><span data-stu-id="d34b6-123">See Also</span></span>  
[<span data-ttu-id="d34b6-124">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="d34b6-124">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
 <span data-ttu-id="d34b6-125">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="d34b6-125">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="d34b6-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="d34b6-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="d34b6-127">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="d34b6-127">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
 <span data-ttu-id="d34b6-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d34b6-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
