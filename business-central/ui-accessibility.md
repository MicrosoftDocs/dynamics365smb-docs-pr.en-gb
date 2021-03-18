---
title: Assistive features
description: Keyboard shortcuts and other assistive features.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/26/2020
ms.author: edupont
ms.openlocfilehash: 8e5d0a2f51eb223c7fef98cbc6076eb73f45fdd3
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5390606"
---
# <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="e98bc-103">Accessibility and Keyboard Shortcuts</span><span class="sxs-lookup"><span data-stu-id="e98bc-103">Accessibility and Keyboard Shortcuts</span></span>

<span data-ttu-id="e98bc-104">This topic provides information about the features that make [!INCLUDE[prod_short](includes/prod_short.md)] readily available to people with disabilities.</span><span class="sxs-lookup"><span data-stu-id="e98bc-104">This topic provides information about the features that make [!INCLUDE[prod_short](includes/prod_short.md)] readily available to people with disabilities.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e98bc-105">supports the following accessibility features:</span><span class="sxs-lookup"><span data-stu-id="e98bc-105">supports the following accessibility features:</span></span>  

- <span data-ttu-id="e98bc-106">Keyboard shortcuts</span><span class="sxs-lookup"><span data-stu-id="e98bc-106">Keyboard shortcuts</span></span>

    <span data-ttu-id="e98bc-107">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md)</span><span class="sxs-lookup"><span data-stu-id="e98bc-107">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md)</span></span>

- <span data-ttu-id="e98bc-108">Navigation</span><span class="sxs-lookup"><span data-stu-id="e98bc-108">Navigation</span></span>  

- <span data-ttu-id="e98bc-109">Headings</span><span class="sxs-lookup"><span data-stu-id="e98bc-109">Headings</span></span>  

- <span data-ttu-id="e98bc-110">Alternative text for images and links</span><span class="sxs-lookup"><span data-stu-id="e98bc-110">Alternative text for images and links</span></span>  

- <span data-ttu-id="e98bc-111">Support for common assistive technologies</span><span class="sxs-lookup"><span data-stu-id="e98bc-111">Support for common assistive technologies</span></span>  

- <span data-ttu-id="e98bc-112">Use keyboard shortcuts to zoom in or out on any page</span><span class="sxs-lookup"><span data-stu-id="e98bc-112">Use keyboard shortcuts to zoom in or out on any page</span></span>

<!-- moved to separate article
##  <a name="Keyboard"></a> Keyboard Shortcuts in the browser
 [!INCLUDE[prod_short](includes/prod_short.md)] supports the keyboard shortcuts that are supported by most web browsers. The keyboard shortcuts described here refer to the U.S. keyboard layout. The layout of the keys on other keyboards may not correspond exactly to the keys on a U.S. keyboard.  

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

## <a name="navigation"></a><a name="Navigation"></a> <span data-ttu-id="e98bc-113">Navigation</span><span class="sxs-lookup"><span data-stu-id="e98bc-113">Navigation</span></span>  
 <span data-ttu-id="e98bc-114">You can navigate between the tabs and actions in the ribbon, elements in the navigation bar, and other controls on [!INCLUDE[prod_short](includes/prod_short.md)] pages and reports using the keyboard.</span><span class="sxs-lookup"><span data-stu-id="e98bc-114">You can navigate between the tabs and actions in the ribbon, elements in the navigation bar, and other controls on [!INCLUDE[prod_short](includes/prod_short.md)] pages and reports using the keyboard.</span></span> <span data-ttu-id="e98bc-115">To move the focus from one tab, action, or control to another, press the Tab key to move forward.</span><span class="sxs-lookup"><span data-stu-id="e98bc-115">To move the focus from one tab, action, or control to another, press the Tab key to move forward.</span></span> <span data-ttu-id="e98bc-116">Press Shift+Tab to move backward.</span><span class="sxs-lookup"><span data-stu-id="e98bc-116">Press Shift+Tab to move backward.</span></span>  

 <span data-ttu-id="e98bc-117">By using the tab order, you can also switch between the main browser page and dialogue boxes that request confirmation, for example, or the login page.</span><span class="sxs-lookup"><span data-stu-id="e98bc-117">By using the tab order, you can also switch between the main browser page and dialog boxes that request confirmation, for example, or the login page.</span></span>  

