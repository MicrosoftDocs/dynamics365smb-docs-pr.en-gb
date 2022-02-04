---
title: 'Issue, Print, Cancel, and Void Cheques'
description: 'Describes how to issue cheques using the payment journal, print cheques, and void or view cheque ledger entries in Business Central.'
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'payment journal, print check, vendor payment, creditor, debt, balance due, AP'
ms.search.form: '256, 404,'
ms.date: 04/01/2021
ms.author: edupont
---
# <a name="make-check-payments"></a>Make Cheque Payments

You can issue electronic and manual checks in [!INCLUDE[prod_short](includes/prod_short.md)]. Both methods use the payment journal to issue checks to suppliers. You can also void cheques and view cheque ledger entries.

The following procedure shows how to pay a supplier with a computer cheque by applying the payment to the relevant supplier invoice, printing the cheque, and then posting the payment as paid. This results in positive supplier ledger entries, applied to negative bank ledger entries, and physical cheques for processing in the bank.

You can pay with two types of cheque. For both types, the **Bal. Account Type** or the **Account Type** field must contain **Bank Account**.

- **Computer Cheque**: Select this option if you want to print a cheque for the amount on the payment journal line. You must print the cheques before you can post the journal lines.
- **Manual Cheque**: Select this option if you have created a cheque manually and want to create a corresponding cheque ledger entry for this amount. By using this option, you cannot print the cheque.

> [!NOTE]  
> To make sure that your bank only clears validated cheques and amounts, you can send them a file that contains supplier, cheque, and payment information. For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).

> [!IMPORTANT]
> Your printer must be correctly set up with the cheque forms, and you must define which cheque layout to use. For more information, see [Select a Cheque Layout](finance-how-define-check-layouts.md). Alternatively, you can send the cheque as a PDF file, for example.  

You can print up to 10 invoices on a page for a cheque stub. If a cheque applies to more than 10 invoices, when you print the stub we void the cheque on the first page and print the word VOID on the cheque. We then print the remainder of the invoices and the total cheque amount on the second page.

## <a name="to-pay-a-vendor-invoice-with-a-computer-check"></a>To pay a supplier invoice with a computer cheque
The following describes how to pay a supplier by cheque. The steps are similar to refund a customer by cheque.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.
2. Fill in the payment journal lines. For more information, see [Record Payments and Refunds](payables-how-post-payments-refunds.md).
3. In the **Payment Method Code** field, select **Cheque**.
4. In the **Bank Payment Type** field, select **Computer Cheque**.
5. Choose the **Print Cheque** action.
6. On the **Cheque** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. If your printer is set up to print cheques, choose the **Print** button. Otherwise, choose the **Send to** button, select the **PDF Document** option, choose the **OK** button, and then print the PDF document.

    The physical cheques can now be sent to the suppliers for processing. Proceed to post the payment as applied to the supplier and thereby paid in the system.
8. Choose the **Post** action.

Fully applied supplier ledger entries and bank ledger entries are created.

> [!NOTE]  
> If you want to print and pay cheques in more than one currency from different bank accounts, you must run the **Print Cheque** batch job separately for each currency and specify the appropriate bank account.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>To cancel printed cheques that are not posted
You can cancel non-posted cheques after they have been printed by using the **Void Cheque** action on the **Payment Journal** page.

1. On the **Payment Journal** page, choose the **Void Cheque**, and then choose which cheques to cancel.

## <a name="to-void-checks"></a>To void cheques

When cheque payment have been posted, you can only cancel (void) cheques from the resulting bank ledger entries.

> [!IMPORTANT]
> If the cheque is applied to an invoice, unapply the cheque first so that the invoice can be repaid, and then void the cheque. If the cheque was printed and did not pay an invoice, then choose **Void Cheque Only** as described in this section.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.
2. Select the relevant bank account, choose the **Edit** action, and then choose the **Cheque Ledger Entries** action.
3. On the **Cheque Ledger Entries** page, choose the **Void Cheque** action.
4. Select the **Void Cheque Only** check box.
5. Choose the **OK** button.

## <a name="to-view-a-summary-of-posted-checks"></a>To view a summary of posted cheques
If you want to review posted cheques, for example to verify multiple cheques paid to one supplier, you can use the **Bank Account - Cheque Details** report.
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Account - Cheque Details**, and then choose the related link.
2. Set filters as relevant, and then choose the **Preview** button.

## <a name="see-also"></a>See Also
[Making Payments](payables-make-payments.md)  
[Managing Payables](payables-manage-payables.md)  
[Setting Up Banking](bank-setup-banking.md)  
[Export a Positive Pay file](finance-how-positive-pay.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]