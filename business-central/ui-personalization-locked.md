---
title: Why Can't I Personalise a Page | Microsoft Docs
description: Explains why you cannot personlaize a page and what yoo can do to unlock it so you can personalise it.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 64995372f68ed2804bc165823dacc34ad6a3194d
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "911703"
---
# <a name="why-a-page-is-locked-from-personalization"></a>Why a Page is Locked from Personalisation

There are two conditions that prevent you from personalising a page. Either the page is locked (as indicated by ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock")) or it is blocked (as indicated by ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked")).

## <a name="locked-from-personalizing"></a>Locked from Personalising

If there is a ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon in the **Personalising** banner when you open a page (as shown), this means that you are currently prevented from making any more personalisation changes to the page.

![Personalise Lock](media/personalization-locked.png "Personalise lock")


<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

There can be two reasons for this:

1. You have personalised the page before, but it was done using an earlier version of the product. We changed the way personalisation works behind the scenes since the last time that you personalised the page. Unfortunately, the old way and new way of doing things do not work together.

2. Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalise the page.

### <a name="unlocking-the-page"></a>Unlocking the Page

If you want to unlock a page and continue personalising it, choose ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock"), and then **Unlock**.  

Before you unlock the page, be aware of the following:

- The current personalisation of the page will be cleared. The page will go back to its original layout, and you will have to start from scratch.

- In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalisation changes made in the Business Central client. Going forward, the personalisation in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.

## <a name="blocked-from-personalizing"></a>Blocked from Personalising

If there is a ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon in the Personalising banner, this means that you are blocked from doing any personalisation to the page.

![Personalise blocked](media/personalization-blocked.png "Personalise lock")

The reason for this is that the Role Centre or profile that is currently associated with your user account modifies this page specifically for your role. Please contact your administrator for assistance or, if it makes sense, try switching to a Role Centre (from  [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central")) that does include role-tailoring for this page.

## <a name="see-also"></a>See Also
[Personalising Your Workspace](ui-personalization-manage.md)  
[Managing Personalisation](ui-personalization-manage.md)  
[Changing Basic Settings](ui-change-basic-settings.md)  
[Changing Which Features are Displayed](ui-experiences.md)  
