---
title: Create Contact Companies| Microsoft Docs
description: Describes how to create a contact for each new company or prospective company you interact with or have a relationship with.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 6a1141c352dd93657d32bb83067ce32077901a47
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-create-contact-companies"></a><span data-ttu-id="02b75-103">How to: Create Contact Companies</span><span class="sxs-lookup"><span data-stu-id="02b75-103">How to: Create Contact Companies</span></span>
<span data-ttu-id="02b75-104">You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.</span><span class="sxs-lookup"><span data-stu-id="02b75-104">You can create a contact for each new company you interact with, for example, a customer, vendor, prospective customer, bank, law firm, consultant, and so on.</span></span>

<span data-ttu-id="02b75-105">There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.</span><span class="sxs-lookup"><span data-stu-id="02b75-105">There are two ways to create a contact: from scratch or from an existing customer, vendor, or bank account.</span></span>

<span data-ttu-id="02b75-106">Before creating a contact, you may want to check the settings in the **Marketing Setup** window.</span><span class="sxs-lookup"><span data-stu-id="02b75-106">Before creating a contact, you may want to check the settings in the **Marketing Setup** window.</span></span> <span data-ttu-id="02b75-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span><span class="sxs-lookup"><span data-stu-id="02b75-107">For more information, see [Setting Up Relationship Management](marketing-setup-marketing.md).</span></span>

## <a name="create-a-company-contact-from-scratch"></a><span data-ttu-id="02b75-108">Create a company contact from scratch</span><span class="sxs-lookup"><span data-stu-id="02b75-108">Create a company contact from scratch</span></span>
1. <span data-ttu-id="02b75-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="02b75-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.</span></span>
2. <span data-ttu-id="02b75-110">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="02b75-110">Choose the **New** action.</span></span>
3. <span data-ttu-id="02b75-111">In the **No. field**, enter a number for the contact.</span><span class="sxs-lookup"><span data-stu-id="02b75-111">In the **No. field**, enter a number for the contact.</span></span>

    <span data-ttu-id="02b75-112">Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number.</span><span class="sxs-lookup"><span data-stu-id="02b75-112">Alternatively, if you have set up a number series for contacts in the **Marketing Setup** window, you can press the Enter key to select the next available contact number.</span></span>  
4. <span data-ttu-id="02b75-113">Set **Type** to **Company**.</span><span class="sxs-lookup"><span data-stu-id="02b75-113">Set **Type** to **Company**.</span></span>
5. <span data-ttu-id="02b75-114">Fill in the other fields as required.</span><span class="sxs-lookup"><span data-stu-id="02b75-114">Fill in the other fields as required.</span></span>

## <a name="to-create-a-company-contact-from-a-customer-vendor-or-bank-account"></a><span data-ttu-id="02b75-115">To create a company contact from a customer, vendor, or bank account</span><span class="sxs-lookup"><span data-stu-id="02b75-115">To create a company contact from a customer, vendor, or bank account</span></span>
<span data-ttu-id="02b75-116">If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data.</span><span class="sxs-lookup"><span data-stu-id="02b75-116">If you have already set up a number of customers, vendors, and bank accounts, you can create contacts on the basis of the existing data.</span></span> <span data-ttu-id="02b75-117">When you create a contact this way, the contact information is synchronised with the customer, vendor, or bank account information.</span><span class="sxs-lookup"><span data-stu-id="02b75-117">When you create a contact this way, the contact information is synchronized with the customer, vendor, or bank account information.</span></span>

> [!NOTE]  
>   <span data-ttu-id="02b75-118">Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span><span class="sxs-lookup"><span data-stu-id="02b75-118">Before you can create contact companies this way, you must specify a business relation code for customers, vendors, and bank accounts in the **Marketing Setup** window.</span></span> <span data-ttu-id="02b75-119">If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.</span><span class="sxs-lookup"><span data-stu-id="02b75-119">If you will be creating contacts from a bank accounts, you must also specify numbers series for bank accounts in the **General Ledger Setup** window.</span></span>

1. <span data-ttu-id="02b75-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="02b75-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter one of the following, depending on from where you want to create contacts, and then choose the related link.</span></span>
   * <span data-ttu-id="02b75-121">**Create Contacts from Customers**</span><span class="sxs-lookup"><span data-stu-id="02b75-121">**Create Contacts from Customers**</span></span>
   * <span data-ttu-id="02b75-122">**Create Contacts from Vendors**</span><span class="sxs-lookup"><span data-stu-id="02b75-122">**Create Contacts from Vendors**</span></span>
   * <span data-ttu-id="02b75-123">**Create Contacts from Bank Accounts**</span><span class="sxs-lookup"><span data-stu-id="02b75-123">**Create Contacts from Bank Accounts**</span></span>
2. <span data-ttu-id="02b75-124">In the batch job window that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.</span><span class="sxs-lookup"><span data-stu-id="02b75-124">In the batch job window that opens, in the **Customer**, **Vendor**, or **Bank Account** section, set filters if you want to create contacts from specific customers, vendors, or bank accounts.</span></span>
3. <span data-ttu-id="02b75-125">Choose the **OK** button to start creating contacts.</span><span class="sxs-lookup"><span data-stu-id="02b75-125">Choose the **OK** button to start creating contacts.</span></span>

    <span data-ttu-id="02b75-126">The next contact numbers in the number series are assigned to the new contacts.</span><span class="sxs-lookup"><span data-stu-id="02b75-126">The next contact numbers in the number series are assigned to the new contacts.</span></span> <span data-ttu-id="02b75-127">The business relation for vendors that is specified in the **Marketing Setup** window is assigned to the newly created contacts.</span><span class="sxs-lookup"><span data-stu-id="02b75-127">The business relation for vendors that is specified in the **Marketing Setup** window is assigned to the newly created contacts.</span></span>

> [!TIP]  
>   <span data-ttu-id="02b75-128">You can also create a customer, vendor, or bank account from a contact.</span><span class="sxs-lookup"><span data-stu-id="02b75-128">You can also create a customer, vendor, or bank account from a contact.</span></span> <span data-ttu-id="02b75-129">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="02b75-129">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="02b75-130">See Also</span><span class="sxs-lookup"><span data-stu-id="02b75-130">See Also</span></span>
[<span data-ttu-id="02b75-131">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="02b75-131">Synchronizing Contacts With Customers, Vendors, and Bank Accounts</span></span>](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[<span data-ttu-id="02b75-132">Assign Business Relations to a Contact</span><span class="sxs-lookup"><span data-stu-id="02b75-132">Assign Business Relations to a Contact</span></span>](marketing-business-relations.md#AssignBusRelContact)  
[<span data-ttu-id="02b75-133">Assign Industry Groups to a Contact</span><span class="sxs-lookup"><span data-stu-id="02b75-133">Assign Industry Groups to a Contact</span></span>](marketing-industry-groups.md#AssignIndustryGroupContact)  
[<span data-ttu-id="02b75-134">Assign Mailing Groups to a Contact</span><span class="sxs-lookup"><span data-stu-id="02b75-134">Assign Mailing Groups to a Contact</span></span>](marketing-mailing-groups.md#AssignMailGroupContact)  
[<span data-ttu-id="02b75-135">How to: Create Contact Persons</span><span class="sxs-lookup"><span data-stu-id="02b75-135">How to: Create Contact Persons</span></span>](marketing-create-contact-persons.md)  
[<span data-ttu-id="02b75-136">Working with Financials</span><span class="sxs-lookup"><span data-stu-id="02b75-136">Working with Financials</span></span>](ui-work-product.md)

