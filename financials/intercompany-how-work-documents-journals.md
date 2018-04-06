---
title: Post Intercompany Documents and Journals| Microsoft Docs
description: Use intercompany documents to post transactions with your intercompany partners.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: IC, group, consolidation, affiliate, subsidiary
ms.date: 06/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 98e0d9012dfdd998431aaed8dade02f592af47c8
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="work-with-intercompany-documents-and-journals"></a><span data-ttu-id="b75f9-103">Work with Intercompany Documents and Journals</span><span class="sxs-lookup"><span data-stu-id="b75f9-103">Work with Intercompany Documents and Journals</span></span>
<span data-ttu-id="b75f9-104">You use intercompany documents or journals to post transactions with your intercompany partners.</span><span class="sxs-lookup"><span data-stu-id="b75f9-104">You use intercompany documents or journals to post transactions with your intercompany partners.</span></span> <span data-ttu-id="b75f9-105">When you post an intercompany document or journal line in your company, a corresponding document or journal line is created in your intercompany outbox that you can transfer to your partner.</span><span class="sxs-lookup"><span data-stu-id="b75f9-105">When you post an intercompany document or journal line in your company, a corresponding document or journal line is created in your intercompany outbox that you can transfer to your partner.</span></span> <span data-ttu-id="b75f9-106">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span><span class="sxs-lookup"><span data-stu-id="b75f9-106">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span></span>

<span data-ttu-id="b75f9-107">For sales and purchase documents, the intercompany partner code on the involved customer or vendor ensures that all orders and invoices generated pertaining to transactions with these companies will produce corresponding documents in the partner company, resulting in correct balancing of the accounts.</span><span class="sxs-lookup"><span data-stu-id="b75f9-107">For sales and purchase documents, the intercompany partner code on the involved customer or vendor ensures that all orders and invoices generated pertaining to transactions with these companies will produce corresponding documents in the partner company, resulting in correct balancing of the accounts.</span></span>

<span data-ttu-id="b75f9-108">For intercompany general journal lines, you do not need to specify the accounts for an individual set of books, but simply give the identification of the partner company.</span><span class="sxs-lookup"><span data-stu-id="b75f9-108">For intercompany general journal lines, you do not need to specify the accounts for an individual set of books, but simply give the identification of the partner company.</span></span> <span data-ttu-id="b75f9-109">Corresponding intercompany general journal lines are then created in the partner company that result in the balancing of the books of both companies involved in a transaction.</span><span class="sxs-lookup"><span data-stu-id="b75f9-109">Corresponding intercompany general journal lines are then created in the partner company that result in the balancing of the books of both companies involved in a transaction.</span></span>

## <a name="to-fill-in-and-send-an-intercompany-sales-order"></a><span data-ttu-id="b75f9-110">To fill in and send an intercompany sales order</span><span class="sxs-lookup"><span data-stu-id="b75f9-110">To fill in and send an intercompany sales order</span></span>
<span data-ttu-id="b75f9-111">You can send sales and purchase orders and return orders before posting.</span><span class="sxs-lookup"><span data-stu-id="b75f9-111">You can send sales and purchase orders and return orders before posting.</span></span> <span data-ttu-id="b75f9-112">Invoices and credit memos cannot be sent until they are posted.</span><span class="sxs-lookup"><span data-stu-id="b75f9-112">Invoices and credit memos cannot be sent until they are posted.</span></span>

<span data-ttu-id="b75f9-113">The following procedure describes how to fill in and send an intercompany sales order.</span><span class="sxs-lookup"><span data-stu-id="b75f9-113">The following procedure describes how to fill in and send an intercompany sales order.</span></span> <span data-ttu-id="b75f9-114">The same steps apply to intercompany purchase orders and return orders, and to posted intercompany invoices and credit memos.</span><span class="sxs-lookup"><span data-stu-id="b75f9-114">The same steps apply to intercompany purchase orders and return orders, and to posted intercompany invoices and credit memos.</span></span>  

