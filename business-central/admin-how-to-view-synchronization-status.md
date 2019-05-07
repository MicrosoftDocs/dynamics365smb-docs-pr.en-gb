---
title: View the Status of a Synchronisation | Microsoft Docs
description: Learn how to view the status of an individual synchronisation job.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: d55d8d5ab916cee6600deaf891702a625d76d7ee
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "940405"
---
# <a name="view-the-status-of-a-synchronization"></a>View the Status of a Synchronisation
You can view the status of the individual synchronisation jobs that have been run for [!INCLUDE[crm_md](includes/crm_md.md)] integration. This includes synchronisation jobs that have been run from the job queue and manual synchronisation jobs that were performed on records from [!INCLUDE[d365fin](includes/d365fin_md.md)]. This is helpful when troubleshooting synchronisation problems because it gives you access to details about specific errors.

### <a name="to-view-all-synchronization-issues"></a>To view all synchronisation issues
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronisation Errors**, and then choose the related link.
2. On the **Coupled Data Synchronisation Errors** page you can view of all issues that occurred in synchronisation of data between [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[d365fin](includes/d365fin_md.md)], filter and sort records in the page by table, error message and take actions such as **Retry** or **Remove Coupling** to resolve issues one by one or in bulk.

### <a name="to-view-synchronization-log-for-specific-manually-synchronized-record"></a>To view synchronisation log for specific (manually synchronised) record
1. Open, for example, customer, item or any other record that is synchronising data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Sales
2. Choose **Synchronisation Log** action to view the synchronisation log for selected record, for example, specific customer you synchronised manually

## <a name="see-also"></a>See Also  
[Setting Up Dynamics 365 for Sales Integration in Business Central](admin-setting-up-integration-with-dynamics-sales.md)  
[Using Dynamics 365 for Sales from Business Central](marketing-integrate-dynamicscrm.md)
