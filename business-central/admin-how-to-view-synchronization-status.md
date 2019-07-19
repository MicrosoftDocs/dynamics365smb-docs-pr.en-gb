---
title: View the Status of Synchronisation Jobs | Microsoft Docs
description: Learn how to view the status after synchronising coupled records.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 06/13/2019
ms.author: bholtorf
ms.openlocfilehash: 8d7421d5fee1a6498c204730f873c3746aafc637
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/04/2019
ms.locfileid: "1726751"
---
# <a name="view-the-status-of-synchronization-jobs"></a>View the Status of Synchronisation Jobs
Use the **Coupled Data Synchronisation Errors** page to view the status of synchronisation jobs that have been run for coupled records in a [!INCLUDE[crm_md](includes/crm_md.md)] integration. This includes jobs that were run from the job queue and manual synchronisation jobs that ran on records from [!INCLUDE[d365fin](includes/d365fin_md.md)]. For example, viewing their status is helpful when troubleshooting because it gives you access to details about errors related to coupled records. Typically, these types of errors are caused by user actions, for example, when:  

* Two people made a change to the same record in both business apps.
* Someone deleted a record in one of the apps, but not both.

> [!Note]
> The **Coupled Data Synchronisation Errors** page shows information about jobs related to coupled records. If you resolve all of the errors but records are still not synchronising, it might have something to do with a setting for the integration. Typically, your administrator will need to resolve those types of errors.   

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098171]

## <a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a>To view and resolve synchronisation errors for coupled records
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronisation Errors**, and then choose the related link.
2. The **Coupled Data Synchronisation Errors** page shows issues that occurred when you synchronised coupled records. The following table includes actions that you can use to resolve issues one by one:

|Action|Description|
|----|----|
|**Remove Coupling**|Uncouples the records and they will no longer synchronise. To resume synchronising the records, you must couple them again.|
|**Retry**|For each record where an error is found, synchronisation is skipped unless you fix the issue manually. Retry will include the record in the next synchronisation.|
|**Synchronise**|The app will try to resolve a conflict where a record was changed in both business apps. You can choose the version of the record to use in both apps.|
|**Restore Records** and **Delete Records**|These are useful when a record was deleted in one of the apps. Delete Records deletes the record in the app where it still exists. Restore recreates the record in the app where it was deleted.|

## <a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a>To view the synchronisation log for a specific (manually synchronised) record
1. Open, for example, a customer, item or any other record that is synchronising data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].
2. Choose the **Synchronisation Log** action to view the synchronisation log for a selected record. For example, a specific customer you synchronised manually.

## <a name="see-also"></a>See Also  
[Setting Up User Accounts for Integrating with Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md)  
[Using Dynamics 365 for Sales from Business Central](marketing-integrate-dynamicscrm.md)
