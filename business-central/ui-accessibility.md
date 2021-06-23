---
title: Assistive features
description: Keyboard shortcuts and other assistive features.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accessibility, shortcuts, charts, tooltips, screen reader
ms.date: 04/29/2021
ms.author: jswymer
ms.openlocfilehash: 5a9b99b367ca732f5b6347462a07b0d0c3f5c522
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115897"
---
# <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="792fb-103">Accessibility and Keyboard Shortcuts</span><span class="sxs-lookup"><span data-stu-id="792fb-103">Accessibility and Keyboard Shortcuts</span></span>

<span data-ttu-id="792fb-104">This article provides information about the features that make [!INCLUDE[prod_short](includes/prod_short.md)] readily available to people with disabilities.</span><span class="sxs-lookup"><span data-stu-id="792fb-104">This article provides information about the features that make [!INCLUDE[prod_short](includes/prod_short.md)] readily available to people with disabilities.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="792fb-105">supports the following accessibility features:</span><span class="sxs-lookup"><span data-stu-id="792fb-105">supports the following accessibility features:</span></span>  

- <span data-ttu-id="792fb-106">Keyboard shortcuts.</span><span class="sxs-lookup"><span data-stu-id="792fb-106">Keyboard shortcuts.</span></span> <span data-ttu-id="792fb-107">See [Keyboard Shortcuts](keyboard-shortcuts.md).</span><span class="sxs-lookup"><span data-stu-id="792fb-107">See [Keyboard Shortcuts](keyboard-shortcuts.md).</span></span>
- <span data-ttu-id="792fb-108">Touch and pen gestures on tablets and phones.</span><span class="sxs-lookup"><span data-stu-id="792fb-108">Touch and pen gestures on tablets and phones.</span></span> <span data-ttu-id="792fb-109">See [Touch and Pen Gestures](touch-gestures.md).</span><span class="sxs-lookup"><span data-stu-id="792fb-109">See [Touch and Pen Gestures](touch-gestures.md).</span></span>
- <span data-ttu-id="792fb-110">Navigation</span><span class="sxs-lookup"><span data-stu-id="792fb-110">Navigation</span></span>  
- <span data-ttu-id="792fb-111">Headings</span><span class="sxs-lookup"><span data-stu-id="792fb-111">Headings</span></span>  
- <span data-ttu-id="792fb-112">Alternative text for images and links</span><span class="sxs-lookup"><span data-stu-id="792fb-112">Alternative text for images and links</span></span>  
- <span data-ttu-id="792fb-113">Support for common assistive technologies</span><span class="sxs-lookup"><span data-stu-id="792fb-113">Support for common assistive technologies</span></span> 
- <span data-ttu-id="792fb-114">Zoom in or out on any page</span><span class="sxs-lookup"><span data-stu-id="792fb-114">Zoom in or out on any page</span></span>
- <span data-ttu-id="792fb-115">Tooltips on elements in the user interface</span><span class="sxs-lookup"><span data-stu-id="792fb-115">Tooltips on elements in the user interface</span></span>

## <a name="navigation"></a><a name="Navigation"></a> <span data-ttu-id="792fb-116">Navigation</span><span class="sxs-lookup"><span data-stu-id="792fb-116">Navigation</span></span>
  
<span data-ttu-id="792fb-117">You can use different combinations of the Tab, Shift, and arrow keys of your keyboard to move between elements on a page.</span><span class="sxs-lookup"><span data-stu-id="792fb-117">You can use different combinations of the Tab, Shift, and arrow keys of your keyboard to move between elements on a page.</span></span> <span data-ttu-id="792fb-118">Elements include actions, fields and columns, parts, and other controls.</span><span class="sxs-lookup"><span data-stu-id="792fb-118">Elements include actions, fields and columns, parts, and other controls.</span></span> <span data-ttu-id="792fb-119">In general, press Tab or Shift+Tab to move to the next or previous element.</span><span class="sxs-lookup"><span data-stu-id="792fb-119">In general, press Tab or Shift+Tab to move to the next or previous element.</span></span>

