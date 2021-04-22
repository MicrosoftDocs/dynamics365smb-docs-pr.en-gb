---
title: QuickBooks Migration Extension | Microsoft Docs
description: Describes how to use the extension to import customers, vendors, items, and accounts from QuickBooks Desktop to Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d6b44ccfc11438930450dd86cab53736f00995c5
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785042"
---
# <a name="the-quickbooks-data-migration-extension"></a><span data-ttu-id="9d990-103">The QuickBooks Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="9d990-103">The QuickBooks Data Migration Extension</span></span>

<span data-ttu-id="9d990-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9d990-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="9d990-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9d990-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  
<span data-ttu-id="9d990-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="9d990-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span></span>

## <a name="data-from-quickbooks-desktop"></a><span data-ttu-id="9d990-107">Data from QuickBooks Desktop</span><span class="sxs-lookup"><span data-stu-id="9d990-107">Data from QuickBooks Desktop</span></span>

<span data-ttu-id="9d990-108">You can import the following data from QuickBooks Online to Business Central:</span><span class="sxs-lookup"><span data-stu-id="9d990-108">You can import the following data from QuickBooks Online to Business Central:</span></span>

- <span data-ttu-id="9d990-109">Customers</span><span class="sxs-lookup"><span data-stu-id="9d990-109">Customers</span></span>  
- <span data-ttu-id="9d990-110">Vendors</span><span class="sxs-lookup"><span data-stu-id="9d990-110">Vendors</span></span>  
- <span data-ttu-id="9d990-111">Items</span><span class="sxs-lookup"><span data-stu-id="9d990-111">Items</span></span>  
- <span data-ttu-id="9d990-112">Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="9d990-112">Chart of Accounts</span></span>  
- <span data-ttu-id="9d990-113">Beginning Balance transactions in General Ledger</span><span class="sxs-lookup"><span data-stu-id="9d990-113">Beginning Balance transactions in General Ledger</span></span>  
- <span data-ttu-id="9d990-114">On-hand Quantities for Inventory Items</span><span class="sxs-lookup"><span data-stu-id="9d990-114">On-hand Quantities for Inventory Items</span></span>  
- <span data-ttu-id="9d990-115">Open documents for customers and vendors, such as invoices, credit memos and payments</span><span class="sxs-lookup"><span data-stu-id="9d990-115">Open documents for customers and vendors, such as invoices, credit memos and payments</span></span>  

<span data-ttu-id="9d990-116">We migrate only full amounts on sales and purchase documents.</span><span class="sxs-lookup"><span data-stu-id="9d990-116">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="9d990-117">We do not update partially paid amounts.</span><span class="sxs-lookup"><span data-stu-id="9d990-117">We do not update partially paid amounts.</span></span> <span data-ttu-id="9d990-118">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span><span class="sxs-lookup"><span data-stu-id="9d990-118">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="9d990-119">If you have received partial payments, you must update these manually, either before or after you migrate data.</span><span class="sxs-lookup"><span data-stu-id="9d990-119">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="9d990-120">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span><span class="sxs-lookup"><span data-stu-id="9d990-120">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]
> <span data-ttu-id="9d990-121">We do not migrate purchase orders or sales orders.</span><span class="sxs-lookup"><span data-stu-id="9d990-121">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="9d990-122">Before You Start</span><span class="sxs-lookup"><span data-stu-id="9d990-122">Before You Start</span></span>

<span data-ttu-id="9d990-123">An important part of the migration process is to specify the accounts to migrate transactions to.</span><span class="sxs-lookup"><span data-stu-id="9d990-123">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="9d990-124">It's a good idea to plan this mapping before you migrate data.</span><span class="sxs-lookup"><span data-stu-id="9d990-124">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="9d990-125">For example, the accounts where you post transactions for:</span><span class="sxs-lookup"><span data-stu-id="9d990-125">For example, the accounts where you post transactions for:</span></span>

- <span data-ttu-id="9d990-126">The sale of items or services to customers</span><span class="sxs-lookup"><span data-stu-id="9d990-126">The sale of items or services to customers</span></span>  
- <span data-ttu-id="9d990-127">The purchase of items or services from vendors</span><span class="sxs-lookup"><span data-stu-id="9d990-127">The purchase of items or services from vendors</span></span>  
- <span data-ttu-id="9d990-128">Adjustments in the general ledger</span><span class="sxs-lookup"><span data-stu-id="9d990-128">Adjustments in the general ledger</span></span>  

