---
title: Why Can't I Personalise a Page | Microsoft Docs
description: Explains why you cannot personlaize a page and what yoo can do to unlock it so you can personalise it.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 64995372f68ed2804bc165823dacc34ad6a3194d
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1251292"
---
# <a name="why-a-page-is-locked-from-personalization"></a><span data-ttu-id="a6dc7-103">Why a Page is Locked from Personalisation</span><span class="sxs-lookup"><span data-stu-id="a6dc7-103">Why a Page is Locked from Personalization</span></span>

<span data-ttu-id="a6dc7-104">There are two conditions that prevent you from personalising a page.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-104">There are two conditions that prevent you from personalizing a page.</span></span> <span data-ttu-id="a6dc7-105">Either the page is locked (as indicated by ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock")) or it is blocked (as indicated by ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked")).</span><span class="sxs-lookup"><span data-stu-id="a6dc7-105">Either the page is locked (as indicated by ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock")) or it is blocked (as indicated by ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked")).</span></span>

## <a name="locked-from-personalizing"></a><span data-ttu-id="a6dc7-106">Locked from Personalising</span><span class="sxs-lookup"><span data-stu-id="a6dc7-106">Locked from Personalizing</span></span>

<span data-ttu-id="a6dc7-107">If there is a ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock") icon in the **Personalising** banner when you open a page (as shown), this means that you are currently prevented from making any more personalisation changes to the page.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-107">If there is a ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock") icon in the **Personalizing** banner when you open a page (as shown), this means that you are currently prevented from making any more personalization changes to the page.</span></span>

<span data-ttu-id="a6dc7-108">![Personalise Lock](media/personalization-locked.png "Personalise lock")</span><span class="sxs-lookup"><span data-stu-id="a6dc7-108">![Personalize Lock](media/personalization-locked.png "Personalize lock")</span></span>


<!-- This is because we changed the way personalization works behind the scenes since the last time that you personalized the page. Unfortunately, the old way and new of doing things do not work together.

The page currently includes the last personalization changes that you made. If you want to continue personalizing the page, then you can choose the lock icon and then **Unlock**. Just be aware that if you choose to unlock the page, the current personalization of the page will be cleared, and you will have to start from scratch.
-->

<span data-ttu-id="a6dc7-109">There can be two reasons for this:</span><span class="sxs-lookup"><span data-stu-id="a6dc7-109">There can be two reasons for this:</span></span>

1. <span data-ttu-id="a6dc7-110">You have personalised the page before, but it was done using an earlier version of the product.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-110">You have personalized the page before, but it was done using an earlier version of the product.</span></span> <span data-ttu-id="a6dc7-111">We changed the way personalisation works behind the scenes since the last time that you personalised the page.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-111">We changed the way personalization works behind the scenes since the last time that you personalized the page.</span></span> <span data-ttu-id="a6dc7-112">Unfortunately, the old way and new way of doing things do not work together.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-112">Unfortunately, the old way and new way of doing things do not work together.</span></span>

2. <span data-ttu-id="a6dc7-113">Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalise the page.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-113">Until now, you have only used the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] to personalize the page.</span></span>

### <a name="unlocking-the-page"></a><span data-ttu-id="a6dc7-114">Unlocking the Page</span><span class="sxs-lookup"><span data-stu-id="a6dc7-114">Unlocking the Page</span></span>

<span data-ttu-id="a6dc7-115">If you want to unlock a page and continue personalising it, choose ![Personalise Lock](media/personalization-lock-icon.png "Personalise lock"), and then **Unlock**.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-115">If you want to unlock a page and continue personalizing it, choose ![Personalize Lock](media/personalization-lock-icon.png "Personalize lock"), and then **Unlock**.</span></span>  

<span data-ttu-id="a6dc7-116">Before you unlock the page, be aware of the following:</span><span class="sxs-lookup"><span data-stu-id="a6dc7-116">Before you unlock the page, be aware of the following:</span></span>

- <span data-ttu-id="a6dc7-117">The current personalisation of the page will be cleared.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-117">The current personalization of the page will be cleared.</span></span> <span data-ttu-id="a6dc7-118">The page will go back to its original layout, and you will have to start from scratch.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-118">The page will go back to its original layout, and you will have to start from scratch.</span></span>

- <span data-ttu-id="a6dc7-119">In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalisation changes made in the Business Central client.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-119">In the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)], the page will remain as-is and will not be affected by the new personalization changes made in the Business Central client.</span></span> <span data-ttu-id="a6dc7-120">Going forward, the personalisation in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-120">Going forward, the personalization in the [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] and Business Central client will be completely separate from each other.</span></span>

## <a name="blocked-from-personalizing"></a><span data-ttu-id="a6dc7-121">Blocked from Personalising</span><span class="sxs-lookup"><span data-stu-id="a6dc7-121">Blocked from Personalizing</span></span>

<span data-ttu-id="a6dc7-122">If there is a ![Personalisation blocked](media/personalization-blocked-icon.png "Personalisation blocked") icon in the Personalising banner, this means that you are blocked from doing any personalisation to the page.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-122">If there is a ![Personalization blocked](media/personalization-blocked-icon.png "Personalization blocked") icon in the Personalizing banner, this means that you are blocked from doing any personalization to the page.</span></span>

<span data-ttu-id="a6dc7-123">![Personalise blocked](media/personalization-blocked.png "Personalise lock")</span><span class="sxs-lookup"><span data-stu-id="a6dc7-123">![Personalize blocked](media/personalization-blocked.png "Personalize lock")</span></span>

<span data-ttu-id="a6dc7-124">The reason for this is that the Role Centre or profile that is currently associated with your user account modifies this page specifically for your role.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-124">The reason for this is that the Role Center or profile that is currently associated with your user account modifies this page specifically for your role.</span></span> <span data-ttu-id="a6dc7-125">Please contact your administrator for assistance or, if it makes sense, try switching to a Role Centre (from  [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central")) that does include role-tailoring for this page.</span><span class="sxs-lookup"><span data-stu-id="a6dc7-125">Please contact your administrator for assistance or, if it makes sense, try switching to a Role Center (from  [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central")) that does include role-tailoring for this page.</span></span>

## <a name="see-also"></a><span data-ttu-id="a6dc7-126">See Also</span><span class="sxs-lookup"><span data-stu-id="a6dc7-126">See Also</span></span>
[<span data-ttu-id="a6dc7-127">Personalising Your Workspace</span><span class="sxs-lookup"><span data-stu-id="a6dc7-127">Personalizing Your Workspace</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="a6dc7-128">Managing Personalisation</span><span class="sxs-lookup"><span data-stu-id="a6dc7-128">Managing Personalization</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="a6dc7-129">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="a6dc7-129">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="a6dc7-130">Changing Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="a6dc7-130">Changing Which Features are Displayed</span></span>](ui-experiences.md)  
