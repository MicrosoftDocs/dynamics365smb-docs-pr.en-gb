---
title: Managing Personalisation as an Administrator in Business Central | Microsoft Docs
description: Learn how to customise the user interface to suit your way of working.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 15d7e4aac7989f95f7becc8aa8ed96381a7dc2de
ms.contentlocale: en-gb
ms.lasthandoff: 11/22/2018

---
# <a name="managing-personalization-as-an-administrator"></a>Managing Personalisation as an Administrator
<!--NAV in the Web client--> Users can personalise their workspace to suit their own preferences. As an administrator, you can control and manage personalisation by disabling the ability for users to personalise pages and clearing any page personalisations that users have made.

## <a name="disable-personalization-for-a-profile"></a>Disable personalisation for a profile
You can prevent all users that belong to a specific profile from being able to personalise their pages.
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles**, and then choose the related link.
2.  Select the profile in the list that you want to modify.
3. Select the **Disable personalisation** check box, and then choose the **OK** button.

## <a name="clear-user-personalizations"></a>Clear user personalisations

Clearing page personalisation changes the page back to its original layout before any personalisation was made. There are two ways to clear the personalisations that users have made to pages: using the **Delete User Personalisation** page and using the **User Personalisation Card** page.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Clear user personalisations by using the Delete User Personalisation page

The **Delete User Personalisation** page enables you to clear personalisations on a per-page basis for each user individually.

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete User Personalisation**, and then choose the related link.

    The page lists all the pages that have been personalised and the user it belongs to.

    >[!NOTE]
    > A check mark in the **Legacy Personalisation** columns indicates that the personalisation was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalisation different than it does now. Users who try to personalise these pages are locked from doing so unless they choose to unlock the page. For more information, see [Why a page is locked from personalising](ui-personalization-locked.md).

2. Select the entry that you want to delete, and then choose the **Delete** action.

    The user will see the changes the next time they sign-in.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Clear user personalisations by using the User Personalisation Card page

The **User Personalisation Card** page enables you to clear the personalisation on all pages for specific user. This requires write permission to Table 2000000072 **Profile**.

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Personalisation**, and then choose the related link.

    The **User Personalisation** page lists all users who potentially have personalised pages. If you cannot find a user in the list, this means that they do not have any personalised pages.

2. Select the user from the list, and then choose the **Edit** action.

3.  On the **Actions** tab, choose **Clear Personalised Pages**.

    The user will see the changes the next time they sign-in.

## <a name="see-also"></a>See Also
[Personalising Your Workspace](ui-personalization-user.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Changing Basic Settings](ui-change-basic-settings.md)  
[Changing Which Features are Displayed](ui-experiences.md)  

