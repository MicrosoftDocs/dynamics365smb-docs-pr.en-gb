---
title: View the Status of Synchronisation Jobs (contains video)
description: Use the Coupled Data Synchronisation Errors page to view the status of Synchronisation jobs that have been run for coupled records in integrations.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'sales, crm, integration, sync, synchronize'
ms.search.form: 6250
ms.date: 06/14/2021
ms.author: bholtorf
---

# <a name="view-the-status-of-synchronization-jobs"></a><a name="view-the-status-of-synchronization-jobs"></a>View the Status of Synchronisation Jobs


Use the **Coupled Data Synchronisation Errors** page to view the status of synchronisation jobs that have been run for coupled records in a Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)] integrations. This includes jobs that were run from the job queue and manual synchronisation jobs that ran on records from [!INCLUDE[prod_short](includes/prod_short.md)]. For example, viewing their status is helpful when troubleshooting because it gives you access to details about errors related to coupled records. Typically, these types of errors are caused by user actions, for example, when:  

* Two people made a change to the same data in both business apps.
* Someone deleted data in one of the apps, but not both.

> [!Note]
> The **Coupled Data Synchronisation Errors** page shows information about jobs related to coupled records. If you resolve all of the errors but records are still not synchronising, it might have something to do with a setting for the integration. Typically, your administrator will need to resolve those types of errors.   

## <a name="example"></a><a name="example"></a>Example
This video shows an example of how to troubleshoot errors that happened while synchronising with [!INCLUDE[prod_short](includes/cds_long_md.md)]. The process will be the same for all integrations. 

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2097304]


## <a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a><a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a>To view and resolve synchronisation errors for coupled records
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronisation Errors**, and then choose the related link.
2. The **Coupled Data Synchronisation Errors** page shows issues that occurred when you synchronised coupled records. The following table includes actions that you can use to resolve issues one by one:

|Action|Description|
|----|----|
|**Remove Coupling**|Uncouples the records and they will no longer synchronise. To restart the synchronisation you must couple them again. |
|**Retry** and **Retry All**|For each record where an error is found, synchronisation is skipped unless you fix the issue. Retry will include the selected record in the next synchronisation and **Retry All** includes all of the records.|
|**Synchronise**|The app will try to resolve a conflict where data was changed in both business apps. You can choose the data to use.|
|**Restore Records** and **Delete Records**|These are useful when a record was deleted in one of the business apps. Delete Records deletes the record or row in the app where it still exists. Restore Records recreates the record or row in the business app where it was deleted.|

> [!NOTE]
> To reduce the number of conflicts you need to resolve, you can set up your integration table mappings to apply these actions automatically. For more information, [Mapping Integration Tables](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).

## <a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a><a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a>To view the synchronisation log for a specific (manually synchronised) record
1. Open, for example, a customer, item or any other record that is synchronising data between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)].
2. Choose the **Synchronisation Log** action to view the synchronisation log for a selected record. For example, a specific customer you synchronised manually.

## <a name="remove-couplings-between-records"></a><a name="remove-couplings-between-records"></a>Remove Couplings Between Records
When something goes wrong in your integration and you need to uncouple records to stop synchronising them, you can do so for one or more records at a time. You can uncouple one or more records from list pages or the **Coupled Data Synchronisation Errors** page by choosing one or more lines and choosing **Delete Coupling**. You can also remove all couplings for one or more table mappings on the **Integration Table Mappings** page. 

If an entity with a unidirectional coupling is deleted in [!INCLUDE[prod_short](includes/prod_short.md)], you must manually delete the broken coupling. To do that, on the **Coupled Data Synchronisation Errors** page, choose the **Find for Deleted** action, and then delete the couplings.

## <a name="see-also"></a><a name="see-also"></a>See Also
[Setting Up User Accounts for Integrating with Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md)  
[Use Dynamics 365 Sales from Business Central](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
