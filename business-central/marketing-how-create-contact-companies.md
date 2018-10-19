---
title: Create Contact Companies| Microsoft Docs
description: Describes how to create a contact for each new company or prospective company you interact with or have a relationship with.
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 64bef8820ec10bb293ccda88e7384d5d9e868e1f
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="create-contact-companies"></a>Create Contact Companies
You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.

There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.

Before creating a contact, you may want to check the settings in the **Marketing Setup** window. For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).

## <a name="create-a-company-contact-from-scratch"></a>Create a company contact from scratch
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.
2. Choose the **New** action.
3. In the **No. field**, enter a number for the contact.

    Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number.  
4. Set **Type** to **Company**.
5. Fill in the other fields as required.

## <a name="to-create-a-company-contact-from-a-customer-vendor-or-bank-account"></a>To create a company contact from a customer, vendor, or bank account
If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data. When you create a contact this way, the contact information is synchronised with the customer, vendor, or bank account information.

> [!NOTE]  
>   Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window. If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.
   * **Create Contacts from Customers**
   * **Create Contacts from Vendors**
   * **Create Contacts from Bank Accounts**
2. In the batch job window that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.
3. Choose the **OK** button to start creating contacts.

    The next contact numbers in the number series are assigned to the new contacts. The business relation for vendors that is specified in the **Marketing Setup** window is assigned to the newly created contacts.

> [!TIP]  
>   You can also create a customer, vendor, or bank account from a contact. For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).

## <a name="see-also"></a>See Also
[Synchronizing Contacts With Customers, Vendors, and Bank Accounts](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Assign Business Relations to a Contact](marketing-business-relations.md#AssignBusRelContact)  
[Assign Industry Groups to a Contact](marketing-industry-groups.md#AssignIndustryGroupContact)  
[Assign Mailing Groups to a Contact](marketing-mailing-groups.md#AssignMailGroupContact)  
[Create Contact Persons](marketing-create-contact-persons.md)  
[Working with Business Central](ui-work-product.md)

