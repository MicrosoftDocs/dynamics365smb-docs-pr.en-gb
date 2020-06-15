---
title: How to Block Sales to Customers
description: If needed, you can block a customer from being included on sales documents and other sales transactions.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 7cc82ab0aaf28b355117571d0d2cc5869141693f
ms.sourcegitcommit: 4545bb597dd9dc4c563b30af762977ee1d815497
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/29/2020
ms.locfileid: "3410723"
---
# <a name="block-customers"></a><span data-ttu-id="c98dc-103">Block Customers</span><span class="sxs-lookup"><span data-stu-id="c98dc-103">Block Customers</span></span>
<span data-ttu-id="c98dc-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span><span class="sxs-lookup"><span data-stu-id="c98dc-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span></span>

<span data-ttu-id="c98dc-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span><span class="sxs-lookup"><span data-stu-id="c98dc-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span></span> <span data-ttu-id="c98dc-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="c98dc-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>   

<span data-ttu-id="c98dc-107">The following table describes the options for blocking customers.</span><span class="sxs-lookup"><span data-stu-id="c98dc-107">The following table describes the options for blocking customers.</span></span>  

|<span data-ttu-id="c98dc-108">Option</span><span class="sxs-lookup"><span data-stu-id="c98dc-108">Option</span></span>|<span data-ttu-id="c98dc-109">Description</span><span class="sxs-lookup"><span data-stu-id="c98dc-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="c98dc-110">**Blank**</span><span class="sxs-lookup"><span data-stu-id="c98dc-110">**Blank**</span></span>|<span data-ttu-id="c98dc-111">Transactions are allowed for this customer.</span><span class="sxs-lookup"><span data-stu-id="c98dc-111">Transactions are allowed for this customer.</span></span>|
|<span data-ttu-id="c98dc-112">**Ship**</span><span class="sxs-lookup"><span data-stu-id="c98dc-112">**Ship**</span></span>|<span data-ttu-id="c98dc-113">New orders and new shipments cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="c98dc-113">New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="c98dc-114">Existing shipments not yet invoiced can be invoiced.</span><span class="sxs-lookup"><span data-stu-id="c98dc-114">Existing shipments not yet invoiced can be invoiced.</span></span>|  
|<span data-ttu-id="c98dc-115">**Invoice**</span><span class="sxs-lookup"><span data-stu-id="c98dc-115">**Invoice**</span></span>|<span data-ttu-id="c98dc-116">New orders, new shipments, and new invoices cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="c98dc-116">New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="c98dc-117">Existing shipments not yet invoiced cannot be invoiced.</span><span class="sxs-lookup"><span data-stu-id="c98dc-117">Existing shipments not yet invoiced cannot be invoiced.</span></span> <span data-ttu-id="c98dc-118">You can still send reminders and finance charge memos to the customer.</span><span class="sxs-lookup"><span data-stu-id="c98dc-118">You can still send reminders and finance charge memos to the customer.</span></span>|  
|<span data-ttu-id="c98dc-119">**All**</span><span class="sxs-lookup"><span data-stu-id="c98dc-119">**All**</span></span>|<span data-ttu-id="c98dc-120">No transaction is allowed for this customer, including payments.</span><span class="sxs-lookup"><span data-stu-id="c98dc-120">No transaction is allowed for this customer, including payments.</span></span>|  

## <a name="to-block-a-customer"></a><span data-ttu-id="c98dc-121">To block a customer</span><span class="sxs-lookup"><span data-stu-id="c98dc-121">To block a customer</span></span>  
1. <span data-ttu-id="c98dc-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c98dc-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="c98dc-123">Select a customer, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="c98dc-123">Select a customer, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="c98dc-124">In the **Blocked** field, choose what to block, as described in the table above.</span><span class="sxs-lookup"><span data-stu-id="c98dc-124">In the **Blocked** field, choose what to block, as described in the table above.</span></span>

## <a name="see-also"></a><span data-ttu-id="c98dc-125">See Also</span><span class="sxs-lookup"><span data-stu-id="c98dc-125">See Also</span></span>  
[<span data-ttu-id="c98dc-126">Register New Customers</span><span class="sxs-lookup"><span data-stu-id="c98dc-126">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="c98dc-127">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="c98dc-127">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="c98dc-128">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="c98dc-128">Managing Receivables</span></span>](receivables-manage-receivables.md)  
