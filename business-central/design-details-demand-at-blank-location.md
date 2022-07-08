---
title: Design Details - Demand and Supply | Microsoft Docs
description: This topic introduces the concept of demand, which is the common term used for any kind of gross demand, such as a sales order and component need from a production order.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 3b5f390343f74bc559cce48b2037edd125f829ca
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2022
ms.locfileid: "8143641"
---
# <a name="design-details-demand-at-blank-location"></a>Design Details: Demand at Blank Location
When a user creates a demand event, such as a sales order line, the program allows the user to sometimes specify a location code and other times not, that is, use blank location.

For demand with or without location codes, the planning system operates in a straight forward way when:

- Demand lines always carry location codes and the system fully uses SKUs, including the relevant location setup.
- Demand lines never carry location codes, and the system does not use SKUs or any location setup (see the last scenario in the following section).

However, if demand events sometimes have location codes and other times do not, the planning system will follow certain rules depending on setup.

## <a name="demand-at-location"></a>Demand at Location
When the planning system detects demand at a location, it will behave in different ways depending on three critical setup values. During a planning run, the system checks for three setup values in sequence and plans accordingly.

1. Is there a check mark in the **Location Mandatory** field?

    If yes, then:

2. Does SKU exist for the item?

    If yes, then:

    The item is planned according to planning parameters on the SKU card.

    If no, then:

3. Does the Components at Location field contain the demanded location code?

  If yes, then:

  The item is planned according to planning parameters on the item card.

  If no, then:

  The item is planned according to: Reordering Policy = Lot-for-Lot, Include Inventory = Yes, all other planning parameters = Empty, items using Reordering Policy = Order will remain using Order along with the other settings.

> [!NOTE]
> The exceptional planning setup that is output as the last reaction in step 3 above is referred to in the following as the “minimal alternative”. This planning setup only covers the exact demand, and all other planning parameters are ignored.

For information about variations of this planning logic, see the Scenarios section below.

## <a name="demand-at-blank-location"></a>Demand at Blank Location
Even if the **Location Mandatory** field is selected, the program will allow demand lines to be created without a location code, also referred to as blank location. This is a deviation for the system because it has various setup values tuned to dealing with locations (see above) and as a result, the planning engine will not create a planning line for such a demand line.

If the **Location Mandatory** field is not selected but any of the location setup values exist, it is also considered a deviation, and the planning system will react by using the “minimal alternative”: The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

## <a name="scenarios"></a>Scenarios
The following scenarios describe variations of demand at blank location and how the planning system resolves to the “minimal alternative.”

### <a name="setup-1"></a>Setup 1:
Location Mandatory = Yes

SKU is set up for RED

Components at Location = BLUE

#### <a name="case-11-demand-is-at-red-location"></a>Case 1.1: Demand is at RED location
The item is planned according to planning parameters on the SKU card.

#### <a name="case-12-demand-is-at-blue-location"></a>Case 1.2: Demand is at BLUE location
The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

#### <a name="case-13-demand-is-at-green-location"></a>Case 1.3: Demand is at GREEN location
The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

#### <a name="case-14-demand-is-at-blank-location"></a>Case 1.4: Demand is at BLANK location
The item is not planned because no location is defined on the demand line.

### <a name="setup-2"></a>Setup 2:
Location Mandatory = Yes

No SKU exists

Components at Location = BLUE

#### <a name="case-21-demand-is-at-red-location"></a>Case 2.1: Demand is at RED location
The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

#### <a name="case-22-demand-is-at-blue-location"></a>Case 2.2: Demand is at BLUE location
The item is planned according to planning parameters on the item card.

### <a name="setup-3"></a>Setup 3:
Location Mandatory = No

No SKU exists

Components at Location = BLUE

#### <a name="case-31-demand-is-at-red-location"></a>Case 3.1: Demand is at RED location
The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

#### <a name="case-32-demand-is-at-blue-location"></a>Case 3.2: Demand is at BLUE location
The item is planned according to planning parameters on the item card.

#### <a name="case-33-demand-is-at-blank-location"></a>Case 3.3: Demand is at BLANK location
The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

### <a name="setup-4"></a>Setup 4:
Location Mandatory = No

No SKU exists

Components at Location = BLANK

#### <a name="case-41-demand-is-at-blue-location"></a>Case 4.1: Demand is at BLUE location
The item is planned according to: Reordering Policy = Lot-for-Lot (Order remains Order), Include Inventory = Yes, all other planning parameters = Empty.

#### <a name="case-42-demand-is-at-blank-location"></a>Case 4.2: Demand is at BLANK location
The item is planned according to planning parameters on the item card.

As illustrated in the last scenario, the only way to get a correct result for a demand line without a location code is to disable all setup values relating to locations. Similarly, the only way to get stable planning results for demand at locations is to use SKUs. Therefore, if companies often plan for demand at locations, they are strongly advised to use the Stockkeeping Units granule.

## <a name="see-also"></a>See Also  
[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md)   
[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]