1. <span data-ttu-id="b75f9-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b75f9-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b75f9-116">Choose **New** to create a new sales order.</span><span class="sxs-lookup"><span data-stu-id="b75f9-116">Choose **New** to create a new sales order.</span></span> <span data-ttu-id="b75f9-117">For more information, see [Sell Products](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="b75f9-117">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>  
3. <span data-ttu-id="b75f9-118">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="b75f9-118">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="b75f9-119">Make sure the customer is an intercompany partner.</span><span class="sxs-lookup"><span data-stu-id="b75f9-119">Make sure the customer is an intercompany partner.</span></span>
5. <span data-ttu-id="b75f9-120">To send the sales order before you post it, choose the **Send IC Sales Order** action.</span><span class="sxs-lookup"><span data-stu-id="b75f9-120">To send the sales order before you post it, choose the **Send IC Sales Order** action.</span></span>

> [!NOTE]
> <span data-ttu-id="b75f9-121">If you do perform step 4, then the sales order will be moved to your intercompany outbox where you can send it later.</span><span class="sxs-lookup"><span data-stu-id="b75f9-121">If you do perform step 4, then the sales order will be moved to your intercompany outbox where you can send it later.</span></span> <span data-ttu-id="b75f9-122">For more information, see [Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="b75f9-122">For more information, see [Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span></span>

## <a name="to-fill-in-and-post-an-intercompany-journal"></a><span data-ttu-id="b75f9-123">To fill in and post an intercompany journal</span><span class="sxs-lookup"><span data-stu-id="b75f9-123">To fill in and post an intercompany journal</span></span>
<span data-ttu-id="b75f9-124">When you post an intercompany general journal line in your company, a corresponding journal line is created in your intercompany outbox that you can transfer to your partner.</span><span class="sxs-lookup"><span data-stu-id="b75f9-124">When you post an intercompany general journal line in your company, a corresponding journal line is created in your intercompany outbox that you can transfer to your partner.</span></span> <span data-ttu-id="b75f9-125">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span><span class="sxs-lookup"><span data-stu-id="b75f9-125">Your partner can then post the corresponding transaction in their company, without having to re-enter the data.</span></span>

1. <span data-ttu-id="b75f9-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IC General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b75f9-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **IC General Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b75f9-127">Open the relevant journal batch.</span><span class="sxs-lookup"><span data-stu-id="b75f9-127">Open the relevant journal batch.</span></span> <span data-ttu-id="b75f9-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="b75f9-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="b75f9-129">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="b75f9-129">Fill in the fields as necessary.</span></span>
4. <span data-ttu-id="b75f9-130">In the **IC Partner G/L Acc. No.** field, enter the intercompany general ledger account that the amount will be posted to in your partner's company.</span><span class="sxs-lookup"><span data-stu-id="b75f9-130">In the **IC Partner G/L Acc. No.** field, enter the intercompany general ledger account that the amount will be posted to in your partner's company.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b75f9-131">This field must be filled in on a line with a bank account or general ledger account in either the **Account No.** field or the **Bal. Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="b75f9-131">This field must be filled in on a line with a bank account or general ledger account in either the **Account No.** field or the **Bal. Account No.** field.</span></span>  
5. <span data-ttu-id="b75f9-132">Choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="b75f9-132">Choose the **Post** action.</span></span>

<span data-ttu-id="b75f9-133">The involved entries are posted in your company and a journal with the corresponding entries are created in your intercompany outbox that you can send to your partner company.</span><span class="sxs-lookup"><span data-stu-id="b75f9-133">The involved entries are posted in your company and a journal with the corresponding entries are created in your intercompany outbox that you can send to your partner company.</span></span> <span data-ttu-id="b75f9-134">For more information, see [Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="b75f9-134">For more information, see [Manage the Intercompany Inbox and Outbox](intercompany-how-manage-intercompany-inbox.md).</span></span> 

## <a name="see-also"></a><span data-ttu-id="b75f9-135">See Also</span><span class="sxs-lookup"><span data-stu-id="b75f9-135">See Also</span></span>
[<span data-ttu-id="b75f9-136">Managing Intercompany Transactions</span><span class="sxs-lookup"><span data-stu-id="b75f9-136">Managing Intercompany Transactions</span></span>](intercompany-manage.md)  
[<span data-ttu-id="b75f9-137">Finance</span><span class="sxs-lookup"><span data-stu-id="b75f9-137">Finance</span></span>](finance.md)  
[<span data-ttu-id="b75f9-138">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="b75f9-138">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="b75f9-139">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="b75f9-139">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="b75f9-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b75f9-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

