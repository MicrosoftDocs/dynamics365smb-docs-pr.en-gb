---
title: How to Set Up Multiple Interest Rates | Microsoft Docs
description: You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fceff1a6cf728608a49182a9704f187d31767fe
ms.openlocfilehash: 0a66bae782a667de78310519ff661c9413acfd38
ms.contentlocale: en-gb
ms.lasthandoff: 05/28/2018

---
# <a name="set-up-multiple-interest-rates"></a><span data-ttu-id="0c81c-104">Set Up Multiple Interest Rates</span><span class="sxs-lookup"><span data-stu-id="0c81c-104">Set Up Multiple Interest Rates</span></span>
<span data-ttu-id="0c81c-105">You can calculate finance charges with multiple interest rates for a specific period.</span><span class="sxs-lookup"><span data-stu-id="0c81c-105">You can calculate finance charges with multiple interest rates for a specific period.</span></span> <span data-ttu-id="0c81c-106">The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.</span><span class="sxs-lookup"><span data-stu-id="0c81c-106">The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.</span></span>  

<span data-ttu-id="0c81c-107">For example, you can charge customers accordingly if they pay late.</span><span class="sxs-lookup"><span data-stu-id="0c81c-107">For example, you can charge customers accordingly if they pay late.</span></span>  

## <a name="to-set-up-multiple-interest-rates"></a><span data-ttu-id="0c81c-108">To set up multiple interest rates</span><span class="sxs-lookup"><span data-stu-id="0c81c-108">To set up multiple interest rates</span></span>  
1. <span data-ttu-id="0c81c-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c81c-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0c81c-110">In the **Finance Charge Terms** window, select the required finance term, and then, on the **Navigate** tab, choose **Interest Rates**.</span><span class="sxs-lookup"><span data-stu-id="0c81c-110">In the **Finance Charge Terms** window, select the required finance term, and then, on the **Navigate** tab, choose **Interest Rates**.</span></span>  
3. <span data-ttu-id="0c81c-111">Fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="0c81c-111">Fill in the fields as described in the following table.</span></span>  


   |           <span data-ttu-id="0c81c-112">Field</span><span class="sxs-lookup"><span data-stu-id="0c81c-112">Field</span></span>            |                           <span data-ttu-id="0c81c-113">Description</span><span class="sxs-lookup"><span data-stu-id="0c81c-113">Description</span></span>                            |
   |----------------------------|------------------------------------------------------------------|
   |       <span data-ttu-id="0c81c-114">**Start Date**</span><span class="sxs-lookup"><span data-stu-id="0c81c-114">**Start Date**</span></span>       | <span data-ttu-id="0c81c-115">Enter the start date for each finance charge interest rate code.</span><span class="sxs-lookup"><span data-stu-id="0c81c-115">Enter the start date for each finance charge interest rate code.</span></span> |
   |     <span data-ttu-id="0c81c-116">**Interest Rate**</span><span class="sxs-lookup"><span data-stu-id="0c81c-116">**Interest Rate**</span></span>      |  <span data-ttu-id="0c81c-117">Enter the percentage that must be used to calculate interest.</span><span class="sxs-lookup"><span data-stu-id="0c81c-117">Enter the percentage that must be used to calculate interest.</span></span>   |
   | <span data-ttu-id="0c81c-118">**Interest Period (Days)**</span><span class="sxs-lookup"><span data-stu-id="0c81c-118">**Interest Period (Days)**</span></span> |     <span data-ttu-id="0c81c-119">Enter the period for each finance charge interest rate.</span><span class="sxs-lookup"><span data-stu-id="0c81c-119">Enter the period for each finance charge interest rate.</span></span>      |


4. <span data-ttu-id="0c81c-120">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0c81c-120">Choose the **OK** button.</span></span>  
5. <span data-ttu-id="0c81c-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c81c-121">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.</span></span>  
6. <span data-ttu-id="0c81c-122">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span><span class="sxs-lookup"><span data-stu-id="0c81c-122">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span></span>  
7. <span data-ttu-id="0c81c-123">In the **Reminder Levels** window, select the **Calculate Interest** field.</span><span class="sxs-lookup"><span data-stu-id="0c81c-123">In the **Reminder Levels** window, select the **Calculate Interest** field.</span></span>  

   <span data-ttu-id="0c81c-124">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span><span class="sxs-lookup"><span data-stu-id="0c81c-124">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span></span> <span data-ttu-id="0c81c-125">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span><span class="sxs-lookup"><span data-stu-id="0c81c-125">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span></span> <span data-ttu-id="0c81c-126">The opening entry on the memo is displayed in bold.</span><span class="sxs-lookup"><span data-stu-id="0c81c-126">The opening entry on the memo is displayed in bold.</span></span> <span data-ttu-id="0c81c-127">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span><span class="sxs-lookup"><span data-stu-id="0c81c-127">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0c81c-128">See Also</span><span class="sxs-lookup"><span data-stu-id="0c81c-128">See Also</span></span>  
[<span data-ttu-id="0c81c-129">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="0c81c-129">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  
[<span data-ttu-id="0c81c-130">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="0c81c-130">Collect Outstanding Balances</span></span>](../../receivables-collect-outstanding-balances.md)   

