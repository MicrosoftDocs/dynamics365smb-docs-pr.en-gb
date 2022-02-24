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
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: 1fa624ecda5914c0ba4e395025f051bc5d8cc457
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3191746"
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
