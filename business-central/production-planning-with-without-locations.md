---
title: Planning With or Without Locations | Microsoft Docs
description: Planning with or without location codes on demand lines is important to understand.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: dd86568c87a9cbb66214ae88b75fcdae8e85b59d
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383182"
---
# <a name="planning-with-or-without-locations"></a>Planning With or Without Locations
Concerning planning with or without location codes on demand lines, the planning system operates in a straight forward way when:  

-   demand lines always carry location codes and the system fully uses stockkeeping units, including the relevant location setup.  
-   demand lines never carry location codes and the system does not use SKUs or any location setup (see last scenario below).  

However, if demand lines sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.  

## <a name="demand-at-location"></a>Demand at Location  
When the planning system detects demand at a location (a line with a location code), it will behave in different ways depending on 3 critical setup values.  

During a planning run, the system checks for the 3 setup values in sequence and plans accordingly:  

1.  Is there a check mark in the **Location Mandatory** field?  

    If yes, then:  

2.  Does SKU exist for the item?  

    If yes, then:  

    The item is planned according to planning parameters on the SKU card.  

    If no, then:  

3.  Does the **Components at Location** field contain the demanded location code?  

    If yes, then:  

    The item is planned according to planning parameters on the item card.  

    If no, then:  

    The item is planned according to: Reordering Policy =  *Lot-for-Lot*, Include Inventory =  *Yes*, all other planning parameters = Empty. (Items using reordering policy  *Order* remain using  *Order* as well as the other settings.)  

> [!NOTE]  
>  This minimal alternative only covers the exact demand. Any planning parameters defined are ignored.  

See variations in the scenarios below.  

## <a name="demand-at-blank-location"></a>Demand at "Blank Location"  
Even if the **Location Mandatory** check box is selected, the system will allow demand lines to be created without a location code – also referred to as *BLANK* location. This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line. If the **Location Mandatory** field is not selected but any of the location setup values exist, then that is also considered a deviation and the planning system will react by outputting the "minimal alternative":   
The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains *Order)*, Include Inventory =  *Yes*, all other planning parameters = Empty.  

See variations in the setup scenarios below.  

### <a name="setup-1"></a>Setup 1:  

-   Location Mandatory = *Yes*  
-   SKU is set up for  *RED*  
-   Component at Location =  *BLUE*  

#### <a name="case-11-demand-is-at--red-location"></a>Case 1.1: Demand is at  *RED* location  

The item is planned according to planning parameters on the SKU card (including possible transfer).  

#### <a name="case-12-demand-is-at--blue-location"></a>Case 1.2: Demand is at  *BLUE* location  

The item is planned according to planning parameters on the item card.  

#### <a name="case-13-demand-is-at--green-location"></a>Case 1.3: Demand is at  *GREEN* location  

The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.  

#### <a name="case-14-demand-is-at--blank-location"></a>Case 1.4: Demand is at  *BLANK* location  

The item is not planned because no location is defined on the demand line.  

### <a name="setup-2"></a>Setup 2:  

-   Location Mandatory = *Yes*  
-   No SKU exists  
-   Component at Location =  *BLUE*  

#### <a name="case-21-demand-is-at--red-location"></a>Case 2.1: Demand is at  *RED* location  

The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.  

#### <a name="case-22-demand-is-at--blue-location"></a>Case 2.2: Demand is at  *BLUE* location  

The item is planned according to planning parameters on the item card.  

### <a name="setup-3"></a>Setup 3:  

-   Location Mandatory = *No*  
-   No SKU exists  
-   Component at Location =  *BLUE*  

#### <a name="case-31-demand-is-at--red-location"></a>Case 3.1: Demand is at  *RED* location  

The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.  

#### <a name="case-32-demand-is-at--blue-location"></a>Case 3.2: Demand is at  *BLUE* location  

The item is planned according to planning parameters on the item card.  

#### <a name="case-33-demand-is-at--blank-location"></a>Case 3.3: Demand is at  *BLANK* location  

The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.  

### <a name="setup-4"></a>Setup 4:  

-   Location Mandatory = *No*  
-   No SKU exists  
-   Component at Location =  *BLANK*  

#### <a name="case-41-demand-is-at--blue-location"></a>Case 4.1: Demand is at  *BLUE* location  

The item is planned according to: Reordering Policy =  *Lot-for-Lot* ( *Order* remains  *Order*), Include Inventory =  *Yes*, all other planning parameters = Empty.  

#### <a name="case-42-demand-is-at--blank-location"></a>Case 4.2: Demand is at  *BLANK* location  

The item is planned according to planning parameters on the item card.  

As you can see from the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations. Similarly, the only way to get stable planning results for demand at locations is to use stockkeeping units.  

Therefore, if you often plan for demand at locations, it is strongly advised to use the Stockkeeping Units feature.  

## <a name="see-also"></a>See Also
[Planning](production-planning.md)    
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Manufacturing](production-manage-manufacturing.md)    
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Design Details: Supply Planning](design-details-supply-planning.md)   
[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]