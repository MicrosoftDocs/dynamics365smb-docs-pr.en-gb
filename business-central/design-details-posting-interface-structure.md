---
title: Design Details - Posting Interface Structure
description: This topic provides an overview of the global procedures and design details in the posting interface structure.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 06/15/2021
ms.author: edupont
ms.openlocfilehash: 80805675a3ecb1c847f0a55c2dc50008faa3b21f
ms.sourcegitcommit: e562b45fda20ff88230e086caa6587913eddae26
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/30/2021
ms.locfileid: "6318391"
---
# <a name="design-details-posting-interface-structure"></a>Design Details: Posting Interface Structure
In the [!INCLUDE[prod_short](includes/prod_short.md)] posting interface structure, there are several global procedures that use the same structure:  
  
* RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.  
* CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.  
* VendPostApplyVendLedgEntry – post supplier application, called from codeunit 227 VendEntry-Apply Posted Entries.  
* UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries  
* UnapplyVendLedgEntry – post unapply of supplier application, called from codeunit 227 VendEntry-Apply Posted Entries  
  
## <a name="see-also"></a>See Also  
[Design Details: Posting Engine Structure](design-details-posting-engine-structure.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]