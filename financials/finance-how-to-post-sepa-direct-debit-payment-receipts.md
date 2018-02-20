---
title: Post SEPA Direct Debit Payments | Microsoft Docs
description: When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 0031017c96172dca76b50542e52c6a437c01427a
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="post-sepa-direct-debit-payment-receipts"></a>Post SEPA Direct Debit Payment Receipts
When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices. For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).  

You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window. Alternatively, you can relay the work to another user by preparing the related journal lines.  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-window"></a>To post a direct-debit payment receipt from the Direct Debit Collections window  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.  
2. Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank. For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).  
3. Choose the **Post Payment Receipts** action.  
4. In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Direct Debit Collection No.**|Specify the direct debit collection that you want to post payment receipt for.|  
    |**General Journal Template**|Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.|  
    |**General Journal Batch Name**|Specify which general journal batch to use for posting the payment receipt.|  
    |**Create Journal Only**|Select this check box if you do not want to post the payment receipt when you choose the **OK** button. The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.|  

5. Choose the **OK** button.  

## <a name="see-also"></a>See Also  
 [Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)   
 [Sales](sales-manage-sales.md)

