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
ms.openlocfilehash: 11e29674c2d12031fdf4e7f66e767be4fcc74795
ms.sourcegitcommit: 04581558f6c5488c705a7ac392cf297be10b5f4f
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/06/2019
ms.locfileid: "1620891"
---
# <a name="view-the-status-of-a-synchronization"></a>View the Status of a Synchronisation
You can view the status of the individual synchronisation jobs that have been run for [!INCLUDE[crm_md](includes/crm_md.md)] integration. This includes synchronisation jobs that have been run from the job queue and manual synchronisation jobs that were performed on records from [!INCLUDE[d365fin](includes/d365fin_md.md)]. This is helpful when troubleshooting synchronisation problems because it gives you access to details about specific errors.

### <a name="to-view-synchronization-issues-for-coupled-records"></a>To view synchronisation issues for coupled records
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronisation Errors**, and then choose the related link.
2. The **Coupled Data Synchronisation Errors** page shows issues that occurred when you synchronised coupled records. You can filter and sort records and take actions such as **Restore** or **Delete Records** to resolve issues one by one.

### <a name="to-view-synchronization-log-for-specific-manually-synchronized-record"></a>To view synchronisation log for specific (manually synchronised) record
1. Open, for example, a customer, item or any other record that is synchronising data between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Sales.
2. Choose the **Synchronisation Log** action to view the synchronisation log for a selected record. For example, a specific customer you synchronised manually.

## <a name="see-also"></a>See Also  
[Setting Up Dynamics 365 for Sales Integration in Business Central](admin-setting-up-integration-with-dynamics-sales.md)  
[Using Dynamics 365 for Sales from Business Central](marketing-integrate-dynamicscrm.md)
