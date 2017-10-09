---
title: Learn About General Ledger and COA| Microsoft Docs
description: Describes the general ledger, the chart of accounts, and account categories.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 63d414f4c81a9e20b4bb81b632edd9c91fb34a87
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="understanding-the-general-ledger-and-the-coa"></a><span data-ttu-id="4d245-103">Understanding the General Ledger and the COA</span><span class="sxs-lookup"><span data-stu-id="4d245-103">Understanding the General Ledger and the COA</span></span>
<span data-ttu-id="4d245-104">The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to.</span><span class="sxs-lookup"><span data-stu-id="4d245-104">The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="4d245-105"> includes a standard chart of accounts that is ready to support your business.</span><span class="sxs-lookup"><span data-stu-id="4d245-105"> includes a standard chart of accounts that is ready to support your business.</span></span>

## <a name="general-ledger-setup-and-general-posting-setup"></a><span data-ttu-id="4d245-106">General Ledger Setup and General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="4d245-106">General Ledger Setup and General Posting Setup</span></span>
<span data-ttu-id="4d245-107">The setup of the general ledger is at the core of financial processes because it defines how you post data.</span><span class="sxs-lookup"><span data-stu-id="4d245-107">The setup of the general ledger is at the core of financial processes because it defines how you post data.</span></span>  

<span data-ttu-id="4d245-108">In the **General Ledger Setup** window, you specify how to handle certain accounting issues in your company, such as:</span><span class="sxs-lookup"><span data-stu-id="4d245-108">In the **General Ledger Setup** window, you specify how to handle certain accounting issues in your company, such as:</span></span>  

* <span data-ttu-id="4d245-109">Invoice rounding details</span><span class="sxs-lookup"><span data-stu-id="4d245-109">Invoice rounding details</span></span>  
* <span data-ttu-id="4d245-110">Address formats</span><span class="sxs-lookup"><span data-stu-id="4d245-110">Address formats</span></span>  
* <span data-ttu-id="4d245-111">Financial reporting</span><span class="sxs-lookup"><span data-stu-id="4d245-111">Financial reporting</span></span>  

<span data-ttu-id="4d245-112">Similarly, in the **General Posting Setup** window, you specify how you want to set up combinations of general business and general product posting groups.</span><span class="sxs-lookup"><span data-stu-id="4d245-112">Similarly, in the **General Posting Setup** window, you specify how you want to set up combinations of general business and general product posting groups.</span></span> <span data-ttu-id="4d245-113">Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="4d245-113">Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts.</span></span> <span data-ttu-id="4d245-114">You fill in a line for each combination of business posting group and product posting group.</span><span class="sxs-lookup"><span data-stu-id="4d245-114">You fill in a line for each combination of business posting group and product posting group.</span></span> <span data-ttu-id="4d245-115">For more information, see [Posting Group Setups](finance-posting-groups.md)</span><span class="sxs-lookup"><span data-stu-id="4d245-115">For more information, see [Posting Group Setups](finance-posting-groups.md)</span></span>  

## <a name="the-chart-of-accounts"></a><span data-ttu-id="4d245-116">The Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="4d245-116">The Chart of Accounts</span></span>
<span data-ttu-id="4d245-117">The chart of accounts shows all general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="4d245-117">The chart of accounts shows all general ledger accounts.</span></span> <span data-ttu-id="4d245-118">From the chart of accounts, you can do things like:</span><span class="sxs-lookup"><span data-stu-id="4d245-118">From the chart of accounts, you can do things like:</span></span>  

* <span data-ttu-id="4d245-119">View reports that show general ledger entries and balances.</span><span class="sxs-lookup"><span data-stu-id="4d245-119">View reports that show general ledger entries and balances.</span></span>  
* <span data-ttu-id="4d245-120">Close your income statement.</span><span class="sxs-lookup"><span data-stu-id="4d245-120">Close your income statement.</span></span>  
* <span data-ttu-id="4d245-121">Open the G/L account card to add or change settings.</span><span class="sxs-lookup"><span data-stu-id="4d245-121">Open the G/L account card to add or change settings.</span></span>  
* <span data-ttu-id="4d245-122">See a list of posting groups that post to that account.</span><span class="sxs-lookup"><span data-stu-id="4d245-122">See a list of posting groups that post to that account.</span></span>
* <span data-ttu-id="4d245-123">View separate debit and credit balances for a single account</span><span class="sxs-lookup"><span data-stu-id="4d245-123">View separate debit and credit balances for a single account</span></span>  

