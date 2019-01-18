---
title: Automatic Transfer and Combined Entries | Microsoft Docs
description: In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting. You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition. The following table describes the different options.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 6f58e569bea6a42a9ee695095ce308e7a69e2a8d
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="0dab6-105">Automatic Transfer and Combined Entries</span><span class="sxs-lookup"><span data-stu-id="0dab6-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="0dab6-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span><span class="sxs-lookup"><span data-stu-id="0dab6-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="0dab6-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span><span class="sxs-lookup"><span data-stu-id="0dab6-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="0dab6-108">The following table describes the different options.</span><span class="sxs-lookup"><span data-stu-id="0dab6-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="0dab6-109">Combine entries</span><span class="sxs-lookup"><span data-stu-id="0dab6-109">Combine entries</span></span>|<span data-ttu-id="0dab6-110">Description</span><span class="sxs-lookup"><span data-stu-id="0dab6-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="0dab6-111">None</span><span class="sxs-lookup"><span data-stu-id="0dab6-111">None</span></span>|<span data-ttu-id="0dab6-112">Each general ledger entry is transferred individually to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="0dab6-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="0dab6-113">Day</span><span class="sxs-lookup"><span data-stu-id="0dab6-113">Day</span></span>|<span data-ttu-id="0dab6-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="0dab6-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="0dab6-115">Month</span><span class="sxs-lookup"><span data-stu-id="0dab6-115">Month</span></span>|<span data-ttu-id="0dab6-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span><span class="sxs-lookup"><span data-stu-id="0dab6-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="0dab6-117">If you have selected the **Auto Transfer from G/L** check box on the **Cost Accounting Setup** page, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="0dab6-117">If you have selected the **Auto Transfer from G/L** check box on the **Cost Accounting Setup** page, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="0dab6-118">Combined entries are not possible.</span><span class="sxs-lookup"><span data-stu-id="0dab6-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0dab6-119">See Also</span><span class="sxs-lookup"><span data-stu-id="0dab6-119">See Also</span></span>  
 <span data-ttu-id="0dab6-120">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="0dab6-120">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="0dab6-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0dab6-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

