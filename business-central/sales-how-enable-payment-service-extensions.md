---
title: Enable Customer Payments Through Payment Services| Microsoft Docs
description: Make it easier for customers to pay their invoices by enabling payment services.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0154f7fc231023542cc5f389ea6c8a3e99c7fffc
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="enable-customer-payments-through-payment-services"></a>Enable Customer Payments Through Payment Services
As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.  

After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers. Customers can use the link to go to the payment service and pay the bill, directly from the sales document. If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.  

The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a>To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Services**, and then choose the related link.  
2. In the **Payment Services** window, choose the **New** action.  
3. Select the payment service, and then close the window.  
4. In the **Payment Services** window, choose the **Setup** action.  
5. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. Close the window.  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a>To select a payment service on a sales invoice
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.  
2. Open the sales invoice that you want to pay by using the payment service.  
3. In the **Payment Service** field, choose the payment service.  

    > [!NOTE]  
    > The **Payment Service** field is available only if you've enabled the payment service.  

## <a name="see-also"></a>See Also  
[Setting Up Sales](sales-setup-sales.md)  
[Sales](sales-manage-sales.md)  
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

