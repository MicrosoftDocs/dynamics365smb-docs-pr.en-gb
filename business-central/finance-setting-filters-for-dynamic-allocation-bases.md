---
title: Setting Filters for Dynamic Allocation Keys | Microsoft Docs
description: The dynamic allocation method is based on changeable values. For example, the number of employees in a cost centre or the items sold of a cost object in a specific time period. There are nine pre-defined allocation bases and twelve dynamic date ranges. You set different filters based on the allocation base.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 5ca8e7008c2bfe4a9abeb9d9b7b467a38e2c1971
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="setting-filters-for-dynamic-allocation-bases"></a>Setting Filters for Dynamic Allocation Bases
The dynamic allocation method is based on changeable values. For example, the number of employees in a cost centre or the items sold of a cost object in a specific time period. There are nine pre-defined allocation bases and twelve dynamic date ranges. You set different filters based on the allocation base.  

## <a name="setting-filters-for-dynamic-allocation-bases"></a>Setting Filters for Dynamic Allocation Bases  
 The following table shows which filters are possible for different allocation bases and which values are valid in the **No. Filter** and **Group Filter** fields. Press F1 in the **Date Filter Code** field to read detailed descriptions.  

|**Base**|**No. Filter**|**Date Filter Code**|**Cost Centre Filter**|**Cost Object Filter**|**Group Filter**|  
|--------------|----------------------------------------|----------------------------------------------|------------------------------------------------|------------------------------------------------|------------------------------------------|  
|G/L Entries|G/L Account|Yes|Yes|Yes|N/A|  
|G/L Budget Entries|G/L Account|Yes|Yes|Yes|G/L Budget Name|  
|Cost Type Entries|Cost Type|Yes|Yes|Yes|N/A|  
|Cost Budget Entries|Cost Type|Yes|Yes|Yes|Budget Name|  
|No of Employees|N/A|Yes|Yes|Yes|N/A|  
|Items Sold (Qty)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Purchased (Qty)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Sold (Amount)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  
|Items Purchased (Amount)|Item No.|Yes|Yes|Yes|Inventory Posting Group|  

## <a name="see-also"></a>See Also  
 [Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
 [Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md)   
 [Defining and Allocating Costs](finance-define-and-allocate-costs.md)

