---
title: Record and Adjust Resource Usage and Prices| Microsoft Docs
description: Describes how you can record the resource usage or consumption associated with a job, to keep track and manage costs, prices, and work types.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: fc51b47b71d37daaccc4133d648c90b84d5a3494
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251752"
---
# <a name="use-resources-for-jobs"></a>Use Resources for Jobs
You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs. For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).

You can also post the usage of a resource in a resource journal. Entries posted in a resource journal have no effect on the general ledger.

## <a name="to-assign-resources-to-jobs"></a>To assign resources to jobs
You assign resources to jobs by creating job planning lines for the job. For more information, see [Create Jobs](projects-how-create-jobs.md).

## <a name="to-record-resource-usage-for-a-job"></a>To record resource usage for a job
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.
2. Open a relevant job journal batch, and then fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. When the journal is complete, choose the **Post** action.

## <a name="to-adjust-resource-prices"></a>To adjust resource prices
If you want to change costs or prices for a large number of resources, you can use a batch job.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.
2. Fill in the fields on a line as necessary, and then choose the **OK** button.

> [!NOTE]  
>   This batch job does not create or adjust alternate costs or prices for resources. It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job. The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a>To get resource price change suggestions based on existing alternate prices
If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.
2. Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.
3. Choose the **OK** button.  
4. When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a>To get resource price change suggestions based on standard prices
If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.
2. Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.  
3. Choose the **OK** button.  
4. When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a>To get resource price change suggestions based on alternate prices
If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.  
2. Fill in the fields as necessary.
3. Choose the **OK** button.  
4. When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.

## <a name="see-also"></a>See Also
[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)     
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
