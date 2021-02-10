---
title: Design Details - Posting Interface Structure | Microsoft Docs
description: This topic provides an overview of the global procedures in the posting interface structure.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: e306b0caeb58bfe7bd04f93ac64d8b593f70f695
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751262"
---
# <a name="design-details-posting-interface-structure"></a>Design Details: Posting Interface Structure
In the [!INCLUDE[prod_short](includes/prod_short.md)] posting interface structure, there are several global procedures that use the same structure:  
  
* RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.  
* CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.  
* VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.  
* UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries  
* UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries  
  
## <a name="see-also"></a>See Also  
[Design Details: Posting Engine Structure](design-details-posting-engine-structure.md)