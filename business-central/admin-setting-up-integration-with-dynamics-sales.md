---
title: Setting Up User Accounts for Integrating with Dynamics 365 Sales | Microsoft Docs
description: Learn how to set up the user accounts that the apps use to exchange data, and that people use to access and synchronise data in the apps.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 64dd9d1e4645b845c02872a8bc09f0925f4fa33c
ms.sourcegitcommit: 3d128a00358668b3fdd105ebf4604ca4e2b6743c
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/20/2019
ms.locfileid: "2910571"
---
# <a name="setting-up-user-accounts-for-integrating-with-dynamics-365-sales"></a>Setting Up User Accounts for Integrating with Dynamics 365 Sales
This article provides an overview of how to set up the user accounts that are required to integrate [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)].  

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2085500]

## <a name="setting-up-the-administrator-user-account-in-sales"></a>Setting Up the Administrator User Account in Sales
You must add your administrator user account for [!INCLUDE[d365fin](includes/d365fin_md.md)] as a user in [!INCLUDE[crm_md](includes/crm_md.md)], and then promote the user to administrator in [!INCLUDE[crm_md](includes/crm_md.md)]. The administrator user account must also have the System Customizer role and at least one other non-administrative user role, such as Sales Manager, in [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="setting-up-the-user-account-for-the-integration"></a>Setting Up the User Account for the Integration
You must create a dedicated user account in your Office 365 subscription that both [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] can use to synchronise data. This user account must be able to sign in to [!INCLUDE[crm_md](includes/crm_md.md)], which means this user must have a licence for [!INCLUDE[crm_md](includes/crm_md.md)] and at least one security role assigned to it in [!INCLUDE[crm_md](includes/crm_md.md)] as described [here](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#create-a-user-account). For more information about how to create users in [!INCLUDE[crm_md](includes/crm_md.md)], see [Manage security, users, and teams](https://go.microsoft.com/fwlink/?LinkID=616518). After the connection is set up, [!INCLUDE[d365fin](includes/d365fin_md.md)] will assign the user account the security roles that it needs in [!INCLUDE[d365fin](includes/d365fin_md.md)] and this account can be set to [non-interactive access mode](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#create-a-non-interactive-user-account) in [!INCLUDE[crm_md](includes/crm_md.md)]

![Assisted setup guide showing place to enter synchronisation user credentials](media/sync-user-setup.png "Visualisation assisted setup wizard page showing place to enter synchronisation user credentials")

> [!IMPORTANT]  
> Do not use the administrator account for [!INCLUDE[crm_md](includes/crm_md.md)] for synchronisation. Doing so will break the synchronisation.
> Also, to avoid constant synchronisation, changes to data that are made by the integration user account are not synchronised. <!--What changes would this account make?--> After the connection is made, we recommend setting the access mode for the user account for integration to non-interactive mode in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information, see [Create a non-interactive user account](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#create-a-non-interactive-user-account).

## <a name="setting-up-accounts-for-salespeople"></a>Setting Up Accounts for Salespeople
You must create user accounts in [!INCLUDE[crm_md](includes/crm_md.md)] for the salespeople from [!INCLUDE[d365fin](includes/d365fin_md.md)]. To make that easier, the Microsoft 365 admin centre offers an Excel template that you can use. On the **Active users** page, choose **More**, and then **Import multiple users**. Choose **Download a CSV file with headers only**, and then enter the information for the salespersons. To see an example, choose **Download a CSV file with headers and sample user information**. After you enter the information about the users, the next step in the import process is to assign the users licences to the Dynamics 365 Customer Engagement Plan.  

After you import the users, and assign them licences for Dynamics 365 Customer Engagement, you must assign the users to the **Salesperson** role in [!INCLUDE[crm_md](includes/crm_md.md)].

![Coupling sales people to users in Dynamics 365 Sales](media/couple-salespeople.png "Visualization of coupling of sales people to users in Dynamics 365 Sales")

## <a name="minimum-permissions-for-user-accounts-in-crm_md"></a>Minimum Permissions for User Accounts in [!INCLUDE[crm_md](includes/crm_md.md)]
When you install the Integration Solution, permissions for the integration user account are configured in [!INCLUDE[crm_md](includes/crm_md.md)]. If those permissions are changed you might need to reset them. You can do that by reinstalling the Integration Solution or by manually resetting them. The following tables list the minimum permissions for the user accounts in [!INCLUDE[crm_md](includes/crm_md.md)].

### <a name="integration-administrator"></a>Integration Administrator
The following table displays the minimum permissions on each tab for each security role that is required for the administrator user.

##### <a name="customization"></a>Customisation
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Model Driven App|Global|||Read|
|Plugin Assembly|Global|Read|Read|Read|
|Plugin Type|Global|Read|Read|Read|
|Relationship|Global|||Read|
|SDK Message|Global|Read|Read|Read|
|SDK Message Proessing Step|Global|Read|Read|Read|
|SDK Message Proessing Step Image|Global|Read|Read|Read|
|System From|Global|||Write|

##### <a name="custom-entities"></a>Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Business Central Account Statistics|Global|Read|Read|Read|
|Business Central Connection|Global|Create, Read, Write, Delete|Create, Read, Write, Delete|Create, Read, Write, Delete|
|Post Configuration|Global|||Write|

#### <a name="integration-user"></a>Integration User
The following table displays the minimum permissions on each tab for each security role that is required for the integration user.

##### <a name="core-records"></a>Core Records
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Account|Global|Create, Read, Write, Append, Append To, Assign|Create, Read, Write, Append, Append To, Assign|Create, Read, Write, Append, Append To, Assign|
|Action Card|Global||Read|Read|
|Connection|Global|Read|Read|Read|
|Contact|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Note|Global|||Create, Read, Write, Delete Append, Assign|
|Opportunity|Global||Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Post|Global|||Create, Read, Append To|
|User Entity UI|User|Create, Read, Write|Create, Read, Write|Create, Read, Write|

##### <a name="sales"></a>Sales
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Invoice|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Order|Global|Read, Write, Append To|Read, Write, Append To|Read, Write, Append, Append To, Assign|
|Product|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Property|Global|Read|Read|Read|
|Property Association|Global|Read|Read|Read|
|Property Option Set Item|Global|Read|Read|Read|
|Quote|Global|Read|Read|Read|

##### <a name="service"></a>Service
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Case|Global|Read|Read|Read|

##### <a name="business-management"></a>Business Management
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Currency|Global|Create, Read, Write|Create, Read, Write|Create, Read, Write|
|Organisation|Global|Read, Write|Read, Write|Read, Write|
|Security Role|Global|||Read|
|User|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|User Settings|Global|Create, Read, Write, Delete, Append To|Create, Read, Write, Delete, Append To|Create, Read, Write, Delete, Append To|
|Act on Behalf of Another User|Global|Yes|Yes|Yes|

##### <a name="customization"></a>Customisation
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Field|Global||Read|Read|
|Plug-in Assembly|Global|Read|Read|Read|
|Plug-in Type|Global|Read|Read|Read|
|SDK Message|Global|Read|Read|Read|
|SDK Message Processing Step|Global|Read|Read|Read|
|Web Resource|Global|Read|Read|Read|

##### <a name="custom-entities"></a>Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Dynamics 365 Business Central Account Statistics|Global|Create, Read, Write, Append To|Create, Read, Write, Append To|Create, Read, Write, Append To|
|Dynamics 365 Business Central Connection|Global|Read|Read|Read|

### <a name="product-availability-user"></a>Product Availability User
You can allow sales people to view inventory levels for the items they sell by granting them the permissions described in the following table.

##### <a name="custom-entities"></a>Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Dynamics 365 Business Central Account Statistics|Global|Create, Read, Write, Append To|Create, Read, Write, Append To|Create, Read, Write, Append To|
|Dynamics 365 Business Central Connection|Global|Read|Read|Read|

## <a name="see-also"></a>See Also  
[Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
