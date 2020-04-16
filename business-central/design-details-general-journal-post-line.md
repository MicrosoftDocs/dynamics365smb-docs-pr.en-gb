---
title: Design Details - General Journal Post Line | Microsoft Docs
description: This topic provides insight into the concepts and principles that are used to redesign the general journal posting line feature in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general journal, posting, codeunit 12
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 1a8654b53dec476b175101a4d9c08f15ab3d6d6f
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3185379"
---
# <a name="design-details-general-journal-post-line"></a><span data-ttu-id="4edf3-103">Design Details: General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="4edf3-103">Design Details: General Journal Post Line</span></span>
<span data-ttu-id="4edf3-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4edf3-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the general journal posting line feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="4edf3-105">The redesign makes codeunit 12 simpler and more maintainable.</span><span class="sxs-lookup"><span data-stu-id="4edf3-105">The redesign makes codeunit 12 simpler and more maintainable.</span></span> <span data-ttu-id="4edf3-106">The documentation starts by describing conceptual overviews of the redesign.</span><span class="sxs-lookup"><span data-stu-id="4edf3-106">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="4edf3-107">Then it explains the technical architecture to show the changes that result from the redesign.</span><span class="sxs-lookup"><span data-stu-id="4edf3-107">Then it explains the technical architecture to show the changes that result from the redesign.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="4edf3-108">In This Section</span><span class="sxs-lookup"><span data-stu-id="4edf3-108">In This Section</span></span>  
[<span data-ttu-id="4edf3-109">General Journal Post Line Overview</span><span class="sxs-lookup"><span data-stu-id="4edf3-109">General Journal Post Line Overview</span></span>](design-details-general-journal-post-line-overview.md)  
[<span data-ttu-id="4edf3-110">Design Details: Posting Interface Structure</span><span class="sxs-lookup"><span data-stu-id="4edf3-110">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="4edf3-111">Design Details: Posting Engine Structure</span><span class="sxs-lookup"><span data-stu-id="4edf3-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="4edf3-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span><span class="sxs-lookup"><span data-stu-id="4edf3-112">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>](design-details-codeunit-12-changes-mapping-global-variables-for-general-journal-post-line.md)  
[<span data-ttu-id="4edf3-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span><span class="sxs-lookup"><span data-stu-id="4edf3-113">Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)  

## <a name="see-also"></a><span data-ttu-id="4edf3-114">See Also</span><span class="sxs-lookup"><span data-stu-id="4edf3-114">See Also</span></span>  
[<span data-ttu-id="4edf3-115">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="4edf3-115">Working with General Journals</span></span>](ui-work-general-journals.md)
