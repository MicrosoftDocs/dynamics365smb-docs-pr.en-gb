---
title: Manual Synchronisation of Table Mappings | Microsoft Docs
description: The synchronisation copies data between Common Data Service entities and Business Central to keep both systems up-to-date.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: ba79088bc386a856f1b3e7727f1f778ebabb7d51
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911337"
---
# <a name="manually-synchronize-table-mappings"></a>Manually Synchronise Table Mappings
An integration table mapping associates a [!INCLUDE[d365fin](includes/d365fin_md.md)] table (record type), such as customer, with a [!INCLUDE[d365fin](includes/cds_long_md.md)] entity, such as an account. Synchronising an integration table mapping enables you to synchronise data in all records of the [!INCLUDE[d365fin](includes/d365fin_md.md)] table and [!INCLUDE[d365fin](includes/cds_long_md.md)] entity that are coupled. Additionally, depending on the configuration of the table mapping, synchronisation can create and couple new records in the destination solution for uncoupled records in the source.  

Manually synchronising integration table mappings can be useful during the initial set up of an integration, and when diagnosing synchronisation errors.  

This article describes three methods for manually synchronising integration table mappings. Each method provides a different level of synchronisation.

## <a name="run-a-full-synchronization"></a>Run a Full Synchronisation
A full synchronisation runs all the default integration synchronisation jobs for synchronising [!INCLUDE[d365fin](includes/d365fin_md.md)] records and [!INCLUDE[d365fin](includes/cds_long_md.md)] entities, as defined on the **Integration Table Mappings** page. 

A full synchronisation performs the following operations For [!INCLUDE[d365fin](includes/d365fin_md.md)] or [!INCLUDE[d365fin](includes/cds_long_md.md)] records that are:

* Not coupled, a new matching record will be created and coupled in the opposing solution.
Whether and where a record gets created depends on the synchronisation direction. For example, when synchronising data from [!INCLUDE[d365fin](includes/d365fin_md.md)] customers to [!INCLUDE[d365fin](includes/cds_long_md.md)] accounts, if there is a customer that is not coupled to an account, then a new account will be automatically added in [!INCLUDE[d365fin](includes/cds_long_md.md)] and coupled to the customer in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The opposite holds true when the synchronisation direction is from [!INCLUDE[d365fin](includes/cds_long_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)]. For each account that is not already coupled to a customer, a new matching customer will be created in [!INCLUDE[d365fin](includes/d365fin_md.md)] and coupled to the account in [!INCLUDE[d365fin](includes/cds_long_md.md)].  

     > [!NOTE]  
     >  To achieve this, the full synchronisation operation temporarily clears the **Synch. Only Coupled Records** option on the integration table mapping that is used by the synchronisation job. At the end of the full synchronisation process, you will be prompted whether you want to keep this option cleared for all jobs.  

* Coupled, the synchronisation direction (for example, from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[d365fin](includes/cds_long_md.md)] or from [!INCLUDE[d365fin](includes/cds_long_md.md)]to [!INCLUDE[d365fin](includes/d365fin_md.md)]) is predetermined by the integration table mappings. For more information, see [Standard Entity Mapping for Synchronisation](admin-synchronizing-business-central-and-sales.md#standard-entity-mapping-for-synchronization).  

> [!IMPORTANT]  
>  You typically only use the full synchronisation when you initially set up integration between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[d365fin](includes/cds_long_md.md)] and only one of solutions contains data, which you want to copy to the other solution. A full synchronisation can be useful in a demonstration environment. Because the full synchronisation automatically creates and couples records between the solutions, it makes it faster to start working with synchronising data between records. On the other hand, you should only run a full synchronisation if you want a record in [!INCLUDE[d365fin](includes/d365fin_md.md)] for each record in [!INCLUDE[d365fin](includes/cds_long_md.md)] for the given table mappings. Otherwise, you can have unwanted or duplicate records in either [!INCLUDE[d365fin](includes/d365fin_md.md)] or [!INCLUDE[d365fin](includes/cds_long_md.md)].  

### <a name="to-run-a-full-synchronization"></a>To run a full synchronisation  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Common Data Service Connection Setup** , and then choose the related link.

    > [!NOTE]
    > If you want to run a full synchronisation for entities through Dynamics 365 Sales, use the **Microsoft Dynamics 365 Sales Connection Setup** page instead.

2.  Choose the **Run Full Synchronisation** action, and then choose the **Yes** button.  
3.  When the full synchronisation is completed, you can specify whether to allow scheduled synchronisation jobs to create new records.  

    If you want all synchronisation jobs to create new records in the destination for uncoupled records in the source, choose **Yes** . This sets the **Synch. Only Coupled Records** field on the table mappings that are used by the synchronisation jobs.  

    If you want synchronisation jobs to run as they did before the full synchronisation with regard to creating new records, choose **No** . This sets the **Synch. Only Coupled Records** field to the setting it had before the full synchronisation.  

You can view the results of the full synchronisation on the **Integration Synchronisation Jobs** page. For more information, see [View the Status of a Synchronisation](admin-how-to-view-synchronization-status.md).  

## <a name="synchronizing-all-modified-records"></a>Synchronising All Modified Records
You can use the **CDS Connection Setup** page to synchronise changes to data in all integration table mappings. This is similar to a full synchronisation. It will synchronise data in all coupled records in the [!INCLUDE[d365fin](includes/d365fin_md.md)] tables and [!INCLUDE[d365fin](includes/cds_long_md.md)] entities that are defined in the table mappings. By default, only records that have been modified since the last time they were synchronised will be synchronised. Synchronisation jobs synchronise table mappings in the following order to avoid coupling dependencies between the entities:  

1.  CURRENCY  
2.  SALESPEOPLE  
3.  VENDOR  
4.  CUSTOMER  
5.  CONTACTS  

You can view the results of the synchronisation on the **Integration Synchronisation Jobs** page. For more information, see [View the Status of a Synchronisation](admin-how-to-view-synchronization-status.md).  

> [!TIP]  
>  By modifying the integration table mapping in advance, you can configure the synchronisation with filters to control which records are synchronised, or configure it to create new records in the destination solution for uncoupled records in the source. For more information, see [Modify Table Mappings for Synchronisation](admin-how-to-modify-table-mappings-for-synchronization.md).

### <a name="to-synchronize-records-for-all-tables"></a>To synchronise records for all tables  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Microsoft Dynamics 365 Sales Connection Setup** , and then choose the related link.
2.  Choose the **Synchronise Modified Records** action, and then choose **Yes** .  

## <a name="synchronize-individual-table-mappings"></a>Synchronise Individual Table Mappings
You can use the **Integration Table Mappings** page to run a synchronisation job specific table mappings. This will synchronise data in all coupled records in the [!INCLUDE[d365fin](includes/d365fin_md.md)] table and [!INCLUDE[d365fin](includes/cds_long_md.md)] entity that are defined by the table mapping. By default, only records that have been modified since the last time they were synchronised will be synchronised.  

By modifying the integration table mapping in advance, you can configure the synchronisation job to create new records in the destination solution for uncoupled records in the source.

### <a name="to-synchronize-records-of-an-integration-table-mapping"></a>To synchronise records of an integration table mapping  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Integration Table Mappings** , and then choose the related link.
2.  Choose the **Synchronise Modified Records** action, and then choose **Yes** .  

## <a name="see-also"></a>See Also  
[Synchronising Business Central and Dynamics 365 Sales](admin-synchronizing-business-central-and-sales.md)   
[Setting Up User Accounts for Integrating with Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md)   
