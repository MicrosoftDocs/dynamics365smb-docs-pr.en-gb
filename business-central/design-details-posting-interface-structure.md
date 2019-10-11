---
title: Design Details - Posting Interface Structure | Microsoft Docs
description: This topic provides an overview of the global procedures in the posting interface structure.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: f484c6474c840b4c2d802494407f8d819256596c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2306947"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="820be-103">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="820be-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="820be-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span><span class="sxs-lookup"><span data-stu-id="820be-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="820be-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span><span class="sxs-lookup"><span data-stu-id="820be-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span></span> <span data-ttu-id="820be-106">Jnl Line.</span><span class="sxs-lookup"><span data-stu-id="820be-106">Jnl Line.</span></span>  
* <span data-ttu-id="820be-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="820be-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="820be-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="820be-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="820be-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="820be-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="820be-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="820be-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="820be-111">See Also</span><span class="sxs-lookup"><span data-stu-id="820be-111">See Also</span></span>  
[<span data-ttu-id="820be-112">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="820be-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)