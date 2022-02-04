---
title: Assign a Priority Level to a Vendor (contains video)
description: You can assign numbers to your suppliers or suppliers to prioritise them and facilitate payment suggestions in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'supplier, payment priority'
ms.search.form: '26, 27'
ms.date: 04/01/2021
ms.author: edupont
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