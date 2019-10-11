---
title: Export data | Invoicing
description: Learn how to export data, such as deleting contacts as part of a data subject request.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 106f9132124226a3dd8650fa257b566119f8e933
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2314380"
---
# <a name="export-or-delete-data-from-included365inv_longincludesd365inv_longmd"></a>Export or delete data from [!INCLUDE[d365inv_long](includes/d365inv_long.md)]

If you want to delete a contact or customer from [!INCLUDE[d365inv](includes/d365inv.md)], it's easy to do.  

## <a name="to-delete-an-existing-customer"></a>To delete an existing customer

1. On your Home page, choose **Customers** to open the list of customers.
2. Find the contact, and then choose the name to open the details.
3. Choose the **Delete** action.

> [!NOTE]
> If you have already sent them an invoice, you cannot delete the customer. Instead, [!INCLUDE[d365inv](includes/d365inv.md)] can mark the customer as blocked for further business. That means that you cannot send them new invoices, for example.  

If the contact has not been added as a customer, you can add them by creating a draft invoice.

## <a name="to-add-a-contact-as-a-customer-and-then-delete-the-customer"></a>To add a contact as a customer and then delete the customer

1. On your Home page, choose **New Invoice**
2. In the **Customer Name** field, start typing the contact’s name.
3. Select your contact from the look-up, and then tab out.
4. Delete the draft invoice that was just created.
5. Follow the steps for deleting the customer as described above.

## <a name="responding-to-requests-about-personal-data"></a>Responding to Requests About Personal Data

Data subjects can request several types of actions regarding their personal data. For example, under the General Data Protection Regulation (GDPR), EU residents have the right to request the export, deletion, and modification of their personal data. This is known as a *Data Subject Request*.  

### <a name="requests-for-deletion"></a>Requests for deletion

A data subject can request that you delete their personal data. If a contact or customer asks you to be deleted in the context of a data subject request, you can follow the steps that are outlined above.  

### <a name="requests-for-exporting-privacy-data"></a>Requests for exporting privacy data

A data subject can make a data portability request, meaning, in part, that you must export the data subject's personal data from your systems and provide it in in a structured, commonly used format.  If a contact or customer asks you to send them their information from [!INCLUDE[d365inv](includes/d365inv.md)], you can email yourself their contact information.  

#### <a name="to-export-privacy-data"></a>To export privacy data

1. On your Home page, choose **Customers** to open the list of customers.
2. Find the relevant customer, and then choose the name to open the details.
3. Expand the **Privacy** tab, and then choose **Export customer privacy data**.
4. In the **Export customer data** page, verify that you are about to send the email to yourself, and then choose the OK button.

The email that you receive includes an Excel book with information about the customer, including invoices that you have sent them. Depending on the original request, you can choose to delete part of the information before you forward the email to the customer.  

### <a name="requests-for-correction"></a>Requests for correction

A data subject can request that you correct inaccurate personal data. If a contact or customer asks you to update the information about them in [!INCLUDE[d365inv](includes/d365inv.md)], you can do that in the customer details.  

## <a name="see-also"></a>See also

[Set up your business information](set-up-business-profile.md)  
[Send an invoice to a new customer](send-invoice.md)  
[Troubleshooting](about-troubleshooting.md)  
