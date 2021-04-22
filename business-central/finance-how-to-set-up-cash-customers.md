---
title: How to Set Up Cash Customers | Microsoft Docs
description: This topic describes the steps to set up customer who pays in cash.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: f047876678d26e7e53bf304433f38a410ba7d7fa
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5770398"
---
# <a name="set-up-cash-customers"></a>Set Up Cash Customers
You cannot create an invoice without a customer number. This is true, even if you make a cash sale and do not have anything to record in a customer account.  

## <a name="to-set-up-a-cash-customer"></a>To set up a cash customer  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer**, and then choose the related link.  
2.  Create a new **Customer** card. For more information, see [Register New Customers](sales-how-register-new-customers.md).
3.  In the **No.** field, enter **Cash**, for example.  
4.  In the **Name** field, enter **Cash Sale**, for example.  
5.  On the **Invoicing** FastTab, fill in the **Customer Posting Group** and the **Gen. Bus. Posting Group** fields.  

 Now you have set up a customer that contains sufficient information for invoicing.  

> [!NOTE]  
>  You may have chosen a posting group that is also used for domestic credit sales. If you want to maintain separate data on cash sales, for example, with a special sales or receivables account, you can set up an extra posting group for this purpose.  
>   
>  You must enter a number for a receivables account for the posting group, even though the balance in this account will always be 0 after you post an invoice.  

## <a name="see-also"></a>See Also
[Managing Receivables](receivables-manage-receivables.md)  
[Register New Customers](sales-how-register-new-customers.md)    
[Finance](finance.md)  



[!INCLUDE[footer-include](includes/footer-banner.md)]