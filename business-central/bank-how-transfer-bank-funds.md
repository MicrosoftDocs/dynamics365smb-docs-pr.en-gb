---
title: Transfer Bank Funds| Microsoft Docs
description: You can transfer amounts from one bank account to another, including different currencies, by posting the transaction in the general journal.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 69e5f439ee8a02ae553d8b148480b655596e2951
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1244177"
---
# <a name="transfer-bank-funds"></a><span data-ttu-id="b1a42-103">Transfer Bank Funds</span><span class="sxs-lookup"><span data-stu-id="b1a42-103">Transfer Bank Funds</span></span>
<span data-ttu-id="b1a42-104">You may sometimes need to transfer an amount from one bank account to another.</span><span class="sxs-lookup"><span data-stu-id="b1a42-104">You may sometimes need to transfer an amount from one bank account to another.</span></span> <span data-ttu-id="b1a42-105">To do this, you must post the a transaction in the general journal.</span><span class="sxs-lookup"><span data-stu-id="b1a42-105">To do this, you must post the a transaction in the general journal.</span></span> <span data-ttu-id="b1a42-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span><span class="sxs-lookup"><span data-stu-id="b1a42-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="b1a42-107">To post a transfer between bank accounts with the same currency code</span><span class="sxs-lookup"><span data-stu-id="b1a42-107">To post a transfer between bank accounts with the same currency code</span></span>
1. <span data-ttu-id="b1a42-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b1a42-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1a42-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="b1a42-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="b1a42-110">In the **Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="b1a42-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="b1a42-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="b1a42-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="b1a42-112">In the **Amount** field, enter the amount to be transferred.</span><span class="sxs-lookup"><span data-stu-id="b1a42-112">In the **Amount** field, enter the amount to be transferred.</span></span>
6. <span data-ttu-id="b1a42-113">Choose the **Show More Columns** action to view all available fields.</span><span class="sxs-lookup"><span data-stu-id="b1a42-113">Choose the **Show More Columns** action to view all available fields.</span></span>
7. <span data-ttu-id="b1a42-114">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="b1a42-114">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
8. <span data-ttu-id="b1a42-115">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="b1a42-115">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
9. <span data-ttu-id="b1a42-116">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="b1a42-116">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="b1a42-117">To post a transfer between bank accounts with different currency codes</span><span class="sxs-lookup"><span data-stu-id="b1a42-117">To post a transfer between bank accounts with different currency codes</span></span>
<span data-ttu-id="b1a42-118">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span><span class="sxs-lookup"><span data-stu-id="b1a42-118">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="b1a42-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b1a42-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="b1a42-120">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="b1a42-120">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="b1a42-121">On the first journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="b1a42-121">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="b1a42-122">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="b1a42-122">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="b1a42-123">In the **Amount** field, enter the amount in the currency of the bank account.</span><span class="sxs-lookup"><span data-stu-id="b1a42-123">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="b1a42-124">Enter credit amounts with a minus sign.</span><span class="sxs-lookup"><span data-stu-id="b1a42-124">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="b1a42-125">Enter debit amounts without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="b1a42-125">Enter debit amounts without a minus sign.</span></span>
6. <span data-ttu-id="b1a42-126">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="b1a42-126">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="b1a42-127">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="b1a42-127">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="b1a42-128">On the second journal line, in the **Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="b1a42-128">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
9. <span data-ttu-id="b1a42-129">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="b1a42-129">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
10. <span data-ttu-id="b1a42-130">In the **Amount** field, enter the amount in the currency of the bank account.</span><span class="sxs-lookup"><span data-stu-id="b1a42-130">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="b1a42-131">Enter credit amounts with a minus sign.</span><span class="sxs-lookup"><span data-stu-id="b1a42-131">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="b1a42-132">Enter debit amounts without a minus sign.</span><span class="sxs-lookup"><span data-stu-id="b1a42-132">Enter debit amounts without a minus sign.</span></span>
11. <span data-ttu-id="b1a42-133">In the **Bal. Account Type** field, select **Bank Account**.</span><span class="sxs-lookup"><span data-stu-id="b1a42-133">In the **Bal. Account Type** field, select **Bank Account**.</span></span>  
12. <span data-ttu-id="b1a42-134">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span><span class="sxs-lookup"><span data-stu-id="b1a42-134">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span></span>

    > [!NOTE]  
    > <span data-ttu-id="b1a42-135">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a third line for the exchange rate gain or loss.</span><span class="sxs-lookup"><span data-stu-id="b1a42-135">If the exchange rates used in the journal are different than the exchange rates on the **Currency Exchange Rates** page, enter a third line for the exchange rate gain or loss.</span></span> <span data-ttu-id="b1a42-136">Enter **G/L Account** in the **Account Type** field.</span><span class="sxs-lookup"><span data-stu-id="b1a42-136">Enter **G/L Account** in the **Account Type** field.</span></span> <span data-ttu-id="b1a42-137">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="b1a42-137">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span> <span data-ttu-id="b1a42-138">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span><span class="sxs-lookup"><span data-stu-id="b1a42-138">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span></span>
13. <span data-ttu-id="b1a42-139">Post the journal.</span><span class="sxs-lookup"><span data-stu-id="b1a42-139">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="b1a42-140">See Also</span><span class="sxs-lookup"><span data-stu-id="b1a42-140">See Also</span></span>
[<span data-ttu-id="b1a42-141">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="b1a42-141">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="b1a42-142">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="b1a42-142">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="b1a42-143">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="b1a42-143">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="b1a42-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b1a42-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
