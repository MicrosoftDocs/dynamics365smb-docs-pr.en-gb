---
title: Why a Page is Locked from Personalisation
description: You might be blocked from personalising a page. Read here about what you can do to unlock it so you can personalise it.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'customize, personalize, personalization, hide columns, remove fields, move fields'
ms.search.form: null
ms.date: 04/01/2021
ms.author: edupont
---
# <a name="why-a-page-is-locked-from-personalization"></a><a name="why-a-page-is-locked-from-personalization"></a>Why a Page is Locked from Personalisation

There are two conditions that prevent you from personalising a page. Either the page is locked (as indicated by the ![Personalise Lock.](media/personalization-lock-icon.png "Personalise lock")) icon or it's blocked (as indicated by the ![Personalisation blocked.](media/personalization-blocked-icon.png "Personalisation blocked") icon).

## <a name="locked-from-personalizing"></a><a name="locked-from-personalizing"></a>Locked from Personalising

If there's a ![Personalise Lock.](media/personalization-lock-icon.png "Personalise lock") icon in the **Personalising** banner when you open a page, you're currently prevented from making any more personalisation changes to the page.

<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

There can be two reasons:

1. You've personalised the page before, but it was done using an earlier version of the product. We changed the way personalisation works behind the scenes since the last time that you personalised the page. Unfortunately, the old way and new way of doing things don't work together.

2. Until now, you've only used the bow deprecated [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalise the page.

### <a name="unlocking-the-page"></a><a name="unlocking-the-page"></a>Unlocking the Page

If you want to unlock a page and continue personalising it, choose the ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon, and then choose the **Unlock** action.  

> [!CAUTION]
> The current personalisation of the page will be cleared. The page will go back to its original layout, and you'll have to start from scratch.  

## <a name="blocked-from-personalizing"></a><a name="blocked-from-personalizing"></a>Blocked from Personalising

If there's a ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon in the **Personalising** banner, you're blocked from doing any personalisation to the page.

<!-- Only text is translated, so removing this image for non-English UX reasons.  ![Personalize blocked.](media/personalization-blocked.png "Personalize lock") -->

The reason is that the Role Centre or role that is currently associated with your user account modifies this page specifically for your role. Contact your administrator for assistance. Alternatively, try switching to a Role Centre that does include role-tailoring for this page. For more information, see [Change Basic Settings](ui-change-basic-settings.md).

## <a name="see-also"></a><a name="see-also"></a>See Also

[Personalise Your Workspace](ui-personalization-user.md)  
[Customise Pages for Profiles](ui-personalization-manage.md)  
[Change Basic Settings](ui-change-basic-settings.md)  
[Change Which Features are Displayed](ui-experiences.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
