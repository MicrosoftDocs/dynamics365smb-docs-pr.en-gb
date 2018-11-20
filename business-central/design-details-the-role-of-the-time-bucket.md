---
title: Design Details - The Role of the Time Bucket | Microsoft Docs
description: The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: c258c13a08e9556caddf55a0d14962ad85cd8ca7
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="design-details-the-role-of-the-time-bucket"></a>Design Details: The Role of the Time Bucket
The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.  

 For reordering policies that use a reorder point, you can define a time bucket. This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed. If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket. The time buckets begin on the planning starting date.  

 The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction. The user needs to define the frequency (the time bucket). For example, the user gathers all item needs from one vendor to place a weekly order.  

 ![Example of time bucket in planning](media/nav_app_supply_planning_2_reorder_cycle.png "Example of time bucket in planning")  

 The time bucket is generally used to avoid a cascade effect. For example, a balanced row of demand and supply where an early demand is cancelled, or a new one is created. The result would be that every supply order (except the last one) is rescheduled.  

## <a name="see-also"></a>See Also  
 [Design Details: Reordering Policies](design-details-reordering-policies.md)   
 [Design Details: Planning Parameters](design-details-planning-parameters.md)   
 [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md)   
 [Design Details: Supply Planning](design-details-supply-planning.md)

