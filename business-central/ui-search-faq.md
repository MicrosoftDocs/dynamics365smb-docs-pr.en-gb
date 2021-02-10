---
title: Frequently Asked Questions about Tell Me | Microsoft Docs
description: This article provides answers to questions that our partners and customers often ask about Tell Me.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 7b880ef5cb49a02dcbb3973f87bc64eae48b2b3a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4760249"
---
# <a name="tell-me-faq"></a>Tell Me FAQ
This topic answers questions that our advanced users often ask about the Tell Me feature.

### <a name="are-all-actions-from-my-current-page-discoverable-in-tell-me"></a>Are all actions from my current page discoverable in Tell Me?
No. Actions in parts, such as the Sales Lines part or FactBoxes, are not displayed in Tell Me.

### <a name="are-the-results-in-tell-me-filtered-by-permissions"></a>Are the results in Tell Me filtered by permissions?
If the user does not have AccessByPermissions then actions are not displayed. However, pages and reports appear in the results but require that the user has permission to access them. A message will display if the user does not have permission to view the object.

### <a name="does-tell-me-display-content-from-my-customizations-or-installed-third-party-extensions"></a>Does Tell Me display content from my customisations or installed third-party extensions?
Actions, pages, and reports that originate from extensions are picked up by Tell Me, but custom help documentation is not. For technical information about how to make custom pages and reports discoverable, see [Adding Pages and Reports to Search](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).

### <a name="what-makes-this-different-from-what-was-previously-known-as-page-search"></a>What makes this different from what was previously known as Page Search?
Page Search has evolved into Tell Me to help you get work done quickly. Page Search could only help you navigate to pages or reports. At a technical level, Tell Me is no longer based on the legacy MenuSuite concept.

### <a name="i-use-on-premises-prod_short-does-that-include-tell-me"></a>I use on-premises [!INCLUDE[prod_short](includes/prod_short.md)]. Does that include Tell Me?
You can use Tell Me in the on-premises Web Client to find actions, pages, and reports, but not documentation, or apps and consulting services on AppSource.

### <a name="is-tell-me-available-for-all-form-factors"></a>Is Tell Me available for all form factors?
Tell Me is only available in the Web Client or Windows desktop app.

### <a name="are-the-documentation-results-available-in-any-language"></a>Are the documentation results available in any language?
The help articles display in the language you have specified in **My Settings**, if help is available in that language.

### <a name="why-dont-i-see-a-bookmark-icon-for-my-search-results"></a>Why don't I see a bookmark icon for my search results?
The bookmark icon is not displayed in the Tell Me window when personalisation is disabled for a user role.


## <a name="see-also"></a>See Also  
[Save and Personalise List Views](ui-views.md)  
[Finding Pages and Information with Tell Me](ui-search.md)  
[Finding Pages with the Role Explorer](ui-role-explorer.md)  
[Bookmark a Page or Report on Your Role Centre](ui-bookmarks.md)
