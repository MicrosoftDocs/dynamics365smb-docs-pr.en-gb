---
title: Learn About General Ledger and COA| Microsoft Docs
description: Describes the general ledger, the chart of accounts, and account categories.
services: project-madeira
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 04/01/2019
ms.author: edupont
ms.openlocfilehash: b16c36bb5e6f3d9a6909f1937e793599062114c6
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1242728"
---
# <a name="understanding-the-general-ledger-and-the-coa"></a><span data-ttu-id="656ab-103">Understanding the General Ledger and the COA</span><span class="sxs-lookup"><span data-stu-id="656ab-103">Understanding the General Ledger and the COA</span></span>
<span data-ttu-id="656ab-104">The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to.</span><span class="sxs-lookup"><span data-stu-id="656ab-104">The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="656ab-105">includes a standard chart of accounts that is ready to support your business.</span><span class="sxs-lookup"><span data-stu-id="656ab-105">includes a standard chart of accounts that is ready to support your business.</span></span>

## <a name="general-ledger-setup-and-general-posting-setup"></a><span data-ttu-id="656ab-106">General Ledger Setup and General Posting Setup</span><span class="sxs-lookup"><span data-stu-id="656ab-106">General Ledger Setup and General Posting Setup</span></span>
<span data-ttu-id="656ab-107">The setup of the general ledger is at the core of financial processes because it defines how you post data.</span><span class="sxs-lookup"><span data-stu-id="656ab-107">The setup of the general ledger is at the core of financial processes because it defines how you post data.</span></span>  

<span data-ttu-id="656ab-108">On the **General Ledger Setup** page, you specify how to handle certain accounting issues in your company, such as:</span><span class="sxs-lookup"><span data-stu-id="656ab-108">On the **General Ledger Setup** page, you specify how to handle certain accounting issues in your company, such as:</span></span>  

* <span data-ttu-id="656ab-109">Invoice rounding details</span><span class="sxs-lookup"><span data-stu-id="656ab-109">Invoice rounding details</span></span>  
* <span data-ttu-id="656ab-110">Address formats</span><span class="sxs-lookup"><span data-stu-id="656ab-110">Address formats</span></span>  
* <span data-ttu-id="656ab-111">Financial reporting</span><span class="sxs-lookup"><span data-stu-id="656ab-111">Financial reporting</span></span>  

<span data-ttu-id="656ab-112">Similarly, on the **General Posting Setup** page, you specify how you want to set up combinations of general business and general product posting groups.</span><span class="sxs-lookup"><span data-stu-id="656ab-112">Similarly, on the **General Posting Setup** page, you specify how you want to set up combinations of general business and general product posting groups.</span></span> <span data-ttu-id="656ab-113">Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="656ab-113">Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts.</span></span> <span data-ttu-id="656ab-114">You fill in a line for each combination of business posting group and product posting group.</span><span class="sxs-lookup"><span data-stu-id="656ab-114">You fill in a line for each combination of business posting group and product posting group.</span></span> <span data-ttu-id="656ab-115">For more information, see [Posting Group Setups](finance-posting-groups.md)</span><span class="sxs-lookup"><span data-stu-id="656ab-115">For more information, see [Posting Group Setups](finance-posting-groups.md)</span></span>  

## <a name="the-chart-of-accounts"></a><span data-ttu-id="656ab-116">The Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="656ab-116">The Chart of Accounts</span></span>
<span data-ttu-id="656ab-117">The chart of accounts shows all general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="656ab-117">The chart of accounts shows all general ledger accounts.</span></span> <span data-ttu-id="656ab-118">From the chart of accounts, you can do things like:</span><span class="sxs-lookup"><span data-stu-id="656ab-118">From the chart of accounts, you can do things like:</span></span>  

* <span data-ttu-id="656ab-119">View reports that show general ledger entries and balances.</span><span class="sxs-lookup"><span data-stu-id="656ab-119">View reports that show general ledger entries and balances.</span></span>  
* <span data-ttu-id="656ab-120">Close your income statement.</span><span class="sxs-lookup"><span data-stu-id="656ab-120">Close your income statement.</span></span>  
* <span data-ttu-id="656ab-121">Open the G/L account card to add or change settings.</span><span class="sxs-lookup"><span data-stu-id="656ab-121">Open the G/L account card to add or change settings.</span></span>  
* <span data-ttu-id="656ab-122">See a list of posting groups that post to that account.</span><span class="sxs-lookup"><span data-stu-id="656ab-122">See a list of posting groups that post to that account.</span></span>
* <span data-ttu-id="656ab-123">View separate debit and credit balances for a single account</span><span class="sxs-lookup"><span data-stu-id="656ab-123">View separate debit and credit balances for a single account</span></span>  

