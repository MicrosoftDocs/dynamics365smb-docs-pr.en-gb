---
title: How to Work with Stock Periods | Microsoft Docs
description: You can control the timeframe in which people can post post changes to stock by defining stock periods.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7d946020bb6f9a1eabf5ab68d3dd64a9af344993
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6442067"
---
# <a name="work-with-inventory-periods"></a>Work with Stock Periods
Stock periods define a period of time in which you can post changes to stock. a Stock period is defined by the date on which it ends, or the ending date. When you close a stock period, you cannot post any changes to stock, either expected or invoiced, before this ending date. You cannot post any new values to stock before the ending date. If you have open item entries in the closed period, meaning positive quantities that have not yet been applied to outbound transactions, you can still apply outbound quantities to these entries, even if the period is closed.  

The following sections describe how to:

* Create stock periods.  
* Close stock periods.  
* Reopen stock periods.  

## <a name="to-create-an-inventory-period"></a>To create a stock period  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stock Periods**, and then choose the related link.  
2. Create a new line.  
3. In the **Ending Date** field, enter the last date in the stock period that you want to define. When the period is closed, you will not be able to post stock changes before this date.  
4. Enter a descriptive name in the **Name** field. Choose the **OK** button.  

## <a name="closing-inventory-periods"></a>Closing Stock Periods  
The **Closed** field indicates whether or not the stock period is closed to stock value changes. You cannot edit this field.  

You can close any stock period, provided that the following is true:  

* There are no open outbound item ledger entries, meaning negative stock, in that period.  
* The cost of all items has been adjusted using the **Adjust Cost – Item Entries** batch job.  

This means that all outbound transaction quantities, such as those from sales orders, outbound transfers, sales invoices, purchase returns, or purchase credit memos, must be applied to existing quantity in stock.  

### <a name="to-close-an-inventory-period"></a>To close a stock period  
1. Before closing a stock period, choose the **Adjust Cost – Item Entries** action to ensure that all cost adjustments are posted.

     Run the **Close Stock Period – Test** report to determine if there are any open outbound item entries within the stock period or any items whose cost has not yet been adjusted.  
2. Choose the **Close Stock Period – Test** action.  

     Run the **Post Stock Cost to G/L** batch job to ensure that all costs are posted to the general ledger.  
3. Choose the **Post Stock to G/L** action.  
4. On the **Stock Periods** page, select the stock period you want to close.  
5. Choose the **Close Period** action. After the stock period has been closed, you cannot post stock changes before the ending date. The cost of all items must be adjusted with the **Adjust Cost – Item Entries** batch job before you close the stock period.  
6. Choose the **Yes** button to confirm that you want to close the period, or choose **No** to cancel the closing.  
7. The stock period is closed and a confirmation message is displayed when it is finished.  

## <a name="reopening-inventory-periods"></a>Reopening Stock Periods  
After you have closed the stock period, you cannot delete the stock period. You can, however, reopen it, if you would like to allow posting before the ending date of the stock period. Reopening a period also reopens all stock periods with ending dates later than the period you reopen.  

### <a name="to-reopen-an-inventory-period"></a>To reopen a stock period  
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stock Periods**, and then choose the related link.  
2. Select the stock period you want to reopen.  
3. Choose the **Reopen Period** period action. Confirm that you want to reopen the period.  
4. All stock periods with ending dates later than the period you selected are reopened.  

## <a name="see-also"></a>See Also  
[Design Details: Stock Periods](design-details-inventory-periods.md)  
[Finance](finance.md)  
[Stock](inventory-manage-inventory.md)  
[Working with Financials](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]