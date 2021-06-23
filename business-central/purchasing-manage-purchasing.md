---
title: Overview of Tasks to Manage Purchasing
description: Outlines tasks to manage your purchasing or procurement processes, including how purchase invoices and purchase orders work.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement, supply, vendor order
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 929e1d62a091c4a01aa6f5e03dd5fcbdaa5bf7c0
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115797"
---
# <a name="purchasing"></a>Purchasing
You create a purchase invoice or purchase order to record the cost of purchases and to track purchase ledger. If you need to control an stock, purchase invoices are also used to dynamically update stock levels so that you can minimise your stock costs and provide better customer service. The purchasing costs, including service expenses, and stock values that result from posting purchase invoices contribute to profit figures and other financial KPIs on your Role Centre.

You must use purchase orders if your purchasing process requires that you record partial receipts of an order quantity, for example, because the full quantity was not available at the supplier. If you sell items by delivering directly from your supplier to your customer, as a drop shipment, then you must also use purchase orders. For more information, see [Make Drop Shipments](sales-how-drop-shipment.md). In all other aspects, purchase orders work the same way as purchase invoices.

You can have purchase invoices created automatically by using the OCR (Optical Character Recognition) service to convert PDF invoices from your suppliers to electronic documents, which are then converted to purchase invoices by a workflow. To use this functionality, you must first sign up for the OCR service, and then perform various setup. For more information, see [Process Incoming Documents](across-process-income-documents.md).      

Products can be both stock items and services. For more information, see [Register New Items](inventory-how-register-new-items.md).

For all purchase processes, you can incorporate an approval workflow, for example, to require that large purchases are approved by the accounting manager. For more information, see [Using Approval Workflows](across-how-use-approval-workflows.md).

The following table describes a sequence of tasks, with links to the topics that describe them.

| To | See |
| --- | --- |
| Create a purchase invoice to record your agreement with a supplier to purchase products on certain delivery and payment terms. |[Record Purchases](purchasing-how-record-purchases.md) |
|Create a purchase quote to reflect a request for quote from your supplier, which you can later convert to a purchase order.|[Request Quotes](purchasing-how-request-quotes.md)|
| Create a purchase invoice for all or selected lines on a sales invoice. |[Purchase Items for a Sale](purchasing-how-purchase-products-sale.md) |
|Understand what happens when you post purchase documents.|[Posting Purchases](ui-post-purchases.md)|
| Perform an action on an unpaid posted purchase invoice to automatically create a credit memo and either cancel the purchase invoice or recreate it so you can make corrections. |[Correct or Cancel Unpaid Sales Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Create a purchase credit memo to revert a specific posted purchase invoice to reflect which products you are returning to the supplier and which payment amount you will collect. |[Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Prepare to invoice multiple receipts from the same supplier once by combining the receipts on one invoice.|[Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
|Convert, for example, electronic invoices from your suppliers to purchase invoices inside Business Central.|[Receive and Convert Electronic Documents](purchasing-how-to-receive-and-convert-electronic-documents.md)|
| Learn how [!INCLUDE[prod_short](includes/prod_short.md)] calculates when you must order an item to receive it on a certain date.|[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md)|
|Resolve confusion when two or more records exist for the same supplier.|[Merge Duplicate Records](sales-how-merge-duplicate-records.md)|
|Manage your commitment to a supplier to purchase large quantities delivered in several shipments over time.|[Work With Blanket Purchase Orders](sales-how-to-create-blanket-sales-orders.md)|

## <a name="external-document-numbers"></a>External document numbers

[!INCLUDE [ext-doc-no-purch](includes/ext-doc-no-purch.md)]

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/paths/purchase-items-services-dynamics-365-business-central/)

## <a name="see-also"></a>See Also
[Setting Up Purchasing](purchasing-setup-purchasing.md)  
[Register New Suppliers](purchasing-how-register-new-vendors.md)  
[Managing Payables](payables-manage-payables.md)  
[Managing Projects](projects-manage-projects.md)    
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[General Business Functionality](ui-across-business-areas.md)

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]