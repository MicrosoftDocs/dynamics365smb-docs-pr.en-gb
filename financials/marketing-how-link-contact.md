---
title: Linking Contacts With Customers, Vendors, and Bank Accounts | Microsoft Docs
description: Describes how to link contacts with customers, vendors, and bank accounts in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 44dff830f293f4a33e6358d816635aa67e8a8de6
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-link-contacts-with-customers-vendors-and-bank-accounts"></a>How to: Link Contacts With Customers, Vendors, and Bank Accounts
If you have contact and either a customer, vendor, or bank account for the same company, you can link the two entities. Linking the two entities enables you to synchronise data that is common so that it is the same in both places.

## <a name="link-a-contact-to-an-existing-customer-vendor-or-bank-account"></a>Link a Contact to an Existing Customer, Vendor, or Bank Account
1. Open the contact that you want to link.
2. Choose the **Link with existing** action, and then choose **Customer**, **Vendor**, or **Bank**.
3. Select the customer, vendor, or bank account to link to.

   In the **Current Master Fields**, you specify which fields should prioritise in case of conflicting information in fields common to the contact and customer, vendor, or account. For example, if the salesperson code is different in the contact than the customer, you can decide, by selecting **Contact**, to use the information in the contact.

## <a name="see-also"></a>See Also
[Synchronizing Contacts With Customers, Vendors, and Bank Accounts](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Creating and Managing Contacts](marketing-contacts.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

