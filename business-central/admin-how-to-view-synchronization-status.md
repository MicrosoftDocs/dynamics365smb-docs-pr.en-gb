---
title: View the Status of Synchronisation Jobs | Microsoft Docs
description: Learn how to view the status after synchronising coupled records.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: b87bd1061adbcaae3a5497fa1af020cfaa412593
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781268"
---
# <a name="view-the-status-of-synchronization-jobs"></a>View the Status of Synchronisation Jobs
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

Use the **Coupled Data Synchronisation Errors** page to view the status of synchronisation jobs that have been run for coupled records in a Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)] integrations. This includes jobs that were run from the job queue and manual synchronisation jobs that ran on records from [!INCLUDE[prod_short](includes/prod_short.md)]. For example, viewing their status is helpful when troubleshooting because it gives you access to details about errors related to coupled records. Typically, these types of errors are caused by user actions, for example, when:  

* Two people made a change to the same data in both business apps.
* Someone deleted data in one of the apps, but not both.

> [!Note]
> The **Coupled Data Synchronisation Errors** page shows information about jobs related to coupled records. If you resolve all of the errors but records are still not synchronising, it might have something to do with a setting for the integration. Typically, your administrator will need to resolve those types of errors.   

<!--

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098171]

-->

## <a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a>To view and resolve synchronisation errors for coupled records
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronisation Errors**, and then choose the related link.
2. The **Coupled Data Synchronisation Errors** page shows issues that occurred when you synchronised coupled records. The following table includes actions that you can use to resolve issues one by one:

|Action|Description|
|----|----|
|**Remove Coupling**|Uncouples the records and they will no longer synchronise. To restart the synchronisation you must couple them again. |
|**Retry** and **Retry All**|For each record where an error is found, synchronisation is skipped unless you fix the issue. Retry will include the selected record in the next synchronisation and **Retry All** includes all of the records.|
|**Synchronise**|The app will try to resolve a conflict where data was changed in both business apps. You can choose the data to use.|
|**Restore Records** and **Delete Records**|These are useful when a record was deleted in one of the business apps. Delete Records deletes the record or row in the app where it still exists. Restore Records recreates the record or row in the business app where it was deleted.|

> [!NOTE]
> To reduce the number of conflicts you need to resolve, you can set up your integration table mappings to apply these actions automatically. For more information, [Mapping Integration Tables](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).

## <a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a>To view the synchronisation log for a specific (manually synchronised) record
1. Open, for example, a customer, item or any other record that is synchronising data between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)].
2. Choose the **Synchronisation Log** action to view the synchronisation log for a selected record. For example, a specific customer you synchronised manually.

## <a name="see-also"></a>See Also  
[Setting Up User Accounts for Integrating with Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md)  
[Using Dynamics 365 Sales from Business Central](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]