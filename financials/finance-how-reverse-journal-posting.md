---
title: Undo a Posting by Posting a Reversing Entry| Microsoft Docs
description: If you have made an erroneous posting in the general journal, then you can use the Reverse Transaction function to undo the posting with a correct audit trail.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 92c0bca970250b8f160ecfc15b086963c8693885
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="reverse-postings"></a>Reverse Postings
To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry. After reversing an entry, you must make the correct entry.

You can only reverse entries that are posted from a general journal line. An entry can only be reversed once.

For more information about posting from a general journal, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).

If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.

If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a>To reverse the journal posting of a general ledger entry
You can reverse entries from all **Ledger Entries** windows. The following procedure is based on the **General Ledger Entries** window.
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.
2. Select the entry that you want to reverse, and then choose the **Reverse Transaction** action. Note that is must originate from a journal posting.
3. In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.
4. Choose the **Yes** button on the confirmation message.

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a>To undo a quantity posting on a posted purchase receipt  

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.  
2.  Open the posted receipt that you want to undo.  
3.  Select the line or lines that you want to undo.  
4.  Choose **Undo Receipt** action.

    A corrective line is inserted under the selected receipt line.  

    If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.  

    The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a>To undo and then redo a quantity posting on a posted return shipment

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.  
2.  Open the posted return shipment that you want to undo.
3. Select the line or lines you want to undo.  

4.  Choose the **Undo Return Shipment** action.  

    A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.  

    Now go back to the purchase return order to redo the posting.  

5.  In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.** field.  
6.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then select the related link.  
7.  Open the return order in question, and then choose the **Reopen** action.  
8.  Correct the entry in the **Quantity** field and post the purchase return order again.  

## <a name="see-also"></a>See Also
[Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md)  
[Working with General Journals](ui-work-general-journals.md)  
[Finance](finance.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

