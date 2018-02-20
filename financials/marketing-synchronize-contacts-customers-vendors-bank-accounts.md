---
title: Synchronise Contacts With Customers and Vendors| Microsoft Docs
description: You couple or synchronise contact information of contacts who are also customers, vendors, or bank accounts, so you only update information in one place.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, CRM, integration, couple
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 2b85c52378a351dbc1a0809ec540b1f53c8074ef
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="synchronizing-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="f0e47-103">Synchronising Contacts With Customers, Vendors, and Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="f0e47-103">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>
<span data-ttu-id="f0e47-104">If some of your contacts are also customers, vendors, or bank accounts, you can synchronise the contact information with the related customer, vendor, or bank account.</span><span class="sxs-lookup"><span data-stu-id="f0e47-104">If some of your contacts are also customers, vendors, or bank accounts, you can synchronize the contact information with the related customer, vendor, or bank account.</span></span> <span data-ttu-id="f0e47-105">Synchronisation makes information that is common between contacts and customers, vendors, or bank account the same.</span><span class="sxs-lookup"><span data-stu-id="f0e47-105">Synchronization makes information that is common between contacts and customers, vendors, or bank account the same.</span></span>  

<span data-ttu-id="f0e47-106">Before you can synchronise your contacts with customers, vendors, or bank accounts, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span><span class="sxs-lookup"><span data-stu-id="f0e47-106">Before you can synchronize your contacts with customers, vendors, or bank accounts, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span></span> <span data-ttu-id="f0e47-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span><span class="sxs-lookup"><span data-stu-id="f0e47-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span></span>

## <a name="different-ways-to-synchronize-contacts-with-customers-vendors-and-bank-accounts"></a><span data-ttu-id="f0e47-108">Different Ways to Synchronise Contacts with Customers, Vendors and Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="f0e47-108">Different Ways to Synchronize Contacts with Customers, Vendors and Bank Accounts</span></span>
<span data-ttu-id="f0e47-109">You can synchronise your contacts with customers, vendors, or bank accounts by three methods:</span><span class="sxs-lookup"><span data-stu-id="f0e47-109">You can synchronize your contacts with customers, vendors, or bank accounts by three methods:</span></span>

* <span data-ttu-id="f0e47-110">Link contacts with existing customers, vendors, or bank accounts from the contact card.</span><span class="sxs-lookup"><span data-stu-id="f0e47-110">Link contacts with existing customers, vendors, or bank accounts from the contact card.</span></span> <span data-ttu-id="f0e47-111">For more information, see [Link Contacts With Customers, Vendors, and Bank Accounts](marketing-how-link-contact.md).</span><span class="sxs-lookup"><span data-stu-id="f0e47-111">For more information, see [Link Contacts With Customers, Vendors, and Bank Accounts](marketing-how-link-contact.md).</span></span>
* <span data-ttu-id="f0e47-112">Create customers, vendors, or bank accounts from the contact.</span><span class="sxs-lookup"><span data-stu-id="f0e47-112">Create customers, vendors, or bank accounts from the contact.</span></span> <span data-ttu-id="f0e47-113">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="f0e47-113">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>
* <span data-ttu-id="f0e47-114">Create contacts from customers, vendors or bank accounts.</span><span class="sxs-lookup"><span data-stu-id="f0e47-114">Create contacts from customers, vendors or bank accounts.</span></span> <span data-ttu-id="f0e47-115">For more information, see [Create a company contact from a customer, vendor, or bank account](marketing-how-create-contact-companies.md).</span><span class="sxs-lookup"><span data-stu-id="f0e47-115">For more information, see [Create a company contact from a customer, vendor, or bank account](marketing-how-create-contact-companies.md).</span></span>

## <a name="consequences-of-synchronization"></a><span data-ttu-id="f0e47-116">Consequences of Synchronisation</span><span class="sxs-lookup"><span data-stu-id="f0e47-116">Consequences of Synchronization</span></span>
<span data-ttu-id="f0e47-117">When the contact is synchronised with the customer, vendor, bank account:</span><span class="sxs-lookup"><span data-stu-id="f0e47-117">When the contact is synchronized with the customer, vendor, bank account:</span></span>

* <span data-ttu-id="f0e47-118">You only have to update information in one place.</span><span class="sxs-lookup"><span data-stu-id="f0e47-118">You only have to update information in one place.</span></span> <span data-ttu-id="f0e47-119">For example, if you modify the phone number on the contact, the phone number is automatically updated with the same modification on the customer, the vendor, or the bank account.</span><span class="sxs-lookup"><span data-stu-id="f0e47-119">For example, if you modify the phone number on the contact, the phone number is automatically updated with the same modification on the customer, the vendor, or the bank account.</span></span>
* <span data-ttu-id="f0e47-120">If you have specified a number series for contacts, when you create a customer card, a vendor card, or a bank account card, a contact card is automatically created for the customer, vendor or bank account.</span><span class="sxs-lookup"><span data-stu-id="f0e47-120">If you have specified a number series for contacts, when you create a customer card, a vendor card, or a bank account card, a contact card is automatically created for the customer, vendor or bank account.</span></span>
* <span data-ttu-id="f0e47-121">You can create sales quotes and orders, and purchase quotes and orders from the contact.</span><span class="sxs-lookup"><span data-stu-id="f0e47-121">You can create sales quotes and orders, and purchase quotes and orders from the contact.</span></span>
* <span data-ttu-id="f0e47-122">You can have your interactions recorded when you perform actions such as printing orders, blanket orders, creating sales service orders, sending e-mails, and so on.</span><span class="sxs-lookup"><span data-stu-id="f0e47-122">You can have your interactions recorded when you perform actions such as printing orders, blanket orders, creating sales service orders, sending e-mails, and so on.</span></span>
* <span data-ttu-id="f0e47-123">If you delete a contact linked to a customer, vendor or bank account, only the contact is removed.</span><span class="sxs-lookup"><span data-stu-id="f0e47-123">If you delete a contact linked to a customer, vendor or bank account, only the contact is removed.</span></span> <span data-ttu-id="f0e47-124">The customer, vendor, or bank account remains.</span><span class="sxs-lookup"><span data-stu-id="f0e47-124">The customer, vendor, or bank account remains.</span></span>
* <span data-ttu-id="f0e47-125">If you delete a customer, vendor, bank account linked to a contact, the contact remains.</span><span class="sxs-lookup"><span data-stu-id="f0e47-125">If you delete a customer, vendor, bank account linked to a contact, the contact remains.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f0e47-126">Some details, such as invoicing and posting details, do not appear on the contact card.</span><span class="sxs-lookup"><span data-stu-id="f0e47-126">Some details, such as invoicing and posting details, do not appear on the contact card.</span></span> <span data-ttu-id="f0e47-127">Therefore, you may want to add them manually on the customer card, vendor card, or bank account card when you create contacts as customers, vendors or bank accounts.</span><span class="sxs-lookup"><span data-stu-id="f0e47-127">Therefore, you may want to add them manually on the customer card, vendor card, or bank account card when you create contacts as customers, vendors or bank accounts.</span></span>

## <a name="see-also"></a><span data-ttu-id="f0e47-128">See Also</span><span class="sxs-lookup"><span data-stu-id="f0e47-128">See Also</span></span>
[<span data-ttu-id="f0e47-129">Managing Contacts</span><span class="sxs-lookup"><span data-stu-id="f0e47-129">Managing Contacts</span></span>](marketing-contacts.md)  
<span data-ttu-id="f0e47-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f0e47-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

