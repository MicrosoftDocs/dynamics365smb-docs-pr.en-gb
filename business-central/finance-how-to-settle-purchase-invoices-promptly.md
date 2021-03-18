---
title: Settle Purchase Invoices Promptly
description: If you need to pay the vendor by cash or cheque, you can have the necessary posting done when you post the invoice.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/06/2020
ms.author: bholtorf
ms.openlocfilehash: 60d3cf3c9e141c8df36eaca2c1975b696fdb105b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5387256"
---
# <a name="settle-purchase-invoices-promptly"></a>Settle Purchase Invoices Promptly

If you need to pay the vendor by cash or cheque, you can post the payment when you post the invoice.  

> [!NOTE]  
> If you frequently pay purchase invoices in cash, by cheque or via bank transfer, it is a good idea to set up a specific payment method with a balancing account and enter this method in the **Payment Method** field on the vendor card. The balancing account number is inserted automatically on the invoice header every time you create a new invoice. For more information, see [Defining Payment Methods](finance-payment-methods.md).  

## <a name="to-settle-purchase-invoices-promptly"></a>To settle purchase invoices promptly

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.  
2. Choose the **New** action.  
3. To pay either in cash or by bank transfer, enter the number of the general ledger cash account or the bank account in the **Bal. Account No.** field.  

> [!IMPORTANT]  
> The **Bal. Account Type** and **Bal. Account No.** fields are not included in the standard layout of the invoice header. In order to post the payment of an invoice, you must contact a Microsoft partner who can add the fields through code.  
>
> This customisation is only required if you do not specify balancing accounts on the payment methods as describe above.

## <a name="see-also"></a>See Also

[Managing Payables](payables-manage-payables.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]