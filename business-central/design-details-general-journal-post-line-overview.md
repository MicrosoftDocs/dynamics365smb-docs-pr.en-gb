---
title: General Journal Post Line Overview | Microsoft Docs
description: This topic introduces changes to Codeunit 12, **Gen. Jnl.-Post Line**, which is the major application object for general ledger posting and is the only place to insert general ledger, VAT, and customer and supplier ledger entries.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general ledger, post
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 1f6060eb7672b332fb570eb13fe027a3b58e6594
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215260"
---
# <a name="general-journal-post-line-overview"></a><span data-ttu-id="c62e4-103">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="c62e4-103">General Journal Post Line Overview</span></span>

<span data-ttu-id="c62e4-104">Codeunit 12, **Gen. Jnl.-Post Line**, is the major application object for general ledger posting and is the only place to insert general ledger, VAT, and customer and supplier ledger entries.</span><span class="sxs-lookup"><span data-stu-id="c62e4-104">Codeunit 12, **Gen. Jnl.-Post Line**, is the major application object for general ledger posting and is the only place to insert general ledger, VAT, and customer and vendor ledger entries.</span></span> <span data-ttu-id="c62e4-105">This codeunit is also used for all Apply, Unapply and Reverse operations.</span><span class="sxs-lookup"><span data-stu-id="c62e4-105">This codeunit is also used for all Apply, Unapply and Reverse operations.</span></span>  
  
<span data-ttu-id="c62e4-106">In Microsoft Dynamics NAV 2013 R2, the codeunit was redesigned because it had become very large, with approximately 7,600 code lines.</span><span class="sxs-lookup"><span data-stu-id="c62e4-106">In Microsoft Dynamics NAV 2013 R2, the codeunit was redesigned because it had become very large, with approximately 7,600 code lines.</span></span> <span data-ttu-id="c62e4-107">The architecture was changed and the codeunit has been made simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="c62e4-107">The architecture was changed and the codeunit has been made simpler and more maintainable.</span></span> <span data-ttu-id="c62e4-108">This documentation describes the changes and provides information that you will need for upgrade.</span><span class="sxs-lookup"><span data-stu-id="c62e4-108">This documentation describes the changes and provides information that you will need for upgrade.</span></span>  
  
## <a name="old-architecture"></a><span data-ttu-id="c62e4-109">Old Architecture</span><span class="sxs-lookup"><span data-stu-id="c62e4-109">Old Architecture</span></span>  
<span data-ttu-id="c62e4-110">The old architecture had the following features:</span><span class="sxs-lookup"><span data-stu-id="c62e4-110">The old architecture had the following features:</span></span>  
  
* <span data-ttu-id="c62e4-111">There was extensive use of global variables, which increased the possibility of hidden errors due to use of variables with the wrong scope.</span><span class="sxs-lookup"><span data-stu-id="c62e4-111">There was extensive use of global variables, which increased the possibility of hidden errors due to use of variables with the wrong scope.</span></span>  
* <span data-ttu-id="c62e4-112">There were many long procedures (with more than 100 code lines) that also had high cyclomatic complexity (that is, a lot of CASE, REPEAT, IF nested statements), which made the code very difficult to read and maintain.</span><span class="sxs-lookup"><span data-stu-id="c62e4-112">There were many long procedures (with more than 100 code lines) that also had high cyclomatic complexity (that is, a lot of CASE, REPEAT, IF nested statements), which made the code very difficult to read and maintain.</span></span>  
* <span data-ttu-id="c62e4-113">Several procedures that were only used locally and were only meant to be used locally were not marked as local.</span><span class="sxs-lookup"><span data-stu-id="c62e4-113">Several procedures that were only used locally and were only meant to be used locally were not marked as local.</span></span>  
* <span data-ttu-id="c62e4-114">Most procedures had no parameters and used global variables.</span><span class="sxs-lookup"><span data-stu-id="c62e4-114">Most procedures had no parameters and used global variables.</span></span> <span data-ttu-id="c62e4-115">Some used parameters and overrode global variables with locals.</span><span class="sxs-lookup"><span data-stu-id="c62e4-115">Some used parameters and overrode global variables with locals.</span></span>  
* <span data-ttu-id="c62e4-116">Code patterns for searching the general ledger accounts and creating general ledger and VAT entries was not standardised and varied from place to place.</span><span class="sxs-lookup"><span data-stu-id="c62e4-116">Code patterns for searching the general ledger accounts and creating general ledger and VAT entries was not standardized and varied from place to place.</span></span> <span data-ttu-id="c62e4-117">In addition, there was a lot of code duplication and broken symmetry between customer and supplier code.</span><span class="sxs-lookup"><span data-stu-id="c62e4-117">In addition, there was a lot of code duplication and broken symmetry between customer and vendor code.</span></span>  
* <span data-ttu-id="c62e4-118">A large part of the code in codeunit 12, approximately 30 percent, related to payment discount and tolerance calculations, although these features are not needed in many countries or regions.</span><span class="sxs-lookup"><span data-stu-id="c62e4-118">A large part of the code in codeunit 12, approximately 30 percent, related to payment discount and tolerance calculations, although these features are not needed in many countries or regions.</span></span>  
* <span data-ttu-id="c62e4-119">Posting, Apply, Unapply, Reverse, Payment Discount and Tolerance, and Exchange Rate Adjustment were married together in codeunit 12 using a long list of global variables.</span><span class="sxs-lookup"><span data-stu-id="c62e4-119">Posting, Apply, Unapply, Reverse, Payment Discount and Tolerance, and Exchange Rate Adjustment were married together in codeunit 12 using a long list of global variables.</span></span>  
  
