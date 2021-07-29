---
title: Create Users According to Licences
description: Describes how to add users to Business Central online or on-premises based on licences.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: access, right, security
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: ba584f11b1ac52146a7539b8ac08cb9ed67bcdba
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6445308"
---
# <a name="create-users-according-to-licenses"></a>Create Users According to Licences

This article describes how administrators create users and define who can sign in to [!INCLUDE[prod_short](includes/prod_short.md)], and which permissions are given to different user types according to the licences.

When you create users in [!INCLUDE[prod_short](includes/prod_short.md)] you can assign specific permissions to them through permission sets and organise users in user groups. User groups make it easier to manage permissions for multiple users at the same time. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).  

For more information about the different types of licences and how licensing works in [!INCLUDE[prod_short](includes/prod_short.md)], [download the Dynamics 365 Licensing Guide](https://go.microsoft.com/fwlink/?LinkId=866544).

> [!NOTE]
> The process of managing users and licences varies depending on whether [!INCLUDE[prod_short](includes/prod_short.md)] is deployed online or on-premises. For [!INCLUDE [prod_short](includes/prod_short.md)] online, you must add users from Microsoft 365. In on-premises deployments, you can create, edit, and delete users directly.  

## <a name="managing-users-and-licenses-in-online-deployments"></a>Managing Users and Licences in Online Deployments

In the online version of [!INCLUDE[prod_short](includes/prod_short.md)], the number of users is defined by the subscription and added to your tenant in the Microsoft Partner Centre, typically by your Microsoft partner. For more information, see [Add a new customer](/partner-center/add-a-new-customer) and [Create, suspend, or cancel customer subscriptions](/partner-center/create-a-new-subscription) in the Microsoft Partner Centre help.

To define who can sign in to [!INCLUDE[prod_short](includes/prod_short.md)], you must assign product licences to users according to the roles that they will perform in [!INCLUDE[prod_short](includes/prod_short.md)]. This can be done in the following ways:

- Your company's Microsoft 365 administrator can do it in the [Microsoft 365 Admin Centre](https://admin.microsoft.com). For more information, see [Add users individually or in bulk to Microsoft 365](/microsoft-365/admin/add-users/add-users).  
- A Microsoft partner can assign licences in the Microsoft 365 Admin Centre or in the Microsoft Partner Centre. For more information, see [User management tasks for customer accounts](/partner-center/assign-licenses-to-users) in the Microsoft Partner Centre Help.

For more information, see [Administration of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-administration) in the administration Help.

### <a name="to-add-users-or-update-user-information-and-license-assignments-in-business-central"></a><a name="adduser"></a>To add users or update user information and licence assignments in Business Central
After you add users or change user information in the Microsoft 365 Admin Centre, you can quickly import the user information to [!INCLUDE[prod_short](includes/prod_short.md)]. This includes licence assignments. 

1. Sign in to [!INCLUDE[prod_short](includes/prod_short.md)] using an administrator account.
2. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.  
3. Choose **Update Users from Microsoft 365**.

If you are adding new users, the next step is to assign user groups and permissions. For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md). If you are updating user information, and the update includes a licence change, the users will be assigned to the appropriate user group and their permission sets will be updated. For more information, see [To manage permissions through user groups](ui-define-granular-permissions.md).  

