---
title: Synchronising Business Central and Common Data Service | Microsoft Docs
description: Learn about synchronising data between Business Central and Common Data Service.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 2f1b79cdf04075159b5e464e384bace89d9f933c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917808"
---
# <a name="scheduling-a-synchronization-between-business-central-and-common-data-service"></a>Scheduling a Synchronisation between Business Central and Common Data Service

You can synchronise [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[cds_long_md](includes/cds_long_md.md)] on scheduled intervals by setting up jobs in the job queue. The synchronisation jobs synchronise data in [!INCLUDE[d365fin](includes/d365fin_md.md)] records and [!INCLUDE[cds_long_md](includes/cds_long_md.md)] records that have been previously coupled together. Or for records that are not already coupled, depending on the synchronisation direction and rules, the synchronisation jobs can create and couple new records in the destination system. 

There are several synchronisation jobs that are available out-of-the-box. The jobs are run in the following order to avoid coupling dependencies between entities. For more information, see [Use Job Queues to Schedule Tasks](/dynamics365/business-central/admin-job-queues-schedule-tasks.md).

1. CURRENCY - Common Data Service synchronisation job.
2. VENDOR - Common Data Service synchronisation job.
3. CONTACT - Common Data Service synchronisation job.
4. CUSTOMER - Common Data Service synchronisation job.
5. SALESPEOPLE - Common Data Service synchronisation job.

You can view the jobs on the **Job Queue Entries** page. For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).

## <a name="default-synchronization-job-queue-entries"></a>Default Synchronisation Job Queue Entries

The following table describes the default synchronisation jobs for [!INCLUDE[cds_long_md](includes/cds_long_md.md)].  

| Job Queue Entry | Description | Direction | Integration Table Mapping | Default Synchronisation Frequency (mins) | Default inactivity sleep time (mins) |
|--|--|--|--|--|--|--|
| CONTACT - Common Data Service synchronisation job | Synchronises [!INCLUDE[cds_long_md](includes/cds_long_md.md)] contacts with [!INCLUDE[d365fin](includes/d365fin_md.md)] contacts. | Bidirectional | CONTACT | 30 | 720 <br>(12 hours) |
| CURRENCY - Common Data Service synchronisation job | Synchronises [!INCLUDE[cds_long_md](includes/cds_long_md.md)] transaction currencies with [!INCLUDE[d365fin](includes/d365fin_md.md)] currencies. | From [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[cds_long_md](includes/cds_long_md.md)] | CURRENCY | 30 | 720 <br> (12 hrs) |
| CUSTOMER - Common Data Service synchronisation job | Synchronises [!INCLUDE[cds_long_md](includes/cds_long_md.md)] accounts with [!INCLUDE[d365fin](includes/d365fin_md.md)] customers. | Bidirectional | CUSTOMER | 30 | 720<br> (12 hrs) |
| VENDOR - Common Data Service synchronisation job | Synchronises [!INCLUDE[cds_long_md](includes/cds_long_md.md)] accounts with [!INCLUDE[d365fin](includes/d365fin_md.md)] customers. | Bidirectional | VENDOR | 30 | 720<br> (12 hrs) |
| SALESPEOPLE - Common Data Service synchronisation job | Synchronises [!INCLUDE[d365fin](includes/d365fin_md.md)] salespeople with [!INCLUDE[cds_long_md](includes/cds_long_md.md)] users. | From [!INCLUDE[cds_long_md](includes/cds_long_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)] | SALESPEOPLE | 30 | 1440<br> (24 hrs) |

## <a name="synchronization-process"></a>Synchronisation Process

Each synchronisation job queue entry uses a specific integration table mapping that specifies which [!INCLUDE[d365fin](includes/d365fin_md.md)] table and [!INCLUDE[cds_long_md](includes/cds_long_md.md)] entity to synchronise. The table mappings also include some settings that control which records in the [!INCLUDE[d365fin](includes/d365fin_md.md)] table and [!INCLUDE[cds_long_md](includes/cds_long_md.md)] entity to synchronise.  

To synchronise data, [!INCLUDE[cds_long_md](includes/cds_long_md.md)] entity records must be coupled to [!INCLUDE[d365fin](includes/d365fin_md.md)] records. For example, a [!INCLUDE[d365fin](includes/d365fin_md.md)] customer must be coupled to a [!INCLUDE[cds_long_md](includes/cds_long_md.md)] account. You can set up couplings manually, before running the synchronisation jobs, or let the synchronisation jobs set up couplings automatically. The following list describes how data is synchronised between Common Data Service and [!INCLUDE[d365fin](includes/d365fin_md.md)] when you are using the synchronisation job queue entries. For more information, see [Couple and Synchronise Records Manually](admin-how-to-couple-and-synchronize-records-manually.md).

