---
title: Setting Up User Accounts for Integrating with Dynamics 365 for Sales | Microsoft Docs
description: Learn how to set up the user accounts that the apps use to exchange data, and that people use to access and synchronise data in the apps.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: c318346c62b7776a550a77a2947173e33d5f17c0
ms.sourcegitcommit: addfb47612cc2e4e98dfd7e338b6f41cde405d5c
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/16/2019
ms.locfileid: "940412"
---
# <a name="setting-up-user-accounts-for-integrating-with-dynamics-365-for-sales"></a>Setting Up User Accounts for Integrating with Dynamics 365 for Sales
This article provides an overview of how to set up the user accounts that are required to integrate [!INCLUDE[crm_md](includes/crm_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)].  

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2085500]

## <a name="setting-up-the-admininstrator-user-account-in-sales"></a>Setting Up the Admininstrator User Account in Sales
You must add your administrator user account for [!INCLUDE[d365fin](includes/d365fin_md.md)] as a user in [!INCLUDE[crm_md](includes/crm_md.md)], and then promote the user to administrator in [!INCLUDE[crm_md](includes/crm_md.md)]. The administrator user account must also have the System Customizer role and at least one other non-administrative user role, such as Sales Manager, in [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="setting-up-the-user-account-for-the-integration"></a>Setting Up the User Account for the Integration
You must create a dedicated user account in your Office 365 subscription that both [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] can use to synchronise data. This user account must be able to sign in to [!INCLUDE[crm_md](includes/crm_md.md)], which means this user must have a licence for [!INCLUDE[crm_md](includes/crm_md.md)]. This account must also be a non-interactive account in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information about how to create users in [!INCLUDE[crm_md](includes/crm_md.md)], see [Manage security, users, and teams](http://go.microsoft.com/fwlink/?LinkID=616518). After the connection is set up, [!INCLUDE[d365fin](includes/d365fin_md.md)] will assign the user account the security roles that it needs in [!INCLUDE[d365fin](includes/d365fin_md.md)].

![Assisted setup guide showing place to enter synchronisation user credentials](media/sync-user-setup.png "Visualisation assisted setup wizard page showing place to enter synchronisation user credentials")

> [!IMPORTANT]  
> Do not use the administrator account for [!INCLUDE[crm_md](includes/crm_md.md)] for synchronisation. Doing so will break the synchronisation.
> Also, to avoid constant synchronisation, changes to data that are made by the integration user account are not synchronised. <!--What changes would this account make?--> After the connection is made, we recommend setting the access mode for the user account for integration to non-interactive mode in [!INCLUDE[crm_md](includes/crm_md.md)]. For more information, see [Create a non-interactive user account](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#create-a-non-interactive-user-account).

## <a name="setting-up-accounts-for-sales-people"></a>Setting Up Accounts for Sales People
You must create user accounts in [!INCLUDE[crm_md](includes/crm_md.md)] for the salespeople from [!INCLUDE[d365fin](includes/d365fin_md.md)]. To make that easier, the Microsoft 365 admin centre offers an Excel template that you can use. On the **Active users** page, choose **More**, and then **Import multiple users**. Choose **Download a CSV file with headers only**, and then enter the information for the salespersons. To see an example, choose **Download a CSV file with headers and sample user information**. After you enter the information about the users, the next step in the import process is to assign the users licences to the Dynamics 365 Customer Engagement Plan.  

After you import the users, and assign them licences for Dynamics 365 Customer Engagement, you must assign the users to the **Salesperson** role in [!INCLUDE[crm_md](includes/crm_md.md)].

![Coupling sales people to users in Dynamics 365 for Sales](media/couple-salespeople.png "Visualization of coupling of sales people to users in Dynamics 365 for Sales")

## <a name="see-also"></a>See Also  
[Integrating with Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