<span data-ttu-id="9d990-129">Business Central requires that general ledger accounts have account numbers assigned to them.</span><span class="sxs-lookup"><span data-stu-id="9d990-129">Business Central requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="9d990-130">Make sure that account numbers are assigned to your accounts in QuickBooks.</span><span class="sxs-lookup"><span data-stu-id="9d990-130">Make sure that account numbers are assigned to your accounts in QuickBooks.</span></span>
<span data-ttu-id="9d990-131">If transactions in QuickBooks have tax amounts, you must set up a tax account for your tax jurisdictions in Business Central before you can post transactions.</span><span class="sxs-lookup"><span data-stu-id="9d990-131">If transactions in QuickBooks have tax amounts, you must set up a tax account for your tax jurisdictions in Business Central before you can post transactions.</span></span>

<span data-ttu-id="9d990-132">In order to get your data out of the QuickBooks desktop application you will need to download the Microsoft Data Exporter Tool.</span><span class="sxs-lookup"><span data-stu-id="9d990-132">In order to get your data out of the QuickBooks desktop application you will need to download the Microsoft Data Exporter Tool.</span></span>  <span data-ttu-id="9d990-133">The instructions for the tool are in the Data Migration Wizard in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9d990-133">The instructions for the tool are in the Data Migration Wizard in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="9d990-134">The tool will connect to your QuickBooks application and export the applicable data to a .zip file.</span><span class="sxs-lookup"><span data-stu-id="9d990-134">The tool will connect to your QuickBooks application and export the applicable data to a .zip file.</span></span>  

> [!NOTE]
> <span data-ttu-id="9d990-135">Currently the data exporter tool only works with QuickBooks 2017 and 2018.</span><span class="sxs-lookup"><span data-stu-id="9d990-135">Currently the data exporter tool only works with QuickBooks 2017 and 2018.</span></span>

## <a name="finding-the-quickbooks-data-migration-extension"></a><span data-ttu-id="9d990-136">Finding the QuickBooks Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="9d990-136">Finding the QuickBooks Data Migration Extension</span></span>

<span data-ttu-id="9d990-137">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="9d990-137">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span></span> <span data-ttu-id="9d990-138">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9d990-138">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.</span></span> <span data-ttu-id="9d990-139">Choose **Migrate business data**, and then follow the steps in the guide.</span><span class="sxs-lookup"><span data-stu-id="9d990-139">Choose **Migrate business data**, and then follow the steps in the guide.</span></span>  

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="9d990-140">What do I do after I migrate Data?</span><span class="sxs-lookup"><span data-stu-id="9d990-140">What do I do after I migrate Data?</span></span>

<span data-ttu-id="9d990-141">After you migrate data, transactions have the status Unposted, so you can review them and make adjustments.</span><span class="sxs-lookup"><span data-stu-id="9d990-141">After you migrate data, transactions have the status Unposted, so you can review them and make adjustments.</span></span> <span data-ttu-id="9d990-142">To review the transactions, go to the page where you would normally find them.</span><span class="sxs-lookup"><span data-stu-id="9d990-142">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="9d990-143">For example, to review unposted sales invoices, go to the Sales Invoices page.</span><span class="sxs-lookup"><span data-stu-id="9d990-143">For example, to review unposted sales invoices, go to the Sales Invoices page.</span></span> <span data-ttu-id="9d990-144">To review payment journals, go to the Payment Journals page.</span><span class="sxs-lookup"><span data-stu-id="9d990-144">To review payment journals, go to the Payment Journals page.</span></span>
<span data-ttu-id="9d990-145">There are a few things in particular that you should do: If the transactions in QuickBooks had markup or discount amounts, you must manually add the amounts to the related transactions in Business Central before you post them.</span><span class="sxs-lookup"><span data-stu-id="9d990-145">There are a few things in particular that you should do: If the transactions in QuickBooks had markup or discount amounts, you must manually add the amounts to the related transactions in Business Central before you post them.</span></span>
<span data-ttu-id="9d990-146">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span><span class="sxs-lookup"><span data-stu-id="9d990-146">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
<span data-ttu-id="9d990-147">Verify the beginning balances for accounts in the general ledger.</span><span class="sxs-lookup"><span data-stu-id="9d990-147">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="9d990-148">QuickBooks does not store the current balance for all accounts, so you might need to correct beginning balances.</span><span class="sxs-lookup"><span data-stu-id="9d990-148">QuickBooks does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="9d990-149">See Also</span><span class="sxs-lookup"><span data-stu-id="9d990-149">See Also</span></span>

[<span data-ttu-id="9d990-150">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="9d990-150">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="9d990-151">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="9d990-151">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]