## <a name="headings-in-content"></a><a name="Headings"></a> <span data-ttu-id="e98bc-118">Headings in Content</span><span class="sxs-lookup"><span data-stu-id="e98bc-118">Headings in Content</span></span>
 
 <span data-ttu-id="e98bc-119">The HTML source for [!INCLUDE[prod_short](includes/prod_short.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span><span class="sxs-lookup"><span data-stu-id="e98bc-119">The HTML source for [!INCLUDE[prod_short](includes/prod_short.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span></span> <span data-ttu-id="e98bc-120">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span><span class="sxs-lookup"><span data-stu-id="e98bc-120">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span></span> <span data-ttu-id="e98bc-121">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span><span class="sxs-lookup"><span data-stu-id="e98bc-121">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span></span>  

## <a name="image-and-links"></a><a name="Images"></a> <span data-ttu-id="e98bc-122">Image and Links</span><span class="sxs-lookup"><span data-stu-id="e98bc-122">Image and Links</span></span>

 <span data-ttu-id="e98bc-123">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span><span class="sxs-lookup"><span data-stu-id="e98bc-123">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span></span> <span data-ttu-id="e98bc-124">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span><span class="sxs-lookup"><span data-stu-id="e98bc-124">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span></span>  

## <a name="assistive-technologies"></a><a name="AssistiveTech"></a> <span data-ttu-id="e98bc-125">Assistive Technologies</span><span class="sxs-lookup"><span data-stu-id="e98bc-125">Assistive Technologies</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e98bc-126">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span><span class="sxs-lookup"><span data-stu-id="e98bc-126">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span></span> <span data-ttu-id="e98bc-127">Some assistive technologies may not work well with certain elements in [!INCLUDE[prod_short](includes/prod_short.md)] pages.</span><span class="sxs-lookup"><span data-stu-id="e98bc-127">Some assistive technologies may not work well with certain elements in [!INCLUDE[prod_short](includes/prod_short.md)] pages.</span></span>  

## <a name="zoom"></a><a name="zoom"></a> <span data-ttu-id="e98bc-128">Zoom</span><span class="sxs-lookup"><span data-stu-id="e98bc-128">Zoom</span></span>

<span data-ttu-id="e98bc-129">Most browsers use standard keyboard shortcuts to zoom in and out on the current page.</span><span class="sxs-lookup"><span data-stu-id="e98bc-129">Most browsers use standard keyboard shortcuts to zoom in and out on the current page.</span></span> <span data-ttu-id="e98bc-130">These keyboard shortcuts are not specific to [!INCLUDE [prod_short](includes/prod_short.md)], but they work when you use [!INCLUDE [prod_short](includes/prod_short.md)] in a browser.</span><span class="sxs-lookup"><span data-stu-id="e98bc-130">These keyboard shortcuts are not specific to [!INCLUDE [prod_short](includes/prod_short.md)], but they work when you use [!INCLUDE [prod_short](includes/prod_short.md)] in a browser.</span></span> <span data-ttu-id="e98bc-131">For a list of supported keyboard shortcuts, see [Keyboard Shortcuts for Zooming In and Out](keyboard-shortcuts.md#zoomshortcuts).</span><span class="sxs-lookup"><span data-stu-id="e98bc-131">For a list of supported keyboard shortcuts, see [Keyboard Shortcuts for Zooming In and Out](keyboard-shortcuts.md#zoomshortcuts).</span></span>  

## <a name="for-more-accessibility-information"></a><span data-ttu-id="e98bc-132">For more accessibility information</span><span class="sxs-lookup"><span data-stu-id="e98bc-132">For more accessibility information</span></span>

<span data-ttu-id="e98bc-133">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span><span class="sxs-lookup"><span data-stu-id="e98bc-133">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span></span>

## <a name="see-also"></a><span data-ttu-id="e98bc-134">See Also</span><span class="sxs-lookup"><span data-stu-id="e98bc-134">See Also</span></span>

[<span data-ttu-id="e98bc-135">Getting Started</span><span class="sxs-lookup"><span data-stu-id="e98bc-135">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="e98bc-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e98bc-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="e98bc-137">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="e98bc-137">Frequently Asked Questions</span></span>](across-faq.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]