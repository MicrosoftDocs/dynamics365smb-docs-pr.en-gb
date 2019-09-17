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
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 051cb40676560bcb531c6708960986a69e7cfdf4
ms.sourcegitcommit: 1fa3d33db7bc71e3a27c826308a80ff24a436a72
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/30/2019
ms.locfileid: "1970885"
---
# <a name="dimension-set-entries-overview"></a><span data-ttu-id="14299-103">Dimension Set Entries Overview</span><span class="sxs-lookup"><span data-stu-id="14299-103">Dimension Set Entries Overview</span></span>
<span data-ttu-id="14299-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="14299-104">This topic describes how dimension set entries are stored and posted in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="dimension-sets"></a><span data-ttu-id="14299-105">Dimension Sets</span><span class="sxs-lookup"><span data-stu-id="14299-105">Dimension Sets</span></span>  
<span data-ttu-id="14299-106">A dimension set is a unique combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="14299-106">A dimension set is a unique combination of dimension values.</span></span> <span data-ttu-id="14299-107">It is stored as dimension set entries in the database.</span><span class="sxs-lookup"><span data-stu-id="14299-107">It is stored as dimension set entries in the database.</span></span> <span data-ttu-id="14299-108">Each dimension set entry represents a single dimension value.</span><span class="sxs-lookup"><span data-stu-id="14299-108">Each dimension set entry represents a single dimension value.</span></span> <span data-ttu-id="14299-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span><span class="sxs-lookup"><span data-stu-id="14299-109">The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.</span></span>  

<span data-ttu-id="14299-110">The following example shows a dimension set that has three dimension set entries.</span><span class="sxs-lookup"><span data-stu-id="14299-110">The following example shows a dimension set that has three dimension set entries.</span></span> <span data-ttu-id="14299-111">The dimension set is identified by a dimension set ID, which is 108.</span><span class="sxs-lookup"><span data-stu-id="14299-111">The dimension set is identified by a dimension set ID, which is 108.</span></span>  

|<span data-ttu-id="14299-112">Dimension Set ID</span><span class="sxs-lookup"><span data-stu-id="14299-112">Dimension Set ID</span></span>|<span data-ttu-id="14299-113">Dimension Code</span><span class="sxs-lookup"><span data-stu-id="14299-113">Dimension Code</span></span>|<span data-ttu-id="14299-114">Dimension Value Code</span><span class="sxs-lookup"><span data-stu-id="14299-114">Dimension Value Code</span></span>|<span data-ttu-id="14299-115">Dimension Value Name</span><span class="sxs-lookup"><span data-stu-id="14299-115">Dimension Value Name</span></span>|  
|----------------------|--------------------|--------------------------|--------------------------|  
|<span data-ttu-id="14299-116">108</span><span class="sxs-lookup"><span data-stu-id="14299-116">108</span></span>|<span data-ttu-id="14299-117">AREA</span><span class="sxs-lookup"><span data-stu-id="14299-117">AREA</span></span>|<span data-ttu-id="14299-118">70</span><span class="sxs-lookup"><span data-stu-id="14299-118">70</span></span>|<span data-ttu-id="14299-119">America North</span><span class="sxs-lookup"><span data-stu-id="14299-119">America North</span></span>|  
|<span data-ttu-id="14299-120">108</span><span class="sxs-lookup"><span data-stu-id="14299-120">108</span></span>|<span data-ttu-id="14299-121">BUSINESSGROUP</span><span class="sxs-lookup"><span data-stu-id="14299-121">BUSINESSGROUP</span></span>|<span data-ttu-id="14299-122">HOME</span><span class="sxs-lookup"><span data-stu-id="14299-122">HOME</span></span>|<span data-ttu-id="14299-123">Home</span><span class="sxs-lookup"><span data-stu-id="14299-123">Home</span></span>|  
|<span data-ttu-id="14299-124">108</span><span class="sxs-lookup"><span data-stu-id="14299-124">108</span></span>|<span data-ttu-id="14299-125">DEPARTMENT</span><span class="sxs-lookup"><span data-stu-id="14299-125">DEPARTMENT</span></span>|<span data-ttu-id="14299-126">SALES</span><span class="sxs-lookup"><span data-stu-id="14299-126">SALES</span></span>|<span data-ttu-id="14299-127">Sales</span><span class="sxs-lookup"><span data-stu-id="14299-127">Sales</span></span>|  

## <a name="dimension-set-entries"></a><span data-ttu-id="14299-128">Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="14299-128">Dimension Set Entries</span></span>  
<span data-ttu-id="14299-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span><span class="sxs-lookup"><span data-stu-id="14299-129">Dimension sets are stored in the **Dimension Set Entry** table as dimension set entries with the same dimension set ID.</span></span>  

<span data-ttu-id="14299-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span><span class="sxs-lookup"><span data-stu-id="14299-130">![Flow of dimension set entries](media/dimensionentrynav7.png "Flow of dimension set entries")</span></span>  

<span data-ttu-id="14299-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span><span class="sxs-lookup"><span data-stu-id="14299-131">When you create a new journal line, document header, or document line, you can specify a combination of dimension values.</span></span> <span data-ttu-id="14299-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span><span class="sxs-lookup"><span data-stu-id="14299-132">Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.</span></span>  

<span data-ttu-id="14299-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span><span class="sxs-lookup"><span data-stu-id="14299-133">When you edit and close the **Edit Dimension Set Entries** page, a check is performed to see whether the combination of dimension values exists as a dimension set in the table.</span></span> <span data-ttu-id="14299-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="14299-134">If the combination occurs in the table, then the corresponding dimension set ID is assigned to the journal line, document header, or document line.</span></span> <span data-ttu-id="14299-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span><span class="sxs-lookup"><span data-stu-id="14299-135">Otherwise, a new dimension set is added to the table, and the new dimension set ID is assigned to the journal line, document header, or document line.</span></span>

## <a name="codeunit-408-dimension-management"></a><span data-ttu-id="14299-136">Codeunit 408 Dimension Management</span><span class="sxs-lookup"><span data-stu-id="14299-136">Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="14299-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span><span class="sxs-lookup"><span data-stu-id="14299-137">Codeunit 408, Dimension Management, is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span>

## <a name="performance-improvement"></a><span data-ttu-id="14299-138">Performance Improvement</span><span class="sxs-lookup"><span data-stu-id="14299-138">Performance Improvement</span></span>  
<span data-ttu-id="14299-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span><span class="sxs-lookup"><span data-stu-id="14299-139">By storing dimension sets once in the database, database space is preserved and overall performance is improved.</span></span>  

## <a name="see-also"></a><span data-ttu-id="14299-140">See Also</span><span class="sxs-lookup"><span data-stu-id="14299-140">See Also</span></span>  
<span data-ttu-id="14299-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="14299-141">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
<span data-ttu-id="14299-142">[Design Details: Table Structure](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="14299-142">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
[<span data-ttu-id="14299-143">Design Details: Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="14299-143">Design Details: Dimension Set Entries</span></span>](design-details-dimension-set-entries.md)   
