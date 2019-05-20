---
title: Assistive features
description: Keyboard shortcuts and other assistive features.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: edupont
ms.openlocfilehash: 99b1b5d5f725a598cc8be77f390d1fcf1c1a4033
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1250372"
---
# <a name="accessibility-and-keyboard-shortcuts-in-included365finincludesd365finmdmd"></a><span data-ttu-id="ff66c-103">Accessibility and Keyboard Shortcuts in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="ff66c-103">Accessibility and Keyboard Shortcuts in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
<span data-ttu-id="ff66c-104">This topic provides information about the features that make [!INCLUDE[d365fin](includes/d365fin_md.md)] readily available to people with disabilities.</span><span class="sxs-lookup"><span data-stu-id="ff66c-104">This topic provides information about the features that make [!INCLUDE[d365fin](includes/d365fin_md.md)] readily available to people with disabilities.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ff66c-105">supports the following accessibility features:</span><span class="sxs-lookup"><span data-stu-id="ff66c-105">supports the following accessibility features:</span></span>  

-   <span data-ttu-id="ff66c-106">Keyboard shortcuts</span><span class="sxs-lookup"><span data-stu-id="ff66c-106">Keyboard shortcuts</span></span>

    <span data-ttu-id="ff66c-107">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md)</span><span class="sxs-lookup"><span data-stu-id="ff66c-107">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md)</span></span>

-   <span data-ttu-id="ff66c-108">Navigation</span><span class="sxs-lookup"><span data-stu-id="ff66c-108">Navigation</span></span>  

-   <span data-ttu-id="ff66c-109">Headings</span><span class="sxs-lookup"><span data-stu-id="ff66c-109">Headings</span></span>  

-   <span data-ttu-id="ff66c-110">Alternative text for images and links</span><span class="sxs-lookup"><span data-stu-id="ff66c-110">Alternative text for images and links</span></span>  

-   <span data-ttu-id="ff66c-111">Support for common assistive technologies</span><span class="sxs-lookup"><span data-stu-id="ff66c-111">Support for common assistive technologies</span></span>  

<!-- moved to separate article
##  <a name="Keyboard"></a> Keyboard Shortcuts in the browser
 [!INCLUDE[d365fin](includes/d365fin_md.md)] supports the keyboard shortcuts that are supported by most web browsers. The keyboard shortcuts described here refer to the U.S. keyboard layout. The layout of the keys on other keyboards may not correspond exactly to the keys on a U.S. keyboard.  

|To do this|Press|  
|----------------|-----------|  
|To move focus to the next or previous control or element on a page, such as buttons, fields, or items in a list.|Tab, Shift+Tab|  
|To enable or access the element or control that is in focus.|Enter|  
|To scroll items up and down in a list.|Up Arrow, Down Arrow|  
|To scroll columns of an item left and right in a list.|Left Arrow, Right Arrow|  
|To open a drop-down list or look up a value for a field.|Alt+Down Arrow|  
|To move focus to the next element outside the list.|Ctrl + Enter|  
|To see the transactions that resulted in a calculated value in a field.|Alt+Right Arrow|  

-->

##  <a name="Navigation"></a> <span data-ttu-id="ff66c-112">Navigation</span><span class="sxs-lookup"><span data-stu-id="ff66c-112">Navigation</span></span>  
 <span data-ttu-id="ff66c-113">You can navigate between the tabs and actions in the ribbon, elements in the navigation bar, and other controls on [!INCLUDE[d365fin](includes/d365fin_md.md)] pages and reports using the keyboard.</span><span class="sxs-lookup"><span data-stu-id="ff66c-113">You can navigate between the tabs and actions in the ribbon, elements in the navigation bar, and other controls on [!INCLUDE[d365fin](includes/d365fin_md.md)] pages and reports using the keyboard.</span></span> <span data-ttu-id="ff66c-114">To move the focus from one tab, action, or control to another, press the Tab key to move forward.</span><span class="sxs-lookup"><span data-stu-id="ff66c-114">To move the focus from one tab, action, or control to another, press the Tab key to move forward.</span></span> <span data-ttu-id="ff66c-115">Press Shift+Tab to move backward.</span><span class="sxs-lookup"><span data-stu-id="ff66c-115">Press Shift+Tab to move backward.</span></span>  

 <span data-ttu-id="ff66c-116">By using the tab order, you can also switch between the main browser page and dialogue boxes that request confirmation, for example, or the login page.</span><span class="sxs-lookup"><span data-stu-id="ff66c-116">By using the tab order, you can also switch between the main browser page and dialog boxes that request confirmation, for example, or the login page.</span></span>  

##  <a name="Headings"></a> <span data-ttu-id="ff66c-117">Headings</span><span class="sxs-lookup"><span data-stu-id="ff66c-117">Headings</span></span>  
 <span data-ttu-id="ff66c-118">The HTML source for [!INCLUDE[d365fin](includes/d365fin_md.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span><span class="sxs-lookup"><span data-stu-id="ff66c-118">The HTML source for [!INCLUDE[d365fin](includes/d365fin_md.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span></span> <span data-ttu-id="ff66c-119">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span><span class="sxs-lookup"><span data-stu-id="ff66c-119">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span></span> <span data-ttu-id="ff66c-120">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span><span class="sxs-lookup"><span data-stu-id="ff66c-120">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span></span>  

##  <a name="Images"></a> <span data-ttu-id="ff66c-121">Image and Links</span><span class="sxs-lookup"><span data-stu-id="ff66c-121">Image and Links</span></span>  
 <span data-ttu-id="ff66c-122">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span><span class="sxs-lookup"><span data-stu-id="ff66c-122">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span></span> <span data-ttu-id="ff66c-123">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span><span class="sxs-lookup"><span data-stu-id="ff66c-123">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span></span>  

##  <a name="AssistiveTech"></a> <span data-ttu-id="ff66c-124">Assistive Technologies</span><span class="sxs-lookup"><span data-stu-id="ff66c-124">Assistive Technologies</span></span>  
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ff66c-125">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span><span class="sxs-lookup"><span data-stu-id="ff66c-125">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span></span> <span data-ttu-id="ff66c-126">Some assistive technologies may not work well with certain elements in [!INCLUDE[d365fin](includes/d365fin_md.md)] pages.</span><span class="sxs-lookup"><span data-stu-id="ff66c-126">Some assistive technologies may not work well with certain elements in [!INCLUDE[d365fin](includes/d365fin_md.md)] pages.</span></span>  

## <a name="for-more-accessibility-information"></a><span data-ttu-id="ff66c-127">For more accessibility information</span><span class="sxs-lookup"><span data-stu-id="ff66c-127">For more accessibility information</span></span>  
<span data-ttu-id="ff66c-128">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span><span class="sxs-lookup"><span data-stu-id="ff66c-128">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span></span>

## <a name="see-also"></a><span data-ttu-id="ff66c-129">See Also</span><span class="sxs-lookup"><span data-stu-id="ff66c-129">See Also</span></span>
[<span data-ttu-id="ff66c-130">Getting Started</span><span class="sxs-lookup"><span data-stu-id="ff66c-130">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="ff66c-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ff66c-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="ff66c-132">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="ff66c-132">Frequently Asked Questions</span></span>](across-faq.md)  