- The **Sync. Only Coupled Records** check box controls whether new records are created when you synchronise. By default, the check box is selected, which means that only records that are coupled will be synchronised. In the integration table mapping, you can change the table mapping between a [!INCLUDE[cds_long_md](includes/cds_long_md.md)] entity and a [!INCLUDE[d365fin](includes/d365fin_md.md)] table so that the integration synchronisation jobs will create new records in the destination database for each record in the source database that is not coupled. For more information, see [Creating New Records](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).

    **Example** If you clear the **Sync. Only Coupled Records** check box, when you synchronise customers in [!INCLUDE[d365fin](includes/d365fin_md.md)] with accounts in [!INCLUDE[cds_long_md](includes/cds_long_md.md)], a new account is created for each customer in [!INCLUDE[d365fin](includes/d365fin_md.md)] and automatically coupled. Additionally, because the synchronisation is bidirectional in this case, a new customer is created and coupled for each [!INCLUDE[cds_long_md](includes/cds_long_md.md)] account that is not already coupled.  

    > [!NOTE]  
    > There are rules and filters that determine what data is synchronised. For more information, see [Synchronisation Rules](admin-synchronizing-business-central-and-sales.md).

- When new records are created in [!INCLUDE[d365fin](includes/d365fin_md.md)], the records use the either the template that is defined for the integration table mapping or the default template that is available for the record type. Fields are populated with data from [!INCLUDE[d365fin](includes/d365fin_md.md)] or [!INCLUDE[cds_long_md](includes/cds_long_md.md)] depending on the synchronisation direction. For more information, see [Modify Table Mappings for Synchronisation](admin-how-to-modify-table-mappings-for-synchronization.md).  

- With subsequent synchronisations, only records that have been modified or added after the last successful synchronisation job for the entity will be updated.  

     New records in [!INCLUDE[cds_long_md](includes/cds_long_md.md)] are added in [!INCLUDE[d365fin](includes/d365fin_md.md)]. If data in fields in [!INCLUDE[cds_long_md](includes/cds_long_md.md)] records has changed, the data is copied to the corresponding field in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

- With bidirectional synchronisation, the job synchronises from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[cds_long_md](includes/cds_long_md.md)], and then from [!INCLUDE[cds_long_md](includes/cds_long_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="about-inactivity-timeouts"></a>About Inactivity Timeouts

Some job queue entries, such as those that schedule synchronisation between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[cds_long_md](includes/cds_long_md.md)], use the **Inactivity Timeout** field on the Job Queue Entry card to prevent the job queue entry from running unnecessarily.  

:::image type="content" source="media/on-hold-with-inactivity-timeout.png" alt-text="Flowchart for when job queue entries are put on hold due to inactivity.":::

When the value in this field is not zero, and the job queue did not find any changes during the last run, [!INCLUDE[d365fin](includes/d365fin_md.md)] puts the job queue entry on hold. When that happens, the **Status of Job Queue** field will show **On Hold Due to Inactivity** , and [!INCLUDE[d365fin](includes/d365fin_md.md)] will wait for the period of time specified in **Inactivity Timeout** field before it runs the job queue entry again.  

For example, by default, the CURRENCY job queue entry, which synchronises currencies in [!INCLUDE[cds_long_md](includes/cds_long_md.md)] with exchange rates in [!INCLUDE[d365fin](includes/d365fin_md.md)], will look for changes to exchange rates every 30 minutes. If no changes are found, [!INCLUDE[d365fin](includes/d365fin_md.md)] puts the CURRENCY job queue entry on hold for 720 minutes (six hours). If an exchange rate is changed in [!INCLUDE[d365fin](includes/d365fin_md.md)] while the job queue entry is on hold, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically reactivate the job queue entry and restart the job queue. 

> [!Note]
> [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically activate job queue entries that are on hold only when changes happen in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Changes in [!INCLUDE[cds_long_md](includes/cds_long_md.md)] will not activate job queue entries.

## <a name="to-view-the-synchronization-job-log"></a>To view the synchronisation job log

1. Choose the :::image type="icon" source="media/ui-search/search_small.png" border="false"::: icon, enter **Integration Synchronisation Log** , and then choose the related link.
2. If one or more error occurred for a synchronisation job, the number of errors appears in the **Failed** column. To view the errors for the job, choose the number.  

    > [!TIP]  
    > You can view all synchronisation job errors by opening the synchronisation job error log directly.

## <a name="to-view-the-synchronization-job-log-from-the-table-mappings"></a>To view the synchronisation job log from the table mappings

1. Choose the :::image type="icon" source="media/ui-search/search_small.png" border="false"::: icon, enter **Integration Table Mappings** , and then choose the related link.
2. In the **Integration Table Mappings** page, select an entry, and then choose **Integration Synch. Job Log** .  

## <a name="to-view-the-synchronization-error-log"></a>To view the synchronisation error log

- Choose the :::image type="icon" source="media/ui-search/search_small.png" border="false"::: icon, enter **Integration Synchronisation Errors** , and then choose the related link.

## <a name="see-also"></a>See Also

[Synchronising Data in Business Central and [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md)  
[Manually Synchronise Table Mappings](admin-manual-synchronization-of-table-mappings.md)  
[Scheduling a Synchronisation between Business Central and [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
[About Integrating Dynamics 365 Business Central with [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)  
