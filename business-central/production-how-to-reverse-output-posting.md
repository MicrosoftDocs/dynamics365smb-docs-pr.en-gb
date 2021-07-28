---
title: How to Reverse Output Posting
description: There are times when output posting must be reversed. This topic outlines the procedure for reversing output posting.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/22/2021
ms.author: edupont
ms.openlocfilehash: b1d3d05876beb452d8a3fd1ac917e40f1ffe7320
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6440360"
---
# <a name="reverse-output-posting"></a>Reverse Output Posting
There are times when output posting must be reversed. An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a works order.  

## <a name="to-reverse-an-output-posting"></a>To reverse an output posting  
1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link. Select your batch.  
2. Fill in the fields as necessary. For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).
3.  In the **Applies-To Entry** field, select the associated item ledger entry. This reverses the capacity and item ledger entries.  
4. Post the reversal by posting the journal.  

The output journal entries are posted to the item ledger as a positive adjustment.  

## <a name="see-also"></a>See Also  
 [Manufacturing](production-manage-manufacturing.md)    
 [Setting Up Manufacturing](production-configure-production-processes.md)  
 [Planning](production-planning.md)      
 [Stock](inventory-manage-inventory.md)  
 [Purchasing](purchasing-manage-purchasing.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]