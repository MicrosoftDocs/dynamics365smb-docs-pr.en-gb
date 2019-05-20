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
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: d04f78b31b9fb0403201cb9e5cb1f98f1ef935e1
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1248026"
---
# <a name="tell-me-faq"></a>Tell Me FAQ
This topic answers questions that our advanced users often ask about the new Tell Me feature, which has replaced the previous Page Search feature known as **Find Pages and Reports**.

### <a name="are-all-actions-from-my-current-page-discoverable-in-tell-me"></a>Are all actions from my current page discoverable in Tell Me?
No. Actions in parts, such as the Sales Lines part or FactBoxes, are not displayed in Tell Me.

### <a name="are-the-results-in-tell-me-filtered-by-permissions"></a>Are the results in Tell Me filtered by permissions?
If the user does not have AccessByPermissions then actions are not displayed. However, pages and reports appear in the results but require that the user has permission to access them. A message will display if the user does not have permission to view the object.

### <a name="does-tell-me-display-content-from-my-customizations-or-installed-third-party-extensions"></a>Does Tell Me display content from my customisations or installed third-party extensions?
Actions, pages, and reports that originate from extensions are picked up by Tell Me, but custom help documentation is not. For technical information about how to make custom pages and reports discoverable, see [Adding Pages and Reports to Search](/dynamics365/business-central/dev-itpro/developer/devenv-al-menusuite-functionality).

### <a name="what-makes-this-different-from-what-was-previously-known-as-page-search"></a>What makes this different from what was previously known as Page Search?
Page Search has evolved into Tell Me to help you get work done quickly. Page Search could only help you navigate to pages or reports. At a technical level, Tell Me is no longer based on the legacy MenuSuite concept.

### <a name="i-use-on-premises-included365finincludesd365finmdmd-does-that-include-tell-me"></a>I use on-premises [!INCLUDE[d365fin](includes/d365fin_md.md)]. Does that include Tell Me?
You can use Tell Me in the on-premises Web Client to find actions, pages, and reports, but not documentation, or apps and consulting services on AppSource. Users connecting to [!INCLUDE[d365fin](includes/d365fin_md.md)] from the Dynamics NAV client continue to use Page Search.

### <a name="is-tell-me-available-for-all-form-factors"></a>Is Tell Me available for all form factors?
Tell Me is only available in the Web Client or Windows desktop app.

### <a name="are-the-documentation-results-available-in-any-language"></a>Are the documentation results available in any language?
The help articles display in the language you have specified in **My Settings**, if help is available in that language.

## <a name="see-also"></a>See Also  
[Finding Features and Information](ui-search.md)
