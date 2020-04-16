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
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c50f045cf1a379d4fb908e0c17d7b9775fd1a9ee
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3184875"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="b310e-103">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="b310e-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="b310e-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span><span class="sxs-lookup"><span data-stu-id="b310e-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="b310e-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span><span class="sxs-lookup"><span data-stu-id="b310e-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span></span> <span data-ttu-id="b310e-106">Jnl Line.</span><span class="sxs-lookup"><span data-stu-id="b310e-106">Jnl Line.</span></span>  
* <span data-ttu-id="b310e-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="b310e-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="b310e-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="b310e-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="b310e-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="b310e-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="b310e-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="b310e-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="b310e-111">See Also</span><span class="sxs-lookup"><span data-stu-id="b310e-111">See Also</span></span>  
[<span data-ttu-id="b310e-112">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="b310e-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)