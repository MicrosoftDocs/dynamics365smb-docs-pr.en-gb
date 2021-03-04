---
title: Assign a Priority Level to a Vendor | Microsoft Docs
description: You can assign numbers to your vendors or suppliers to prioritise them and facilitate payment suggestions in Business Central.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 87d2f7c7fe2d395d16b41b288500f22e16bd0ba0
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4758549"
---
# <a name="prioritize-vendors"></a>Prioritise Vendors
[!INCLUDE[prod_short](includes/prod_short.md)] can suggest various payments to vendors, for example, payments that will be due soon or payments where a discount is available. For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).

First, you must prioritise your vendors by assigning numbers to them.
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE3PRGa?rel=0]

## <a name="to-prioritize-vendors"></a>To prioritise vendors
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.
2. Select the relevant vendor, and then choose **Edit**.
3. In the **Priority** field, enter a number.

[!INCLUDE[prod_short](includes/prod_short.md)] considers the lowest number, except 0, to have the highest priority. So, for example, if you use 1, 2, and 3, then 1 will have the highest priority.

If you do not want to prioritise a vendor, leave the **Priority** field blank. Then, if you use the payment suggestion feature, the vendor will be listed after all the vendors that have a priority number. You can enter as many priority levels as necessary.

## <a name="see-also"></a>See Also
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Managing Payables](payables-manage-payables.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]