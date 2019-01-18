---
title: Best practices for global planning setup | Microsoft Docs
description: The Planning FastTab in the Manufacturing Setup page contains several fields that define global rules for supply planning.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: d1f6333c689d6af06d68e45104020a523be7f865
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="setup-best-practices-global-planning-setup"></a>Setup Best Practices: Global Planning Setup
The **Planning** FastTab on the **Manufacturing Setup** page contains several fields that define global rules for supply planning.  

 The following table provides best practices on how to set up selected global planning parameter fields. For more information about a field, choose the link in the **Setup field** column.  

|Setup field|Best practice|Comment|  
|-----------------|-------------------|-------------|  
|Use Forecast on Locations|Select if you have forecasts for specific locations.||  
|Components at Location|If items are not defined as SKUs, select the location code of your main warehouse.|This also applies if you only use the requisition worksheet.|  
|Blank Overflow Level|Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.|Use only if you want to allow all or some of your items to overflow the reorder point.|  
|Default Dampener Period|Set between 1D and 5D.<br /><br /> If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.|When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.|  
|Default Dampener Quantity|Set between 5 and 20 percent of the item’s lot size.||  

## <a name="see-also"></a>See Also  
 [Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md)   
 [Design Details: Supply Planning](design-details-supply-planning.md)   
 [Set Up Complex Application Areas Using Best Practices](set-up-complex-application-areas-using-best-practices.md)  
 [Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

