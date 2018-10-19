---
title: How to Set Up Multiple Interest Rates
description: You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.
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
ms.openlocfilehash: 3d4c111af62db5858b81b76f9f51a9093c01e5e6
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-multiple-interest-rates"></a><span data-ttu-id="3e567-104">Set Up Multiple Interest Rates</span><span class="sxs-lookup"><span data-stu-id="3e567-104">Set Up Multiple Interest Rates</span></span>
<span data-ttu-id="3e567-105">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span><span class="sxs-lookup"><span data-stu-id="3e567-105">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span></span> <span data-ttu-id="3e567-106">For example, a government specifies the maximum interest to be levied for a consumer.</span><span class="sxs-lookup"><span data-stu-id="3e567-106">For example, a government specifies the maximum interest to be levied for a consumer.</span></span> <span data-ttu-id="3e567-107">This interest rate can be changed twice a year on 01 January and 01 July.</span><span class="sxs-lookup"><span data-stu-id="3e567-107">This interest rate can be changed twice a year on 01 January and 01 July.</span></span> <span data-ttu-id="3e567-108">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span><span class="sxs-lookup"><span data-stu-id="3e567-108">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span></span> <span data-ttu-id="3e567-109">The announced rate is usually four percent more than the normal bank interest.</span><span class="sxs-lookup"><span data-stu-id="3e567-109">The announced rate is usually four percent more than the normal bank interest.</span></span>

<span data-ttu-id="3e567-110">When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods.</span><span class="sxs-lookup"><span data-stu-id="3e567-110">When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods.</span></span> <span data-ttu-id="3e567-111">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="3e567-111">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>

## <a name="to-set-up-multiple-interest-rates"></a><span data-ttu-id="3e567-112">To set up multiple interest rates</span><span class="sxs-lookup"><span data-stu-id="3e567-112">To set up multiple interest rates</span></span>  
1.  <span data-ttu-id="3e567-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3e567-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="3e567-114">In the **Finance Charge Terms** window, select the required finance term, and then choose the **Interest Rates** action.</span><span class="sxs-lookup"><span data-stu-id="3e567-114">In the **Finance Charge Terms** window, select the required finance term, and then choose the **Interest Rates** action.</span></span>  
3.  <span data-ttu-id="3e567-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="3e567-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="3e567-116">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="3e567-116">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="3e567-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3e567-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Reminder Terms**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="3e567-118">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span><span class="sxs-lookup"><span data-stu-id="3e567-118">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span></span>  
7.  <span data-ttu-id="3e567-119">In the **Reminder Levels** window, select the **Calculate Interest** field.</span><span class="sxs-lookup"><span data-stu-id="3e567-119">In the **Reminder Levels** window, select the **Calculate Interest** field.</span></span>  

<span data-ttu-id="3e567-120">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span><span class="sxs-lookup"><span data-stu-id="3e567-120">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span></span> <span data-ttu-id="3e567-121">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span><span class="sxs-lookup"><span data-stu-id="3e567-121">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span></span> <span data-ttu-id="3e567-122">The opening entry on the memo is displayed in bold.</span><span class="sxs-lookup"><span data-stu-id="3e567-122">The opening entry on the memo is displayed in bold.</span></span> <span data-ttu-id="3e567-123">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span><span class="sxs-lookup"><span data-stu-id="3e567-123">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3e567-124">See Also</span><span class="sxs-lookup"><span data-stu-id="3e567-124">See Also</span></span>  
[<span data-ttu-id="3e567-125">Collect Outstanding Balances</span><span class="sxs-lookup"><span data-stu-id="3e567-125">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="3e567-126">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="3e567-126">Setting Up Finance</span></span>](finance-setup-finance.md)

