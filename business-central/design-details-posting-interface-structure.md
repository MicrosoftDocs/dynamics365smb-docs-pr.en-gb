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
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="b71bd-103">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="b71bd-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="b71bd-104">In the [!INCLUDE[prod_short](includes/prod_short.md)] posting interface structure, there are several global procedures that use the same structure:</span><span class="sxs-lookup"><span data-stu-id="b71bd-104">In the [!INCLUDE[prod_short](includes/prod_short.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="b71bd-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span><span class="sxs-lookup"><span data-stu-id="b71bd-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span></span> <span data-ttu-id="b71bd-106">Jnl Line.</span><span class="sxs-lookup"><span data-stu-id="b71bd-106">Jnl Line.</span></span>  
* <span data-ttu-id="b71bd-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="b71bd-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="b71bd-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="b71bd-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="b71bd-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="b71bd-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="b71bd-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="b71bd-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="b71bd-111">See Also</span><span class="sxs-lookup"><span data-stu-id="b71bd-111">See Also</span></span>  
[<span data-ttu-id="b71bd-112">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="b71bd-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)