---
title: Updating Currency Exchange Rates| Microsoft Docs
description: To use multiple currencies in your business, you can set up a code for each currency and use an external exchange rate service.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies
ms.date: 12/19/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa1e7b13cf6cc56df1a6922a9b123e7cc19580c6
ms.openlocfilehash: 7fafae0cba12ba985de2faa795b434d4c670a8ca
ms.contentlocale: en-gb
ms.lasthandoff: 12/19/2018

---
# <a name="update-currency-exchange-rates"></a><span data-ttu-id="8bc68-103">Update Currency Exchange Rates</span><span class="sxs-lookup"><span data-stu-id="8bc68-103">Update Currency Exchange Rates</span></span>
<span data-ttu-id="8bc68-104">As companies operate in increasingly more countries/regions, it becomes more important that they be able to trade and report financials in more than one currency.</span><span class="sxs-lookup"><span data-stu-id="8bc68-104">As companies operate in increasingly more countries/regions, it becomes more important that they be able to trade and report financials in more than one currency.</span></span> <span data-ttu-id="8bc68-105">You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.</span><span class="sxs-lookup"><span data-stu-id="8bc68-105">You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.</span></span>

<span data-ttu-id="8bc68-106">Your general ledger is set up to use your local currency (LCY), but you can set it up to also use another currency with a current exchange rate assigned.</span><span class="sxs-lookup"><span data-stu-id="8bc68-106">Your general ledger is set up to use your local currency (LCY), but you can set it up to also use another currency with a current exchange rate assigned.</span></span> <span data-ttu-id="8bc68-107">By designating a second currency as a so-called additional reporting currency, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically record amounts in both LCY and this additional reporting currency on each G/L entry and other entries, such as VAT entries.</span><span class="sxs-lookup"><span data-stu-id="8bc68-107">By designating a second currency as a so-called additional reporting currency, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically record amounts in both LCY and this additional reporting currency on each G/L entry and other entries, such as VAT entries.</span></span> <span data-ttu-id="8bc68-108">For more information, see [Set Up an Additional Reporting Currency](finance-how-setup-additional-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="8bc68-108">For more information, see [Set Up an Additional Reporting Currency](finance-how-setup-additional-currencies.md).</span></span>

## <a name="adjusting-exchange-rates"></a><span data-ttu-id="8bc68-109">Adjusting Exchange Rates</span><span class="sxs-lookup"><span data-stu-id="8bc68-109">Adjusting Exchange Rates</span></span>
<span data-ttu-id="8bc68-110">Because exchange rates fluctuate constantly, additional currency equivalents in your system must be adjusted periodically.</span><span class="sxs-lookup"><span data-stu-id="8bc68-110">Because exchange rates fluctuate constantly, additional currency equivalents in your system must be adjusted periodically.</span></span> <span data-ttu-id="8bc68-111">If these adjustments are not done, amounts that have been converted from foreign (or additional) currencies and posted to the general ledger in LCY may be misleading.</span><span class="sxs-lookup"><span data-stu-id="8bc68-111">If these adjustments are not done, amounts that have been converted from foreign (or additional) currencies and posted to the general ledger in LCY may be misleading.</span></span> <span data-ttu-id="8bc68-112">In addition, daily entries posted before a daily exchange rate is entered into the program must be updated after the daily exchange rate information is entered.</span><span class="sxs-lookup"><span data-stu-id="8bc68-112">In addition, daily entries posted before a daily exchange rate is entered into the program must be updated after the daily exchange rate information is entered.</span></span> <span data-ttu-id="8bc68-113">The Adjust Exchange Rates batch job is used to adjust the exchange rates of posted customer, vendor and bank account entries.</span><span class="sxs-lookup"><span data-stu-id="8bc68-113">The Adjust Exchange Rates batch job is used to adjust the exchange rates of posted customer, vendor and bank account entries.</span></span> <span data-ttu-id="8bc68-114">It can also update additional reporting currency amounts on G/L entries.</span><span class="sxs-lookup"><span data-stu-id="8bc68-114">It can also update additional reporting currency amounts on G/L entries.</span></span>

## <a name="to-set-up-a-currency-exchange-rate-service"></a><span data-ttu-id="8bc68-115">To set up a currency exchange rate service</span><span class="sxs-lookup"><span data-stu-id="8bc68-115">To set up a currency exchange rate service</span></span>
<span data-ttu-id="8bc68-116">You can use an external service to keep your currency exchange rates up to date, such as FloatRates.</span><span class="sxs-lookup"><span data-stu-id="8bc68-116">You can use an external service to keep your currency exchange rates up to date, such as FloatRates.</span></span>

1. <span data-ttu-id="8bc68-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currency Exchange Rate Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8bc68-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currency Exchange Rate Services**, and then choose the related link.</span></span>
2. <span data-ttu-id="8bc68-118">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="8bc68-118">Choose the **New** action.</span></span>
3. <span data-ttu-id="8bc68-119">On the **Currency Exchange Rate Service** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="8bc68-119">On the **Currency Exchange Rate Service** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="8bc68-120">Choose the **Enabled** check box to enable the service.</span><span class="sxs-lookup"><span data-stu-id="8bc68-120">Choose the **Enabled** check box to enable the service.</span></span>

## <a name="to-update-currency-exchange-rates-through-a-service"></a><span data-ttu-id="8bc68-121">To update currency exchange rates through a service</span><span class="sxs-lookup"><span data-stu-id="8bc68-121">To update currency exchange rates through a service</span></span>
1. <span data-ttu-id="8bc68-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8bc68-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Currencies**, and then choose the related link.</span></span>
2. <span data-ttu-id="8bc68-123">Choose the **Update Exchange Rates** action.</span><span class="sxs-lookup"><span data-stu-id="8bc68-123">Choose the **Update Exchange Rates** action.</span></span>

<span data-ttu-id="8bc68-124">The value in the **Exchange Rate** field on the **Currencies** page is updated with the latest currency exchange rate.</span><span class="sxs-lookup"><span data-stu-id="8bc68-124">The value in the **Exchange Rate** field on the **Currencies** page is updated with the latest currency exchange rate.</span></span>

## <a name="see-also"></a><span data-ttu-id="8bc68-125">See Also</span><span class="sxs-lookup"><span data-stu-id="8bc68-125">See Also</span></span>
[<span data-ttu-id="8bc68-126">Set Up an Additional Reporting Currency</span><span class="sxs-lookup"><span data-stu-id="8bc68-126">Set Up an Additional Reporting Currency</span></span>](finance-how-setup-additional-currencies.md)  
[<span data-ttu-id="8bc68-127">Closing Years and Periods</span><span class="sxs-lookup"><span data-stu-id="8bc68-127">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="8bc68-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8bc68-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

