---
title: Assign a Priority Level to a Supplier | Microsoft Docs
description: You can assign numbers to your suppliers or suppliers to prioritise them and facilitate payment suggestions in Business Central.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d83fe736298e4cae3b6b86a495e0567057df2cc5
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6443301"
---
# <a name="prioritize-vendors"></a>Prioritise Suppliers
[!INCLUDE[prod_short](includes/prod_short.md)] can suggest various payments to suppliers, for example, payments that will be due soon or payments where a discount is available. For more information, see [Suggest Supplier Payments](payables-how-suggest-vendor-payments.md).

First, you must prioritise your suppliers by assigning numbers to them.
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE3PRGa?rel=0]

## <a name="to-prioritize-vendors"></a>To prioritise suppliers
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suppliers**, and then choose the related link.
2. Select the relevant supplier, and then choose **Edit**.
3. In the **Priority** field, enter a number.

[!INCLUDE[prod_short](includes/prod_short.md)] considers the lowest number, except 0, to have the highest priority. So, for example, if you use 1, 2, and 3, then 1 will have the highest priority.

If you do not want to prioritise a supplier, leave the **Priority** field blank. Then, if you use the payment suggestion feature, the supplier will be listed after all the suppliers that have a priority number. You can enter as many priority levels as necessary.

## <a name="see-also"></a>See Also
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Managing Payables](payables-manage-payables.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]