<span data-ttu-id="792fb-120">When you focus on an area that contains actions, like the navigation bar on the top of role centre or action bar on other pages, use the arrows keys to move through the different actions and groups.</span><span class="sxs-lookup"><span data-stu-id="792fb-120">When you focus on an area that contains actions, like the navigation bar on the top of role center or action bar on other pages, use the arrows keys to move through the different actions and groups.</span></span> <span data-ttu-id="792fb-121">Press Enter on a group to open its underlying actions, and then continue using the arrows keys.</span><span class="sxs-lookup"><span data-stu-id="792fb-121">Press Enter on a group to open its underlying actions, and then continue using the arrows keys.</span></span> <span data-ttu-id="792fb-122">Press Tab or Shift+Tab to move out of the action area.</span><span class="sxs-lookup"><span data-stu-id="792fb-122">Press Tab or Shift+Tab to move out of the action area.</span></span>

<span data-ttu-id="792fb-123">By using the tab order, you can also switch between the main browser page and dialogue boxes that request confirmation, for example, or the sign-in page.</span><span class="sxs-lookup"><span data-stu-id="792fb-123">By using the tab order, you can also switch between the main browser page and dialog boxes that request confirmation, for example, or the sign-in page.</span></span>  

## <a name="headings-in-content"></a><a name="Headings"></a> <span data-ttu-id="792fb-124">Headings in Content</span><span class="sxs-lookup"><span data-stu-id="792fb-124">Headings in Content</span></span>

