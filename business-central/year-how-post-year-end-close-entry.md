---
title: Post the Year-End Closing Entry
description: Describes how to open the journal you specified in the Close Income Statement batch job, and then review and post the year-end closing entry.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 5c822685ae5723bc6b13f9fedad45dbddefdb956
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776599"
---
# <a name="post-the-year-end-closing-entry"></a><span data-ttu-id="63a59-103">Post the Year-End Closing Entry</span><span class="sxs-lookup"><span data-stu-id="63a59-103">Post the Year-End Closing Entry</span></span>

<span data-ttu-id="63a59-104">After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.</span><span class="sxs-lookup"><span data-stu-id="63a59-104">After you use the **Close Income Statement** batch job to generate the year-end closing entry or entries, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>  

> [!TIP]
> <span data-ttu-id="63a59-105">Depending on your organisations work processes, you can choose to close or not close accounting periods and fiscal years in [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="63a59-105">Depending on your organizations work processes, you can choose to close or not close accounting periods and fiscal years in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="63a59-106">The following procedure assumes that you have closed the fiscal year using the *Accounting Periods* option, generated a year-end closing entry using the **Close Income Statement** batch job, and are now ready to post the year-end closing entry along with the offsetting equity account entries.</span><span class="sxs-lookup"><span data-stu-id="63a59-106">The following procedure assumes that you have closed the fiscal year using the *Accounting Periods* option, generated a year-end closing entry using the **Close Income Statement** batch job, and are now ready to post the year-end closing entry along with the offsetting equity account entries.</span></span> <span data-ttu-id="63a59-107">Your organisation can choose to work differently, such as post the year-end closing entry as part of closing the fiscal year.</span><span class="sxs-lookup"><span data-stu-id="63a59-107">Your organization can choose to work differently, such as post the year-end closing entry as part of closing the fiscal year.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="63a59-108">To post the year end closing entry</span><span class="sxs-lookup"><span data-stu-id="63a59-108">To post the year end closing entry</span></span>

1. <span data-ttu-id="63a59-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63a59-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="63a59-110">On the **General Journal** page, in the **Batch Name** field, select the batch that contains the closing entries.</span><span class="sxs-lookup"><span data-stu-id="63a59-110">On the **General Journal** page, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="63a59-111">Review the entries.</span><span class="sxs-lookup"><span data-stu-id="63a59-111">Review the entries.</span></span>
4. <span data-ttu-id="63a59-112">To post the journal, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="63a59-112">To post the journal, choose the **Post** action.</span></span>

> [!NOTE]  
> <span data-ttu-id="63a59-113">If an error is detected, an error message is displayed.</span><span class="sxs-lookup"><span data-stu-id="63a59-113">If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="63a59-114">If the posting is successful, the posted entries are removed from the journal.</span><span class="sxs-lookup"><span data-stu-id="63a59-114">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="63a59-115">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span><span class="sxs-lookup"><span data-stu-id="63a59-115">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="63a59-116">See Also</span><span class="sxs-lookup"><span data-stu-id="63a59-116">See Also</span></span>

[<span data-ttu-id="63a59-117">Close Accounting Periods</span><span class="sxs-lookup"><span data-stu-id="63a59-117">Close Accounting Periods</span></span>](year-close-account-periods.md)  
[<span data-ttu-id="63a59-118">Closing Books</span><span class="sxs-lookup"><span data-stu-id="63a59-118">Closing Books</span></span>](year-close-books.md)  
[<span data-ttu-id="63a59-119">Close Income Statement</span><span class="sxs-lookup"><span data-stu-id="63a59-119">Close Income Statement</span></span>](year-close-income-statement.md)  
<span data-ttu-id="63a59-120">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="63a59-120">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]