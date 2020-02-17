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
ms.date: 01/06/2020
ms.author: sgroespe
ms.openlocfilehash: e07636b6211eb57205d41d982bfbfb4bc2d5b330
ms.sourcegitcommit: 0cb8a646dcba8f6d6336ebd008587874d25f4629
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/07/2020
ms.locfileid: "3030059"
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

When users with a [!INCLUDE[d365fin](includes/d365fin_md.md)] licence are created in Office 365, they can be imported into the **Users** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Get New Users from Office 365** action.

### <a name="to-add-a-user-in-business-central"></a>To add a user in Business Central
To add users from the Microsoft 365 Admin Centre to [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you use a dedicated import function.  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Choose the **Get New Users from Office 365** action.

Any new user that has been created for your Office 365 subscription will be added on the **Users** page. Users are assigned permission sets according to the licence assigned to the user in Office 365. You can then proceed to assign more detailed permissions to users and to organise them in user groups for easy permission management. For more information, see [To assign permission sets to users](ui-define-granular-permissions.md#to-assign-permission-sets-to-users).

> [!NOTE]
> If you use an external accountant to manage your books and financial reporting, you can invite them to your Business Central so they can work with you on your fiscal data. For more information, see [Inviting Your External Accountant to Your Business Central](finance-accounting.md#inviteaccountant)

### <a name="to-remove-a-users-access-to-the-system"></a>To remove a user's access to the system
In online deployments, you can remove a user's access to the system by setting the **State** field to **Disabled**. All references to the user will be retained, but the user can no longer sign in to the system and active sessions for the user will be terminated.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Open the **User Card** page for the relevant user, and then, in the **State** field, select **Disabled**.
3. To give the user access again, set the **State** field to **Enabled**.

In addition to disabling a user, you can unassign the licence from a user in the Microsoft 365 Admin Centre. The user is then unable to sign in. For more information, see [Unassign licences from users](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users).

### <a name="to-change-the-assigned-license-for-a-user"></a>To change the assigned licence for a user
Sometimes you may need to change the licence that is assigned to a user. For example, if you decide to use the Service Management module and therefore need to upgrade all Essential licences to Premium. Or if a user’s responsibility has changed and you need to replace a Team Member licence to Essential.

1. Change the licence in the Microsoft 365 Admin Centre. For more information, see [Add users individually or in bulk to Office 365](https://aka.ms/CreateOffice365Users).
2. Sign in to [!INCLUDE[d365fin](includes/d365fin_md.md)] as an administrator.
3. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
4. On the **Users** page, choose the **Restore User Default User Groups** action.

The users will be moved to a proper user group and the permission sets will be updated. For more information, see [To manage permissions through user groups](ui-define-granular-permissions.md#to-manage-permissions-through-user-groups).

> [!NOTE]
> All regular users in a solution must be assigned the same licence, Essential or Premium.
> For information about licensing, see [Microsoft Dynamics 365 Business Central Licensing Guide](https://aka.ms/BusinessCentralLicensing).

### <a name="synchronization-with-office-365"></a>Synchronisation with Office 365
When a licence is assigned to a user in Office 365, there are two ways to create the user in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The system will do it automatically when the user signs in for the first time, or the administrator can add the user by choosing the **Get Users from Office 365** action on the **Users** page.

In both cases, a number of additional settings are made automatically. These are listed in the second and third columns in the table below.

If you change the user in Office 365 afterwards, and you need to synchronise the changes to [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use different actions on the **Users** page depending on what exactly you want to synchronise. These are listed in the last three columns in the table below.

|What happens when:|First sign-in|Get Users from Office 365|Update Users from Office 365|Restore User Default User Groups|Refresh User Groups|
|-|-|-|-|-|-|
|Scope:|Current user|New users in Office 365|Multiple selected users|Single selected user (except current)|Multiple selected users|
|Create the new user and assign SUPER permission set.<br /><br />Platform|**X**|**X**| | | |
|Update the user record based on actual information in Office 365: County, Full Name, Contact Email, Authentication Email.<br /><br />Codeunit "Azure AD   Graph User".UpdateUserFromAzureGraph|**X**|**X**|**X**|**X**| |
|Synchronise user plans (licences) with licences and roles assigned in Office 365.<br /><br />Codeunit "Azure AD   Graph User".UpdateUserPlans|**X**|**X**| |**X**|**X**|
|Add the user to user groups according to the current user plans. Revoke SUPER permission set. (At least one SUPER is needed. Do not revoke from [administrators](/dynamics365/business-central/dev-itpro/administration/tenant-administration).)<br /><br />Codeunit "Permission Manager". AddUserToDefaultUserGroups|**X**|**X**| |**X**<br /><br />Overwrite: Remove the user from other groups. Remove manually assigned permission sets.|**X**<br /><br />Additive: Keep the current membership in  the user group and assigned permission sets intact. Only add user to groups if needed.|

## <a name="the-device-license"></a>The Device Licence
With the Dynamics 365 Business Central Device licence, multiple users can use a device that is licenced with the Device licence to operate a point of sale device, shop floor device, or warehouse device. For more information, see [Microsoft Dynamics 365 Business Central Licensing Guide](https://aka.ms/BusinessCentralLicensing).

The Device licence is implemented as a concurrent-user model. When you have purchased X number of device licences, up to X number of users from the designated group called Dynamics 365 Business Central Device Users can log in concurrently.

Your company's Office 365 administrator or Microsoft partner should create the designated device group and add device users as members of that group. They can do this in the [Microsoft 365 Admin Centre](https://admin.microsoft.com/) or on the [Azure Portal](https://portal.azure.com/).

### <a name="device-user-limitations"></a>Device User Limitations
Users with the Device licence cannot perform the following tasks in [!INCLUDE[d365fin](includes/d365fin_md.md)]:

-   Set up jobs to run as scheduled tasks in the job queue. Device users are concurrent users and, therefore, we cannot ensure that the involved user is present in the system when a task is executed, which is required.

-   A device user cannot be the first user to log in. A user of type Administrator, Full User, or External Accountant must be the first to log in so they can set [!INCLUDE[d365fin](includes/d365fin_md.md)] up. For more information, see [Administrators](/dynamics365/business-central/dev-itpro/administration/tenant-administration).

### <a name="to-create-a-dynamics-365-business-central-device-users-group"></a>To create a Dynamics 365 Business Central Device Users group
1.  In the Microsoft 365 Admin Centre, go to the **Groups** page.
2.  Choose the **Add a group** action.
3.  On the **Choose a group type** page, choose the **Security** action, and then choose the **Add** action.
4.  On the **Basics** page, type *Dynamics 365 Business Central Device Users* as the name of the group.

    > [!Note]
    > The name of the group must be spelled exactly as above, also in a non-English setup.
5. Choose the **Close** button.

> [!NOTE]
> You can also create a group of type Office 365. For more information, see [Compare Groups](https://docs.microsoft.com/office365/admin/create-groups/compare-groups)

### <a name="to-add-members-to-the-group"></a>To add members to the group
1.  In the Microsoft 365 Admin Centre, refresh the **Groups** page so your new group appears.
2.  Select the **Dynamics 365 Business Central Device Users** group, and then choose the **View all and manage members** action.
3.  Choose the **Add members** action.
4.  Select the users that you want to add, and then choose the **Save** button.
5.  Choose the **Close** button three times.

You can add as many users to the Dynamics 365 Business Central Device Users group as you need. The number of devices that users can log in to simultaneously is defined by the number of purchased device licences.

> [!NOTE]
> You do not need to assign a [!INCLUDE[d365fin](includes/d365fin_md.md)] licence to users that are members of the Dynamics 365 Business Central Device Users group.

## <a name="managing-users-and-licenses-in-on-premises-deployments"></a>Managing Users and Licences in On-premises Deployments
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
