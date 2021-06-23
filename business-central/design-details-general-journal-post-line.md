---
title: Design Details - General Journal Post Line | Microsoft Docs
description: This topic provides insight into the concepts and principles that are used to redesign the general journal posting line feature in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 8492c83437be4cd850bafdaaa5dc70d00a075674
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215235"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="b1ebc-103">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="b1ebc-103">Design Details: General Journal Post Line</span></span>

<span data-ttu-id="b1ebc-104">This documentation provides detailed technical insight into the concepts and principles that were used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b1ebc-104">This documentation provides detailed technical insight into the concepts and principles that were used to redesign the general journal posting line feature in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b1ebc-105">The redesign made codeunit 12 simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="b1ebc-105">The redesign made codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="b1ebc-106">The documentation starts by describing conceptual overviews of the redesign.</span><span class="sxs-lookup"><span data-stu-id="b1ebc-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="b1ebc-107">Then it explains the technical architecture to show the changes that result from the redesign.</span><span class="sxs-lookup"><span data-stu-id="b1ebc-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="b1ebc-108">The information in this section applies to the redesign in an earlier version of the product, Microsoft Dynamics NAV 2013 R2.</span><span class="sxs-lookup"><span data-stu-id="b1ebc-108">The information in this section applies to the redesign in an earlier version of the product, Microsoft Dynamics NAV 2013 R2.</span></span>

## <a name="in-this-section"></a><span data-ttu-id="b1ebc-109">In This Section</span><span class="sxs-lookup"><span data-stu-id="b1ebc-109">In This Section</span></span>

[<span data-ttu-id="b1ebc-110">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="b1ebc-110">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="b1ebc-111">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="b1ebc-111">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="b1ebc-112">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="b1ebc-112">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  

## <a name="see-also"></a><span data-ttu-id="b1ebc-113">See Also</span><span class="sxs-lookup"><span data-stu-id="b1ebc-113">See Also</span></span>

<span data-ttu-id="b1ebc-114">[Working with General Journals](ui-work-general-journals.md)
[Design Details: General Journal Post Line (Dynamics NAV)](/dynamics-nav-app/design-details-general-journal-post-line)</span><span class="sxs-lookup"><span data-stu-id="b1ebc-114">[Working with General Journals](ui-work-general-journals.md)
[Design Details: General Journal Post Line (Dynamics NAV)](/dynamics-nav-app/design-details-general-journal-post-line)</span></span>  

[!INCLUDE[footer-include](includes/footer-banner.md)]