---
title: How to Set Up Reverse Charges on VAT | Microsoft Docs
description: Learn how you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC).
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: a41b91769f824f52b42619720ae65add79a23417
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676620"
---
# <a name="set-up-reverse-charge-vat"></a><span data-ttu-id="7c8e2-103">Set Up Reverse Charge VAT</span><span class="sxs-lookup"><span data-stu-id="7c8e2-103">Set Up Reverse Charge VAT</span></span>
<span data-ttu-id="7c8e2-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud.</span></span> <span data-ttu-id="7c8e2-105">This feature is supplemented by the **Reverse Charge Sales List** report.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-105">This feature is supplemented by the **Reverse Charge Sales List** report.</span></span> <span data-ttu-id="7c8e2-106">The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-106">The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units.</span></span> <span data-ttu-id="7c8e2-107">These goods will apply to reverse charges.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-107">These goods will apply to reverse charges.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="7c8e2-108">Legislative information may be subject to change by HM Revenue & Customs (HMRC).</span><span class="sxs-lookup"><span data-stu-id="7c8e2-108">Legislative information may be subject to change by HM Revenue & Customs (HMRC).</span></span> <span data-ttu-id="7c8e2-109">For more information, see the [HMRC website](https://www.gov.uk/government/organisations/hm-revenue-customs).</span><span class="sxs-lookup"><span data-stu-id="7c8e2-109">For more information, see the [HMRC website](https://www.gov.uk/government/organisations/hm-revenue-customs).</span></span>  

## <a name="to-reverse-charges-on-vat"></a><span data-ttu-id="7c8e2-110">To reverse charges on VAT</span><span class="sxs-lookup"><span data-stu-id="7c8e2-110">To reverse charges on VAT</span></span>  

1.  <span data-ttu-id="7c8e2-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Business Posting Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Business Posting Groups**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7c8e2-112">Create a new VAT business posting group.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-112">Create a new VAT business posting group.</span></span> <span data-ttu-id="7c8e2-113">Set up the needed VAT product posting groups.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-113">Set up the needed VAT product posting groups.</span></span>  
3.  <span data-ttu-id="7c8e2-114">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-114">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="7c8e2-115">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-115">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
5.  <span data-ttu-id="7c8e2-116">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-116">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="7c8e2-117">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-117">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span>
7.  <span data-ttu-id="7c8e2-118">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup** and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-118">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup** and then choose the related link.</span></span>  
6.  <span data-ttu-id="7c8e2-119">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-119">On the **Reverse Charge** FastTab, fill in the fields as necessary.</span></span>
9. <span data-ttu-id="7c8e2-120">To set up items subject to reverse charge, select the item, and open the **Item Card** page.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-120">To set up items subject to reverse charge, select the item, and open the **Item Card** page.</span></span>  
10. <span data-ttu-id="7c8e2-121">On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-121">On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.</span></span>  

## <a name="reverse-charge-sales-list"></a><span data-ttu-id="7c8e2-122">Reverse Charge Sales List</span><span class="sxs-lookup"><span data-stu-id="7c8e2-122">Reverse Charge Sales List</span></span>
<span data-ttu-id="7c8e2-123">This report displays sales of goods which are subject to reverse charge.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-123">This report displays sales of goods which are subject to reverse charge.</span></span> <span data-ttu-id="7c8e2-124">The report is based on information in the VAT Entry table.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-124">The report is based on information in the VAT Entry table.</span></span> <span data-ttu-id="7c8e2-125">You use this to report to the customs and tax authorities the reverse charge sales.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-125">You use this to report to the customs and tax authorities the reverse charge sales.</span></span>  

<span data-ttu-id="7c8e2-126">Examples of goods subject to reverse charge:</span><span class="sxs-lookup"><span data-stu-id="7c8e2-126">Examples of goods subject to reverse charge:</span></span>  

- <span data-ttu-id="7c8e2-127">Mobile telephones.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-127">Mobile telephones.</span></span>  
- <span data-ttu-id="7c8e2-128">Computer chips</span><span class="sxs-lookup"><span data-stu-id="7c8e2-128">Computer chips</span></span>  

<span data-ttu-id="7c8e2-129">Consult the [HMRC website](https://www.gov.uk/government/organisations/hm-revenue-customs) for the list of goods subject to reverse charge.</span><span class="sxs-lookup"><span data-stu-id="7c8e2-129">Consult the [HMRC website](https://www.gov.uk/government/organisations/hm-revenue-customs) for the list of goods subject to reverse charge.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7c8e2-130">See Also</span><span class="sxs-lookup"><span data-stu-id="7c8e2-130">See Also</span></span>  
[<span data-ttu-id="7c8e2-131">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="7c8e2-131">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  
