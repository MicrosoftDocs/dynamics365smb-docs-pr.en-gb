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
ms.openlocfilehash: 231148c304c5f2dabba5c69c442dfd0cfdc6397d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921949"
---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="d6a40-103">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="d6a40-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="d6a40-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span><span class="sxs-lookup"><span data-stu-id="d6a40-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="d6a40-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span><span class="sxs-lookup"><span data-stu-id="d6a40-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen.</span></span> <span data-ttu-id="d6a40-106">Jnl Line.</span><span class="sxs-lookup"><span data-stu-id="d6a40-106">Jnl Line.</span></span>  
* <span data-ttu-id="d6a40-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="d6a40-107">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="d6a40-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span><span class="sxs-lookup"><span data-stu-id="d6a40-108">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="d6a40-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="d6a40-109">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="d6a40-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span><span class="sxs-lookup"><span data-stu-id="d6a40-110">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="d6a40-111">See Also</span><span class="sxs-lookup"><span data-stu-id="d6a40-111">See Also</span></span>  
[<span data-ttu-id="d6a40-112">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="d6a40-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)