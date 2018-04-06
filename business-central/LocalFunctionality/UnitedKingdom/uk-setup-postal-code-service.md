---
title: Set Up the GetAddress.io UK Postcodes Extension | Microsoft Docs
description: Describes the general functionality you use to interact with data in Business Central, such as entering values, sorting data, and changing views.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: getaddress.io, postcodes, extension
ms.date: 03/05/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 9f01c2bd43462eee494a956bdbabb95caf9ac65c
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-the-getaddressio-uk-postcodes-extension"></a><span data-ttu-id="3e2cf-103">Set Up the GetAddress.io UK Postcodes Extension</span><span class="sxs-lookup"><span data-stu-id="3e2cf-103">Set Up the GetAddress.io UK Postcodes Extension</span></span>
<span data-ttu-id="3e2cf-104">This extension makes it easy to enter addresses in the United Kingdom (UK) for entities like customers, contacts, employees, vendors, bank accounts, and so on.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-104">This extension makes it easy to enter addresses in the United Kingdom (UK) for entities like customers, contacts, employees, vendors, bank accounts, and so on.</span></span>

<span data-ttu-id="3e2cf-105">The GetAddress.io UK Postcodes extension uses the getAddress API to find addresses in postcodes in the UK.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-105">The GetAddress.io UK Postcodes extension uses the getAddress API to find addresses in postcodes in the UK.</span></span> <span data-ttu-id="3e2cf-106">To use the extension, you need to get a plan and an API Key for the getAddress API.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-106">To use the extension, you need to get a plan and an API Key for the getAddress API.</span></span> <span data-ttu-id="3e2cf-107">We help you do that when you set up the GetAddress.io UK Postcodes extension.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-107">We help you do that when you set up the GetAddress.io UK Postcodes extension.</span></span> <span data-ttu-id="3e2cf-108">Plans are based on use, or what are sometimes referred to as "calls."</span><span class="sxs-lookup"><span data-stu-id="3e2cf-108">Plans are based on use, or what are sometimes referred to as "calls."</span></span> <span data-ttu-id="3e2cf-109">A call, in this case, is when [!INCLUDE[d365fin](../../includes/d365fin_md.md)] displays a list of addresses in a postcode.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-109">A call, in this case, is when [!INCLUDE[d365fin](../../includes/d365fin_md.md)] displays a list of addresses in a postcode.</span></span> <span data-ttu-id="3e2cf-110">Depending on how often you add addresses, choose the plan that is best for you.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-110">Depending on how often you add addresses, choose the plan that is best for you.</span></span> <span data-ttu-id="3e2cf-111">If you just choose **Get API Key** you will use the **Free** plan, which lets you add 20 addresses per day, and is valid for 30 days.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-111">If you just choose **Get API Key** you will use the **Free** plan, which lets you add 20 addresses per day, and is valid for 30 days.</span></span>

##<a name="to-set-up-the-getaddressio-uk-postcodes-extension"></a><span data-ttu-id="3e2cf-112">To set up the GetAddress.io UK Postcodes extension</span><span class="sxs-lookup"><span data-stu-id="3e2cf-112">To set up the GetAddress.io UK Postcodes extension</span></span>
1. <span data-ttu-id="3e2cf-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Connections**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Connections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3e2cf-114">In the **Service Connections** window, choose **UK Postcode Service**.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-114">In the **Service Connections** window, choose **UK Postcode Service**.</span></span>
3. <span data-ttu-id="3e2cf-115">In the **Postcode provider configuration** page, choose **Disabled**.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-115">In the **Postcode provider configuration** page, choose **Disabled**.</span></span>
4. <span data-ttu-id="3e2cf-116">In the **Postal code service selection** window, choose **GetAddress.io**.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-116">In the **Postal code service selection** window, choose **GetAddress.io**.</span></span>
5. <span data-ttu-id="3e2cf-117">In the **GetAddress.io Config** window, choose **Get API Key** to open the **Plans** page on the website for the getAddress API.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-117">In the **GetAddress.io Config** window, choose **Get API Key** to open the **Plans** page on the website for the getAddress API.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="3e2cf-118">You might need to allow pop-ups in your browser.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-118">You might need to allow pop-ups in your browser.</span></span>

6. <span data-ttu-id="3e2cf-119">Purchase a plan, or just choose **Get API Key**, and then provide your email address.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-119">Purchase a plan, or just choose **Get API Key**, and then provide your email address.</span></span>
7. <span data-ttu-id="3e2cf-120">Open the email from getAddress.io, and copy the API key.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-120">Open the email from getAddress.io, and copy the API key.</span></span> <span data-ttu-id="3e2cf-121">The key is under the **Your API Key** heading.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-121">The key is under the **Your API Key** heading.</span></span>
8. <span data-ttu-id="3e2cf-122">In the **GetAddress.io Config** window, paste the API key in the **API Key** field, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-122">In the **GetAddress.io Config** window, paste the API key in the **API Key** field, and then choose **OK**.</span></span>
9. <span data-ttu-id="3e2cf-123">In the **Service Connections** page, verify that the **Address Provider** field shows **GetAddress.io**.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-123">In the **Service Connections** page, verify that the **Address Provider** field shows **GetAddress.io**.</span></span> <span data-ttu-id="3e2cf-124">If it does, the service is enabled.</span><span class="sxs-lookup"><span data-stu-id="3e2cf-124">If it does, the service is enabled.</span></span>

## <a name="see-also"></a><span data-ttu-id="3e2cf-125">See Also</span><span class="sxs-lookup"><span data-stu-id="3e2cf-125">See Also</span></span>
[<span data-ttu-id="3e2cf-126">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="3e2cf-126">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  
[<span data-ttu-id="3e2cf-127">GetAddress.io UK Postcodes</span><span class="sxs-lookup"><span data-stu-id="3e2cf-127">GetAddress.io UK Postcodes</span></span>](../../ui-extensions-getaddressio.md)  
<span data-ttu-id="3e2cf-128">[Customising [!INCLUDE[d365fin](../../includes/d365fin_md.md)] Using Extensions](../../ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="3e2cf-128">[Customizing [!INCLUDE[d365fin](../../includes/d365fin_md.md)] Using Extensions](../../ui-extensions.md)</span></span>  
<span data-ttu-id="3e2cf-129">[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3e2cf-129">[Working with [!INCLUDE[d365fin](../../includes/d365fin_md.md)]](../../ui-work-product.md)</span></span>  

