---
title: Managing Personalisation as an Administrator in Financials | Microsoft Docs
description: Learn how to customise the user interface to suit your way of working.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 07/26/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 7c346455a9e27d7274b116754f1d594484b95d67
ms.openlocfilehash: 2d9b45bf21d325e60beadedfc94827d7f3fda075
ms.contentlocale: en-gb
ms.lasthandoff: 04/18/2018

---
# <a name="managing-personalization-as-an-administrator"></a><span data-ttu-id="9b263-103">Managing Personalisation as an Administrator</span><span class="sxs-lookup"><span data-stu-id="9b263-103">Managing Personalization as an Administrator</span></span>
<!--NAV in the Web client-->
<span data-ttu-id="9b263-104">Users can personalise their workspace to suit their own preferences.</span><span class="sxs-lookup"><span data-stu-id="9b263-104">Users can personalize their workspace to suit their own preferences.</span></span> <span data-ttu-id="9b263-105">As an administrator, you can control and manage personalisation by disabling the ability for users to personalise pages and clearing any page personalisations that users have made.</span><span class="sxs-lookup"><span data-stu-id="9b263-105">As an administrator, you can control and manage personalization by disabling the ability for users to personalize pages and clearing any page personalizations that users have made.</span></span>

## <a name="disable-personalization-for-a-profile"></a><span data-ttu-id="9b263-106">Disable personalisation for a profile</span><span class="sxs-lookup"><span data-stu-id="9b263-106">Disable personalization for a profile</span></span>
<span data-ttu-id="9b263-107">You can prevent all users that belong to a specific profile from being able to personalise their pages.</span><span class="sxs-lookup"><span data-stu-id="9b263-107">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span></span>
1.  <span data-ttu-id="9b263-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9b263-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>
2.  <span data-ttu-id="9b263-109">Select the profile in the list that you want to modify.</span><span class="sxs-lookup"><span data-stu-id="9b263-109">Select the profile in the list that you want to modify.</span></span>
3. <span data-ttu-id="9b263-110">Select the **Disable personalisation** check box, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="9b263-110">Select the **Disable personalization** check box, and then choose the **OK** button.</span></span>

## <a name="clear-user-personalizations"></a><span data-ttu-id="9b263-111">Clear user personalisations</span><span class="sxs-lookup"><span data-stu-id="9b263-111">Clear user personalizations</span></span>

<span data-ttu-id="9b263-112">Clearing page personalisation changes the page back to its original layout before any personalisation was made.</span><span class="sxs-lookup"><span data-stu-id="9b263-112">Clearing page personalization changes the page back to its original layout before any personalization was made.</span></span> <span data-ttu-id="9b263-113">There are two ways to clear the personalisations that users have made to pages: using the **Delete User Personalisation** page and using the **User Personalisation Card** page.</span><span class="sxs-lookup"><span data-stu-id="9b263-113">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span></span>

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a><span data-ttu-id="9b263-114">Clear user personalisations by using the Delete User Personalisation page</span><span class="sxs-lookup"><span data-stu-id="9b263-114">Clear user personalizations by using the Delete User Personalization page</span></span>

<span data-ttu-id="9b263-115">The **Delete User Personalisation** page enables you to clear personalisations on a per-page basis for each user individually.</span><span class="sxs-lookup"><span data-stu-id="9b263-115">The **Delete User Personalization** page enables you to clear personalizations on a per-page basis for each user individually.</span></span>

1.  <span data-ttu-id="9b263-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalisation**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9b263-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="9b263-117">The page lists all the pages that have been personalised and the user it belongs to.</span><span class="sxs-lookup"><span data-stu-id="9b263-117">The page lists all the pages that have been personalized and the user it belongs to.</span></span>

    >[!NOTE]
    > <span data-ttu-id="9b263-118">A check mark in the **Legacy Personalisation** columns indicates that the personalisation was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalisation different than it does now.</span><span class="sxs-lookup"><span data-stu-id="9b263-118">A check mark in the **Legacy Personalization** columns indicates that the personalization was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalization different than it does now.</span></span> <span data-ttu-id="9b263-119">Users who try to personalise these pages are locked from doing so unless they choose to unlock the page.</span><span class="sxs-lookup"><span data-stu-id="9b263-119">Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.</span></span> <span data-ttu-id="9b263-120">For more information, see [Why a page is locked from personalising](ui-personalization-locked.md).</span><span class="sxs-lookup"><span data-stu-id="9b263-120">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).</span></span>

2. <span data-ttu-id="9b263-121">Select the entry that you want to delete, and then choose the **Delete** action.</span><span class="sxs-lookup"><span data-stu-id="9b263-121">Select the entry that you want to delete, and then choose the **Delete** action.</span></span>

    <span data-ttu-id="9b263-122">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="9b263-122">The user will see the changes the next time they sign-in.</span></span>

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a><span data-ttu-id="9b263-123">Clear user personalisations by using the User Personalisation Card page</span><span class="sxs-lookup"><span data-stu-id="9b263-123">Clear user personalizations by using the User Personalization Card page</span></span>

<span data-ttu-id="9b263-124">The **User Personalisation Card** page enables you to clear the personalisation on all pages for specific user.</span><span class="sxs-lookup"><span data-stu-id="9b263-124">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span></span> <span data-ttu-id="9b263-125">This requires write permission to Table 2000000072 **Profile**.</span><span class="sxs-lookup"><span data-stu-id="9b263-125">This requires write permission to Table 2000000072 **Profile**.</span></span>

1.  <span data-ttu-id="9b263-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalisation**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9b263-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="9b263-127">The **User Personalisation** page lists all users who potentially have personalised pages.</span><span class="sxs-lookup"><span data-stu-id="9b263-127">The **User Personalization** page lists all users who potentially have personalized pages.</span></span> <span data-ttu-id="9b263-128">If you cannot find a user in the list, this means that they do not have any personalised pages.</span><span class="sxs-lookup"><span data-stu-id="9b263-128">If you cannot find a user in the list, this means that they do not have any personalized pages.</span></span>

2. <span data-ttu-id="9b263-129">Select the user from the list, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="9b263-129">Select the user from the list, and then choose the **Edit** action.</span></span>

3.  <span data-ttu-id="9b263-130">On the **Actions** tab, choose **Clear Personalised Pages**.</span><span class="sxs-lookup"><span data-stu-id="9b263-130">On the **Actions** tab, choose **Clear Personalized Pages**.</span></span>

    <span data-ttu-id="9b263-131">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="9b263-131">The user will see the changes the next time they sign-in.</span></span>

## <a name="see-also"></a><span data-ttu-id="9b263-132">See Also</span><span class="sxs-lookup"><span data-stu-id="9b263-132">See Also</span></span>
[<span data-ttu-id="9b263-133">Personalising Your Workspace</span><span class="sxs-lookup"><span data-stu-id="9b263-133">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
<span data-ttu-id="9b263-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9b263-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="9b263-135">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="9b263-135">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="9b263-136">Changing Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="9b263-136">Changing Which Features are Displayed</span></span>](ui-experiences.md)  

