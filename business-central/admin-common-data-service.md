---
title: Using Common Data Service
description: Introduction to Common Data Service and its components.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 10/01/2019
ms.openlocfilehash: bb21647b4cd07d4d4e2d37ae597551d9ca50d210
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196905"
---
# <a name="integrating-with-common-data-service"></a>Integrating with Common Data Service
Business apps often use data from more than one source. [!INCLUDE[d365fin](includes/cds_long_md.md)] combines data into a single set of logic that makes it easier to connect other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)] or your own application built on top of [!INCLUDE[d365fin](includes/cds_long_md.md)], to [!INCLUDE[d365fin_md](includes/d365fin_md.md)]. For more information about [!INCLUDE[d365fin](includes/cds_long_md.md)], see [What is Common Data Service?](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro)

The following steps provide an overview of the steps to integrate [!INCLUDE[d365fin](includes/cds_long_md.md)] with [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!Note]  
> These tasks require the **System Administrator** security role in [!INCLUDE[d365fin](includes/cds_long_md.md)] and [!INCLUDE[d365fin](includes/d365fin_md.md)].  

1. In the Microsoft 365 admin centre, set up a user account for connecting to and synchronising data with [!INCLUDE[d365fin](includes/cds_long_md.md)]. For more information, see [Setting Up User Accounts for Integrating with Common Data Service](admin-setting-up-integration-with-dynamics-sales.md).

2. Assign licences for [!INCLUDE[d365fin](includes/cds_long_md.md)] to the [!INCLUDE[d365fin](includes/d365fin_md.md)] users who will use the integrated apps.

3. Set up a connection to [!INCLUDE[d365fin](includes/cds_long_md.md)]. For more information, see [Connect to Common Data Service](admin-how-to-set-up-a-dynamics-crm-connection.md).  

4. Synchronise data between the apps. For more information, see [Synchronising Business Central and Common Data Service](admin-synchronizing-business-central-and-sales.md). 

## <a name="getting-started-with-d365fin"></a>Getting Started with [!INCLUDE[d365fin](includes/cds_long_md.md)]
To get started with [!INCLUDE[d365fin](includes/cds_long_md.md)] you will need a Microsoft Power Apps account. If you do not already have a Power Apps account, you can get one for free by visiting [powerapps.com](https://web.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) and choosing the **Get started free** link. To learn more about how to get started with [!INCLUDE[d365fin](includes/cds_long_md.md)], see the [Integrating with Common Data Service](https://docs.microsoft.com/learn/modules/get-started-with-powerapps-common-data-service/) module from Microsft Learn.

## <a name="bi-directional-or-uni-directional-data-synchronization"></a>Bi-Directional or Uni-directional Data Synchronisation
Depending on your business needs, you can set up the integration to synchronise data either to or from one Dynamics 365 business app to another, or in both directions in near-real time through [!INCLUDE[d365fin](includes/cds_long_md.md)]. For example, if you integrate [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[crm_md](includes/crm_md.md)] through [!INCLUDE[d365fin](includes/cds_long_md.md)], a salesperson can create a sales order in [!INCLUDE[crm_md](includes/crm_md.md)] and the order will be synchronised to [!INCLUDE[d365fin](includes/d365fin_md.md)]. Conversely, from [!INCLUDE[crm_md](includes/crm_md.md)], the salesperson can view information from [!INCLUDE[d365fin](includes/d365fin_md.md)] about the availability of the item on the order. 

## <a name="standard-and-custom-entities"></a>Standard and Custom Entities
[!INCLUDE[d365fin](includes/cds_long_md.md)] securely stores data in a set of entities, which are sets of records similar to how a table stores data within a database. [!INCLUDE[d365fin](includes/cds_long_md.md)] includes a base set of standard entities that cover typical scenarios, but you can also create custom entities specific to your organisation. In [!INCLUDE[d365fin](includes/d365fin_md.md)], you can view standard and custom entities being synchronised on the Integration Table Mappings page.

## <a name="about-the-base-cds-integration-solution"></a>About the Base CDS Integration Solution
The Base CDS Integration Solution is a key component of the integration. The solution adds the required roles and access levels to the user accounts for the integration, and it creates entities needed to map [!INCLUDE[d365fin](includes/d365fin_md.md)] company to business unit in [!INCLUDE[d365fin](includes/cds_long_md.md)]. 

By default, the **Set up [!INCLUDE[d365fin](includes/cds_long_md.md)] connection** assisted setup guide will import the solution. To do that, the setup guide uses an administrator user account that you specify. This account must be a valid user in [!INCLUDE[d365fin](includes/cds_long_md.md)] with the following security roles:

* System Administrator  
* Solution Customizer  

For more information, see [Setting Up User Accounts for Integrating with [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) and [Create users in Microsoft Dynamics 365 (online) and assign security roles](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles.md). 

The administrator account is used only one time during the setup due to configuration changes Base CDS Solution is making in [!INCLUDE[d365fin](includes/cds_long_md.md)]. After the solution is imported the account is no longer needed. Integration will continue to use the user account that was created specifically for the integration.

In addition to customising [!INCLUDE[d365fin](includes/cds_long_md.md)], the solution also creates the following roles in [!INCLUDE[d365fin](includes/cds_long_md.md)] for the integration:

* **Integration Administrator** - Allows users to manage the connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[d365fin](includes/cds_long_md.md)]. Typically, this is assigned only to the user account for synchronisation.  
* **Integration User** - Allows users to access synchronised data. Typically, this is assigned to the user account for synchronisation and other users who need to view or access the synchronised data.

For details about each role, such as the permissions and access levels, see [Setting Up User Accounts for Integrating with [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).

During connection setup, integration table mappings that are needed to synchronise data, are created. Entities in Common Data Service are mapped to tables and table fields in Business Central through integration tables. For more information, see [Standard Entity Mapping for Synchronisation](admin-synchronizing-business-central-and-sales.md#standard-entity-mapping-for-synchronization).

## <a name="see-also"></a>See Also
[Data Ownership Models](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Common Data Service](docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-custom-cds-integration) -->



