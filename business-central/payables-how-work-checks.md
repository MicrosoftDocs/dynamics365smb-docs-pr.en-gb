---
title: Issue, Print, Cancel, and Void Checks| Microsoft Docs
description: Describes how to issue cheques using the payment journal, print cheques, and void or view cheque ledger entries in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment journal, print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: cbadcd345f1df5dda886a24e058a4aad74e32fdd
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-checks"></a>Work With Cheques
You can issue electronic and manual checks in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Both methods use the payment journal to issue checks to vendors. You can also void cheques and view cheque ledger entries.

The process of issuing cheques suggests payments, creates ledger entries, and prints the computer cheques.

> [!NOTE]  
>   To make sure that your bank only clears validated cheques and amounts, you can send them a file that contains vendor, cheque, and payment information. For more information, see [Export a Positive Pay file](finance-how-positive-pay.md).

Your printer must be correctly set up with the cheque forms, and you must define which cheque layout to use. For more information, see [Define Cheque Layouts](finance-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>To issue cheques
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.
2. Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function. For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).
3. In the **Bank Payment Type** field on journal lines for payment that you want to make with cheques, select one of the following options:

   * **Computer Cheque**: Select this option if you want to print a cheque for the amount on the payment journal line. You must print the checks before you can post the journal lines. You can only select **Computer Cheque** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.
   * **Manual Cheque**: Select this option if you have created a cheque manually and want to create a corresponding cheque ledger entry for this amount. By using this option, you cannot print checks from [!INCLUDE[d365fin](includes/d365fin_md.md)]. You can only select **Manual Cheque** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.

     > [!NOTE]  
     >   You must print computer cheques before you post the related journal lines.
4. In case of computer cheques, choose **Print Cheque**.
5. In the **Check** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
6. Choose the **Print** button.

> [!NOTE]  
>   If you want to print cheques in more than one currency from different bank accounts, you must run the **Print Cheque** batch job separately for each currency and specify the appropriate bank account.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>To cancel printed cheques that are not posted
You can cancel non-posted cheques after they have been printed by using the **Void Cheque** action in the **Payment Journal** window.

1. In the **Payment Journal** window, choose the **Void Cheque**, and then choose which cheques to cancel.

## <a name="to-void-checks"></a>To void cheques
When cheque payment have been posted, you can only cancel (void) cheques from the resulting bank ledger entries.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.
2. Select the relevant bank account, choose the **Edit** action, and then choose the **Cheque Ledger Entries** action.
3. In the **Cheque Ledger Entries** window, choose the **Void Cheque** action.
4. Select the **Void Cheque Only** check box.
5. Choose the **OK** button.

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Setting Up Banking](bank-setup-banking.md)  
[Export a Positive Pay file](finance-how-positive-pay.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

