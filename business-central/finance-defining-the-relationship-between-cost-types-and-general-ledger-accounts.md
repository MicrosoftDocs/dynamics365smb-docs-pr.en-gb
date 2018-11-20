---
title: Defining the Relationship Between Cost Types and General Ledger Accounts | Microsoft Docs
description: Learn how to define the relationship between the cost type and the general ledger account.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 11/13/2018
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.translationtype: HT
ms.sourcegitcommit: 67400e424305cc705db5c1bd52a8e4de17ecc5a9
ms.openlocfilehash: f80e9b6276d26adffb5e3208ffefbf98d7f7ff96
ms.contentlocale: en-gb
ms.lasthandoff: 11/20/2018

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="83401-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span><span class="sxs-lookup"><span data-stu-id="83401-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="83401-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span><span class="sxs-lookup"><span data-stu-id="83401-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="83401-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span><span class="sxs-lookup"><span data-stu-id="83401-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="83401-106">The **Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="83401-106">The **Cost Type No.**</span></span> <span data-ttu-id="83401-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span><span class="sxs-lookup"><span data-stu-id="83401-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="83401-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span><span class="sxs-lookup"><span data-stu-id="83401-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="83401-109">Relationship Between General Ledger Accounts and Cost Types</span><span class="sxs-lookup"><span data-stu-id="83401-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="83401-110">There is an n:1 relationship between general ledger accounts and cost types.</span><span class="sxs-lookup"><span data-stu-id="83401-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="83401-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="83401-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="83401-112">The following table describes the details in the relationship.</span><span class="sxs-lookup"><span data-stu-id="83401-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="83401-113">Relationship</span><span class="sxs-lookup"><span data-stu-id="83401-113">Relationship</span></span>|<span data-ttu-id="83401-114">**G/L Account Range**</span><span class="sxs-lookup"><span data-stu-id="83401-114">**G/L Account Range**</span></span>|<span data-ttu-id="83401-115">**Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="83401-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="83401-116">One general ledger account for each cost type</span><span class="sxs-lookup"><span data-stu-id="83401-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="83401-117">One general ledger account</span><span class="sxs-lookup"><span data-stu-id="83401-117">One general ledger account</span></span>|<span data-ttu-id="83401-118">One cost type</span><span class="sxs-lookup"><span data-stu-id="83401-118">One cost type</span></span>|  
|<span data-ttu-id="83401-119">Several general ledger accounts for one cost type</span><span class="sxs-lookup"><span data-stu-id="83401-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="83401-120">General ledger account range, for example, 7110..7193 for each general ledger account</span><span class="sxs-lookup"><span data-stu-id="83401-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="83401-121">For each general ledger account in the range, there is only one cost type</span><span class="sxs-lookup"><span data-stu-id="83401-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="83401-122">Cost types without corresponding general ledger accounts</span><span class="sxs-lookup"><span data-stu-id="83401-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="83401-123">General ledger accounts whose entries will not be transferred</span><span class="sxs-lookup"><span data-stu-id="83401-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="83401-124">Cost Types Without a Relationship to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="83401-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="83401-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span><span class="sxs-lookup"><span data-stu-id="83401-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="83401-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span><span class="sxs-lookup"><span data-stu-id="83401-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="83401-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span><span class="sxs-lookup"><span data-stu-id="83401-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="83401-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="83401-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="83401-129">See Also</span><span class="sxs-lookup"><span data-stu-id="83401-129">See Also</span></span>  
[<span data-ttu-id="83401-130">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="83401-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="83401-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="83401-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="83401-132">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="83401-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="83401-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="83401-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

