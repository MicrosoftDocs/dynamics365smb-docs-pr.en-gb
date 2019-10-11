---
title: Design Details - The Role of the Reorder Point | Microsoft Docs
description: This topic highlights the importance of setting a reorder point, so that you when to order more inventory.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: 760bc475be2606e9bc4d72f09ae76e794418d904
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2306755"
---
# <a name="design-details-the-role-of-the-reorder-point"></a>Design Details: The Role of the Reorder Point
In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.  

A reorder point represents demand during lead time. When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity. Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.  

Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.  

The reorder point reflects a certain inventory level. However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.  

## <a name="see-also"></a>See Also  
[Design Details: Reordering Policies](design-details-reordering-policies.md)   
[Design Details: Planning Parameters](design-details-planning-parameters.md)   
[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md)   
[Design Details: Supply Planning](design-details-supply-planning.md)
