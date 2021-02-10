---
title: Design Details - Searching for Dimension Combinations | Microsoft Docs
description: When you close a page after you edit a set of dimensions, Business Central evaluates whether the edited set of dimensions exists. If the set does not exist, a new set is created and the dimension combination ID is returned.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: c3867c45f659f054a3bdee1605f2d8541e72dec1
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751137"
---
# <a name="design-details-searching-for-dimension-combinations"></a><span data-ttu-id="c66aa-104">Design Details: Searching for Dimension Combinations</span><span class="sxs-lookup"><span data-stu-id="c66aa-104">Design Details: Searching for Dimension Combinations</span></span>
<span data-ttu-id="c66aa-105">When you close a page after you edit a set of dimensions, [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether the edited set of dimensions exists.</span><span class="sxs-lookup"><span data-stu-id="c66aa-105">When you close a page after you edit a set of dimensions, [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether the edited set of dimensions exists.</span></span> <span data-ttu-id="c66aa-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span><span class="sxs-lookup"><span data-stu-id="c66aa-106">If the set does not exist, a new set is created and the dimension combination ID is returned.</span></span>  

## <a name="building-search-tree"></a><span data-ttu-id="c66aa-107">Building Search Tree</span><span class="sxs-lookup"><span data-stu-id="c66aa-107">Building Search Tree</span></span>  
 <span data-ttu-id="c66aa-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span><span class="sxs-lookup"><span data-stu-id="c66aa-108">Table 481 **Dimension Set Tree Node** is used when [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether a set of dimensions already exists in table 480 **Dimension Set Entry** table.</span></span> <span data-ttu-id="c66aa-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span><span class="sxs-lookup"><span data-stu-id="c66aa-109">The evaluation is performed by recursively traversing the search tree starting at the top level numbered 0.</span></span> <span data-ttu-id="c66aa-110">The top level 0 represents a dimension set with no dimension set entries.</span><span class="sxs-lookup"><span data-stu-id="c66aa-110">The top level 0 represents a dimension set with no dimension set entries.</span></span> <span data-ttu-id="c66aa-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span><span class="sxs-lookup"><span data-stu-id="c66aa-111">The children of this dimension set represent dimension sets with only one dimension set entry.</span></span> <span data-ttu-id="c66aa-112">The children of these dimension sets represent dimension sets with two children, and so on.</span><span class="sxs-lookup"><span data-stu-id="c66aa-112">The children of these dimension sets represent dimension sets with two children, and so on.</span></span>  

### <a name="example-1"></a><span data-ttu-id="c66aa-113">Example 1</span><span class="sxs-lookup"><span data-stu-id="c66aa-113">Example 1</span></span>  
 <span data-ttu-id="c66aa-114">The following diagram represents a search tree with six dimension sets.</span><span class="sxs-lookup"><span data-stu-id="c66aa-114">The following diagram represents a search tree with six dimension sets.</span></span> <span data-ttu-id="c66aa-115">Only the distinguishing dimension set entry is displayed in the diagram.</span><span class="sxs-lookup"><span data-stu-id="c66aa-115">Only the distinguishing dimension set entry is displayed in the diagram.</span></span>  

 <span data-ttu-id="c66aa-116">![Example of dimension tree structure](media/nav2013_dimension_tree.png "Example of dimension tree structure")</span><span class="sxs-lookup"><span data-stu-id="c66aa-116">![Example of dimension tree structure](media/nav2013_dimension_tree.png "Example of dimension tree structure")</span></span>  

 <span data-ttu-id="c66aa-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span><span class="sxs-lookup"><span data-stu-id="c66aa-117">The following table describes a complete list of dimension set entries that make up each dimension set.</span></span>  

|<span data-ttu-id="c66aa-118">Dimension Sets</span><span class="sxs-lookup"><span data-stu-id="c66aa-118">Dimension Sets</span></span>|<span data-ttu-id="c66aa-119">Dimension Set Entries</span><span class="sxs-lookup"><span data-stu-id="c66aa-119">Dimension Set Entries</span></span>|  
|--------------------|---------------------------|  
|<span data-ttu-id="c66aa-120">Set 0</span><span class="sxs-lookup"><span data-stu-id="c66aa-120">Set 0</span></span>|<span data-ttu-id="c66aa-121">None</span><span class="sxs-lookup"><span data-stu-id="c66aa-121">None</span></span>|  
|<span data-ttu-id="c66aa-122">Set 1</span><span class="sxs-lookup"><span data-stu-id="c66aa-122">Set 1</span></span>|<span data-ttu-id="c66aa-123">AREA 30</span><span class="sxs-lookup"><span data-stu-id="c66aa-123">AREA 30</span></span>|  
|<span data-ttu-id="c66aa-124">Set 2</span><span class="sxs-lookup"><span data-stu-id="c66aa-124">Set 2</span></span>|<span data-ttu-id="c66aa-125">AREA 30, DEPT ADM</span><span class="sxs-lookup"><span data-stu-id="c66aa-125">AREA 30, DEPT ADM</span></span>|  
|<span data-ttu-id="c66aa-126">Set 3</span><span class="sxs-lookup"><span data-stu-id="c66aa-126">Set 3</span></span>|<span data-ttu-id="c66aa-127">AREA 30, DEPT PROD</span><span class="sxs-lookup"><span data-stu-id="c66aa-127">AREA 30, DEPT PROD</span></span>|  
|<span data-ttu-id="c66aa-128">Set 4</span><span class="sxs-lookup"><span data-stu-id="c66aa-128">Set 4</span></span>|<span data-ttu-id="c66aa-129">AREA 30, DEPT ADM, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="c66aa-129">AREA 30, DEPT ADM, PROJ VW</span></span>|  
|<span data-ttu-id="c66aa-130">Set 5</span><span class="sxs-lookup"><span data-stu-id="c66aa-130">Set 5</span></span>|<span data-ttu-id="c66aa-131">AREA 40</span><span class="sxs-lookup"><span data-stu-id="c66aa-131">AREA 40</span></span>|  
|<span data-ttu-id="c66aa-132">Set 6</span><span class="sxs-lookup"><span data-stu-id="c66aa-132">Set 6</span></span>|<span data-ttu-id="c66aa-133">AREA 40, PROJ VW</span><span class="sxs-lookup"><span data-stu-id="c66aa-133">AREA 40, PROJ VW</span></span>|  

### <a name="example-2"></a><span data-ttu-id="c66aa-134">Example 2</span><span class="sxs-lookup"><span data-stu-id="c66aa-134">Example 2</span></span>  
 <span data-ttu-id="c66aa-135">This example shows how [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span><span class="sxs-lookup"><span data-stu-id="c66aa-135">This example shows how [!INCLUDE[prod_short](includes/prod_short.md)] evaluates whether a dimension set that consists of the dimension set entries AREA 40, DEPT PROD exists.</span></span>  

 <span data-ttu-id="c66aa-136">First, [!INCLUDE[prod_short](includes/prod_short.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span><span class="sxs-lookup"><span data-stu-id="c66aa-136">First, [!INCLUDE[prod_short](includes/prod_short.md)] also updates the **Dimension Set Tree Node** table to make sure that the search tree looks like the following diagram.</span></span> <span data-ttu-id="c66aa-137">Thus dimension set 7 becomes a child of the dimension set 5.</span><span class="sxs-lookup"><span data-stu-id="c66aa-137">Thus dimension set 7 becomes a child of the dimension set 5.</span></span>  

 <span data-ttu-id="c66aa-138">![Example of dimension tree structure in NAV 2013](media/nav2013_dimension_tree_example2.png "Example of dimension tree structure in NAV 2013")</span><span class="sxs-lookup"><span data-stu-id="c66aa-138">![Example of dimension tree structure in NAV 2013](media/nav2013_dimension_tree_example2.png "Example of dimension tree structure in NAV 2013")</span></span>  

### <a name="finding-dimension-set-id"></a><span data-ttu-id="c66aa-139">Finding Dimension Set ID</span><span class="sxs-lookup"><span data-stu-id="c66aa-139">Finding Dimension Set ID</span></span>  
 <span data-ttu-id="c66aa-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[prod_short](includes/prod_short.md)] traverses the tree in the same order as the dimension entries.</span><span class="sxs-lookup"><span data-stu-id="c66aa-140">At a conceptual level, **Parent ID**, **Dimension**, and **Dimension Value**, in the search tree, are combined and used as the primary key because [!INCLUDE[prod_short](includes/prod_short.md)] traverses the tree in the same order as the dimension entries.</span></span> <span data-ttu-id="c66aa-141">The GET function (record) is used to search for dimension set ID.</span><span class="sxs-lookup"><span data-stu-id="c66aa-141">The GET function (record) is used to search for dimension set ID.</span></span> <span data-ttu-id="c66aa-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span><span class="sxs-lookup"><span data-stu-id="c66aa-142">The following code example shows how to find the dimension set ID when there are three dimension values.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet."Parent ID",UserDim.DimCode,UserDim.DimValueCode);  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

<span data-ttu-id="c66aa-143">However, to preserve the ability of [!INCLUDE[prod_short](includes/prod_short.md)] to rename both a dimension and a dimension value, table 349, **Dimension Value**, is extended with an integer field, **Dimension Value ID**.</span><span class="sxs-lookup"><span data-stu-id="c66aa-143">However, to preserve the ability of [!INCLUDE[prod_short](includes/prod_short.md)] to rename both a dimension and a dimension value, table 349, **Dimension Value**, is extended with an integer field, **Dimension Value ID**.</span></span> <span data-ttu-id="c66aa-144">This table converts the field pair, **Dimension** and **Dimension Value**, to an integer value.</span><span class="sxs-lookup"><span data-stu-id="c66aa-144">This table converts the field pair, **Dimension** and **Dimension Value**, to an integer value.</span></span> <span data-ttu-id="c66aa-145">When you rename the dimension and dimension value, the integer value is not changed.</span><span class="sxs-lookup"><span data-stu-id="c66aa-145">When you rename the dimension and dimension value, the integer value is not changed.</span></span>  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet.ParentID,UserDim."Dimension Value ID");  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

## <a name="see-also"></a><span data-ttu-id="c66aa-146">See Also</span><span class="sxs-lookup"><span data-stu-id="c66aa-146">See Also</span></span>  
 <span data-ttu-id="c66aa-147">[GET Function (Record)](/dynamics-nav/GET-Function--Record-)  </span><span class="sxs-lookup"><span data-stu-id="c66aa-147">[GET Function (Record)](/dynamics-nav/GET-Function--Record-)  </span></span>  
 <span data-ttu-id="c66aa-148">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="c66aa-148">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="c66aa-149">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="c66aa-149">[Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 [<span data-ttu-id="c66aa-150">Design Details: Table Structure</span><span class="sxs-lookup"><span data-stu-id="c66aa-150">Design Details: Table Structure</span></span>](design-details-table-structure.md)   
 