<span data-ttu-id="656ab-124">You can add, change, or delete general ledger accounts.</span><span class="sxs-lookup"><span data-stu-id="656ab-124">You can add, change, or delete general ledger accounts.</span></span> <span data-ttu-id="656ab-125">However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="656ab-125">However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.</span></span>  

## <a name="account-categories"></a><span data-ttu-id="656ab-126">Account Categories</span><span class="sxs-lookup"><span data-stu-id="656ab-126">Account Categories</span></span>
<span data-ttu-id="656ab-127">You can personalise the structure of your financial statements by mapping general ledger accounts to account categories.</span><span class="sxs-lookup"><span data-stu-id="656ab-127">You can personalize the structure of your financial statements by mapping general ledger accounts to account categories.</span></span>  

<span data-ttu-id="656ab-128">The **G/L Account Categories** page shows your categories and subcategories, and the G/L accounts that are assigned to them.</span><span class="sxs-lookup"><span data-stu-id="656ab-128">The **G/L Account Categories** page shows your categories and subcategories, and the G/L accounts that are assigned to them.</span></span> <span data-ttu-id="656ab-129">You can create new subcategories and assign those categories to existing accounts.</span><span class="sxs-lookup"><span data-stu-id="656ab-129">You can create new subcategories and assign those categories to existing accounts.</span></span>  

<span data-ttu-id="656ab-130">You create a category group by indenting other subcategories under a line on the **G/L Account Categories** page.</span><span class="sxs-lookup"><span data-stu-id="656ab-130">You create a category group by indenting other subcategories under a line on the **G/L Account Categories** page.</span></span> <span data-ttu-id="656ab-131">This makes it easy for you to get an overview, because each grouping shows a total balance.</span><span class="sxs-lookup"><span data-stu-id="656ab-131">This makes it easy for you to get an overview, because each grouping shows a total balance.</span></span> <span data-ttu-id="656ab-132">For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.</span><span class="sxs-lookup"><span data-stu-id="656ab-132">For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.</span></span>  

<span data-ttu-id="656ab-133">You can specify whether the accounts in each subcategory must be included in specific types of reports.</span><span class="sxs-lookup"><span data-stu-id="656ab-133">You can specify whether the accounts in each subcategory must be included in specific types of reports.</span></span> <span data-ttu-id="656ab-134">The account categories help define the layout of your financial statements.</span><span class="sxs-lookup"><span data-stu-id="656ab-134">The account categories help define the layout of your financial statements.</span></span>  

<span data-ttu-id="656ab-135">For example, the default balance statement has a subcategory for Cash under Current Assets.</span><span class="sxs-lookup"><span data-stu-id="656ab-135">For example, the default balance statement has a subcategory for Cash under Current Assets.</span></span> <span data-ttu-id="656ab-136">If you want the balance statement consider petty cash and chequing, you can:</span><span class="sxs-lookup"><span data-stu-id="656ab-136">If you want the balance statement consider petty cash and checking, you can:</span></span>  

1. <span data-ttu-id="656ab-137">Add two new subcategories.</span><span class="sxs-lookup"><span data-stu-id="656ab-137">Add two new subcategories.</span></span> <span data-ttu-id="656ab-138">One for petty cash, and one for your current account.</span><span class="sxs-lookup"><span data-stu-id="656ab-138">One for petty cash, and one for your checking account.</span></span>  
2. <span data-ttu-id="656ab-139">Specify the additional report definition **Cash Accounts** for these subcategories.</span><span class="sxs-lookup"><span data-stu-id="656ab-139">Specify the additional report definition **Cash Accounts** for these subcategories.</span></span>  
3. <span data-ttu-id="656ab-140">Indent them under the **Cash** subcategory.</span><span class="sxs-lookup"><span data-stu-id="656ab-140">Indent them under the **Cash** subcategory.</span></span>  

<span data-ttu-id="656ab-141">The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the current account.</span><span class="sxs-lookup"><span data-stu-id="656ab-141">The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the checking account.</span></span>  

## <a name="see-also"></a><span data-ttu-id="656ab-142">See Also</span><span class="sxs-lookup"><span data-stu-id="656ab-142">See Also</span></span>
[<span data-ttu-id="656ab-143">Finance</span><span class="sxs-lookup"><span data-stu-id="656ab-143">Finance</span></span>](finance.md)  
[<span data-ttu-id="656ab-144">Setting Up or Changing the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="656ab-144">Setting Up or Changing the Chart of Accounts</span></span>](finance-setup-chart-accounts.md)  
[<span data-ttu-id="656ab-145">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="656ab-145">Business Intelligence</span></span>](bi.md)  
