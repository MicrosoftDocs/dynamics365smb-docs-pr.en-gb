---
title: Modify Table Mappings for Synchronisation | Microsoft Docs
description: Learn how to change the table mappings that are used when synchronising data between Business Central and Dynamics 365 for Sales.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize, table mapping
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: c2b2df393afe7cf27964b1540deddf7760747a9d
ms.sourcegitcommit: 92c7b6c5f0a5d8becbef106ab85258906765bc3e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/13/2019
ms.locfileid: "1540207"
---
# <a name="modify-table-mappings-for-synchronization"></a>Modify Table Mappings for Synchronisation
An integration table mapping links a table in [!INCLUDE[d365fin](includes/d365fin_md.md)] to an integration table for the [!INCLUDE[crm_md](includes/crm_md.md)] entity. For each entity in [!INCLUDE[crm_md](includes/crm_md.md)] that you want to synchronise with corresponding data in [!INCLUDE[d365fin](includes/d365fin_md.md)]], there must be a corresponding integration table mapping. An integration table mapping includes several settings that enable you to control how records in a [!INCLUDE[d365fin](includes/d365fin_md.md)] table and a [!INCLUDE[crm_md](includes/crm_md.md)] entity are synchronised by the corresponding integration synchronisation jobs.  

## <a name="filtering-records"></a>Filtering Records  
 If you do not want to synchronise all records for a specific entity in [!INCLUDE[crm_md](includes/crm_md.md)] or table in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can set up filters to limit the records that are synchronised. You set up filters on the **Integration Table Mappings** page.  

#### <a name="to-filter-records-for-synchronization"></a>To filter records for synchronisation  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings**, and then choose the related link.

2.  To filter the [!INCLUDE[d365fin](includes/d365fin_md.md)] records, set the **Table Filter** field.  

3.  To filter the [!INCLUDE[crm_md](includes/crm_md.md)] records, set the **Integration Table Filter** field.  

## <a name="creating-new-records"></a>Creating New Records  
 By default, only records in [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)] that are coupled will be synchronised by the integration synchronisation jobs. You can set up table mappings so that new records will be created in the destination (for example, [!INCLUDE[d365fin](includes/d365fin_md.md)]) for each record in the source (for example, [!INCLUDE[crm_md](includes/crm_md.md)]) that is not already coupled.  

 For example, the SALESPEOPLE - Dynamics 365 for Sales synchronisation job uses the table mapping SALESPEOPLE. The synchronisation job copies data from user records in [!INCLUDE[crm_md](includes/crm_md.md)] to salesperson records in [!INCLUDE[d365fin](includes/d365fin_md.md)]. If you set up the table mapping to create new records, for every user in [!INCLUDE[crm_md](includes/crm_md.md)] that is not already coupled to a salesperson in [!INCLUDE[d365fin](includes/d365fin_md.md)], a new salesperson record is created in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

#### <a name="to-create-new-records-during-synchronization"></a>To create new records during synchronisation  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings**, and then choose the related link.

2.  In the table mapping entry in the list, clear the **Synch. Only Coupled Records** field.  

## <a name="using-configuration-templates-on-table-mappings"></a>Using Configuration Templates on Table Mappings
You can assign configuration templates to table mappings to use for new records that are created in [!INCLUDE[d365fin](includes/d365fin_md.md)] or [!INCLUDE[crm_md](includes/crm_md.md)]. For each table mapping, you can specify a configuration template to use for new [!INCLUDE[d365fin](includes/d365fin_md.md)] records and another template to use new [!INCLUDE[crm_md](includes/crm_md.md)] records.  

If you install the default synchronisation setup, most of the time, two configuration templates will be automatically created and used on the table mapping for [!INCLUDE[d365fin](includes/d365fin_md.md)] customers and [!INCLUDE[crm_md](includes/crm_md.md)] accounts: **CRMCUST** and **CRMACCOUNT**.  

-   **CRMCUST** is used to create and synchronise new customers in [!INCLUDE[d365fin](includes/d365fin_md.md)] based on an account in [!INCLUDE[crm_md](includes/crm_md.md)].  

     This template is created by copying an existing configuration template for customers in the application. The **CRMCUST** is created only if there is an existing configuration template and the **Currency Code** field in the template is blank. If a field in the configuration template contains a value, the value will be used instead of the value in the mapped field for the [!INCLUDE[crm_md](includes/crm_md.md)] account. For example, if the **Country/Region** field in an account in [!INCLUDE[crm_md](includes/crm_md.md)] contains *U.S.* and the **Country/Region** field in the configuration template is *GB*, then *GB* is used as the **Country/Region** for the customer in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

-   **CRMACCOUNT** creates and synchronises new accounts in [!INCLUDE[crm_md](includes/crm_md.md)] based on an account in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

#### <a name="to-specify-configuration-templates-on-a-table-mapping"></a>To specify configuration templates on a table mapping  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings**, and then choose the related link.

2.  In the table mapping entry in the list, in the **Table Config Template Code** field, choose to the configuration template to use for new records in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

3.  Set the **Int. Tbl. Config Template Code** field to the configuration template to use for new records in [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="see-also"></a>See Also  
[About Integrating Dynamics 365 Business Central with Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md )   
[Synchronising Business Central and Dynamics 365 for Sales](admin-synchronizing-business-central-and-sales.md)   
[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
