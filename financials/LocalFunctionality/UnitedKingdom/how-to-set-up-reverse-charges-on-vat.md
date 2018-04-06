---
title: How to Set Up Reverse Charges on VAT | Microsoft Docs
description: Learn how you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC).
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/17/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f200e7f937f739c5881bc8b2e5b60f3ab1750727
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-multiple-interest-rates"></a><span data-ttu-id="ed90d-103">Set Up Multiple Interest Rates</span><span class="sxs-lookup"><span data-stu-id="ed90d-103">Set Up Multiple Interest Rates</span></span>
<span data-ttu-id="ed90d-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud.</span><span class="sxs-lookup"><span data-stu-id="ed90d-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud.</span></span> <span data-ttu-id="ed90d-105">This feature is supplemented by the **Reverse Charge Sales List** report.</span><span class="sxs-lookup"><span data-stu-id="ed90d-105">This feature is supplemented by the **Reverse Charge Sales List** report.</span></span> <span data-ttu-id="ed90d-106">The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units.</span><span class="sxs-lookup"><span data-stu-id="ed90d-106">The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units.</span></span> <span data-ttu-id="ed90d-107">These goods will apply to reverse charges.</span><span class="sxs-lookup"><span data-stu-id="ed90d-107">These goods will apply to reverse charges.</span></span>

> [!IMPORTANT]  
>  <span data-ttu-id="ed90d-108">Legislative information may be subject to change by HM Revenue & Customs (HMRC).</span><span class="sxs-lookup"><span data-stu-id="ed90d-108">Legislative information may be subject to change by HM Revenue & Customs (HMRC).</span></span> <span data-ttu-id="ed90d-109">For more information, see the [HMRC website](http://www.hmrc.gov.uk/index.htm).</span><span class="sxs-lookup"><span data-stu-id="ed90d-109">For more information, see the [HMRC website](http://www.hmrc.gov.uk/index.htm).</span></span>  

## <a name="to-reverse-charges-on-vat"></a><span data-ttu-id="ed90d-110">To reverse charges on VAT</span><span class="sxs-lookup"><span data-stu-id="ed90d-110">To reverse charges on VAT</span></span>  

1.  <span data-ttu-id="ed90d-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Business Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed90d-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Business Posting Groups**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ed90d-112">Create a new VAT business posting group.</span><span class="sxs-lookup"><span data-stu-id="ed90d-112">Create a new VAT business posting group.</span></span> <span data-ttu-id="ed90d-113">Set up the needed VAT product posting groups.</span><span class="sxs-lookup"><span data-stu-id="ed90d-113">Set up the needed VAT product posting groups.</span></span>  
3.  <span data-ttu-id="ed90d-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed90d-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="ed90d-115">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ed90d-115">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
5.  <span data-ttu-id="ed90d-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed90d-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="ed90d-117">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ed90d-117">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span>
7.  <span data-ttu-id="ed90d-118">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup** and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ed90d-118">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup** and then choose the related link.</span></span>  
6.  <span data-ttu-id="ed90d-119">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="ed90d-119">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span>
9. <span data-ttu-id="ed90d-120">To set up items subject to reverse charge, select the item, and open the **Item Card** window.</span><span class="sxs-lookup"><span data-stu-id="ed90d-120">To set up items subject to reverse charge, select the item, and open the **Item Card** window.</span></span>  
10. <span data-ttu-id="ed90d-121">On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.</span><span class="sxs-lookup"><span data-stu-id="ed90d-121">On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.</span></span>  

## <a name="reverse-charge-sales-list"></a><span data-ttu-id="ed90d-122">Reverse Charge Sales List</span><span class="sxs-lookup"><span data-stu-id="ed90d-122">Reverse Charge Sales List</span></span>
<span data-ttu-id="ed90d-123">This report displays sales of goods which are subject to reverse charge.</span><span class="sxs-lookup"><span data-stu-id="ed90d-123">This report displays sales of goods which are subject to reverse charge.</span></span> <span data-ttu-id="ed90d-124">The report is based on information in the VAT Entry table.</span><span class="sxs-lookup"><span data-stu-id="ed90d-124">The report is based on information in the VAT Entry table.</span></span> <span data-ttu-id="ed90d-125">You use this to report to the customs and tax authorities the reverse charge sales.</span><span class="sxs-lookup"><span data-stu-id="ed90d-125">You use this to report to the customs and tax authorities the reverse charge sales.</span></span>  

<span data-ttu-id="ed90d-126">Examples of goods subject to reverse charge:</span><span class="sxs-lookup"><span data-stu-id="ed90d-126">Examples of goods subject to reverse charge:</span></span>  

-   <span data-ttu-id="ed90d-127">Mobile telephones.</span><span class="sxs-lookup"><span data-stu-id="ed90d-127">Mobile telephones.</span></span>  
-   <span data-ttu-id="ed90d-128">Computer chips</span><span class="sxs-lookup"><span data-stu-id="ed90d-128">Computer chips</span></span>  

<span data-ttu-id="ed90d-129">Consult the [HMRC website](http:\\www.hmrc.gov.uk) for the list of goods subject to reverse charge.</span><span class="sxs-lookup"><span data-stu-id="ed90d-129">Consult the [HMRC website](http:\\www.hmrc.gov.uk) for the list of goods subject to reverse charge.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ed90d-130">See Also</span><span class="sxs-lookup"><span data-stu-id="ed90d-130">See Also</span></span>  
[<span data-ttu-id="ed90d-131">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="ed90d-131">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  

