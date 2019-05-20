---
title: Specify the Layout of a Cheque| Microsoft Docs
description: You can design and print your checks in different formats to conform with standards.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 04/24/2019
ms.author: edupont
ms.openlocfilehash: f2b7fa01cff36e3aab335f7d5921954343c69b74
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1243602"
---
# <a name="define-check-layouts"></a>Define Cheque Layouts
You can design your cheques to conform with the standards set by the local authorities. Cheque images can be printed in English, French, or Spanish.

Cheques are designed to print in both the United States and Canadian cheque image formats in either a cheque-stub-cheque format or a stub-stub-cheque format.

## <a name="to-define-check-layouts"></a>To define cheque layouts
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.
2. On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Cheque**.
3. Select one of the following report IDs.

  | Report ID | Report Name | Description |
  | --- | --- | --- |
  | 1401 |Cheque |This is the default report. |
  | 10411 |Cheque (Stub/Stub/Cheque) |This report is designed to print cheques in a stub/stub/cheque format. |
  | 10412 |Cheque (Stub/Cheque/Stub) |This report is designed to print cheques in a stub/cheque/stub format. |
  | 10413 |Three Cheques per Page |This report is designed to print three cheques on each page. |

When you have set up cheque layouts, you can print cheques from the **Payment Journal** page. For more information, see [Work with Cheques](payables-how-work-checks.md).

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Managing Bank Accounts](bank-manage-bank-accounts.md)   
[Completing Period-End Processes](year-how-complete-period-end-processes.md)  
[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)
