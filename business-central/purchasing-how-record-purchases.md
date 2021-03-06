---
title: Record Purchases with Purchase Invoices
description: Describes how to purchase stock, non-stock items, or resources by creating and posting purchase invoices or orders.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3822566d239d6fda0cc314a3c9f20ac909943886
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115847"
---
# <a name="record-purchases-with-purchase-invoices"></a>Record Purchases with Purchase Invoices

You create a purchase invoice or purchase order to record the cost of purchases and to track purchase ledger. If you need to control an stock, purchase invoices and purchase orders are also used to dynamically update stock levels so that you can minimise your stock costs and provide better customer service. The purchasing costs, including service expenses, and stock values that result from posting purchase invoices or orders contribute to profit figures and other financial KPIs on your Role Centre.

## <a name="create-purchase-invoices"></a>Create purchase invoices

In addition to buying physical items (**Stock** item type), which affect stock valuation, you can purchase services represented by time units. You can do this either with the **Service** item type or with the **Resource** line type.

> [!NOTE]  
> You must use purchase orders if your purchasing process requires that you record partial receipts of an order quantity, for example, because the full quantity was not available at the supplier. If you sell items by delivering directly from your supplier to your customer, as a drop shipment, then you must also use purchase orders. For more information, see [Make Drop Shipments](sales-how-drop-shipment.md). In all other aspects, purchase orders work the same way as purchase invoices. The following procedure is based on a purchase invoice. The steps are similar for a purchase order.

When you receive the stock items or when the purchased service is completed, you post the purchase invoice or order to update stock and financial records and to activate payment to the supplier according to the payment terms. For more information, see [Posting Purchases](ui-post-purchases.md) and [Making Payments](payables-make-payments.md).

> [!CAUTION]  
> Do not post a purchase invoice for physical items until you receive the items and know the final cost of the purchase, including any additional charges. Otherwise, your stock value and profit figures may be skewed.

The item card can be of type **Stock**, **Service**, and **Non-stock** to specify if the item is a physical stock unit, a labour time unit, or a physical unit that is not kept on stock. For more information, see [Register New Items](inventory-how-register-new-items.md). The purchase invoice process is the same for all three item types.

> [!NOTE]
> With the **Resource** purchase line type, you can also purchase external resources, for example, to invoice a supplier for work delivered. For more information, see [Set Up Resources](projects-how-setup-resources.md).
>
> To use a purchased resource, you may need to set the resource's capacity and manually assign it to a job. Purchasing a resource will create a resource ledger entry, however, resource ledger entries are not tracked for quantity and value as, for example, items are. If quantity and value tracking is required, then consider using other line item types.

You can fill supplier fields on the purchase invoice in two ways depending on whether the supplier is already registered.
<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE4b3tt?rel=0]

### <a name="to-create-a-purchase-invoice"></a>To create a purchase invoice

The following describes how to create a purchase invoice. The steps are similar for a purchase order. The main difference is that purchase orders have additional fields and actions for physical handling of items.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.  
2. In the **Supplier** field, enter the name of an existing supplier.

    Other fields on the **Purchase Invoice** page are now filled with the standard information of the selected supplier. If the supplier is not registered, then follow these steps:

    1. In the **Supplier** field, enter the name of the new supplier.
    2. In the dialogue box about registering the new supplier, choose the **Yes** button.
    3. On the **Select a template for a new supplier** page, choose a template to base the new supplier card on, and then choose the **OK** button.
    4. A new supplier card opens, prefilled with the information on the selected supplier template. The **Name** field is prefilled with the new supplier's name that you entered on the purchase invoice.
    5. Proceed to fill in the remaining fields on the supplier card. For more information, see [Register New Suppliers](purchasing-how-register-new-vendors.md).  
    6. When you have completed the supplier card, choose the **OK** button to return to the **Purchase Invoice** page.

    Several fields on the **Purchase Invoice** page are filled with information that you specified on the new supplier card.
3. Fill in the remaining fields on the **Purchase Invoice** page as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    You are now ready to fill in the purchase invoice lines with items or resources that you have purchased from the supplier.

    > [!NOTE]  
    > If you have set up recurring purchase lines for the supplier, such as a monthly replenishment order, then you can insert these lines on the invoice by choosing the **Get Recurring Purchase Lines** action.
4. On the **Lines** FastTab, in the **Item No.** field, enter the number of an stock item or service.
5. In the **Quantity** field, enter the number of items to be purchased.

    > [!NOTE]  
    > For items of type **Service** and for lines of type **Resource**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measurement Code** field on the line.

    The **Line Amount** field is updated to show the value in the **Direct Unit Cost** field multiplied by the value in the **Quantity** field.

    The price and line amount are shown with or without VAT depending on what you selected in the **Prices Including Tax** field on the supplier card.

    The totals fields under the lines are automatically updated as you create or modify lines to display the amounts that will be posted to the ledgers.

    > [!NOTE]
    > In rare cases, the posted amounts may deviate from what is displayed in the totals fields. This is typically due to rounding calculations in relation to VAT or sales tax.
    >
    > To check the amounts that will actually be posted, you can use the **Statistics** page, which takes into account the rounding calculations. Also, if you choose the **Release** action, the totals fields will be updated to include rounding calculations.

6. In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. VAT** field at the bottom of the invoice.

    > [!NOTE]  
    > If you have set up invoice discounts for the supplier, then the specified percentage value is automatically inserted in the **Supplier Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Invoice Discount Amount** field.
7. When you receive the purchased items or services, choose **Post**.

The purchase is now reflected in stock, resource ledgers, and financial records, and the supplier payment is activated. The purchase invoice is removed from the list of purchase invoices and replaced with a new document in the list of posted purchase invoices.  

## <a name="posted-invoices"></a>Posted invoices

[!INCLUDE [posted-invoices](includes/posted-invoices.md)]

You can easily correct or cancel a posted purchase invoice before you pay the supplier. This is useful if you want to correct a typing mistake or if you want to change the purchase early in the order process. For more information, see [Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md). If you have already paid for items or services on the posted purchase invoice, then you must create a purchase credit memo to reverse the purchase. For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).

[Open the **Posted Purchase Invoices** list](https://businesscentral.dynamics.com/?page=146) in [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="external-document-number"></a>External document number

[!INCLUDE [ext-doc-no-purch](includes/ext-doc-no-purch.md)]

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/processing-invoices-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Purchasing](purchasing-manage-purchasing.md)  
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Set Up Resources](projects-how-setup-resources.md)  
[Posting Purchases](ui-post-purchases.md)  
[Request Quotes](purchasing-how-request-quotes.md)  
[Purchase Items for a Sale](purchasing-how-purchase-products-sale.md)  
[Register New Suppliers](purchasing-how-register-new-vendors.md)  
[Prepare Drop Shipments](sales-how-drop-shipment.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]