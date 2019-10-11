---
title: How to Create Service Quotes | Microsoft Docs
description: You can use the **Service Quote** page to create documents where you enter information about a service, such as repairs and maintenance, on service items by customer request. You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: e3689096a2bcdfed5ceb92a2fc9163549f2d53de
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2315931"
---
# <a name="create-service-quotes"></a>Create Service Quotes
You can think of service quotes as the basis for service orders. In fact, they are almost identical. They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.
 
You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.  
  
## <a name="to-create-a-service-quote"></a>To create a service quote  
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.  
2. Create a new service quote.  
3. In the **No.** field, enter a number for the service quote. Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.  
4. In the **Customer No.**  field, select the relevant customer from the list.  

  > [!Note]  
  >  The customer fields are filled in automatically with information from the **Customer** card. If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote. Fill in the relevant fields, and then choose the **Create Customer** action.  
  
5. Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.  
6. Fill in the service item lines.  
7. Register estimated costs on the service lines.  
  
## <a name="see-also"></a>See Also  
[Create Service Orders](service-how-to-create-service-orders.md)  
[Work on Service tasks](service-how-to-work-on-service-tasks.md)  

 