---
title: Manage database access intent in Business Central | Microsoft Docs
description: Change the database access intent for reports, API pages, and queries.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 5fe04fc290f10324105d4d9ca01e13166bf2ad8f
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773086"
---
# <a name="managing-database-access-intent"></a><span data-ttu-id="4eba4-103">Managing Database Access Intent</span><span class="sxs-lookup"><span data-stu-id="4eba4-103">Managing Database Access Intent</span></span> 

<span data-ttu-id="4eba4-104">As a super user or administrator, you can change the database access intent on reports, pages of the type API, and queries to improve performance of the service.</span><span class="sxs-lookup"><span data-stu-id="4eba4-104">As a super user or administrator, you can change the database access intent on reports, pages of the type API, and queries to improve performance of the service.</span></span>

## <a name="overview"></a><span data-ttu-id="4eba4-105">Overview</span><span class="sxs-lookup"><span data-stu-id="4eba4-105">Overview</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="4eba4-106">can be set up to use read-only replicas of the primary (read-write) database.</span><span class="sxs-lookup"><span data-stu-id="4eba4-106">can be set up to use read-only replicas of the primary (read-write) database.</span></span> <span data-ttu-id="4eba4-107">Using the database replica reduces the load on the primary database.</span><span class="sxs-lookup"><span data-stu-id="4eba4-107">Using the database replica reduces the load on the primary database.</span></span> <span data-ttu-id="4eba4-108">In some cases, it will also improve the performance when viewing data in the client.</span><span class="sxs-lookup"><span data-stu-id="4eba4-108">In some cases, it will also improve the performance when viewing data in the client.</span></span> <span data-ttu-id="4eba4-109">Replicas are beneficial for objects, like reports, queries, and API pages, that are used for viewing data only, not modifying data.</span><span class="sxs-lookup"><span data-stu-id="4eba4-109">Replicas are beneficial for objects, like reports, queries, and API pages, that are used for viewing data only, not modifying data.</span></span>

<span data-ttu-id="4eba4-110">When objects run, the database access intent determines whether to use a read-only replica, if one is available, or the primary database.</span><span class="sxs-lookup"><span data-stu-id="4eba4-110">When objects run, the database access intent determines whether to use a read-only replica, if one is available, or the primary database.</span></span> <span data-ttu-id="4eba4-111">Reports, API pages, and queries are developed with a predefined database access intent (see [DatabaseAccessIntent property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataaccessintent-property)).</span><span class="sxs-lookup"><span data-stu-id="4eba4-111">Reports, API pages, and queries are developed with a predefined database access intent (see [DatabaseAccessIntent property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataaccessintent-property)).</span></span>

<span data-ttu-id="4eba4-112">The **Database Access Intent List** page lets you override the predefined database access intent for objects when they're run.</span><span class="sxs-lookup"><span data-stu-id="4eba4-112">The **Database Access Intent List** page lets you override the predefined database access intent for objects when they're run.</span></span>

<span data-ttu-id="4eba4-113">In database terms, this feature is commonly known as *read scale-out*. For more information about read-scale out and data access intent in [!INCLUDE[prod_short](includes/prod_short.md)], see [Utilising Read Scale-Out for Better Performance](/dynamics365/business-central/dev-itpro/administration/database-read-scale-out-overview) in the [!INCLUDE[prod_short](includes/prod_short.md)] Developer and Administration help.</span><span class="sxs-lookup"><span data-stu-id="4eba4-113">In database terms, this feature is commonly known as *read scale-out*. For more information about read-scale out and data access intent in [!INCLUDE[prod_short](includes/prod_short.md)], see [Utilizing Read Scale-Out for Better Performance](/dynamics365/business-central/dev-itpro/administration/database-read-scale-out-overview) in the [!INCLUDE[prod_short](includes/prod_short.md)] Developer and Administration help.</span></span>

