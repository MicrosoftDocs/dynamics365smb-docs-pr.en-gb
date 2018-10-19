---
title: Service Statistics | Microsoft Docs
description: Get a quick overview of the contents of service documents such as orders, quotes, invoices, or credit memos, the details on the specific service lines, and the service items.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 5af0da45b27c70bc2b25fbad22f83479e9543432
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---

# <a name="viewing-service-statistics"></a>Viewing Service Statistics
You can use statistics to analyse service documents and determine how well you are managing your service processes. You can analyse service contracts, items, quotes, orders, invoices, and credit memos by choosing the **Statistics** action. For service items and contracts, you can also use the **Service Item Trendscape** or **Contract Trendscape** to view a summary of service ledger entries for a specific service item.   

## <a name="viewing-statistics-for-service-orders"></a>Viewing Statistics for Service Orders
The service order statistics feature gives you a quick overview of the contents of the entire service order, the details on the specific service lines, and information related to invoicing, shipping and consuming, and the customer's balance.  

The statistical data is displayed for a service order in the **Service Order Statistics** window for the relevant order. You can open the relevant statistics window from a service order. In the **Service Orders** window, choose **Statistics**. The FastTabs in this window show information such as quantity, amount, VAT, cost, profit, and customer credit limit. The amounts in the window are in the currency of the service order, unless otherwise indicated.  

### <a name="view-totals-for-a-service-order"></a>View totals for a service order  
You can view the total amount on the service lines, including and excluding VAT, VAT part, cost, and profit on the service lines. The window also displays item-specific information, such as weight, volume, and the quantity of parcels.  

### <a name="view-shipping-information"></a>View shipping information  
You can see information about the items, resources, or costs to be shipped. To provide the information, the values specified in the **Qty. to Ship** field are used on each service line in the order.  

### <a name="view-order-details"></a>View order details  
You can view information about the items, resource hours, and costs to be invoiced and consumed. The following table describes this information.  

|Column | Description|  
|------------|---------------------------------------|  
|**Invoicing**|Displays amounts that are to be posted as invoiced from the service order.|  
|**Consuming**|Displays the quantity and cost of items, or resources that will be posted as consumed.|  
|**Total**|Displays the total amounts on the service order that result from adding the invoicing amounts to the consuming amounts.|  

### <a name="analyze-service-order-lines"></a>Analyse service order lines  
You can analyse the information by the types of service lines included in the service order. The amounts are shown separately for:  

* Items  
* Resources  
* Costs and general ledger accounts  

### <a name="view-customer-information"></a>View customer information  
See the balance on the customer's account, in addition to the maximum credit that can be endued to the customer who you created the service document for.

## <a name="viewing-service-item-statistics"></a>Viewing Service Item Statistics
In the **Service Item Statistics** window, you can see up-to-date information about a service item based the following service ledger entry types:  

* Resources  
* Items  
* Service cost  
* Service contracts  
* Total  

For each entry type, you can see the invoiced amount, usage (amount), cost amount, quantity, quantity invoiced and quantity consumed, profit amount and profit percentage. The profit percentage is calculated according to the following formula:  

* (Invoiced Amount - Usage (Cost)) x 100 / Invoiced Amount  

## <a name="using-trendscapes"></a>Using Trendscapes
For service items and service contracts, the **Service Item Trendscape** or **Service Contract Trendscape** windows provides a scrollable summary of service ledger entries in a period of time for a specific service item or contract. To view the trendscape, open the service item or service contract, choose the **Statistics** action, and then choose **Trendscape**.

When you scroll the list, the amounts are calculated in the local currency according to the specified time interval. All amounts are calculated from service ledger entries, which are entries that are created when you post service orders or service invoices.

You can filter the list by specifing the service items to include.  

> [!Tip]  
>  If you have set the time interval to **Day** and you want to scroll over a long period, you can do it faster by shifting to a larger interval such as **Quarter**. When you have found the desired period, you can shift back to the original interval to see the data in more detail.   

## <a name="viewing-gains-and-losses-on-contracts"></a>Viewing Gains and Losses on Contracts  
A contract gain or loss entry is generated when a contract quote is converted to a service contract, when contract lines are added or removed from a service contract, or when a contract is cancelled. You can view contract gains or losses on the following pages.  

|Page | Description|  
|----------------|---------------------------------------|  
|**Contract Gain/Loss (Contracts)**|To view the contract gain/loss by service contract.|  
|**Contract Gain/Loss (Groups)**|To view the contract gain/loss by service contract group.|  
|**Contract Gain/Loss (Customers)**|To view the contract gain/loss by customer.|  
|**Contract Gain/Loss (Reasons)**|To view the contract gain/loss by reason code.|  
|**Contract Gain/Loss (Resp.Ctr)**|To view the contract gain/loss by responsibility centre.|  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter the name of the page to display, and then choose the related link.  
2. Fill in the filter criteria you want to apply. For example, in the **Contract Gain/Loss (Reasons)** window, choose a value for **Reason Code Filter**.  
3. Choose the **Show Matrix** action.

## <a name="viewing-statistics-for-posted-service-documents"></a>Viewing Statistics for Posted Service Documents
The service statistics feature lets you gain a statistical overview of the contents of posted service documents, such as a posted shipment, posted invoice, and posted credit memo.  

The statistical information is displayed in the statistics window for the corresponding posted service document. You can open the relevant statistics window from posted service shipment, posted service invoice, or posted service credit memo documents. For each of these document types, in the **Home** tab, in the **Process** group, choose **Statistics**. For example, from the **Posted Service Invoices** window, on the **Home** tab, in the **Process** group, choose **Statistics**.  

### <a name="posted-service-shipment-statistics"></a>Posted Service Shipment Statistics  
The **Service Shipment Statistics** window provides an overview of a posted service shipment. This includes information about the physical contents of the shipment, such as quantity of the shipped items, resource hours or costs, and weight and volume of the shipped items.  

### <a name="posted-service-invoice-statistics"></a>Posted Service Invoice Statistics  
You can see a statistical summary on a posted service invoice in the **Service Invoice Statistics** window. You can view the totals of the posted service invoice. The data includes total amount on the service lines (including and excluding VAT) that has been posted as invoiced, VAT part, cost, and profit on the posted invoice. The window also displays information about the following:  

* The items on the service invoice lines, such as weight, volume, and the quantity of parcels.  
* The balance on the customer's account, and the maximum credit that you can extend the customer.  

### <a name="posted-service-credit-memo-statistics"></a>Posted Service Credit Memo Statistics  
You can use the **Service Credit Memo Statistics** window to get a statistical overview of the lines in a posted service credit memo. The overview can include:

* The total amounts on the posted credit memo, displayed as quantity, amount, VAT, cost and profit. There is also information about the items on the service lines of the posted credit memo, such as quantity, weight, and volume.  
* General information about the customer, such as the customer's credit limit and balance on the account.  

## <a name="see-also"></a>See Also  
[Create Service Orders](service-how-to-create-service-orders.md)   
[Create Service Items](service-how-to-create-service-items.md)   
[Planning Service](service-plan-service.md)  

