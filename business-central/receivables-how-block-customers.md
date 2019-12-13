---
title: How to Block Sales to Customers  Items from Sales or Purchasing
description: In Business Central, an item can be marked as blocked for sales, blocked for purchase, or blocked for all purposes.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: c1b055e5101b99f0b0e1b69169d5c9f2f7e21d09
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/03/2019
ms.locfileid: "2883001"
---
# <a name="block-customers"></a><span data-ttu-id="874ce-103">Block Customers</span><span class="sxs-lookup"><span data-stu-id="874ce-103">Block Customers</span></span>
<span data-ttu-id="874ce-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span><span class="sxs-lookup"><span data-stu-id="874ce-104">You can block a customer, for example because of insolvency, so that the customer cannot be added to sales documents or so that no transactions can be posted for the customer.</span></span>

<span data-ttu-id="874ce-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span><span class="sxs-lookup"><span data-stu-id="874ce-105">In addition to blocking a customer, you can set receivable transactions for the customer to be on hold in connection with reminders.</span></span> <span data-ttu-id="874ce-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="874ce-106">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>   

<span data-ttu-id="874ce-107">The following table describes the different blocking options.</span><span class="sxs-lookup"><span data-stu-id="874ce-107">The following table describes the different blocking options.</span></span>  

|<span data-ttu-id="874ce-108">Option</span><span class="sxs-lookup"><span data-stu-id="874ce-108">Option</span></span>|<span data-ttu-id="874ce-109">Description</span><span class="sxs-lookup"><span data-stu-id="874ce-109">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="874ce-110">**Blank**</span><span class="sxs-lookup"><span data-stu-id="874ce-110">**Blank**</span></span>|<span data-ttu-id="874ce-111">Transactions are allowed for this customer.</span><span class="sxs-lookup"><span data-stu-id="874ce-111">Transactions are allowed for this customer.</span></span>|
|<span data-ttu-id="874ce-112">**Ship**</span><span class="sxs-lookup"><span data-stu-id="874ce-112">**Ship**</span></span>|<span data-ttu-id="874ce-113">New orders and new shipments cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="874ce-113">New orders and new shipments cannot be created for this customer.</span></span> <span data-ttu-id="874ce-114">Existing shipments not yet invoiced can be invoiced.</span><span class="sxs-lookup"><span data-stu-id="874ce-114">Existing shipments not yet invoiced can be invoiced.</span></span>|  
|<span data-ttu-id="874ce-115">**Invoice**</span><span class="sxs-lookup"><span data-stu-id="874ce-115">**Invoice**</span></span>|<span data-ttu-id="874ce-116">New orders, new shipments, and new invoices cannot be created for this customer.</span><span class="sxs-lookup"><span data-stu-id="874ce-116">New orders, new shipments, and new invoices cannot be created for this customer.</span></span> <span data-ttu-id="874ce-117">Existing shipments not yet invoiced cannot be invoiced.</span><span class="sxs-lookup"><span data-stu-id="874ce-117">Existing shipments not yet invoiced cannot be invoiced.</span></span>|  
|<span data-ttu-id="874ce-118">**All**</span><span class="sxs-lookup"><span data-stu-id="874ce-118">**All**</span></span>|<span data-ttu-id="874ce-119">No transaction is allowed for this customer, including payments.</span><span class="sxs-lookup"><span data-stu-id="874ce-119">No transaction is allowed for this customer, including payments.</span></span>|  

## <a name="to-block-a-customer"></a><span data-ttu-id="874ce-120">To block a customer</span><span class="sxs-lookup"><span data-stu-id="874ce-120">To block a customer</span></span>  
1. <span data-ttu-id="874ce-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="874ce-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="874ce-122">Select a customer, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="874ce-122">Select a customer, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="874ce-123">Fill in the **Blocked** field with one of the options described above.</span><span class="sxs-lookup"><span data-stu-id="874ce-123">Fill in the **Blocked** field with one of the options described above.</span></span>

## <a name="see-also"></a><span data-ttu-id="874ce-124">See Also</span><span class="sxs-lookup"><span data-stu-id="874ce-124">See Also</span></span>  
[<span data-ttu-id="874ce-125">Register New Customers</span><span class="sxs-lookup"><span data-stu-id="874ce-125">Register New Customers</span></span>](sales-how-register-new-customers.md)  
[<span data-ttu-id="874ce-126">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="874ce-126">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="874ce-127">Managing Receivables</span><span class="sxs-lookup"><span data-stu-id="874ce-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  
