---
title: Set Up Payment Methods (contains video)
description: You use payment methods, for example, cheque, bank transfer, cash, or PayPal, to define how sales and purchase invoices will be paid.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, bank transfer, cash, PayPal
ms.search.form: 427
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: abe1d874658c393b0d9795c1710e642b4e33add0
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2022
ms.locfileid: "8512965"
---
# <a name="set-up-payment-methods"></a>Set Up Payment Methods

Payment methods define the way you prefer for customers to pay you, and how you like to pay your suppliers. The method can vary for each customer or supplier. Examples of typical payment methods are **bank**, **cash**, **cheque**, or **account**.

You can assign a payment method to customers and suppliers so that the same method is always used on the sales and purchase documents you create for them. If needed, you can change the method on the sales or purchase document. For example, if you want to pay a particular purchase invoice in cash rather than by cheque. This does not change the default payment method assigned to the supplier.

The same payment methods are used for sales and purchase documents. For example, a _cash_ payment method is used both when you make payments and when you receive them. [!INCLUDE[prod_short](includes/prod_short.md)] knows that when you are creating a sales invoice you expect to receive payment, and the opposite for purchase invoices.

Credit memos for returns, however, are exceptions because money is flowing in the opposite directions, from you to your customer and from your supplier to you. Therefore, a default payment method is not assigned to credit memos. There is, however, a workaround if you have specified terms of payment for the customer or supplier. Though the **Calc. Pmt. Disc. on Cr. Memos** field is not intended for this, if you choose the check box on the **Payment Terms** page a default payment method will be added when you create a credit memo. <br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE476Ys?rel=0]

## <a name="to-set-up-a-payment-method"></a>To set up a payment method

[!INCLUDE[prod_short](includes/prod_short.md)] provides a few payment methods that businesses often use. You can, however, add as many as you need.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Methods**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Optionally, add payment terms to your payment method. For more information, see [Set Up Payment Terms](finance-payment-terms.md).  

## <a name="to-assign-a-payment-method-to-a-customer-or-vendor"></a>To assign a payment method to a customer or supplier

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer** or **Supplier**, and then choose the related link.
2. In the **Payment Method Code** field, choose the method to use by default for the customer or supplier.

## <a name="see-also"></a>See Also

[Register New Customers](sales-how-register-new-customers.md)  
[Set Up Payment Terms](finance-payment-terms.md)  
[Finance](finance.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]