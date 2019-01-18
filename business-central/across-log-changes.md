---
title: Track User Activity in a Change Log| Microsoft Docs
description: You can activate a user log so that you have a history of any changes made to data in tracked tables.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 11/14/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 3f158d7ed56445d6d2acf2ef8e5e9ab8e7487531
ms.openlocfilehash: bd0751ad5a4c0c7d9c3f7d5621bb7e6a62c3be2a
ms.contentlocale: en-gb
ms.lasthandoff: 12/04/2018

---
# <a name="logging-changes-in-business-central"></a><span data-ttu-id="4931f-103">Logging Changes in Business Central</span><span class="sxs-lookup"><span data-stu-id="4931f-103">Logging Changes in Business Central</span></span>

<span data-ttu-id="4931f-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span><span class="sxs-lookup"><span data-stu-id="4931f-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="4931f-105">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span><span class="sxs-lookup"><span data-stu-id="4931f-105">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="4931f-106">The change log collects all changes that are made to the table.</span><span class="sxs-lookup"><span data-stu-id="4931f-106">The change log collects all changes that are made to the table.</span></span>

> [!Important]
> <span data-ttu-id="4931f-107">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span><span class="sxs-lookup"><span data-stu-id="4931f-107">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span></span>
<br />
> * <span data-ttu-id="4931f-108">The session expired and was refreshed.</span><span class="sxs-lookup"><span data-stu-id="4931f-108">The session expired and was refreshed.</span></span>
> * <span data-ttu-id="4931f-109">The user selected another company or Role Centre.</span><span class="sxs-lookup"><span data-stu-id="4931f-109">The user selected another company or Role Center.</span></span>
> * <span data-ttu-id="4931f-110">The user signed out and back in.</span><span class="sxs-lookup"><span data-stu-id="4931f-110">The user signed out and back in.</span></span>

## <a name="working-with-the-change-log"></a><span data-ttu-id="4931f-111">Working with the Change Log</span><span class="sxs-lookup"><span data-stu-id="4931f-111">Working with the Change Log</span></span>

<span data-ttu-id="4931f-112">A common problem in many financial systems is to locate the origin of errors and changes in data.</span><span class="sxs-lookup"><span data-stu-id="4931f-112">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="4931f-113">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="4931f-113">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="4931f-114">The change log lets you track all direct modifications a user makes to data in the database.</span><span class="sxs-lookup"><span data-stu-id="4931f-114">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="4931f-115">You must specify each table and field that you want the system to log, and then you must activate the change log.</span><span class="sxs-lookup"><span data-stu-id="4931f-115">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="4931f-116">You activate and deactivate the change log on the **Change Log Setup** page.</span><span class="sxs-lookup"><span data-stu-id="4931f-116">You activate and deactivate the change log on the **Change Log Setup** page.</span></span> <span data-ttu-id="4931f-117">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span><span class="sxs-lookup"><span data-stu-id="4931f-117">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span>

<span data-ttu-id="4931f-118">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span><span class="sxs-lookup"><span data-stu-id="4931f-118">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="4931f-119">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span><span class="sxs-lookup"><span data-stu-id="4931f-119">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span></span> <span data-ttu-id="4931f-120">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span><span class="sxs-lookup"><span data-stu-id="4931f-120">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4931f-121">See Also</span><span class="sxs-lookup"><span data-stu-id="4931f-121">See Also</span></span>
[<span data-ttu-id="4931f-122">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="4931f-122">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="4931f-123">Sorting</span><span class="sxs-lookup"><span data-stu-id="4931f-123">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="4931f-124">Using Search for Page or Report</span><span class="sxs-lookup"><span data-stu-id="4931f-124">Using Search for Page or Report</span></span>](ui-search.md)  
<span data-ttu-id="4931f-125">[Managing Users and Permissions](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="4931f-125">[Managing Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="4931f-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4931f-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

