---
title: Review and Post the Year-End Closing Entry | Microsoft Docs
description: Describes how to open the journal you specified in the Close Income Statement batch job, and then review and post the year-end closing entry.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 878079fd02a2d54ae6b878fa54c7006dee779c15
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "914911"
---
# <a name="post-the-year-end-closing-entry"></a>Post the Year-End Closing Entry
After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.

## <a name="to-post-the-year-end-closing-entry"></a>To post the year end closing entry
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.
2. On the **General Journal** page, in the **Batch Name** field, select the batch that contains the closing entries.
3. Review the entries.
4. To post the journal, choose the **Post** action.

> [!NOTE]  
>   If an error is detected, an error message is displayed. If the posting is successful, the posted entries are removed from the journal. After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.

## <a name="see-also"></a>See Also
[Close Accounting Periods](year-close-account-periods.md)  
[Closing Books](year-close-books.md)  
[Close Income Statement](year-close-income-statement.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
