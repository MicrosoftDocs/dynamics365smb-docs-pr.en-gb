---
title: Review and Post the Year-End Closing Entry | Microsoft Docs
description: Describes how to open the journal you specified in the Close Income Statement batch job, and then review and post the year-end closing entry.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 03/29/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 68017b8b031ee4bd368936b6fb4de157328d7030
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-post-the-year-end-closing-entry"></a>How to: Post the Year-End Closing Entry
After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.

## <a name="to-post-the-year-end-closing-entry"></a>To post the year end closing entry
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.
2. In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.
3. Review the entries.
4. To post the journal, choose the **Post** action.

> [!NOTE]  
>   If an error is detected, an error message is displayed. If the posting is successful, the posted entries are removed from the journal. After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.

## <a name="see-also"></a>See Also
[How to: Close Accounting Periods](year-close-account-periods.md)  
[Closing Books](year-close-books.md)  
[Close Income Statement](year-close-income-statement.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

