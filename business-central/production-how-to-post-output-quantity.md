---
title: How to Batch Post Production Output and Run Times| Microsoft Docs
description: The output quantity represents the work progress in the form of the finished quantity.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 82e28246f1a1c65c7bd702023d9c68c614383cc2
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4759149"
---
# <a name="batch-post-output-and-run-times"></a>Batch Post Output and Run Times
The output quantity represents the work progress in the form of the finished quantity.  

> [!NOTE]
> Only when you post output quantity on the last operation, the inventory is updated automatically.  

## <a name="to-post-output-quantities-for-one-or-more-production-order-lines"></a>To post output quantities for one or more production order lines
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.  
2. Fill in the fields with the production order data and the output data. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. If the operation has been completed, select the **Finished** field.  

    If the warehouse location where the items should be put away uses bins but does not require put-away processing,  assign a bin code to the journal line to specify where the items should be placed in the warehouse. For more information, see [Put Away Production or Assembly Output](warehouse-how-to-put-away-production-output.md).  

4. Choose the **Post** acto post the operations. The output quantity will be posted. The item is now available for shipping.  

## <a name="to-post-run-times-for-one-or-more-production-order-lines"></a>To post run times for one or more production order lines
The run time represents work progress in the form of the necessary working time.    

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.  
2. Fill in the fields with the production order data and the output data.  
3.  If the operation is completed, select the **Finished** field.  
4. Choose the **Post** action to post the time spent per operation. Capacity ledger entries are updated for the used work or machine centres.

## <a name="see-also"></a>See Also  
[Manufacturing](production-manage-manufacturing.md)    
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Planning](production-planning.md)      
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)
