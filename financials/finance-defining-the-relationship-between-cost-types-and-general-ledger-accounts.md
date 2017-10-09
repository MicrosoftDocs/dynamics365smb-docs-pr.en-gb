---
title: Defining the Relationship Between Cost Types and General Ledger Accounts | Microsoft Docs
description: Learn how to define the relationship between the cost type and the general ledger account.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0f2f30b8b56ae4afcff230a7934a6bcac4d205db
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="bd4f6-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span><span class="sxs-lookup"><span data-stu-id="bd4f6-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="bd4f6-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="bd4f6-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="bd4f6-106">The **Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="bd4f6-106">The **Cost Type No.**</span></span> <span data-ttu-id="bd4f6-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="bd4f6-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="bd4f6-109">Relationship Between General Ledger Accounts and Cost Types</span><span class="sxs-lookup"><span data-stu-id="bd4f6-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="bd4f6-110">There is an n:1 relationship between general ledger accounts and cost types.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="bd4f6-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="bd4f6-112">The following table describes the details in the relationship.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="bd4f6-113">Relationship</span><span class="sxs-lookup"><span data-stu-id="bd4f6-113">Relationship</span></span>|<span data-ttu-id="bd4f6-114">**G/L Account Range**</span><span class="sxs-lookup"><span data-stu-id="bd4f6-114">**G/L Account Range**</span></span>|<span data-ttu-id="bd4f6-115">**Cost Type No.**</span><span class="sxs-lookup"><span data-stu-id="bd4f6-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="bd4f6-116">One general ledger account for each cost type</span><span class="sxs-lookup"><span data-stu-id="bd4f6-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="bd4f6-117">One general ledger account</span><span class="sxs-lookup"><span data-stu-id="bd4f6-117">One general ledger account</span></span>|<span data-ttu-id="bd4f6-118">One cost type</span><span class="sxs-lookup"><span data-stu-id="bd4f6-118">One cost type</span></span>|  
|<span data-ttu-id="bd4f6-119">Several general ledger accounts for one cost type</span><span class="sxs-lookup"><span data-stu-id="bd4f6-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="bd4f6-120">General ledger account range, for example, 7110..7193 for each general ledger account</span><span class="sxs-lookup"><span data-stu-id="bd4f6-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="bd4f6-121">For each general ledger account in the range, there is only one cost type</span><span class="sxs-lookup"><span data-stu-id="bd4f6-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="bd4f6-122">Cost types without corresponding general ledger accounts</span><span class="sxs-lookup"><span data-stu-id="bd4f6-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="bd4f6-123">General ledger accounts whose entries will not be transferred</span><span class="sxs-lookup"><span data-stu-id="bd4f6-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="bd4f6-124">Cost Types Without a Relationship to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="bd4f6-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="bd4f6-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span><span class="sxs-lookup"><span data-stu-id="bd4f6-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="bd4f6-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="bd4f6-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="bd4f6-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span><span class="sxs-lookup"><span data-stu-id="bd4f6-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bd4f6-129">See Also</span><span class="sxs-lookup"><span data-stu-id="bd4f6-129">See Also</span></span>  
[<span data-ttu-id="bd4f6-130">Accounting for Costs</span><span class="sxs-lookup"><span data-stu-id="bd4f6-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="bd4f6-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="bd4f6-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="bd4f6-132">About Cost Accounting</span><span class="sxs-lookup"><span data-stu-id="bd4f6-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="bd4f6-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bd4f6-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

