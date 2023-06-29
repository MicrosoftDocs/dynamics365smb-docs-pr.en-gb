---
title: Using Microsoft Dataverse
description: Introduction to how to integrate and use Microsoft Dataverse and its components to connect to other Dynamics 365 applications.
author: brentholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.topic: conceptual
ms.date: 06/14/2021
---

# <a name="integrating-with-microsoft-dataverse"></a><a name="integrating-with-microsoft-dataverse"></a>Integrating with Microsoft Dataverse

Business apps often use data from more than one source. [!INCLUDE[prod_short](includes/cds_long_md.md)] combines data into a single set of logic that makes it easier to connect other Dynamics 365 applications, such as [!INCLUDE[crm_md](includes/crm_md.md)] or your own application built on top of [!INCLUDE[prod_short](includes/cds_long_md.md)], to [!INCLUDE[prod_short_md](includes/prod_short.md)]. For more information about [!INCLUDE[prod_short](includes/cds_long_md.md)], see [What is Dataverse?](/powerapps/maker/common-data-service/data-platform-intro)

The following steps provide an overview of the steps to integrate [!INCLUDE[prod_short](includes/cds_long_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)].

> [!Note]  
> These tasks require the **System Administrator** security role in [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)].  

1. Assign licences for [!INCLUDE[prod_short](includes/cds_long_md.md)] to the [!INCLUDE[prod_short](includes/prod_short.md)] users who will use the integrated apps.

2. Set up a connection to [!INCLUDE[prod_short](includes/cds_long_md.md)]. For more information, see [Connect to Dataverse](admin-how-to-set-up-a-dynamics-crm-connection.md).  

3. Synchronise data between the apps. For more information, see [Synchronising Business Central and Dataverse](admin-synchronizing-business-central-and-sales.md). 

## <a name="getting-started-with-"></a><a name="getting-started-with-"></a>Getting Started with [!INCLUDE[prod_short](includes/cds_long_md.md)]

To get started with [!INCLUDE[prod_short](includes/cds_long_md.md)] you will need a Microsoft Power Apps account. If you do not already have a Power Apps account, you can get one for free by visiting [powerapps.com](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) and choosing the **Get started free** link. To learn more about how to get started with [!INCLUDE[prod_short](includes/cds_long_md.md)], see the [Get started with Dataverse](/training/modules/get-started-with-powerapps-common-data-service/) module from Microsoft training.

## <a name="bi-directional-or-uni-directional-data-synchronization"></a><a name="bi-directional-or-uni-directional-data-synchronization"></a>Bi-Directional or Uni-directional Data Synchronisation

Depending on your business needs, you can set up the integration to synchronise data either to or from one Dynamics 365 business app to another, or in both directions in near-real time through [!INCLUDE[prod_short](includes/cds_long_md.md)]. For example, if you integrate [!INCLUDE[prod_short](includes/prod_short.md)] with [!INCLUDE[crm_md](includes/crm_md.md)] through [!INCLUDE[prod_short](includes/cds_long_md.md)], a salesperson can create a sales order in [!INCLUDE[crm_md](includes/crm_md.md)] and the order will be synchronised to [!INCLUDE[prod_short](includes/prod_short.md)]. Conversely, from [!INCLUDE[crm_md](includes/crm_md.md)], the salesperson can view information from [!INCLUDE[prod_short](includes/prod_short.md)] about the availability of the item on the order. 

## <a name="standard-and-custom-entities"></a><a name="standard-and-custom-entities"></a>Standard and Custom Entities

[!INCLUDE[prod_short](includes/cds_long_md.md)] securely stores data in a set of tables, which are sets of records similar to how a table stores data within a database. [!INCLUDE[prod_short](includes/cds_long_md.md)] includes a base set of standard tables that cover typical scenarios, but you can also create custom tables specific to your organisation. In [!INCLUDE[prod_short](includes/prod_short.md)], you can view standard and custom tables being synchronised on the Integration Table Mappings page.

## <a name="about-the-business-central-base-integration-solution"></a><a name="about-the-business-central-base-integration-solution"></a>About the Business Central Base Integration Solution

The Base Integration Solution is a key component of the integration. The solution adds the required roles and access levels to the user accounts for the integration, and it creates tables needed to map [!INCLUDE[prod_short](includes/prod_short.md)] company to business unit in [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

By default, the **Set up [!INCLUDE[prod_short](includes/cds_long_md.md)] connection** assisted setup guide will import the solution. To do that, the setup guide uses an administrator user account that you specify. This account must be a valid user in [!INCLUDE[prod_short](includes/cds_long_md.md)] with the following security role:

* System Administrator  

For more information, see [Setting Up User Accounts for Integrating with [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) and [Create users in Microsoft Dynamics 365 (online) and assign security roles](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles). 

The administrator account is used only one time during the setup for the configuration changes that the Base Integration Solution makes in [!INCLUDE[prod_short](includes/cds_long_md.md)]. After the solution is imported the account is no longer needed. Integration will continue to use the user account that is automatically created specifically for the integration.

In addition to customising [!INCLUDE[prod_short](includes/cds_long_md.md)], the solution also creates the following roles in [!INCLUDE[prod_short](includes/cds_long_md.md)] for the integration:

* **Integration Administrator** - Allows users to manage the connection between [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)]. Typically, this is assigned only to the automatically created user account for synchronisation.  
* **Integration User** - Allows users to access synchronised data. Typically, this is assigned to the automatically created user account for synchronisation and other users who need to view or access the synchronised data.

For details about each role, such as the permissions and access levels, see [Setting Up User Accounts for Integrating with [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).

During connection setup, integration table mappings that are needed to synchronise data, are created. Entities in [!INCLUDE[prod_short](includes/cds_long_md.md)] are mapped to tables and table fields in Business Central through integration tables. For more information, see [Standard Entity Mapping for Synchronisation](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization).

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>See related [Microsoft training](/training/modules/use-model-driven-apps-common-data-service/)

## <a name="see-also"></a><a name="see-also"></a>See also

[Data Ownership Models](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Dataverse](\dynamics365\business-central\dev-itpro\administration\administration-custom-cds-integration) -->


[!INCLUDE[footer-include](includes/footer-banner.md)]
