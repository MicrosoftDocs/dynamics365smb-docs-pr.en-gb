---
title: Managing Personalisation as an Administrator in Business Central | Microsoft Docs
description: Learn how to customise the user interface to suit your way of working.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 08/16/2019
ms.author: jswymer
ms.openlocfilehash: 268d61e05f84643abe8eeeb283bd035e0247fe1c
ms.sourcegitcommit: 81b6062194bf04d8052a3cd394cc0b41e3f53e6d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/20/2019
ms.locfileid: "1887744"
---
# <a name="managing-personalization-as-an-administrator"></a>Managing Personalisation as an Administrator

Users can personalise their workspace to suit their own preferences. As an administrator, you control and manage personalisation by:

-   Enabling or disabling the personalisation feature for the entire the application (on-premises installation only).
-   Enabling or disabling the personalisation feature for users of a specific profile.
-   Clearing any page personalisations that users have made.

## <a name="EnablePersonalization"></a>To enable or disable personalisation (On-Premises Only)

By default, personalisation is not enabled in the client. You enable or disable personalisation by modifying the configuration file (navsettings.json) of the Business Central Web Server instance that serves the clients.

1. To enable personalisation, add the following line in the navsettings.json file:

    ```
    "PersonalizationEnabled": "true"
    ```

    To disable personalisation, remove this line or change it to:

    ```
    "PersonalizationEnabled": "false"
    ```

    For more information about how to modify the navsettings.json file, see [Modify the navsettings.json file directly](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-web-server?branch=master#Settings).

2. Generate and download the application symbols.

    This step is optional, and not required to enable personalisation. However, it ensures that new pages that are created by developers can be personalised.

    1. First, you generate the symbols by running finsql.exe with `generatesymbolreference` command. The finsql.exe file is located in the installation folder for the [!INCLUDE[server](includes/server.md)] and Dynamics NAV Development Environment (CSIDE). To generate the symbols, open a command prompt, change to the directory where the file is store, and the run the following command:

        ```
        finsql.exe Command=generatesymbolreference, Database="<Database Name>", ServerName=<SQL Server Name\<Server Instance>
        ```
    For example:

        ```
        finsql.exe Command=generatesymbolreference, Database="Demo Database BC", ServerName=MySQLServer\BCDEMO
        ```

    For more information, see [Running C/SIDE and AL Side-by-Side](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-running-cside-and-al-side-by-side).

    2. Configure [!INCLUDE[nav_server_md](includes/nav_server_md.md)] instance to **Enable loading application symbol references at server startup** (EnableSymbolLoadingAtServerStartup). For more information, see [Configuring Business Central Server](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-server-instance#development-settings).

## <a name="to-disable-personalization-for-a-profile"></a>To disable personalisation for a profile

You can prevent all users that belong to a specific profile from being able to personalise their pages.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles**, and then choose the related link.
2. Select the profile in the list that you want to modify.
3. Select the **Disable personalisation** cheque box, and then choose the **OK** button.

> [!NOTE]  
> In Business Central online, you can only disable personalisation for a tenant profile, not for system profiles. 

## <a name="to-clear-user-personalizations"></a>To clear user personalisations

Clearing page personalisation changes the page back to its original layout before any personalisation was made. There are two ways to clear the personalisations that users have made to pages: using the **Delete User Personalisation** page and using the **User Personalisation Card** page.

### <a name="to-clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>To clear user personalisations by using the Delete User Personalisation page

The **Delete User Personalisation** page enables you to clear personalisations on a per-page basis for each user individually.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete User Personalisation**, and then choose the related link.

    The page lists all the pages that have been personalised and the user it belongs to.

    >[!NOTE]
    > A check mark in the **Legacy Personalisation** columns indicates that the personalisation was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalisation different than it does now. Users who try to personalise these pages are locked from doing so unless they choose to unlock the page. For more information, see [Why a page is locked from personalising](ui-personalization-locked.md).

2. Select the entry that you want to delete, and then choose the **Delete** action.

    The user will see the changes the next time they sign-in.

### <a name="to-clear-user-personalizations-by-using-the-user-personalization-card-page"></a>To clear user personalisations by using the User Personalisation Card page

The **User Personalisation Card** page enables you to clear the personalisation on all pages for specific user. This requires write permission to Table 2000000072 **Profile**.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Personalisation**, and then choose the related link.

    The **User Personalisation** page lists all users who potentially have personalised pages. If you cannot find a user in the list, this means that they do not have any personalised pages.

2. Select the user from the list, and then choose the **Edit** action.

3. On the **Actions** tab, choose **Clear Personalised Pages**.

    The user will see the changes the next time they sign-in.

## <a name="see-also"></a>See Also
[Personalising Your Workspace](ui-personalization-user.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Changing Basic Settings](ui-change-basic-settings.md)  
[Changing Which Features are Displayed](ui-experiences.md)  
