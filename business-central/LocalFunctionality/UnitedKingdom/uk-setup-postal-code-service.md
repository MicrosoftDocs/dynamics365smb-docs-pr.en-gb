---
title: Set Up the GetAddress.io UK Postcodes Extension
description: Learn how to configure the GetAddress.io extension in the British version of Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: getaddress.io, postcodes, extension
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: eee9e091c96a47f3b93559221f5409527c6450b5
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753127"
---
# <a name="set-up-the-getaddressio-uk-postcodes-extension"></a><span data-ttu-id="5f8b5-103">Set Up the GetAddress.io UK Postcodes Extension</span><span class="sxs-lookup"><span data-stu-id="5f8b5-103">Set Up the GetAddress.io UK Postcodes Extension</span></span>

<span data-ttu-id="5f8b5-104">This extension makes it easy to enter addresses in the United Kingdom (UK) for entities like customers, contacts, employees, vendors, bank accounts, and so on.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-104">This extension makes it easy to enter addresses in the United Kingdom (UK) for entities like customers, contacts, employees, vendors, bank accounts, and so on.</span></span>

<span data-ttu-id="5f8b5-105">The GetAddress.io UK Postcodes extension uses the getAddress API to find addresses in postcodes in the UK.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-105">The GetAddress.io UK Postcodes extension uses the getAddress API to find addresses in postcodes in the UK.</span></span> <span data-ttu-id="5f8b5-106">To use the extension, you need to get a plan and an API Key for the getAddress API.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-106">To use the extension, you need to get a plan and an API Key for the getAddress API.</span></span> <span data-ttu-id="5f8b5-107">We help you do that when you set up the GetAddress.io UK Postcodes extension.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-107">We help you do that when you set up the GetAddress.io UK Postcodes extension.</span></span> <span data-ttu-id="5f8b5-108">Plans are based on use, or what are sometimes referred to as "calls."</span><span class="sxs-lookup"><span data-stu-id="5f8b5-108">Plans are based on use, or what are sometimes referred to as "calls."</span></span> <span data-ttu-id="5f8b5-109">A call, in this case, is when [!INCLUDE[prod_short](../../includes/prod_short.md)] displays a list of addresses in a postcode.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-109">A call, in this case, is when [!INCLUDE[prod_short](../../includes/prod_short.md)] displays a list of addresses in a postcode.</span></span> <span data-ttu-id="5f8b5-110">Depending on how often you add addresses, choose the plan that is best for you.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-110">Depending on how often you add addresses, choose the plan that is best for you.</span></span> <span data-ttu-id="5f8b5-111">If you just choose **Get API Key** you will use the **Free** plan, which lets you add 20 addresses per day, and is valid for 30 days.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-111">If you just choose **Get API Key** you will use the **Free** plan, which lets you add 20 addresses per day, and is valid for 30 days.</span></span>

##<a name="to-set-up-the-getaddressio-uk-postcodes-extension"></a><span data-ttu-id="5f8b5-112">To set up the GetAddress.io UK Postcodes extension</span><span class="sxs-lookup"><span data-stu-id="5f8b5-112">To set up the GetAddress.io UK Postcodes extension</span></span>
1. <span data-ttu-id="5f8b5-113">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-113">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="5f8b5-114">On the **Service Connections** page, choose **UK Postcode Service**.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-114">On the **Service Connections** page, choose **UK Postcode Service**.</span></span>
3. <span data-ttu-id="5f8b5-115">On the **Postcode provider configuration** page, choose **Disabled**.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-115">On the **Postcode provider configuration** page, choose **Disabled**.</span></span>
4. <span data-ttu-id="5f8b5-116">On the **Postcode service selection** page, choose **GetAddress.io**.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-116">On the **Postal code service selection** page, choose **GetAddress.io**.</span></span>
5. <span data-ttu-id="5f8b5-117">On the **GetAddress.io Config** page, choose **Get API Key** to open the **Plans** page on the website for the getAddress API.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-117">On the **GetAddress.io Config** page, choose **Get API Key** to open the **Plans** page on the website for the getAddress API.</span></span>  

    > [!NOTE]  
    >   <span data-ttu-id="5f8b5-118">You might need to allow pop-ups in your browser.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-118">You might need to allow pop-ups in your browser.</span></span>

6. <span data-ttu-id="5f8b5-119">Purchase a plan, or just choose **Get API Key**, and then provide your email address.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-119">Purchase a plan, or just choose **Get API Key**, and then provide your email address.</span></span>
7. <span data-ttu-id="5f8b5-120">Open the email from getAddress.io, and copy the API key.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-120">Open the email from getAddress.io, and copy the API key.</span></span> <span data-ttu-id="5f8b5-121">The key is under the **Your API Key** heading.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-121">The key is under the **Your API Key** heading.</span></span>
8. <span data-ttu-id="5f8b5-122">On the **GetAddress.io Config** page, paste the API key in the **API Key** field, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-122">On the **GetAddress.io Config** page, paste the API key in the **API Key** field, and then choose **OK**.</span></span>
9. <span data-ttu-id="5f8b5-123">On the **Service Connections** page, verify that the **Address Provider** field shows **GetAddress.io**.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-123">On the **Service Connections** page, verify that the **Address Provider** field shows **GetAddress.io**.</span></span> <span data-ttu-id="5f8b5-124">If it does, the service is enabled.</span><span class="sxs-lookup"><span data-stu-id="5f8b5-124">If it does, the service is enabled.</span></span>

## <a name="see-also"></a><span data-ttu-id="5f8b5-125">See Also</span><span class="sxs-lookup"><span data-stu-id="5f8b5-125">See Also</span></span>

[<span data-ttu-id="5f8b5-126">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="5f8b5-126">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)  
[<span data-ttu-id="5f8b5-127">The GetAddress.io UK Postcodes Extension</span><span class="sxs-lookup"><span data-stu-id="5f8b5-127">The GetAddress.io UK Postcodes Extension</span></span>](ui-extensions-getaddressio.md)  
<span data-ttu-id="5f8b5-128">[Customising [!INCLUDE[prod_short](../../includes/prod_short.md)] Using Extensions](../../ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="5f8b5-128">[Customizing [!INCLUDE[prod_short](../../includes/prod_short.md)] Using Extensions](../../ui-extensions.md)</span></span>  
<span data-ttu-id="5f8b5-129">[Working with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5f8b5-129">[Working with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)</span></span>  
