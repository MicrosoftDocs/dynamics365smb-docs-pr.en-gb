---
title: How to Block Sales to Customers  Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: a2dee70270df135bc61ddef38e661758431b02a9
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251361"
---
# <a name="block-customers"></a>Block Customers
You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.

In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders. For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).   

The following table describes the different blocking options.  

|Option|Description|  
|--------------------|------------|  
|**Blank**|Transactions are allowed for this customer.|
|**Ship**|New orders and new shipments cannot be created for this customer. Existing shipments not yet invoiced can be invoiced.|  
|**Invoice**|New orders, new shipments, and new invoices cannot be created for this customer. Existing shipments not yet invoiced cannot be invoiced.|  
|**All**|No transaction is allowed for this customer, including payments.|  

## <a name="to-block-a-customer"></a>To block a customer  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Select a customer, and then choose the **Edit** action.
3. Fill in the **Blocked** field with one of the options described above.

## <a name="see-also"></a>See Also  
[Register New Customers](sales-how-register-new-customers.md)  
[Collect Outstanding Balances](receivables-collect-outstanding-balances.md)  
[Managing Receivables](receivables-manage-receivables.md)  
