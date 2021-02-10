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
ms.date: 11/26/2020
ms.author: edupont
ms.openlocfilehash: 5636f4b449a944e6b4d67e3dcae9f4c6657e5e06
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4757724"
---
# <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="5c3a5-103">Accessibility and Keyboard Shortcuts</span><span class="sxs-lookup"><span data-stu-id="5c3a5-103">Accessibility and Keyboard Shortcuts</span></span>

<span data-ttu-id="5c3a5-104">This topic provides information about the features that make [!INCLUDE[prod_short](includes/prod_short.md)] readily available to people with disabilities.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-104">This topic provides information about the features that make [!INCLUDE[prod_short](includes/prod_short.md)] readily available to people with disabilities.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="5c3a5-105">supports the following accessibility features:</span><span class="sxs-lookup"><span data-stu-id="5c3a5-105">supports the following accessibility features:</span></span>  

- <span data-ttu-id="5c3a5-106">Keyboard shortcuts</span><span class="sxs-lookup"><span data-stu-id="5c3a5-106">Keyboard shortcuts</span></span>

    <span data-ttu-id="5c3a5-107">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md)</span><span class="sxs-lookup"><span data-stu-id="5c3a5-107">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md)</span></span>

- <span data-ttu-id="5c3a5-108">Navigation</span><span class="sxs-lookup"><span data-stu-id="5c3a5-108">Navigation</span></span>  

- <span data-ttu-id="5c3a5-109">Headings</span><span class="sxs-lookup"><span data-stu-id="5c3a5-109">Headings</span></span>  

- <span data-ttu-id="5c3a5-110">Alternative text for images and links</span><span class="sxs-lookup"><span data-stu-id="5c3a5-110">Alternative text for images and links</span></span>  

- <span data-ttu-id="5c3a5-111">Support for common assistive technologies</span><span class="sxs-lookup"><span data-stu-id="5c3a5-111">Support for common assistive technologies</span></span>  

- <span data-ttu-id="5c3a5-112">Use keyboard shortcuts to zoom in or out on any page</span><span class="sxs-lookup"><span data-stu-id="5c3a5-112">Use keyboard shortcuts to zoom in or out on any page</span></span>

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

## <a name="navigation"></a><a name="Navigation"></a> <span data-ttu-id="5c3a5-113">Navigation</span><span class="sxs-lookup"><span data-stu-id="5c3a5-113">Navigation</span></span>  
 <span data-ttu-id="5c3a5-114">You can navigate between the tabs and actions in the ribbon, elements in the navigation bar, and other controls on [!INCLUDE[prod_short](includes/prod_short.md)] pages and reports using the keyboard.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-114">You can navigate between the tabs and actions in the ribbon, elements in the navigation bar, and other controls on [!INCLUDE[prod_short](includes/prod_short.md)] pages and reports using the keyboard.</span></span> <span data-ttu-id="5c3a5-115">To move the focus from one tab, action, or control to another, press the Tab key to move forward.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-115">To move the focus from one tab, action, or control to another, press the Tab key to move forward.</span></span> <span data-ttu-id="5c3a5-116">Press Shift+Tab to move backward.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-116">Press Shift+Tab to move backward.</span></span>  

 <span data-ttu-id="5c3a5-117">By using the tab order, you can also switch between the main browser page and dialogue boxes that request confirmation, for example, or the login page.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-117">By using the tab order, you can also switch between the main browser page and dialog boxes that request confirmation, for example, or the login page.</span></span>  

## <a name="headings-in-content"></a><a name="Headings"></a> <span data-ttu-id="5c3a5-118">Headings in Content</span><span class="sxs-lookup"><span data-stu-id="5c3a5-118">Headings in Content</span></span>
 
 <span data-ttu-id="5c3a5-119">The HTML source for [!INCLUDE[prod_short](includes/prod_short.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-119">The HTML source for [!INCLUDE[prod_short](includes/prod_short.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span></span> <span data-ttu-id="5c3a5-120">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-120">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span></span> <span data-ttu-id="5c3a5-121">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span><span class="sxs-lookup"><span data-stu-id="5c3a5-121">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span></span>  

## <a name="image-and-links"></a><a name="Images"></a> <span data-ttu-id="5c3a5-122">Image and Links</span><span class="sxs-lookup"><span data-stu-id="5c3a5-122">Image and Links</span></span>

 <span data-ttu-id="5c3a5-123">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-123">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span></span> <span data-ttu-id="5c3a5-124">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-124">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span></span>  

## <a name="assistive-technologies"></a><a name="AssistiveTech"></a> <span data-ttu-id="5c3a5-125">Assistive Technologies</span><span class="sxs-lookup"><span data-stu-id="5c3a5-125">Assistive Technologies</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="5c3a5-126">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-126">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span></span> <span data-ttu-id="5c3a5-127">Some assistive technologies may not work well with certain elements in [!INCLUDE[prod_short](includes/prod_short.md)] pages.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-127">Some assistive technologies may not work well with certain elements in [!INCLUDE[prod_short](includes/prod_short.md)] pages.</span></span>  

## <a name="zoom"></a><a name="zoom"></a> <span data-ttu-id="5c3a5-128">Zoom</span><span class="sxs-lookup"><span data-stu-id="5c3a5-128">Zoom</span></span>

<span data-ttu-id="5c3a5-129">Most browsers use standard keyboard shortcuts to zoom in and out on the current page.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-129">Most browsers use standard keyboard shortcuts to zoom in and out on the current page.</span></span> <span data-ttu-id="5c3a5-130">These keyboard shortcuts are not specific to [!INCLUDE [prod_short](includes/prod_short.md)], but they work when you use [!INCLUDE [prod_short](includes/prod_short.md)] in a browser.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-130">These keyboard shortcuts are not specific to [!INCLUDE [prod_short](includes/prod_short.md)], but they work when you use [!INCLUDE [prod_short](includes/prod_short.md)] in a browser.</span></span> <span data-ttu-id="5c3a5-131">For a list of supported keyboard shortcuts, see [Keyboard Shortcuts for Zooming In and Out](keyboard-shortcuts.md#zoomshortcuts).</span><span class="sxs-lookup"><span data-stu-id="5c3a5-131">For a list of supported keyboard shortcuts, see [Keyboard Shortcuts for Zooming In and Out](keyboard-shortcuts.md#zoomshortcuts).</span></span>  

## <a name="for-more-accessibility-information"></a><span data-ttu-id="5c3a5-132">For more accessibility information</span><span class="sxs-lookup"><span data-stu-id="5c3a5-132">For more accessibility information</span></span>

<span data-ttu-id="5c3a5-133">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span><span class="sxs-lookup"><span data-stu-id="5c3a5-133">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span></span>

## <a name="see-also"></a><span data-ttu-id="5c3a5-134">See Also</span><span class="sxs-lookup"><span data-stu-id="5c3a5-134">See Also</span></span>

[<span data-ttu-id="5c3a5-135">Getting Started</span><span class="sxs-lookup"><span data-stu-id="5c3a5-135">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="5c3a5-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5c3a5-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="5c3a5-137">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="5c3a5-137">Frequently Asked Questions</span></span>](across-faq.md)  
