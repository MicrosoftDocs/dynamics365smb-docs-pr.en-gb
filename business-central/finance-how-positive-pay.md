---
title: Export Positive Pay Files| Microsoft Docs
description: You can ensure your bank only clears validated checks and amounts by exporting a Positive Pay file that contains vendor and payment information.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: be71a8edc556708f88d00b088f49b52e2fd5ee45
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778925"
---
# <a name="export-a-positive-pay-file"></a><span data-ttu-id="ae59d-103">Export a Positive Pay File</span><span class="sxs-lookup"><span data-stu-id="ae59d-103">Export a Positive Pay File</span></span>
<span data-ttu-id="ae59d-104">To make sure that your bank only clears validated cheques and amounts, you can export a Positive Pay file that contains vendor information, cheque number, and payment amount, which you send to the bank for reference when you process payments.</span><span class="sxs-lookup"><span data-stu-id="ae59d-104">To make sure that your bank only clears validated checks and amounts, you can export a Positive Pay file that contains vendor information, check number, and payment amount, which you send to the bank for reference when you process payments.</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ae59d-105">is preconfigured to support Positive Pay files for Bank of America and City Bank.</span><span class="sxs-lookup"><span data-stu-id="ae59d-105">is preconfigured to support Positive Pay files for Bank of America and City Bank.</span></span>

## <a name="to-set-up-a-bank-account-for-positive-pay"></a><span data-ttu-id="ae59d-106">To set up a bank account for Positive Pay</span><span class="sxs-lookup"><span data-stu-id="ae59d-106">To set up a bank account for Positive Pay</span></span>
1. <span data-ttu-id="ae59d-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ae59d-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ae59d-108">Open the card for the bank that you want to use Positive Pay for.</span><span class="sxs-lookup"><span data-stu-id="ae59d-108">Open the card for the bank that you want to use Positive Pay for.</span></span>
3. <span data-ttu-id="ae59d-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span><span class="sxs-lookup"><span data-stu-id="ae59d-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span></span>
4. <span data-ttu-id="ae59d-110">Close the page.</span><span class="sxs-lookup"><span data-stu-id="ae59d-110">Close the page.</span></span>

## <a name="to-export-a-positive-pay-file"></a><span data-ttu-id="ae59d-111">To export a Positive Pay file</span><span class="sxs-lookup"><span data-stu-id="ae59d-111">To export a Positive Pay file</span></span>
1. <span data-ttu-id="ae59d-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ae59d-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ae59d-113">Select the bank account that you want to export a Positive Pay file for.</span><span class="sxs-lookup"><span data-stu-id="ae59d-113">Select the bank account that you want to export a Positive Pay file for.</span></span>
3. <span data-ttu-id="ae59d-114">Choose **Positive Pay Export** action.</span><span class="sxs-lookup"><span data-stu-id="ae59d-114">Choose **Positive Pay Export** action.</span></span>

    <span data-ttu-id="ae59d-115">The **Positive Pay Export** page opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span><span class="sxs-lookup"><span data-stu-id="ae59d-115">The **Positive Pay Export** page opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span></span>
4. <span data-ttu-id="ae59d-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span><span class="sxs-lookup"><span data-stu-id="ae59d-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span></span>
5. <span data-ttu-id="ae59d-117">Choose the **Export** action.</span><span class="sxs-lookup"><span data-stu-id="ae59d-117">Choose the **Export** action.</span></span>
6. <span data-ttu-id="ae59d-118">On the **Export File** page, choose the **Save** button, and then save the file to a convenient location.</span><span class="sxs-lookup"><span data-stu-id="ae59d-118">On the **Export File** page, choose the **Save** button, and then save the file to a convenient location.</span></span>
7. <span data-ttu-id="ae59d-119">Upload the file to your electronic bank site.</span><span class="sxs-lookup"><span data-stu-id="ae59d-119">Upload the file to your electronic bank site.</span></span>
8. <span data-ttu-id="ae59d-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span><span class="sxs-lookup"><span data-stu-id="ae59d-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span></span>

<span data-ttu-id="ae59d-121">To view exported Positive Pay records</span><span class="sxs-lookup"><span data-stu-id="ae59d-121">To view exported Positive Pay records</span></span>

1. <span data-ttu-id="ae59d-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ae59d-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ae59d-123">Select the bank account that you want to view Positive Pay export records for.</span><span class="sxs-lookup"><span data-stu-id="ae59d-123">Select the bank account that you want to view Positive Pay export records for.</span></span>
3. <span data-ttu-id="ae59d-124">Choose the **Positive Pay Entries** action.</span><span class="sxs-lookup"><span data-stu-id="ae59d-124">Choose the **Positive Pay Entries** action.</span></span>

    <span data-ttu-id="ae59d-125">On the **Positive Pay Entries** page, you can see all the Positive Pay export records for the bank account.</span><span class="sxs-lookup"><span data-stu-id="ae59d-125">On the **Positive Pay Entries** page, you can see all the Positive Pay export records for the bank account.</span></span>
4. <span data-ttu-id="ae59d-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span><span class="sxs-lookup"><span data-stu-id="ae59d-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span></span>
5. <span data-ttu-id="ae59d-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span><span class="sxs-lookup"><span data-stu-id="ae59d-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span></span>

<span data-ttu-id="ae59d-128">To reexport Positive Pay files</span><span class="sxs-lookup"><span data-stu-id="ae59d-128">To reexport Positive Pay files</span></span>

1. <span data-ttu-id="ae59d-129">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ae59d-129">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="ae59d-130">Select the bank account that you want to reexport Positive Pay files for.</span><span class="sxs-lookup"><span data-stu-id="ae59d-130">Select the bank account that you want to reexport Positive Pay files for.</span></span>
3. <span data-ttu-id="ae59d-131">Choose the **Positive Pay Entries** action.</span><span class="sxs-lookup"><span data-stu-id="ae59d-131">Choose the **Positive Pay Entries** action.</span></span>
4. <span data-ttu-id="ae59d-132">Select the line for the Positive Pay export file that you want to reexport.</span><span class="sxs-lookup"><span data-stu-id="ae59d-132">Select the line for the Positive Pay export file that you want to reexport.</span></span>
5. <span data-ttu-id="ae59d-133">On the **Positive Pay Entries** page, choose the **Reexport Positive Pay to File** action.</span><span class="sxs-lookup"><span data-stu-id="ae59d-133">On the **Positive Pay Entries** page, choose the **Reexport Positive Pay to File** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="ae59d-134">See Also</span><span class="sxs-lookup"><span data-stu-id="ae59d-134">See Also</span></span>
[<span data-ttu-id="ae59d-135">Finance</span><span class="sxs-lookup"><span data-stu-id="ae59d-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="ae59d-136">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="ae59d-136">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="ae59d-137">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="ae59d-137">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="ae59d-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ae59d-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
