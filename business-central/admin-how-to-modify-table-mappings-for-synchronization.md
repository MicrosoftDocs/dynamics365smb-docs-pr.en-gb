---
title: Mapping the Tables and Fields to Synchronise | Microsoft Docs
description: Learn how to map tables and fields for synchronising data between Business Central and Microsoft Dataverse.
author: bholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize, table mapping
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 844b053a307d88bd93d945a7927726fd28518000
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2022
ms.locfileid: "8147145"
---
# <a name="mapping-the-tables-and-fields-to-synchronize"></a>Mapping the Tables and Fields to Synchronise


The basis of synchronising data is mapping the tables and fields in [!INCLUDE[prod_short](includes/prod_short.md)] with tables and columns in [!INCLUDE[prod_short](includes/cds_long_md.md)], so they can exchange the data. Mapping happens through integration tables. 

## <a name="mapping-integration-tables"></a>Mapping Integration Tables
An integration table is a table in the [!INCLUDE[prod_short](includes/prod_short.md)] database that represents an table, such as an account, in [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Integration tables include fields that correspond to columns in the [!INCLUDE[cds_long_md](includes/cds_long_md.md)] table. For example, the Account integration table connects to the Accounts table in [!INCLUDE[cds_short_md](includes/cds_long_md.md)]. There must be a integration table mapping for each table in [!INCLUDE[cds_short_md](includes/cds_short_md.md)] that you want to synchronise with data in [!INCLUDE[prod_short](includes/prod_short.md)].

When you create the connection between the apps, [!INCLUDE[prod_short](includes/prod_short.md)] sets up some default mappings. You can change the table mappings if you want. For more information, see [Standard Table Mapping for Synchronisation](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization). If you have changed the default mappings and want to revert your changes, on the **Integration Table Mappings** page, choose **Use Default Synchronisation Setup**.

> [!Note]
> If you are using an on-premises version of [!INCLUDE[prod_short](includes/prod_short.md)], the integration table mappings are stored in table 5335 Integration Table Mappings, where you can view and edit the mappings. Complex mappings and synchronisation rules are defined in codeunit 5341. 

### <a name="synchronization-rules"></a>Synchronisation Rules
An integration table mapping also includes rules that control how integration synchronisation jobs synchronise records in a [!INCLUDE[prod_short](includes/prod_short.md)] table and an table in [!INCLUDE[prod_short](includes/cds_long_md.md)]. <!--For examples of rules for an integration with Sales, see [Synchronization Rules](admin-synchronizing-business-central-and-sales.md#synchronization-rules). need to verify link -->

### <a name="strategies-for-auto-resolving-conflicts"></a>Strategies for Auto-Resolving Conflicts
Data conflicts can easily occur when business applications exchange data on an ongoing basis. For example, someone might delete or change a row in one of the applications, or both. To reduce the number of conflicts that you will have to manually resolve, you can specify resolution strategies and [!INCLUDE[prod_short](includes/prod_short.md)] will automatically resolve conflicts according to the rules in the strategies.

Integration table mappings include rules that control how synchronisation jobs synchronise records. On the **Integration Table Mapping** page, in the **Resolve Deletion Conflicts** and **Resolve Update Conflicts** columns, you can specify how [!INCLUDE[prod_short](includes/prod_short.md)] will resolve conflicts that occur because records were deleted in tables in one or the other business application, or updated in both. 

In the **Resolve Deletion Conflicts** column, you can choose to have [!INCLUDE[prod_short](includes/prod_short.md)] automatically restore deleted records, remove the coupling between the records, or do nothing. If you do nothing, you must manually resolve conflicts. 

In the **Resolve Update Conflicts** column, you can choose to have [!INCLUDE[prod_short](includes/prod_short.md)] automatically send a data update to the integration table when sending data to [!INCLUDE[prod_short](includes/cds_long_md.md)], or to get a data update from the integration table when getting data from [!INCLUDE[prod_short](includes/cds_long_md.md)], or do nothing. If you do nothing, you must manually resolve conflicts.

After you specify the strategy, on the **Coupled Data synchronisation Errors** page, you can choose the **Retry All** action to automatically resolve conflicts. 

## <a name="mapping-integration-fields"></a>Mapping Integration Fields
Mapping tables is only the first step. You must also map the fields on the tables. Integration field mappings link fields in [!INCLUDE[prod_short](includes/prod_short.md)] tables with corresponding columns in [!INCLUDE[prod_short](includes/cds_long_md.md)], and determine whether to synchronise data in each table. The standard table mapping that [!INCLUDE[prod_short](includes/prod_short.md)] provides includes field mappings, but you can change those if you want. For more information, see [Viewing Table Mappings](admin-synchronizing-business-central-and-sales.md#tip-for-admins-viewing-table-mappings).

> [!Note]
> If you are using an on-premises version of [!INCLUDE[prod_short](includes/prod_short.md)], integration field mappings are defined in table 5336 Integration Field Mapping.

You can manually map the fields, or you can automate the process by mapping multiple fields at the same time based on criteria for matching their values. For more information, see [To couple multiple records based on field value matching](admin-how-to-couple-and-synchronize-records-manually.md).

### <a name="handling-differences-in-field-values"></a>Handling Differences in Field Values
Sometimes the values in the fields that you want to map are different. For example, in [!INCLUDE[crm_md](includes/crm_md.md)] the language code for the United States is "U.S.," but in [!INCLUDE[prod_short](includes/prod_short.md)] it's "US." That means you must transform the value when you synchronise data. This happens through transformation rules that you define for the fields. You define transformation rules on the **Integration Table Mappings** page by choosing **Mapping**, and then **Fields**. Predefined rules are provided, but you can also create your own. For more information, see [Transformation Rules](across-how-to-set-up-data-exchange-definitions.md#transformation-rules).

### <a name="handling-missing-option-values-in-mapping"></a>Handling Missing Option Values in Mapping
[!INCLUDE[prod_short](includes/cds_long_md.md)] contains option set columns that provide values that you can map to [!INCLUDE[prod_short](includes/prod_short.md)] fields of the type **Option** for automatic synchronisation. During synchronisation, non-mapped options are ignored and the missing options are appended to the related [!INCLUDE[prod_short](includes/prod_short.md)] table and added to the **CDS Option Mapping** system table to be handled manually later. For example, by adding the missing options in either product and then updating the mapping. For more information, see [Handling Missing Option Values](admin-cds-missing-option-values.md).

## <a name="coupling-records"></a>Coupling Records
Coupling links rows in [!INCLUDE[prod_short](includes/cds_long_md.md)] to records in [!INCLUDE[prod_short](includes/prod_short.md)]. For example, accounts in [!INCLUDE[prod_short](includes/cds_long_md.md)] are typically coupled with customers in [!INCLUDE[prod_short](includes/prod_short.md)]. Coupling records offers the following benefits:

* It makes synchronisation possible.
* Users can open records or rows in one business app from the other. This requires that the apps are already integrated.

Couplings can be set up automatically by using the synchronisation jobs, or manually by editing the record in [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Synchronising Data in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md) and [Couple and Synchronise Records Manually](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings).

## <a name="filtering-records-and-rows"></a>Filtering Records and Rows  
If you do not want to synchronise all rows for a specific table in [!INCLUDE[prod_short](includes/cds_long_md.md)] or table in [!INCLUDE[prod_short](includes/prod_short.md)], you can set up filters to limit the data that is synchronised. You set up filters on the **Integration Table Mappings** page.  

#### <a name="to-filter-records-or-rows-for-synchronization"></a>To filter records or rows for synchronisation  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings**, and then choose the related link.

2.  To filter the [!INCLUDE[prod_short](includes/prod_short.md)] records, set the **Table Filter** field.  

3.  To filter the [!INCLUDE[prod_short](includes/cds_long_md.md)] rows, set the **Integration Table Filter** field.  

## <a name="creating-new-records"></a>Creating New Records  
By default, only records in [!INCLUDE[prod_short](includes/prod_short.md)] and rows in [!INCLUDE[prod_short](includes/cds_long_md.md)] that are coupled will be synchronised by the integration synchronisation jobs. You can set up table mappings so that new records or rows will be created in the destination (for example, [!INCLUDE[prod_short](includes/prod_short.md)]) for each row in the source (for example, [!INCLUDE[prod_short](includes/cds_long_md.md)]) that is not already coupled.  

For example, the SALESPEOPLE - Dynamics 365 Sales synchronisation job uses the table mapping SALESPEOPLE. The synchronisation job copies data from users in [!INCLUDE[prod_short](includes/cds_long_md.md)] to salespersons in [!INCLUDE[prod_short](includes/prod_short.md)]. If you set up the table mapping to create new records, for every user in [!INCLUDE[prod_short](includes/cds_long_md.md)] that is not already coupled to a salesperson in [!INCLUDE[prod_short](includes/prod_short.md)], a new salesperson row is created in [!INCLUDE[prod_short](includes/prod_short.md)].  

#### <a name="to-create-new-records-during-synchronization"></a>To create new records during synchronisation  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings**, and then choose the related link.

2.  In the table mapping entry in the list, clear the **Synch. Only Coupled Records** field.  

## <a name="using-configuration-templates-on-table-mappings"></a>Using Configuration Templates on Table Mappings
You can assign configuration templates to table mappings to use for new records or rows that are created in [!INCLUDE[prod_short](includes/prod_short.md)] or [!INCLUDE[prod_short](includes/cds_long_md.md)]. For each table mapping, you can specify a configuration template to use for new [!INCLUDE[prod_short](includes/prod_short.md)] records and another template to use new [!INCLUDE[prod_short](includes/cds_long_md.md)] rows.  

If you install the default synchronisation setup, most of the time, two configuration templates will be automatically created and used on the table mapping for [!INCLUDE[prod_short](includes/prod_short.md)] customers and [!INCLUDE[crm_md](includes/crm_md.md)] accounts: **CDSCUST** and **CDSACCOUNT**.  

-   **CDSCUST** is used to create and synchronise new customers in [!INCLUDE[prod_short](includes/prod_short.md)] based on an account in [!INCLUDE[crm_md](includes/crm_md.md)].  

     This template is created by copying an existing configuration template for customers in the application. The **CDSCUST** is created only if there is an existing configuration template and the **Currency Code** field in the template is blank. If a field in the configuration template contains a value, the value will be used instead of the value in the mapped column for the [!INCLUDE[prod_short](includes/cds_long_md.md)] account. For example, if the **Country/Region** column in an account in [!INCLUDE[prod_short](includes/cds_long_md.md)] contains *U.S.* and the **Country/Region** field in the configuration template is *GB*, then *GB* is used as the **Country/Region** for the customer in [!INCLUDE[prod_short](includes/prod_short.md)].  

-   **CDSACCOUNT** creates and synchronises new accounts in [!INCLUDE[prod_short](includes/cds_long_md.md)] based on an account in [!INCLUDE[prod_short](includes/prod_short.md)].  

#### <a name="to-specify-configuration-templates-on-a-table-mapping"></a>To specify configuration templates on a table mapping  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings**, and then choose the related link.

2.  In the table mapping entry in the list, in the **Table Config Template Code** field, choose to the configuration template to use for new records in [!INCLUDE[prod_short](includes/prod_short.md)].  

3.  Set the **Int. Tbl. Config Template Code** field to the configuration template to use for new records in [!INCLUDE[prod_short](includes/cds_long_md.md)].

## <a name="see-also"></a>See Also  
[About Integrating Dynamics 365 Business Central with [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md )   
[Synchronising Business Central and [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md)   
[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]