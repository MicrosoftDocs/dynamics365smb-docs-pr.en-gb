---
title: Assign a Priority Level to a Vendor | Microsoft Docs
description: You can assign numbers to your vendors or suppliers to prioritise them and facilitate payment suggestions in Financials.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 2c91b28daf27ddd2b698ffe4338bbf92fd1f9adf
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-prioritize-vendors"></a>How to: Prioritise Vendors
[!INCLUDE[d365fin](includes/d365fin_md.md)] can suggest various payments to vendors, for example, payments that will be due soon or payments where a discount is available. For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).

First, you must prioritise your vendors by assigning numbers to them.

## <a name="to-prioritize-vendors"></a>To prioritise vendors
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.
2. Select the relevant vendor, and then choose **Edit**.
3. In the **Priority** field, enter a number.

[!INCLUDE[d365fin](includes/d365fin_md.md)] considers the lowest number, except 0, to have the highest priority. So, for example, if you use 1, 2, and 3, then 1 will have the highest priority.

If you do not want to prioritise a vendor, leave the **Priority** field blank. Then, if you use the payment suggestion feature, the vendor will be listed after all the vendors that have a priority number. You can enter as many priority levels as necessary.

## <a name="see-also"></a>See Also
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Managing Payables](payables-manage-payables.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

