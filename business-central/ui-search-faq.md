---
title: Frequently Asked Questions about Tell Me
description: This article provides answers to questions that our partners and customers often ask about the Tell Me feature.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.search.form: TellMe
ms.date: 05/23/2022
ms.author: bholtorf
---
# <a name="tell-me-faq" />Tell Me FAQ
This article answers questions that our advanced users often ask about the Tell Me feature.

### <a name="are-all-actions-from-my-current-page-discoverable-in-tell-me" />Are all actions from my current page discoverable in Tell Me?

No. Actions in parts, such as the Sales Lines part or FactBoxes, are not displayed in Tell Me.

### <a name="are-the-results-in-tell-me-filtered-by-permissions" />Are the results in Tell Me filtered by permissions?

If the user does not have AccessByPermissions then actions are not displayed. However, pages and reports appear in the results but require that the user has permission to access them. A message will display if the user does not have permission to view the object.

### <a name="does-tell-me-display-content-from-my-customizations-or-installed-third-party-extensions" />Does Tell Me display content from my customisations or installed third-party extensions?

Actions, pages, and reports that originate from extensions are picked up by Tell Me. For technical information about how to make custom pages and reports discoverable, see [Adding Pages and Reports to Search](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).

### <a name="what-makes-this-different-from-what-was-previously-known-as-page-search" />What makes this different from what was previously known as Page Search?

Page Search has evolved into Tell Me to help you get work done quickly. Page Search could only help you navigate to pages or reports. At a technical level, Tell Me is no longer based on the legacy MenuSuite concept.

### <a name="i-use-on-premises--does-that-include-tell-me" />I use on-premises [!INCLUDE[prod_short](includes/prod_short.md)]. Does that include Tell Me?

You can use Tell Me in the on-premises Web Client to find actions, pages, and reports, but not apps and consulting services on AppSource.

### <a name="is-tell-me-available-for-all-form-factors" />Is Tell Me available for all form factors?

Tell Me is only available in the Web Client or Windows desktop app.

<!-- removed in v20 because of Help pane
### <a name="are-the-documentation-results-available-in-any-language" />Are the documentation results available in any language?
The help articles display in the language you have specified in **My Settings**, if help is available in that language.
-->

### <a name="does-tell-me-give-me-help-on-how-to-use-pages-reports-and-other-things" />Does Tell Me give me help on how to use pages, reports, and other things?

No, but you can easily get this information from the Help pane. Just select the **Help** menu item (the question mark in the top-right corner) or select <kbd>Ctrl</kbd>+<kbd>F1</kbd> on your keyboard. For more information, see [Help pane](product-help-and-support.md#help-pane).

### <a name="why-dont-i-see-a-bookmark-icon-for-my-search-results" />Why don't I see a bookmark icon for my search results?

The bookmark icon is not displayed in the Tell Me window when personalisation is disabled for a user role.


## <a name="see-also" />See Also
[Save and Personalise List Views](ui-views.md)  
[Finding Pages and Information with Tell Me](ui-search.md)  
[Finding Pages with the Role Explorer](ui-role-explorer.md)  
[Bookmark a Page or Report on Your Role Centre](ui-bookmarks.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
