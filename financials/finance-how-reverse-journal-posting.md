---
title: Undo a Journal Posting by Posting a Reversing Entry| Microsoft Docs
description: If you have made an erroneous posting in the general journal, then you can use the Reverse Transaction function to undo the posting with a correct audit trail.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 06/15/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 8126a53d59e72276eb1558fd65fe3c0cd53600cc
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-reverse-journal-posting"></a><span data-ttu-id="1434e-103">How to: Reverse Journal Posting</span><span class="sxs-lookup"><span data-stu-id="1434e-103">How to: Reverse Journal Posting</span></span>
<span data-ttu-id="1434e-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span><span class="sxs-lookup"><span data-stu-id="1434e-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="1434e-105">After reversing an entry, you must make the correct entry.</span><span class="sxs-lookup"><span data-stu-id="1434e-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="1434e-106">You can only reverse entries that are posted from a general journal line.</span><span class="sxs-lookup"><span data-stu-id="1434e-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="1434e-107">An entry can only be reversed once.</span><span class="sxs-lookup"><span data-stu-id="1434e-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="1434e-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="1434e-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="1434e-109">You can reverse entries from all **Ledger Entries** windows.</span><span class="sxs-lookup"><span data-stu-id="1434e-109">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="1434e-110">The following procedure is based on the **General Ledger Entries** window.</span><span class="sxs-lookup"><span data-stu-id="1434e-110">The following procedure is based on the **General Ledger Entries** window.</span></span>

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="1434e-111">To reverse the journal posting of a general ledger entry</span><span class="sxs-lookup"><span data-stu-id="1434e-111">To reverse the journal posting of a general ledger entry</span></span>
1. <span data-ttu-id="1434e-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="1434e-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="1434e-113">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span><span class="sxs-lookup"><span data-stu-id="1434e-113">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="1434e-114">Note that is must originate from a journal posting.</span><span class="sxs-lookup"><span data-stu-id="1434e-114">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="1434e-115">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span><span class="sxs-lookup"><span data-stu-id="1434e-115">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="1434e-116">Choose the **Yes** button on the confirmation message.</span><span class="sxs-lookup"><span data-stu-id="1434e-116">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="see-also"></a><span data-ttu-id="1434e-117">See Also</span><span class="sxs-lookup"><span data-stu-id="1434e-117">See Also</span></span>
[<span data-ttu-id="1434e-118">How to: Post Transactions Directly to the General Ledger</span><span class="sxs-lookup"><span data-stu-id="1434e-118">How to: Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="1434e-119">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="1434e-119">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="1434e-120">Finance</span><span class="sxs-lookup"><span data-stu-id="1434e-120">Finance</span></span>](finance.md)  
<span data-ttu-id="1434e-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1434e-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