<span data-ttu-id="792fb-125">The HTML source for [!INCLUDE[prod_short](includes/prod_short.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span><span class="sxs-lookup"><span data-stu-id="792fb-125">The HTML source for [!INCLUDE[prod_short](includes/prod_short.md)] content uses tags to help users of assistive technology to understand the structure and content of the page.</span></span> <span data-ttu-id="792fb-126">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span><span class="sxs-lookup"><span data-stu-id="792fb-126">For example, on list pages, the columns are defined in TH tags and the column headings are set with TITLE attribute inside the tag.</span></span> <span data-ttu-id="792fb-127">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span><span class="sxs-lookup"><span data-stu-id="792fb-127">Captions for elements, such as FastTabs, FactBoxes, and fields are included in heading tags (H1, H2, H3, and H4).</span></span>  

## <a name="image-and-links"></a><a name="Images"></a> <span data-ttu-id="792fb-128">Image and Links</span><span class="sxs-lookup"><span data-stu-id="792fb-128">Image and Links</span></span>

<span data-ttu-id="792fb-129">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span><span class="sxs-lookup"><span data-stu-id="792fb-129">A descriptive text for images is set with the ALT attribute inside the IMG tag.</span></span> <span data-ttu-id="792fb-130">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span><span class="sxs-lookup"><span data-stu-id="792fb-130">A descriptive text for hyperlinks is set with the title attribute inside the A tag.</span></span>  

## <a name="assistive-technologies"></a><a name="AssistiveTech"></a> <span data-ttu-id="792fb-131">Assistive Technologies</span><span class="sxs-lookup"><span data-stu-id="792fb-131">Assistive Technologies</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="792fb-132">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span><span class="sxs-lookup"><span data-stu-id="792fb-132">supports various assistive technologies, such as high contrast, screen readers, and voice recognition software.</span></span> <span data-ttu-id="792fb-133">Some assistive technologies may not work well with certain elements in [!INCLUDE[prod_short](includes/prod_short.md)] pages.</span><span class="sxs-lookup"><span data-stu-id="792fb-133">Some assistive technologies may not work well with certain elements in [!INCLUDE[prod_short](includes/prod_short.md)] pages.</span></span>  

## <a name="zoom"></a><a name="zoom"></a> <span data-ttu-id="792fb-134">Zoom</span><span class="sxs-lookup"><span data-stu-id="792fb-134">Zoom</span></span>

<span data-ttu-id="792fb-135">Most browsers use standard keyboard shortcuts to zoom in and out on the current page.</span><span class="sxs-lookup"><span data-stu-id="792fb-135">Most browsers use standard keyboard shortcuts to zoom in and out on the current page.</span></span> <span data-ttu-id="792fb-136">These keyboard shortcuts aren't specific to [!INCLUDE [prod_short](includes/prod_short.md)], but they work when you use [!INCLUDE [prod_short](includes/prod_short.md)] in a browser.</span><span class="sxs-lookup"><span data-stu-id="792fb-136">These keyboard shortcuts aren't specific to [!INCLUDE [prod_short](includes/prod_short.md)], but they work when you use [!INCLUDE [prod_short](includes/prod_short.md)] in a browser.</span></span> <span data-ttu-id="792fb-137">For a list of supported keyboard shortcuts, see [Keyboard Shortcuts for Zooming In and Out](keyboard-shortcuts.md#zoomshortcuts).</span><span class="sxs-lookup"><span data-stu-id="792fb-137">For a list of supported keyboard shortcuts, see [Keyboard Shortcuts for Zooming In and Out](keyboard-shortcuts.md#zoomshortcuts).</span></span>

## <a name="tooltips"></a><span data-ttu-id="792fb-138">Tooltips</span><span class="sxs-lookup"><span data-stu-id="792fb-138">Tooltips</span></span>

<span data-ttu-id="792fb-139">Tooltips are available on most elements in the user interface, like page fields and columns, actions, cues tiles, and charts.</span><span class="sxs-lookup"><span data-stu-id="792fb-139">Tooltips are available on most elements in the user interface, like page fields and columns, actions, cues tiles, and charts.</span></span> <span data-ttu-id="792fb-140">A tooltip provides extra text that explains an element to help you better understand its purpose.</span><span class="sxs-lookup"><span data-stu-id="792fb-140">A tooltip provides extra text that explains an element to help you better understand its purpose.</span></span> 

<span data-ttu-id="792fb-141">Tooltips are accessed in different ways, depending on the client (web or mobile) and the device that you're working with.</span><span class="sxs-lookup"><span data-stu-id="792fb-141">Tooltips are accessed in different ways, depending on the client (web or mobile) and the device that you're working with.</span></span> <span data-ttu-id="792fb-142">Use the following table as a guide.</span><span class="sxs-lookup"><span data-stu-id="792fb-142">Use the following table as a guide.</span></span> <span data-ttu-id="792fb-143">Some tooltips can be read by screen-readers.</span><span class="sxs-lookup"><span data-stu-id="792fb-143">Some tooltips can be read by screen-readers.</span></span> <span data-ttu-id="792fb-144">In this case, you access the tooltips as described in the table, then use the screen reader to navigate to the tooltip as you would with any other element.</span><span class="sxs-lookup"><span data-stu-id="792fb-144">In this case, you access the tooltips as described in the table, then use the screen reader to navigate to the tooltip as you would with any other element.</span></span>

#### <a name="accessing-tooltips"></a><span data-ttu-id="792fb-145">Accessing tooltips</span><span class="sxs-lookup"><span data-stu-id="792fb-145">Accessing tooltips</span></span>

|<span data-ttu-id="792fb-146">Element</span><span class="sxs-lookup"><span data-stu-id="792fb-146">Element</span></span>|<span data-ttu-id="792fb-147">Mouse action for web client</span><span class="sxs-lookup"><span data-stu-id="792fb-147">Mouse action for web client</span></span>|<span data-ttu-id="792fb-148">Keyboard shortcut for web client</span><span class="sxs-lookup"><span data-stu-id="792fb-148">Keyboard shortcut for web client</span></span>|<span data-ttu-id="792fb-149">Touch gesture on tablet/phone for mobile app</span><span class="sxs-lookup"><span data-stu-id="792fb-149">Touch gesture on tablet/phone for mobile app</span></span>|<span data-ttu-id="792fb-150">Screen reader support</span><span class="sxs-lookup"><span data-stu-id="792fb-150">Screen reader support</span></span>|
|-------|-----------------|------------|--------------------------|---------------------|
|<span data-ttu-id="792fb-151">Page fields and column headings</span><span class="sxs-lookup"><span data-stu-id="792fb-151">Page fields and column headings</span></span>|<span data-ttu-id="792fb-152">Hover over or click the field caption or column heading</span><span class="sxs-lookup"><span data-stu-id="792fb-152">Hover over or click the field caption or column heading</span></span>|<span data-ttu-id="792fb-153">Move focus to the field or column heading, and press Alt+Up Arrow keys</span><span class="sxs-lookup"><span data-stu-id="792fb-153">Move focus to the field or column heading, and press Alt+Up Arrow keys</span></span>|<span data-ttu-id="792fb-154">Tap the field caption</span><span class="sxs-lookup"><span data-stu-id="792fb-154">Tap the field caption</span></span> |<span data-ttu-id="792fb-155">yes</span><span class="sxs-lookup"><span data-stu-id="792fb-155">yes</span></span>|
|<span data-ttu-id="792fb-156">Charts elements, like a bar, line, pie slice</span><span class="sxs-lookup"><span data-stu-id="792fb-156">Charts elements, like a bar, line, pie slice</span></span>|<span data-ttu-id="792fb-157">Hover over the element</span><span class="sxs-lookup"><span data-stu-id="792fb-157">Hover over the element</span></span>|<span data-ttu-id="792fb-158">Move focus to element, for example, by using arrow keys</span><span class="sxs-lookup"><span data-stu-id="792fb-158">Move focus to element, for example, by using arrow keys</span></span>|<span data-ttu-id="792fb-159">Tap and hold the element</span><span class="sxs-lookup"><span data-stu-id="792fb-159">Tap and hold the element</span></span>|<span data-ttu-id="792fb-160">yes</span><span class="sxs-lookup"><span data-stu-id="792fb-160">yes</span></span>|
|<span data-ttu-id="792fb-161">Actions</span><span class="sxs-lookup"><span data-stu-id="792fb-161">Actions</span></span>|<span data-ttu-id="792fb-162">Hover over the action</span><span class="sxs-lookup"><span data-stu-id="792fb-162">Hover over the action</span></span>|<span data-ttu-id="792fb-163">none</span><span class="sxs-lookup"><span data-stu-id="792fb-163">none</span></span>|<span data-ttu-id="792fb-164">none</span><span class="sxs-lookup"><span data-stu-id="792fb-164">none</span></span> |<span data-ttu-id="792fb-165">no</span><span class="sxs-lookup"><span data-stu-id="792fb-165">no</span></span>|
|<span data-ttu-id="792fb-166">Cue tiles</span><span class="sxs-lookup"><span data-stu-id="792fb-166">Cue tiles</span></span>|<span data-ttu-id="792fb-167">Hover over the tile</span><span class="sxs-lookup"><span data-stu-id="792fb-167">Hover over the tile</span></span> |<span data-ttu-id="792fb-168">none</span><span class="sxs-lookup"><span data-stu-id="792fb-168">none</span></span>|<span data-ttu-id="792fb-169">none</span><span class="sxs-lookup"><span data-stu-id="792fb-169">none</span></span>|<span data-ttu-id="792fb-170">no</span><span class="sxs-lookup"><span data-stu-id="792fb-170">no</span></span>|


<!--
- With a mouse, hover over the element.
- With keyboard, press the Alt+Up Arrow keys.
- On a tablet or phone, tap and hold on the element. To learn about more gestures, see [Touch and Pen Gestures](touch-gestures.md)

-->

## <a name="for-more-accessibility-information"></a><span data-ttu-id="792fb-171">For more accessibility information</span><span class="sxs-lookup"><span data-stu-id="792fb-171">For more accessibility information</span></span>

<span data-ttu-id="792fb-172">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span><span class="sxs-lookup"><span data-stu-id="792fb-172">You can find additional information about accessibility with Microsoft products and assistive technologies on the [Microsoft Accessibility](https://go.microsoft.com/fwlink/?LinkId=262160) site.</span></span>

## <a name="see-also"></a><span data-ttu-id="792fb-173">See Also</span><span class="sxs-lookup"><span data-stu-id="792fb-173">See Also</span></span>

[<span data-ttu-id="792fb-174">Getting Ready for Doing Business</span><span class="sxs-lookup"><span data-stu-id="792fb-174">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
<span data-ttu-id="792fb-175">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="792fb-175">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="792fb-176">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="792fb-176">Frequently Asked Questions</span></span>](across-faq.yml)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