> [!NOTE]
> All users must be assigned to the same licence, either Essential or Premium. For more information, see the Microsoft Dynamics 365 Business Central Licensing Guide. The guide is available for download on the [Business Central](https://dynamics.microsoft.com/business-central/overview/) website.

For more information about Synchronising user information with Microsoft 365, see the [synchronisation with Microsoft 365](#m365) section.

> [!NOTE]
> If you use an external accountant to manage your books and financial reporting, you can invite them to your Business Central so they can work with you on your financial data. For more information, see [Inviting Your External Accountant to Your Business Central](finance-accounting.md#inviteaccountant).

### <a name="to-remove-a-users-access-to-the-system"></a>To remove a user's access to the system

In online deployments, you can remove a user's access to [!INCLUDE[prod_short](includes/prod_short.md)]. All references to the user are kept, but the user cannot sign in and active sessions for the user are stopped.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Open the **User Card** page for the relevant user, and then, in the **Status** field, select **Disabled**.
3. To give the user access again, set the **Status** field to **Enabled**.

You can also remove the licence from a user in the Microsoft 365 Admin Centre. The user is then unable to sign in. For more information, see [Remove licences from users](/microsoft-365/admin/manage/remove-licenses-from-users).

### <a name="synchronization-with-microsoft-365"></a><a name="m365"></a>Synchronisation with Microsoft 365

When you assign a licence for [!INCLUDE[prod_short](includes/prod_short.md)] to a user in Microsoft 365, there are two ways to create the user in [!INCLUDE[prod_short](includes/prod_short.md)].  

- The administrator can add the user by choosing the **Update Users from Microsoft 365** action on the **Users** page as described in the [To add a user or update user information in Business Central](#adduser) section.
- The licence information will update automatically when the user signs in for the first time.

In both cases, a number of settings are made automatically. These are listed in the second and third columns in the table below.

If you change user information in Microsoft 365 you can update [!INCLUDE[prod_short](includes/prod_short.md)] to reflect the change. Depending on what you want to update, use one of the actions on the **Users** page. The actions are described in the last three columns in the table below.

> [!NOTE]
> The actions described in the following table are accurate, however, the only one that you need is **Update Users from Microsoft 365**, which was added to simplify the process. The other actions will be removed in a future version of [!INCLUDE[prod_short](includes/prod_short.md)].

|What happens when:|First user, first sign-in|Get Users from Microsoft 365|Update Users from Microsoft 365|Restore User Default User Groups|Refresh User Groups|Update user information from Microsoft 365|
|-|-|-|-|-|-|-|
|Scope:|Current user|New users in Microsoft 365|Multiple selected users|Single selected user (except current)|Multiple selected users|Multiple selected users|
|Create the new user and assign SUPER permission set.<br /><br /><!--Platform-->|**X**||**X** | | | |
|Update the user based on information in Microsoft 365: Status, Full Name, Contact Email, Authentication Email.<!--<br /><br />Codeunit "Azure AD   Graph User".UpdateUserFromAzureGraph-->|**X**|**X**|**X**|**X**||**X**|
|Synchronise user plans (licences) with licences and roles assigned in Microsoft 365.<!--<br /><br />Codeunit "Azure AD   Graph User".UpdateUserPlans-->|**X**|**X**|**X**|**X**|**X**| |
|Add the user to user groups according to the current user plans. Remove the SUPER permission set for all users other than the first user to sign in and [administrators](/dynamics365/business-central/dev-itpro/administration/tenant-administration). At least one SUPER is required.<!--<br /><br />Codeunit "Permission Manager". AddUserToDefaultUserGroups-->|**X**|**X**|**X**|**X**<br /><br />Removes manually assigned user groups and permissions.|**X**<br /><br />Update user group assignments.| |

## <a name="the-device-license"></a>The Device Licence

The Dynamics 365 Business Central Device licence allows multiple users to simultaneously use a device that is covered by the licence. For example, this might be a point of sales, shop floor, or warehouse device. When you have purchased a number of device licences, up to that number of users assigned to the Dynamics 365 Business Central Device Users group can sign in at the same time. For more information, see the Microsoft Dynamics 365 Business Central Licensing Guide. The guide is available for download on the [Business Central](https://dynamics.microsoft.com/business-central/overview/) website.

Your company's Microsoft 365 administrator or Microsoft partner can create the Dynamics 365 Business Central Device Users group and add device users as members in the [Microsoft 365 Admin Centre](https://admin.microsoft.com/) or on the [Azure Portal](https://portal.azure.com/).

### <a name="device-user-limitations"></a>Device User Limitations

Users with the Device licence cannot perform the following tasks in [!INCLUDE[prod_short](includes/prod_short.md)]:

- Set up jobs to run as scheduled tasks in the job queue. Device users are concurrent users and, therefore, we cannot ensure that the involved user is present in the system when a task is executed, which is required.

- A device user cannot be the first user to sign in. A user of type Administrator, Full User, or External Accountant must be the first to sign in so they can set up [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Administration of Business Central Online](/dynamics365/business-central/dev-itpro/administration/tenant-administration) in the administration Help.

### <a name="to-create-a-dynamics-365-business-central-device-users-group"></a>To create a Dynamics 365 Business Central Device Users group

1. In the Microsoft 365 Admin Centre, go to the **Groups** page.
2. Choose the **Add a group** action.
3. On the **Choose a group type** page, choose the **Security** option, and then choose the **Add** action.
4. On the **Basics** page, enter **Dynamics 365 Business Central Device Users** as the name of the group.
  
   >[!NOTE]
   >The name of the group must be spelled in English exactly as shown in step 4, even if you are using another language. If you have copied the name of the group from a document, such as a PDF, verify that the name does not contain extra spaces.
5. Choose the **Close** button.

> [!NOTE]
> You can also create a group of type Microsoft 365. For more information, see [Compare Groups](/microsoft-365/admin/create-groups/compare-groups)

### <a name="to-add-members-to-the-group"></a>To add members to the group

1. In the Microsoft 365 Admin Centre, refresh the **Groups** page so your new group appears.
2. Select the **Dynamics 365 Business Central Device Users** group, and then choose the **View all and manage members** action.
3. Choose the **Add members** action.
4. Select the users that you want to add, and then choose the **Save** button.
5. Choose the **Close** button three times.

You can add as many users to the Dynamics 365 Business Central Device Users group as you need. However, the number of devices that users can sign in to simultaneously is defined by the number of purchased device licences.

> [!NOTE]
> You do not need to assign a [!INCLUDE[prod_short](includes/prod_short.md)] licence to users that are members of the Dynamics 365 Business Central Device Users group.

## <a name="managing-users-and-licenses-in-on-premises-deployments"></a>Managing Users and Licences in On-premises Deployments

For on-premises deployments, the number of user licences is specified in the licence file (.flf). When an administrator or Microsoft partner uploads the licence file, the administrator can specify which users can sign in to [!INCLUDE[prod_short](includes/prod_short.md)].

For on-premises deployments, the administrator creates, edits, and deletes users directly from the **Users** page.

### <a name="to-edit-or-delete-a-user-in-an-on-premises-deployment"></a>To edit or delete a user in an on-premises deployment

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Users**, and then choose the related link.
2. Select the user that you want to edit, and then choose the **Edit** action.
3. On the **User Card** page, change the information as necessary.  
4. To delete a user, select the user that you want to delete, and then choose the **Delete** action.

> [!NOTE]
> For on-premises deployments an administrator can specify how to authenticate user credentials in the [!INCLUDE[server](includes/server.md)] instance. When you create a user, you provide the credential type that you are using.
>
> For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the administration Help for [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="see-also"></a>See Also

[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  
[Manage Profiles](admin-users-profiles-roles.md)  
[Change Which Features are Displayed](ui-experiences.md)  
[Customising [!INCLUDE[prod_short](includes/prod_short.md)]](ui-customizing-overview.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Administration](admin-setup-and-administration.md)  
[Add Users to Microsoft 365 for business](/microsoft-365/admin/add-users/add-users)  
[Security and Protection in Business Central (administration content)](/dynamics365/business-central/dev-itpro/security/security-and-protection)  


[!INCLUDE[footer-include](includes/footer-banner.md)]