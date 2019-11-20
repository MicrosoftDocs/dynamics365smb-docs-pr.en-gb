---
title: Assign or Edit User Permissions  | Microsoft Docs
description: Describes how to add Office 365 users to Business Central, and then assign permissions, access rights, and security settings.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: access, right, security
ms.date: 11/07/2019
ms.author: sgroespe
ms.openlocfilehash: c64a14ed66668f8c3cbe09e8db3430a7dc25db5c
ms.sourcegitcommit: 2a6d629cf290645606356b714a77ef2872bdec64
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 11/07/2019
ms.locfileid: "2774826"
---
# <a name="create-users-according-to-licenses"></a>Create Users According to Licences
The following describes how you as an administrator create users and define who can sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)], and which fundamental rights different user types have according to the licences.

When users are created in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can proceed to assign specific permissions to users through permission sets and to organise users in user groups for easy permission management. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).  

> [!NOTE]
> The process of managing users and licences varies depending on whether your solution is deployed online or on-premises. For example, in online deployments, you can only disable and enable a user once added to [!INCLUDE[d365fin](includes/d365fin_md.md)]. In on-premises deployments, you can create, edit, and delete users.  

## <a name="managing-users-and-licenses-in-online-deployments"></a>Managing Users and Licences in Online Deployments
In [!INCLUDE[d365fin](includes/d365fin_md.md)] online, the number of users is defined by the subscription and added to your tenant in the Microsoft Partner Centre, typically by your Microsoft partner. For more information, see [Add a new customer](https://docs.microsoft.com/partner-center/add-a-new-customer) and [Create, suspend, or cancel customer subscriptions](https://docs.microsoft.com/partner-center/create-a-new-subscription) in the Microsoft Partner Centre help.

To define who can sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)], the product licences must be assigned to users according to the roles that they will perform in [!INCLUDE[d365fin](includes/d365fin_md.md)]. This can be done in the following ways:
- Your company's Office 365 administrator can do it in the [Microsoft 365 Admin Centre](https://admin.microsoft.com). For more information, see [Add users individually or in bulk to Office 365](https://aka.ms/CreateOffice365Users).  
- A Microsoft partner can assign licences in the Microsoft 365 Admin Centre or in the Microsoft Partner Centre. For more information, see [User management tasks for customer accounts](https://docs.microsoft.com/partner-center/assign-licenses-to-users) in the Microsoft Partner Centre help.

For more information, see [Administration of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-administration) in the Developer and ITPro help.

When users with a [!INCLUDE[d365fin](includes/d365fin_md.md)] licence are created in Office 365, they can be imported into the **Users** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Get Users from Office 365** action.

### <a name="to-add-a-user-in-business-central"></a>To add a user in Business Central
To add users from the Microsoft 365 Admin Centre to [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you use a dedicated import function.  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Choose the **Get Users from Office 365** action.

Any new user that has been created for your Office 365 subscription will be added on the **Users** page. Users are assigned permission sets according to the licence assigned to the user in Office 365. You can then proceed to assign more detailed permissions to users and to organise them in user groups for easy permission management. For more information, see [To assign permission sets to users](ui-define-granular-permissions.md#to-assign-permission-sets-to-users).

### <a name="to-remove-a-users-access-to-the-system"></a>To remove a user's access to the system
In online deployments, you can remove a user's access to the system by setting the **State** field to **Disabled**. All references to the user will be retained, but the user can no longer sign in to the system and active sessions for the user will be terminated.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Open the **User Card** page for the relevant user, and then, in the **State** field, select **Disabled**.
3. To give the user access again, set the **State** field to **Enabled**.

In addition to disabling a user, you can unassign the licence from a user in the Office 365 Admin Centre. The user is then unable to sign in. For more information, see [Unassign licences from users](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users).

### <a name="to-change-the-assigned-license-for-a-user"></a>To change the assigned licence for a user
Sometimes you may need to change the licence that is assigned to a user. For example, if you decide to use the Service Management module and therefore need to upgrade all Essential licences to Premium. Or if a user’s responsibility has changed and you need to replace a Team Member licence to Essential.

1. Change the licence in the Office 365 Admin Centre. For more information, see [Add users individually or in bulk to Office 365](https://aka.ms/CreateOffice365Users).
2. Sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)] as an administrator.
3. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
4. On the **Users** page, choose the **Refresh all User Groups** action.
The users will be moved to a proper user group and the permission sets will be updated. For more information, see [To manage permissions through user groups](ui-define-granular-permissions.md#to-manage-permissions-through-user-groups).

> [!NOTE]
> All regular users in a solution must be assigned the same licence, Essential or Premium.
> For information about licensing, see [Microsoft Dynamics 365 Business Central Licensing Guide](https://aka.ms/BusinessCentralLicensing).

## <a name="managing-users-and-licenses-in-online-deployments"></a>Managing Users and Licences in Online Deployments
For on-premises deployments, a number of licensed users is specified in the licence file (.flf). When the administrator or Microsoft partner uploads the licence file, the administrator can specify which users can sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)].

For on-premises deployments, the administrator creates, edits, and deletes users directly from the **Users** page.

### <a name="to-edit-or-delete-a-user-on-premises"></a>To edit or delete a user on-premises
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Select the user that you want to edit, and then choose the **Edit** action.
3. On the **User Card** page, change the information as necessary.    
4. To delete a user, select the user that you want to delete, and then choose the **delete** action.

> [!NOTE]
> For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorisation mechanisms for users. Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.<br /><br />
> For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="see-also"></a>See Also
[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  
[Manage Profiles](admin-users-profiles-roles.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Administration](admin-setup-and-administration.md)  
[Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users)  
[Microsoft Dynamics 365 Business Central Licensing Guide](https://aka.ms/BusinessCentralLicensing)  
[Security and Protection in Business Central](/dynamics365/business-central/dev-itpro/security/security-and-protection) in Developer and IT-pro Help
