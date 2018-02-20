---
title: Use Invoicing and Finance and Operations, Business edition | Microsoft Docs
description: Workaround for accessing Microsoft Invoicing when you have signed up for Dynamics 365 for Finance and Operations, Business edition.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/22/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: abceec5b1bc588e2842d0f512240c30eccbf6f8e
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="using-the-same-office-365-account-in-included365finincludesd365finlongmdmd-and-microsoft-invoicing"></a><span data-ttu-id="52b48-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span><span class="sxs-lookup"><span data-stu-id="52b48-103">Using the same Office 365 Account in [!INCLUDE[d365fin](includes/d365fin_long_md.md)] and Microsoft Invoicing</span></span>
<span data-ttu-id="52b48-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="52b48-104">When you sign up for a trial with [!INCLUDE[d365fin](includes/d365fin_md.md)], you can move to a 30-day evaluation phase, you can start a subscription, or you can stop using [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="52b48-105">In all cases, if you log into the Office Portal, you might see a tile called **Business centre** and click it.</span><span class="sxs-lookup"><span data-stu-id="52b48-105">In all cases, if you log into the Office Portal, you might see a tile called **Business center** and click it.</span></span> <span data-ttu-id="52b48-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span><span class="sxs-lookup"><span data-stu-id="52b48-106">This is part of the Office 365 Business Premium subscription, so not everyone will see that tile in the Office Portal.</span></span>  

<span data-ttu-id="52b48-107">If you do access the Business centre, you will see a section called **Invoicing**.</span><span class="sxs-lookup"><span data-stu-id="52b48-107">If you do access the Business center, you will see a section called **Invoicing**.</span></span> <span data-ttu-id="52b48-108">If you access that section, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="52b48-108">If you access that section, you will see a message that you cannot access Microsoft Invoicing because your account is used in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="52b48-109">You see a similar message if you install the mobile app for Invoicing.</span><span class="sxs-lookup"><span data-stu-id="52b48-109">You see a similar message if you install the mobile app for Invoicing.</span></span>  

## <a name="workaround"></a><span data-ttu-id="52b48-110">Workaround</span><span class="sxs-lookup"><span data-stu-id="52b48-110">Workaround</span></span>
<span data-ttu-id="52b48-111">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span><span class="sxs-lookup"><span data-stu-id="52b48-111">Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)] have a shared platform.</span></span> <span data-ttu-id="52b48-112">That means that you are recognised as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Business centre.</span><span class="sxs-lookup"><span data-stu-id="52b48-112">That means that you are recognized as an existing user of [!INCLUDE[d365fin](includes/d365fin_md.md)] when you click Invoicing in the Business center.</span></span> <span data-ttu-id="52b48-113">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="52b48-113">The reason is that Invoicing cannot use the same company as [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="52b48-114">So you will have to log into [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span><span class="sxs-lookup"><span data-stu-id="52b48-114">So you will have to log into [!INCLUDE[d365fin](includes/d365fin_md.md)] and rename your existing company, and then create a new company that you can then use in Invoicing.</span></span> <span data-ttu-id="52b48-115">No data is moved or overwritten during this workaround.</span><span class="sxs-lookup"><span data-stu-id="52b48-115">No data is moved or overwritten during this workaround.</span></span>

### <a name="to-rename-your-company"></a><span data-ttu-id="52b48-116">To rename your company</span><span class="sxs-lookup"><span data-stu-id="52b48-116">To rename your company</span></span>
1.  <span data-ttu-id="52b48-117">Sign in to your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="52b48-117">Sign in to your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
2.  <span data-ttu-id="52b48-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Companies**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="52b48-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Companies**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="52b48-119">In the **Companies** window, choose the **Edit List** button.</span><span class="sxs-lookup"><span data-stu-id="52b48-119">In the **Companies** window, choose the **Edit List** button.</span></span>  
4.  <span data-ttu-id="52b48-120">Change the name of the *My Company* entry to something else.</span><span class="sxs-lookup"><span data-stu-id="52b48-120">Change the name of the *My Company* entry to something else.</span></span>  

    <span data-ttu-id="52b48-121">Wait a number of minutes.</span><span class="sxs-lookup"><span data-stu-id="52b48-121">Wait a number of minutes.</span></span> <span data-ttu-id="52b48-122">We’ll be making a number of changes in the underlying database, and that takes a while.</span><span class="sxs-lookup"><span data-stu-id="52b48-122">We’ll be making a number of changes in the underlying database, and that takes a while.</span></span>
5.  <span data-ttu-id="52b48-123">When the system is ready again, choose the **Create New Company** button.</span><span class="sxs-lookup"><span data-stu-id="52b48-123">When the system is ready again, choose the **Create New Company** button.</span></span>  
6.  <span data-ttu-id="52b48-124">In the dialogue that appears, specify the name as *My Company*, and choose the **Suite Production – Setup Data Only** option.</span><span class="sxs-lookup"><span data-stu-id="52b48-124">In the dialog that appears, specify the name as *My Company*, and choose the **Suite Production – Setup Data Only** option.</span></span>  

<span data-ttu-id="52b48-125">This again takes a number of minutes.</span><span class="sxs-lookup"><span data-stu-id="52b48-125">This again takes a number of minutes.</span></span> <span data-ttu-id="52b48-126">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span><span class="sxs-lookup"><span data-stu-id="52b48-126">When the process completes, you will be able to access Invoicing as part of your Office 365 Business Premium experience.</span></span>  

### <a name="what-about-my-data"></a><span data-ttu-id="52b48-127">What about my data?</span><span class="sxs-lookup"><span data-stu-id="52b48-127">What about my data?</span></span>
<span data-ttu-id="52b48-128">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span><span class="sxs-lookup"><span data-stu-id="52b48-128">When you rename the original My Company, the database tables that store your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] data are renamed, but the data itself is not touched.</span></span>  

<span data-ttu-id="52b48-129">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span><span class="sxs-lookup"><span data-stu-id="52b48-129">If you use both Invoicing and [!INCLUDE[d365fin](includes/d365fin_md.md)], the data is stored in two different containers (the two companies).</span></span> <span data-ttu-id="52b48-130">Nothing is shared, so you'll have to manage customers and items in both companies.</span><span class="sxs-lookup"><span data-stu-id="52b48-130">Nothing is shared, so you'll have to manage customers and items in both companies.</span></span>  

## <a name="see-also"></a><span data-ttu-id="52b48-131">See Also</span><span class="sxs-lookup"><span data-stu-id="52b48-131">See Also</span></span>
[<span data-ttu-id="52b48-132">Frequently Asked Questions</span><span class="sxs-lookup"><span data-stu-id="52b48-132">Frequently Asked Questions</span></span>](across-faq.md)  
[<span data-ttu-id="52b48-133">Setup and Administration</span><span class="sxs-lookup"><span data-stu-id="52b48-133">Setup and Administration</span></span>](admin-setup-and-administration.md)  

