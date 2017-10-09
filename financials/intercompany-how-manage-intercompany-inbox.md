---
title: Process Incoming and Outgoing IC Transactions| Microsoft Docs
description: Intercompany transactions that you receive from your intercompany partners are listed in the intercompany inbox where you process them manually or automatically.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoming document
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5cf49fa7b1c2d4385cd05f44e10237078e1214a4
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-manage-the-intercompany-inbox-and-outbox"></a>How to: Manage the Intercompany Inbox and Outbox
All of the intercompany transactions that you receive electronically from your intercompany partners are listed in the intercompany Inbox.  

## <a name="organizing-the-inbox"></a>Organizing the Inbox  
 You can use the filter fields at the top of the inbox window to determine which transactions are shown in the window. For example, if you only want to look at transactions a particular partner created, you can enter filters in the **Transaction Source** and **Intercompany Partner Code** filters.  

### <a name="transaction-source"></a>Transaction Source  
What you can do with a transaction depends whether it was:  

- Created by your intercompany partner  
- Rejected by your intercompany partner and returned to you  

You can use the **Show Transaction Source** field to filter the **Intercompany Inbox Transactions** window so that it displays only one of these types of transactions. (You can also filter by intercompany partner, or by the contents of the **Line Action** field.)  

#### <a name="created-by-intercompany-partner"></a>Created by Intercompany Partner  
 When you receive a new transaction that was created by your partner, you can choose to either:

- Accept the transaction  
- Reject the transaction (Return to partner)  
- Cancel the transaction (Delete the transaction but do not return it to your partner)  

#### <a name="returned-from-intercompany-partner"></a>Returned from Intercompany Partner  
 If the transaction was rejected by your intercompany partner, your only choice is to cancel the transaction in the inbox. Then you must create correction lines or reverse the journal or document in your company.  

## <a name="re-creating-inbox-entries"></a>Re-creating Inbox Entries  
 If you accepted a transaction in your inbox but then deleted the document or journal instead of posting it, you can re-create the inbox entry and accept it again.  

## <a name="getting-an-overview-of-intercompany-transactions-for-a-period"></a>Getting an Overview of Intercompany Transactions for a Period  
 You can get an overview of all of the intercompany transactions that you have sent and received in a period. The **Intercompany Transactions** report lists all intercompany G/L entries, customer ledger entries, and vendor ledger entries.

 > [!NOTE]  
 > If the intercompany partners are in the same database, then transactions are transferred without the need for file or email. See the **Transfer Type** field in the **Intercompany Partner** window. <br /><br />
In that case, you can set the system up to bypass the inbox and outbox by selecting the **Auto. Accept Transactions** check box in the **Intercompany Partner** window and the **Auto. Send Transactions** check box in the **Intercompany Setup** window respectively.

## <a name="to-import-intercompany-transactions-from-a-file"></a>To import intercompany transactions from a file  
If you have an intercompany partner that is not in the same database as your company, you can receive intercompany transactions from that partner in an .xml file. Then you must import the transactions into your inbox.  

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information** , and then choose the related link.
2. Save the file to the location that you specified in the **Intercompany Inbox Details** field in the **Company Information** window.  
3. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intercompany Inbox Transactions**, and then choose the related link.
4. In the **Intercompany Inbox Transactions** window, choose the **Import Transaction File** action.  
5. In the window that appears, select the .xml file that contains the transactions, and then choose the **Open** button.  

The transactions are imported into the inbox and you can now process them.

## <a name="to-process-incoming-intercompany-transactions"></a>To process incoming intercompany transactions  
When your intercompany partners send you intercompany transactions, the transactions end up in your intercompany inbox. You must evaluate each transaction in your inbox and act upon it.  

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intercompany Inbox Transactions**, and then choose the related link.  
2. In the **Intercompany Inbox Transactions** window, select a line, and then choose an action, such as **Accept**, to process the line.
3. In the **Complete IC Inbox Action** window, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choose the **OK** button.  

For lines that you processed with the **Accept** action, document or journal lines will be created in your company. Open each document or journal, make any necessary changes, and then post them.  

Lines that you processed with the **Return to Partner** action will be moved to the outbox from where you can then send them to your partner.

For lines that you processed with the **Returned by Partner** action, you must now post a correction to the original transaction that you posted in your company.

## <a name="to-process-outgoing-intercompany-transactions"></a>To process outgoing intercompany transactions  
When you post an intercompany journal or document, or send an intercompany order confirmation, the transactions are sent to your intercompany outbox. In order for them to be sent on to your intercompany partners, you must open the outbox and process them.  

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intercompany Outbox Transactions**, and then choose the related link.  
2. In the **Intercompany Outbox Transactions** window, select a line, and then choose an action, such as **Return to Inbox**, to process the line.

Lines that you processed with the **Send to Intercompany Partner** action will be sent to the relevant partner's inbox.

Lines that you processed with the **Return to Inbox** action will be moved to the inbox where you can then accept them to create documents or journal lines in your company.  

For lines that you processed with the **Cancel** action, you must now post a correction to the original transaction that you posted in your company.  

## <a name="to-recreate-intercompany-inbox-transactions"></a>To recreate intercompany inbox transactions  
Occasionally, you may want to re-create a transaction in the inbox or outbox. For example, if you accepted a transaction in your inbox but then deleted the document or journal instead of posting it, you can re-create the inbox entry and accept it again.  

The following procedure describes to re-create inbox transactions, but the same steps also apply to the outbox.

  1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Handled IC Inbox Transactions**, and then choose the related link.  

  2.  In the **Handled IC Inbox Transactions** window, select the line with the transaction that you want to re-create in the inbox, and then choose the **Re-create Inbox Transaction** action.  

## <a name="see-also"></a>See Also
[Managing Intercompany Transactions](intercompany-manage.md)  
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[Working with General Journals](ui-work-general-journals.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

