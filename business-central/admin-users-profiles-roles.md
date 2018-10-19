---
title: Manage users and roles | Microsoft Docs
description: Learn how to manage users and Role Centres in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, users
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 1a94d023424c6eceb93af6e9ca89a90a3a94e996
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="understanding-users-profiles-and-role-centers"></a>Understanding Users, Profiles, and Role Centres

In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.  

Access to functionality is managed through *user groups* and *profiles*. As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.  

## <a name="adding-users"></a>Adding Users

To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Centre. For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).

Then, the administrator can assign permissions to each user and groups of users. For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).  

### <a name="users-of-on-premises-deployments"></a>Users of on-premises deployments

For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorisation mechanisms for users. Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance. For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="profiles"></a>Profiles

The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Centre*.

Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center. A Role Centre is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.  

> [!NOTE]  
>  In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.  

## <a name="configuration-and-personalization"></a>Configuration and Personalisation
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->
Users personalise the user interface of their personal version by customising the user interface under their own user logon. This personalisation can be deleted by the administrator. For more information, see [Personalising Your Workspace](ui-personalization-user.md).  

## <a name="see-also"></a>See Also  
[Managing Users and Permissions](ui-how-users-permissions.md)  
[Managing Personalisation as an Administrator](ui-personalization-manage.md)  
[Personalising Your Workspace](ui-personalization-user.md)  

