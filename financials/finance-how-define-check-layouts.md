---
title: 'How to: Define Cheque Layouts| Microsoft Docs'
description: Learn about the cheque layouts that are available in Financials.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 03/24/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 6081b6d09fa75b868138817442d6df4d9a8d0d7f
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-define-check-layouts"></a>How to: Define Cheque Layouts
You can design your cheques to conform with the standards set by the local authorities. Cheque images can be printed in English, French, or Spanish.

Cheques are designed to print in both the United States and Canadian cheque image formats in either a cheque-stub-cheque format or a stub-stub-cheque format.

## <a name="to-define-check-layouts"></a>To define cheque layouts
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Report Selections Bank Account**, and choose the related link.
2. In the **Report Selection - Bank Acc.** window, in the **Usage** field, select **Cheque**.
3. Select one of the following report IDs.

| Report ID | Report Name | Description |
| --- | --- | --- |
| 1401 |Cheque |This is the default report. |
| 10401 |Cheque (Stub/Stub/Cheque) |This report is designed to print cheques in a stub/stub/cheque format. |
| 10411 |Cheque (Stub/Cheque/Stub) |This report is designed to print cheques in a cheque/stub/cheque format. |

When you have set up cheque layouts, you can print cheques from the **Payment Journal** window. For more information, see [Work With Cheques](payables-how-work-checks.md).

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Managing Bank Accounts](bank-manage-bank-accounts.md)   
[Completing Period-End Processes](year-how-complete-period-end-processes.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)