### <a name="new-architecture"></a><span data-ttu-id="c62e4-120">New Architecture</span><span class="sxs-lookup"><span data-stu-id="c62e4-120">New Architecture</span></span>  
<span data-ttu-id="c62e4-121">In [!INCLUDE[prod_short](includes/prod_short.md)], codeunit 12 has had the following improvements:</span><span class="sxs-lookup"><span data-stu-id="c62e4-121">In [!INCLUDE[prod_short](includes/prod_short.md)], codeunit 12 has had the following improvements:</span></span>  
  
* <span data-ttu-id="c62e4-122">Codeunit 12 has been refactored into smaller procedures (all less than 100 code lines).</span><span class="sxs-lookup"><span data-stu-id="c62e4-122">Codeunit 12 has been refactored into smaller procedures (all less than 100 code lines).</span></span>  
* <span data-ttu-id="c62e4-123">Standardised patterns for the search of general ledger accounts have been implemented by using helper functions from Posting Group tables.</span><span class="sxs-lookup"><span data-stu-id="c62e4-123">Standardized patterns for the search of general ledger accounts have been implemented by using helper functions from Posting Group tables.</span></span>  
* <span data-ttu-id="c62e4-124">A Posting Engine Framework has been implemented to manage the start and finish of transactions and to isolate the creation to general ledger and VAT entries, the collection of VAT adjustment, and the calculation of additional currency amounts.</span><span class="sxs-lookup"><span data-stu-id="c62e4-124">A Posting Engine Framework has been implemented to manage the start and finish of transactions and to isolate the creation to general ledger and VAT entries, the collection of VAT adjustment, and the calculation of additional currency amounts.</span></span>  
* <span data-ttu-id="c62e4-125">Code duplication has been eliminated.</span><span class="sxs-lookup"><span data-stu-id="c62e4-125">Code duplication has been eliminated.</span></span>  
* <span data-ttu-id="c62e4-126">Many helper functions have been transferred to corresponding customer and supplier ledger entry tables.</span><span class="sxs-lookup"><span data-stu-id="c62e4-126">Many helper functions have been transferred to corresponding customer and vendor ledger entry tables.</span></span>  
* <span data-ttu-id="c62e4-127">The use of global variables has been minimised, so that each procedure uses parameters and encapsulates its own application logic.</span><span class="sxs-lookup"><span data-stu-id="c62e4-127">The use of global variables has been minimized, so that each procedure uses parameters and encapsulates its own application logic.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="c62e4-128">See Also</span><span class="sxs-lookup"><span data-stu-id="c62e4-128">See Also</span></span>

[<span data-ttu-id="c62e4-129">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="c62e4-129">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="c62e4-130">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="c62e4-130">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="c62e4-131">Design Details: General Journal Post Line (Dynamics NAV)</span><span class="sxs-lookup"><span data-stu-id="c62e4-131">Design Details: General Journal Post Line (Dynamics NAV)</span></span>](/dynamics-nav-app/design-details-general-journal-post-line)  


[!INCLUDE[footer-include](includes/footer-banner.md)]