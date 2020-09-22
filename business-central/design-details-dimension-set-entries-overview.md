---
title: Dimension Set Entries Overview | Microsoft Docs
description: This topic describes how dimension set entries are stored and posted in Dynamcis 365.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dimension
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: b9b69b539228e92776e1a7ee4c2fb491b20c1a15
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3788003"
---
# <a name="dimension-set-entries-overview"></a><span data-ttu-id="4af7d-103">Dimension Set Entries Overview</span><span class="sxs-lookup"><span data-stu-id="4af7d-103">Dimension Set Entries Overview</span></span>
<span data-ttu-id="4af7d-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4af7d-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="dimension-sets"></a><span data-ttu-id="4af7d-105">Dimension Sets</span><span class="sxs-lookup"><span data-stu-id="4af7d-105">Dimension Sets</span></span>  
<span data-ttu-id="4af7d-106">A dimension set is a unique combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="4af7d-106">A dimension set is a unique combination of dimension values.</span></span> <span data-ttu-id="4af7d-107">It is stored as dimension set entries in the database.</span><span class="sxs-lookup"><span data-stu-id="4af7d-107">It is stored as dimension set entries in the database.</span></span> <span data-ttu-id="4af7d-108">Each dimension set entry represents a single dimension value.</span><span class="sxs-lookup"><span data-stu-id="4af7d-108">Each dimension set entry represents a single dimension value.</span></span> <span data-ttu-id="4af7d-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span><span class="sxs-lookup"><span data-stu-id="4af7d-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span></span>  

<span data-ttu-id="4af7d-110">The following example shows a dimension set that has three dimension set entries.</span><span class="sxs-lookup"><span data-stu-id="4af7d-110">The following example shows a dimension set that has three dimension set entries.</span></span> <span data-ttu-id="4af7d-111">The dimension set is identified by a dimension set ID, which is 108.</span><span class="sxs-lookup"><span data-stu-id="4af7d-111">The dimension set is identified by a dimension set ID, which is 108.</span></span>  

|<span data-ttu-id="4af7d-112">Dimension Set ID</span><span class="sxs-lookup"><span data-stu-id="4af7d-112">Dimension Set ID</span></span>|<span data-ttu-id="4af7d-113">Dimension Code</span><span class="sxs-lookup"><span data-stu-id="4af7d-113">Dimension Code</span></span>|<span data-ttu-id="4af7d-114">Dimension Value Code</span><span class="sxs-lookup"><span data-stu-id="4af7d-114">Dimension Value Code</span></span>|<span data-ttu-id="4af7d-115">Dimension Value Name</span><span class="sxs-lookup"><span data-stu-id="4af7d-115">Dimension Value Name</span></span>|  
|----------------------|--------------------|--------------------------|--------------------------|  
|<span data-ttu-id="4af7d-116">108</span><span class="sxs-lookup"><span data-stu-id="4af7d-116">108</span></span>|<span data-ttu-id="4af7d-117">AREA</span><span class="sxs-lookup"><span data-stu-id="4af7d-117">AREA</span></span>|<span data-ttu-id="4af7d-118">70</span><span class="sxs-lookup"><span data-stu-id="4af7d-118">70</span></span>|<span data-ttu-id="4af7d-119">America North</span><span class="sxs-lookup"><span data-stu-id="4af7d-119">America North</span></span>|  
|<span data-ttu-id="4af7d-120">108</span><span class="sxs-lookup"><span data-stu-id="4af7d-120">108</span></span>|<span data-ttu-id="4af7d-121">BUSINESSGROUP</span><span class="sxs-lookup"><span data-stu-id="4af7d-121">BUSINESSGROUP</span></span>|<span data-ttu-id="4af7d-122">HOME</span><span class="sxs-lookup"><span data-stu-id="4af7d-122">HOME</span></span>|<span data-ttu-id="4af7d-123">Home</span><span class="sxs-lookup"><span data-stu-id="4af7d-123">Home</span></span>|  
|<span data-ttu-id="4af7d-124">108</span><span class="sxs-lookup"><span data-stu-id="4af7d-124">108</span></span>|<span data-ttu-id="4af7d-125">DEPARTMENT</span><span class="sxs-lookup"><span data-stu-id="4af7d-125">DEPARTMENT</span></span>|<span data-ttu-id="4af7d-126">SALES</span><span class="sxs-lookup"><span data-stu-id="4af7d-126">SALES</span></span>|<span data-ttu-id="4af7d-127">Sales</span><span class="sxs-lookup"><span data-stu-id="4af7d-127">Sales</span></span>|  

## <a name="dimension-set-entries"></a><span data-ttu-id="4af7d-128">Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="4af7d-128">Dimension Set Entries</span></span>  
<span data-ttu-id="4af7d-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span><span class="sxs-lookup"><span data-stu-id="4af7d-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span></span>  

<span data-ttu-id="4af7d-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span><span class="sxs-lookup"><span data-stu-id="4af7d-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span></span>  

<span data-ttu-id="4af7d-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="4af7d-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span></span> <span data-ttu-id="4af7d-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span><span class="sxs-lookup"><span data-stu-id="4af7d-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span></span>  

<span data-ttu-id="4af7d-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span><span class="sxs-lookup"><span data-stu-id="4af7d-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span></span> <span data-ttu-id="4af7d-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="4af7d-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span></span> <span data-ttu-id="4af7d-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="4af7d-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span></span>

## <a name="codeunit-408-dimension-management"></a><span data-ttu-id="4af7d-136">Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="4af7d-136">Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="4af7d-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="4af7d-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span>

## <a name="performance-improvement"></a><span data-ttu-id="4af7d-138">Performance Improvement</span><span class="sxs-lookup"><span data-stu-id="4af7d-138">Performance Improvement</span></span>  
<span data-ttu-id="4af7d-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span><span class="sxs-lookup"><span data-stu-id="4af7d-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4af7d-140">See Also</span><span class="sxs-lookup"><span data-stu-id="4af7d-140">See Also</span></span>  
<span data-ttu-id="4af7d-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="4af7d-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
<span data-ttu-id="4af7d-142">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="4af7d-142">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
[<span data-ttu-id="4af7d-143">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="4af7d-143">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   
