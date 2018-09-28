---
title: Linking Contacts With Customers and Vendors| Microsoft Docs
description: Describes how to link a contact with a customer, vendor, or bank account from the same company, so that you can synchronise common data.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 2613e32873c91fe24c4734456338bb1f7e18849d
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="link-contacts-with-customers-vendors-and-bank-accounts"></a>Link Contacts With Customers, Vendors, and Bank Accounts
If you have contact and either a customer, vendor, or bank account for the same company, you can link the two entities. Linking the two entities enables you to synchronise data that is common so that it is the same in both places.

## <a name="link-a-contact-to-an-existing-customer-vendor-or-bank-account"></a>Link a Contact to an Existing Customer, Vendor, or Bank Account
1. Open the contact that you want to link.
2. Choose the **Link with existing** action, and then choose **Customer**, **Vendor**, or **Bank**.
3. Select the customer, vendor, or bank account to link to.

   In the **Current Master Fields**, you specify which fields should prioritise in case of conflicting information in fields common to the contact and customer, vendor, or account. For example, if the salesperson code is different in the contact than the customer, you can decide, by selecting **Contact**, to use the information in the contact.

## <a name="see-also"></a>See Also
[Synchronizing Contacts With Customers, Vendors, and Bank Accounts](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Creating and Managing Contacts](marketing-contacts.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

