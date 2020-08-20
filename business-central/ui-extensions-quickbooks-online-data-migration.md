---
title: QuickBooks Online Migration Extension | Microsoft Docs
description: Describes how to use the extension to migrate customers, vendors, items, and accounts from QuickBooks Online to Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 07/23/2020
ms.author: bholtorf
ms.openlocfilehash: 33de4d2b6d75f79c140c7c2fdf5b84b7a77521d6
ms.sourcegitcommit: 7b5c927ea9a59329daf1b60633b8290b552d6531
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/23/2020
ms.locfileid: "3617793"
---
# <a name="the-quickbooks-online-data-migration-extension"></a><span data-ttu-id="4ff9d-103">The QuickBooks Online Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="4ff9d-103">The QuickBooks Online Data Migration Extension</span></span>

<span data-ttu-id="4ff9d-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4ff9d-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="4ff9d-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4ff9d-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="4ff9d-106">What data can I import from QuickBooks Online?</span><span class="sxs-lookup"><span data-stu-id="4ff9d-106">What data can I import from QuickBooks Online?</span></span>

<span data-ttu-id="4ff9d-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="4ff9d-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="4ff9d-108">Customers</span><span class="sxs-lookup"><span data-stu-id="4ff9d-108">Customers</span></span>
* <span data-ttu-id="4ff9d-109">Vendors</span><span class="sxs-lookup"><span data-stu-id="4ff9d-109">Vendors</span></span>
* <span data-ttu-id="4ff9d-110">Items</span><span class="sxs-lookup"><span data-stu-id="4ff9d-110">Items</span></span>
* <span data-ttu-id="4ff9d-111">Chart of accounts</span><span class="sxs-lookup"><span data-stu-id="4ff9d-111">Chart of accounts</span></span>
* <span data-ttu-id="4ff9d-112">Beginning balance transaction in the general ledger</span><span class="sxs-lookup"><span data-stu-id="4ff9d-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="4ff9d-113">On-hand quantities for inventory items</span><span class="sxs-lookup"><span data-stu-id="4ff9d-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="4ff9d-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span><span class="sxs-lookup"><span data-stu-id="4ff9d-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="4ff9d-115">We migrate only full amounts on sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="4ff9d-116">We do not update partially paid amounts.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="4ff9d-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="4ff9d-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="4ff9d-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
> <span data-ttu-id="4ff9d-120">We do not migrate purchase orders or sales orders.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="4ff9d-121">Before you start</span><span class="sxs-lookup"><span data-stu-id="4ff9d-121">Before you start</span></span>

<span data-ttu-id="4ff9d-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="4ff9d-123">It's a good idea to plan this mapping before you migrate data.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="4ff9d-124">For example, the accounts where you post transactions for:</span><span class="sxs-lookup"><span data-stu-id="4ff9d-124">For example, the accounts where you post transactions for:</span></span>  

* <span data-ttu-id="4ff9d-125">The sale of items or services to customers.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="4ff9d-126">The purchase of items or services from vendors.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="4ff9d-127">Adjustments in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="4ff9d-128">requires that general ledger accounts have account numbers assigned to them.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-128">requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="4ff9d-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="4ff9d-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="4ff9d-131">How do I start using the extension?</span><span class="sxs-lookup"><span data-stu-id="4ff9d-131">How do I start using the extension?</span></span>

<span data-ttu-id="4ff9d-132">Getting started is easy.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-132">Getting started is easy.</span></span> <span data-ttu-id="4ff9d-133">All you need to do is run the **Data Migration** assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="4ff9d-134">Here's how:</span><span class="sxs-lookup"><span data-stu-id="4ff9d-134">Here's how:</span></span>

1. <span data-ttu-id="4ff9d-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="4ff9d-136">Follow the instructions on each step in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="4ff9d-137">What do I do after I migrate data?</span><span class="sxs-lookup"><span data-stu-id="4ff9d-137">What do I do after I migrate data?</span></span>

<span data-ttu-id="4ff9d-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="4ff9d-139">To review the transactions, go to the page where you would normally find them.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="4ff9d-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="4ff9d-141">To review payment journals, go to the **Payment Journals** page.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-141">To review payment journals, go to the **Payment Journals** page.</span></span>  

<span data-ttu-id="4ff9d-142">There are a few things in particular that you should do:</span><span class="sxs-lookup"><span data-stu-id="4ff9d-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="4ff9d-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="4ff9d-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="4ff9d-145">Verify the beginning balances for accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="4ff9d-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span><span class="sxs-lookup"><span data-stu-id="4ff9d-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="4ff9d-147">See Also</span><span class="sxs-lookup"><span data-stu-id="4ff9d-147">See Also</span></span>

[<span data-ttu-id="4ff9d-148">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="4ff9d-148">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="4ff9d-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="4ff9d-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
