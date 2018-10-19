---
title: How to Set Up Reverse Charges on VAT | Microsoft Docs
description: Learn how you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC).
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 96e49d8dcb90cf264bf238848af3340c76d9d20d
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-multiple-interest-rates"></a><span data-ttu-id="63eaa-103">Set Up Multiple Interest Rates</span><span class="sxs-lookup"><span data-stu-id="63eaa-103">Set Up Multiple Interest Rates</span></span>
<span data-ttu-id="63eaa-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud.</span><span class="sxs-lookup"><span data-stu-id="63eaa-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud.</span></span> <span data-ttu-id="63eaa-105">This feature is supplemented by the **Reverse Charge Sales List** report.</span><span class="sxs-lookup"><span data-stu-id="63eaa-105">This feature is supplemented by the **Reverse Charge Sales List** report.</span></span> <span data-ttu-id="63eaa-106">The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units.</span><span class="sxs-lookup"><span data-stu-id="63eaa-106">The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units.</span></span> <span data-ttu-id="63eaa-107">These goods will apply to reverse charges.</span><span class="sxs-lookup"><span data-stu-id="63eaa-107">These goods will apply to reverse charges.</span></span>

> [!IMPORTANT]  
>  <span data-ttu-id="63eaa-108">Legislative information may be subject to change by HM Revenue & Customs (HMRC).</span><span class="sxs-lookup"><span data-stu-id="63eaa-108">Legislative information may be subject to change by HM Revenue & Customs (HMRC).</span></span> <span data-ttu-id="63eaa-109">For more information, see the [HMRC website](https://www.hmrc.gov.uk/index.htm).</span><span class="sxs-lookup"><span data-stu-id="63eaa-109">For more information, see the [HMRC website](https://www.hmrc.gov.uk/index.htm).</span></span>  

## <a name="to-reverse-charges-on-vat"></a><span data-ttu-id="63eaa-110">To reverse charges on VAT</span><span class="sxs-lookup"><span data-stu-id="63eaa-110">To reverse charges on VAT</span></span>  

1.  <span data-ttu-id="63eaa-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Business Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63eaa-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Business Posting Groups**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="63eaa-112">Create a new VAT business posting group.</span><span class="sxs-lookup"><span data-stu-id="63eaa-112">Create a new VAT business posting group.</span></span> <span data-ttu-id="63eaa-113">Set up the needed VAT product posting groups.</span><span class="sxs-lookup"><span data-stu-id="63eaa-113">Set up the needed VAT product posting groups.</span></span>  
3.  <span data-ttu-id="63eaa-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63eaa-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="63eaa-115">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="63eaa-115">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
5.  <span data-ttu-id="63eaa-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63eaa-116">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="63eaa-117">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="63eaa-117">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span>
7.  <span data-ttu-id="63eaa-118">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup** and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63eaa-118">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup** and then choose the related link.</span></span>  
6.  <span data-ttu-id="63eaa-119">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="63eaa-119">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span>
9. <span data-ttu-id="63eaa-120">To set up items subject to reverse charge, select the item, and open the **Item Card** window.</span><span class="sxs-lookup"><span data-stu-id="63eaa-120">To set up items subject to reverse charge, select the item, and open the **Item Card** window.</span></span>  
10. <span data-ttu-id="63eaa-121">On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.</span><span class="sxs-lookup"><span data-stu-id="63eaa-121">On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.</span></span>  

## <a name="reverse-charge-sales-list"></a><span data-ttu-id="63eaa-122">Reverse Charge Sales List</span><span class="sxs-lookup"><span data-stu-id="63eaa-122">Reverse Charge Sales List</span></span>
<span data-ttu-id="63eaa-123">This report displays sales of goods which are subject to reverse charge.</span><span class="sxs-lookup"><span data-stu-id="63eaa-123">This report displays sales of goods which are subject to reverse charge.</span></span> <span data-ttu-id="63eaa-124">The report is based on information in the VAT Entry table.</span><span class="sxs-lookup"><span data-stu-id="63eaa-124">The report is based on information in the VAT Entry table.</span></span> <span data-ttu-id="63eaa-125">You use this to report to the customs and tax authorities the reverse charge sales.</span><span class="sxs-lookup"><span data-stu-id="63eaa-125">You use this to report to the customs and tax authorities the reverse charge sales.</span></span>  

<span data-ttu-id="63eaa-126">Examples of goods subject to reverse charge:</span><span class="sxs-lookup"><span data-stu-id="63eaa-126">Examples of goods subject to reverse charge:</span></span>  

-   <span data-ttu-id="63eaa-127">Mobile telephones.</span><span class="sxs-lookup"><span data-stu-id="63eaa-127">Mobile telephones.</span></span>  
-   <span data-ttu-id="63eaa-128">Computer chips</span><span class="sxs-lookup"><span data-stu-id="63eaa-128">Computer chips</span></span>  

<span data-ttu-id="63eaa-129">Consult the [HMRC website](http:\\www.hmrc.gov.uk) for the list of goods subject to reverse charge.</span><span class="sxs-lookup"><span data-stu-id="63eaa-129">Consult the [HMRC website](http:\\www.hmrc.gov.uk) for the list of goods subject to reverse charge.</span></span>  

## <a name="see-also"></a><span data-ttu-id="63eaa-130">See Also</span><span class="sxs-lookup"><span data-stu-id="63eaa-130">See Also</span></span>  
[<span data-ttu-id="63eaa-131">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="63eaa-131">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  

