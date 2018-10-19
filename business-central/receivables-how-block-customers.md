---
title: How to Block Sales to Customers  Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 268d098318b77cb89a369e8edc14729a44bedae6
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="block-customers"></a><span data-ttu-id="475ad-103">Block Customers</span><span class="sxs-lookup"><span data-stu-id="475ad-103">Block Customers</span></span>
<span data-ttu-id="475ad-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span><span class="sxs-lookup"><span data-stu-id="475ad-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span></span>

<span data-ttu-id="475ad-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span><span class="sxs-lookup"><span data-stu-id="475ad-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span></span> <span data-ttu-id="475ad-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="475ad-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>   

<span data-ttu-id="475ad-107">The following table describes the different blocking options.</span><span class="sxs-lookup"><span data-stu-id="475ad-107">The following table describes the different blocking options.</span></span>  

|<span data-ttu-id="475ad-108">Option</span><span class="sxs-lookup"><span data-stu-id="475ad-108">Option</span></span>|<span data-ttu-id="475ad-109">Description</span><span class="sxs-lookup"><span data-stu-id="475ad-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="475ad-110">**Blank**</span><span class="sxs-lookup"><span data-stu-id="475ad-110">**Blank**</span></span>|<span data-ttu-id="475ad-111">Transactions are allowed for this customer.</span><span class="sxs-lookup"><span data-stu-id="475ad-111">Transactions are allowed for this customer.</span></span>|
|<span data-ttu-id="475ad-112">**Ship**</span><span class="sxs-lookup"><span data-stu-id="475ad-112">**Ship**</span></span>|<span data-ttu-id="475ad-113">New orders and new shipments cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="475ad-113">New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="475ad-114">Existing shipments not yet invoiced can be invoiced.</span><span class="sxs-lookup"><span data-stu-id="475ad-114">Existing shipments not yet invoiced can be invoiced.</span></span>|  
|<span data-ttu-id="475ad-115">**Invoice**</span><span class="sxs-lookup"><span data-stu-id="475ad-115">**Invoice**</span></span>|<span data-ttu-id="475ad-116">New orders, new shipments, and new invoices cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="475ad-116">New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="475ad-117">Existing shipments not yet invoiced cannot be invoiced.</span><span class="sxs-lookup"><span data-stu-id="475ad-117">Existing shipments not yet invoiced cannot be invoiced.</span></span>|  
|<span data-ttu-id="475ad-118">**All**</span><span class="sxs-lookup"><span data-stu-id="475ad-118">**All**</span></span>|<span data-ttu-id="475ad-119">No transaction is allowed for this customer, including payments.</span><span class="sxs-lookup"><span data-stu-id="475ad-119">No transaction is allowed for this customer, including payments.</span></span>|  

## <a name="to-block-a-customer"></a><span data-ttu-id="475ad-120">To block a customer</span><span class="sxs-lookup"><span data-stu-id="475ad-120">To block a customer</span></span>  
1. <span data-ttu-id="475ad-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="475ad-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="475ad-122">Select a customer, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="475ad-122">Select a customer, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="475ad-123">Fill in the **Blocked** field with one of the options described above.</span><span class="sxs-lookup"><span data-stu-id="475ad-123">Fill in the **Blocked** field with one of the options described above.</span></span>

## <a name="see-also"></a><span data-ttu-id="475ad-124">See Also</span><span class="sxs-lookup"><span data-stu-id="475ad-124">See Also</span></span>  
[<span data-ttu-id="475ad-125">Register New Customers</span><span class="sxs-lookup"><span data-stu-id="475ad-125">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="475ad-126">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="475ad-126">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="475ad-127">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="475ad-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  

