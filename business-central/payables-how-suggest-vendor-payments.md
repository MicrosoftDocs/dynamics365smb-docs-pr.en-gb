---
title: Suggest Vendor Payments Batch Job
description: You can specify supplier payment settings to get suggestions or proposals for payments that are due soon or where a discount is available.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'vendor payment, creditor, debt, balance due, AP'
ms.search.form: 256
ms.date: 04/01/2021
ms.author: edupont
---
# <a name="suggest-vendor-payments"></a>Suggest Supplier Payments

On the **Payment Journal** page, you can use the **Suggest Supplier Payments** batch job to suggest payment lines. Lines for payments that are due soon or payments where a payment discount is available are suggested based on your settings.

To benefit fully from payment suggestions, you must first prioritise your suppliers. For more information, see [Prioritise Suppliers](purchasing-how-prioritize-vendors.md).  

> [!NOTE]  
> Supplier ledger entries that are **On Hold** are not included in the batch job.  

> [!IMPORTANT]  
>   If you want to take advantage of payment discounts, and have entered an available amount, the amount will be used for:  
    * Prioritised overdue supplier entries first in order of priority.   
    * Overdue supplier entries that are not prioritised.  
    * Open supplier entries that qualify for payment discounts, arranged by supplier number.  

## <a name="to-use-the-suggest-vendor-payments-function"></a>To use the Suggest Supplier Payments function
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.  
2. Open the relevant journal, and then choose the **Suggest Supplier Payments** action.  
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. Choose the **OK** button.  

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>To insert the due date as posting date on payment journal lines
When you use the **Suggest Supplier Payments** batch job to create payment lines for your suppliers, you can fill two special fields to make sure that the generated lines use the due date to calculate the posting date. These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.  

> [!IMPORTANT]  
>   You cannot use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarise per Supplier** field. If the posting date is based on the due date, some payment discounts may not calculate correctly because the posting date is after the payment discount date.  

Also, if the calculated posting date is in the past, then the posting date is moved up to the work date, and a warning is displayed.  

Alternatively, you can manually create payment lines using the due date to calculate the posting date. After you apply supplier ledger entries, you can use the **Calculate Posting Date** action to update the posting date on the journal line with the due date of the related purchase invoice. For more information, see [Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).  

> [!NOTE]  
>   If the purchase invoice is overdue, the posting date is set to the work date, and the font on the line becomes red.  

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Making Payments](payables-make-payments.md)  
[Working with General Journals](ui-work-general-journals.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]