<span data-ttu-id="4d245-124">You can add, change, or delete general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="4d245-124">You can add, change, or delete general ledger accounts.</span></span> <span data-ttu-id="4d245-125">However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="4d245-125">However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.</span></span>  

## <a name="account-categories"></a><span data-ttu-id="4d245-126">Account Categories</span><span class="sxs-lookup"><span data-stu-id="4d245-126">Account Categories</span></span>
<span data-ttu-id="4d245-127">You can personalise the structure of your financial statements by mapping general ledger accounts to account categories.</span><span class="sxs-lookup"><span data-stu-id="4d245-127">You can personalize the structure of your financial statements by mapping general ledger accounts to account categories.</span></span>  

<span data-ttu-id="4d245-128">The **G/L Account Categories** window shows your categories and subcategories, and the G/L accounts that are assigned to them.</span><span class="sxs-lookup"><span data-stu-id="4d245-128">The **G/L Account Categories** window shows your categories and subcategories, and the G/L accounts that are assigned to them.</span></span> <span data-ttu-id="4d245-129">You can create new subcategories and assign those categories to existing accounts.</span><span class="sxs-lookup"><span data-stu-id="4d245-129">You can create new subcategories and assign those categories to existing accounts.</span></span>  

<span data-ttu-id="4d245-130">You create a category group by indenting other subcategories under a line in the **G/L Account Categories** window.</span><span class="sxs-lookup"><span data-stu-id="4d245-130">You create a category group by indenting other subcategories under a line in the **G/L Account Categories** window.</span></span> <span data-ttu-id="4d245-131">This makes it easy for you to get an overview, because each grouping shows a total balance.</span><span class="sxs-lookup"><span data-stu-id="4d245-131">This makes it easy for you to get an overview, because each grouping shows a total balance.</span></span> <span data-ttu-id="4d245-132">For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.</span><span class="sxs-lookup"><span data-stu-id="4d245-132">For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.</span></span>  

<span data-ttu-id="4d245-133">You can specify whether the accounts in each subcategory must be included in specific types of reports.</span><span class="sxs-lookup"><span data-stu-id="4d245-133">You can specify whether the accounts in each subcategory must be included in specific types of reports.</span></span> <span data-ttu-id="4d245-134">The account categories help define the layout of your financial statements.</span><span class="sxs-lookup"><span data-stu-id="4d245-134">The account categories help define the layout of your financial statements.</span></span>  

<span data-ttu-id="4d245-135">For example, the default balance statement has a subcategory for Cash under Current Assets.</span><span class="sxs-lookup"><span data-stu-id="4d245-135">For example, the default balance statement has a subcategory for Cash under Current Assets.</span></span> <span data-ttu-id="4d245-136">If you want the balance statement consider petty cash and chequing, you can:</span><span class="sxs-lookup"><span data-stu-id="4d245-136">If you want the balance statement consider petty cash and checking, you can:</span></span>  

1. <span data-ttu-id="4d245-137">Add two new subcategories.</span><span class="sxs-lookup"><span data-stu-id="4d245-137">Add two new subcategories.</span></span> <span data-ttu-id="4d245-138">One for petty cash, and one for your current account.</span><span class="sxs-lookup"><span data-stu-id="4d245-138">One for petty cash, and one for your checking account.</span></span>  
2. <span data-ttu-id="4d245-139">Specify the additional report definition **Cash Accounts** for these subcategories.</span><span class="sxs-lookup"><span data-stu-id="4d245-139">Specify the additional report definition **Cash Accounts** for these subcategories.</span></span>  
3. <span data-ttu-id="4d245-140">Indent them under the **Cash** subcategory.</span><span class="sxs-lookup"><span data-stu-id="4d245-140">Indent them under the **Cash** subcategory.</span></span>  

<span data-ttu-id="4d245-141">The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the current account.</span><span class="sxs-lookup"><span data-stu-id="4d245-141">The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the checking account.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4d245-142">See Also</span><span class="sxs-lookup"><span data-stu-id="4d245-142">See Also</span></span>
[<span data-ttu-id="4d245-143">Finance</span><span class="sxs-lookup"><span data-stu-id="4d245-143">Finance</span></span>](finance.md)  
[<span data-ttu-id="4d245-144">Setting Up or Changing the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="4d245-144">Setting Up or Changing the Chart of Accounts</span></span>](finance-setup-chart-accounts.md)  
[<span data-ttu-id="4d245-145">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="4d245-145">Business Intelligence</span></span>](bi.md)  