## <a name="to-change-the-database-access-intent"></a><span data-ttu-id="4eba4-114">To change the database access intent</span><span class="sxs-lookup"><span data-stu-id="4eba4-114">To change the database access intent</span></span>

1. <span data-ttu-id="4eba4-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Database Access Intent List**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="4eba4-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Database Access Intent List**, and then choose the related link.</span></span>

    <span data-ttu-id="4eba4-116">The page lists all reports, pages, and queries.</span><span class="sxs-lookup"><span data-stu-id="4eba4-116">The page lists all reports, pages, and queries.</span></span> <span data-ttu-id="4eba4-117">The **Access Intent** column includes one of the following values:</span><span class="sxs-lookup"><span data-stu-id="4eba4-117">The **Access Intent** column includes one of the following values:</span></span>

    |<span data-ttu-id="4eba4-118">**Setting**</span><span class="sxs-lookup"><span data-stu-id="4eba4-118">**Setting**</span></span>|<span data-ttu-id="4eba4-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="4eba4-119">**Description**</span></span>|  
    |------------|-------------|  
    |<span data-ttu-id="4eba4-120">**Default**</span><span class="sxs-lookup"><span data-stu-id="4eba4-120">**Default**</span></span>|<span data-ttu-id="4eba4-121">Indicates that the object uses the predefined database access intent.</span><span class="sxs-lookup"><span data-stu-id="4eba4-121">Indicates that the object uses the predefined database access intent.</span></span>|
    |<span data-ttu-id="4eba4-122">**Allow Write**</span><span class="sxs-lookup"><span data-stu-id="4eba4-122">**Allow Write**</span></span>|<span data-ttu-id="4eba4-123">Sets the object to use the primary database, allowing the user to modify data.</span><span class="sxs-lookup"><span data-stu-id="4eba4-123">Sets the object to use the primary database, allowing the user to modify data.</span></span>|
    |<span data-ttu-id="4eba4-124">**Read Only**</span><span class="sxs-lookup"><span data-stu-id="4eba4-124">**Read Only**</span></span>|<span data-ttu-id="4eba4-125">Sets the object to use the database replica, which means that the user can only view data, not change data.</span><span class="sxs-lookup"><span data-stu-id="4eba4-125">Sets the object to use the database replica, which means that the user can only view data, not change data.</span></span>|

2. <span data-ttu-id="4eba4-126">Choose the **Edit List** action.</span><span class="sxs-lookup"><span data-stu-id="4eba4-126">Choose the **Edit List** action.</span></span>

3. <span data-ttu-id="4eba4-127">On the **Edit - Database Access Intent List** page, change the **Access Intent** field for the objects.</span><span class="sxs-lookup"><span data-stu-id="4eba4-127">On the **Edit - Database Access Intent List** page, change the **Access Intent** field for the objects.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4eba4-128">If an object that is editable, like the Customer Card, is set to **Read Only**, the primary database will still be used, regardless of the access intent, allowing users to make changes as normal.</span><span class="sxs-lookup"><span data-stu-id="4eba4-128">If an object that is editable, like the Customer Card, is set to **Read Only**, the primary database will still be used, regardless of the access intent, allowing users to make changes as normal.</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="4eba4-129">See Related Training at [Microsoft Learn](/learn/paths/deploy-configure-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="4eba4-129">See Related Training at [Microsoft Learn](/learn/paths/deploy-configure-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="4eba4-130">See Also</span><span class="sxs-lookup"><span data-stu-id="4eba4-130">See Also</span></span>
[<span data-ttu-id="4eba4-131">Business Functionality</span><span class="sxs-lookup"><span data-stu-id="4eba4-131">Business Functionality</span></span>](across-business-functionality.md)  
[<span data-ttu-id="4eba4-132">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="4eba4-132">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="4eba4-133">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4eba4-133">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="4eba4-134">Getting Ready for Doing Business</span><span class="sxs-lookup"><span data-stu-id="4eba4-134">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)    

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]