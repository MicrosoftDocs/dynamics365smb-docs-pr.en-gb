---
title: Set Up Time Sheets and Their Approval| Microsoft Docs
description: You set up time sheets to track the time used on jobs and using resources, helping you with project management, staffing, and capacity
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff, resource
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: a5b2027649e2adddfd3e59b4376303059f575a99
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-time-sheets"></a><span data-ttu-id="f287a-103">Set Up Time Sheets</span><span class="sxs-lookup"><span data-stu-id="f287a-103">Set Up Time Sheets</span></span>
<span data-ttu-id="f287a-104">Time sheets in [!INCLUDE[d365fin](includes/d365fin_md.md)] handle time registration in weekly increments of seven days.</span><span class="sxs-lookup"><span data-stu-id="f287a-104">Time sheets in [!INCLUDE[d365fin](includes/d365fin_md.md)] handle time registration in weekly increments of seven days.</span></span> <span data-ttu-id="f287a-105">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span><span class="sxs-lookup"><span data-stu-id="f287a-105">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span></span> <span data-ttu-id="f287a-106">Before you can use time sheets, you must specify how you want them to be set up and configured.</span><span class="sxs-lookup"><span data-stu-id="f287a-106">Before you can use time sheets, you must specify how you want them to be set up and configured.</span></span>

<span data-ttu-id="f287a-107">After you have set up how your organisation will use time sheets, you can specify if and how time sheets are approved.</span><span class="sxs-lookup"><span data-stu-id="f287a-107">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span></span> <span data-ttu-id="f287a-108">Depending on the needs of your organisation, you can designate:</span><span class="sxs-lookup"><span data-stu-id="f287a-108">Depending on the needs of your organization, you can designate:</span></span>

* <span data-ttu-id="f287a-109">One or more users as the time sheet administrator and approver for all time sheets.</span><span class="sxs-lookup"><span data-stu-id="f287a-109">One or more users as the time sheet administrator and approver for all time sheets.</span></span>
* <span data-ttu-id="f287a-110">A time sheet approver for each resource.</span><span class="sxs-lookup"><span data-stu-id="f287a-110">A time sheet approver for each resource.</span></span>

<span data-ttu-id="f287a-111">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span><span class="sxs-lookup"><span data-stu-id="f287a-111">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span></span> <span data-ttu-id="f287a-112">For more information, see [Use Time Sheets](projects-how-use-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="f287a-112">For more information, see [Use Time Sheets](projects-how-use-time-sheets.md).</span></span>

## <a name="to-set-up-general-information-for-time-sheets"></a><span data-ttu-id="f287a-113">To set up general information for time sheets</span><span class="sxs-lookup"><span data-stu-id="f287a-113">To set up general information for time sheets</span></span>
1. <span data-ttu-id="f287a-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resources Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f287a-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resources Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f287a-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="f287a-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="f287a-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="f287a-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span></span>

| <span data-ttu-id="f287a-117">Option</span><span class="sxs-lookup"><span data-stu-id="f287a-117">Option</span></span> | <span data-ttu-id="f287a-118">Description</span><span class="sxs-lookup"><span data-stu-id="f287a-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="f287a-119">**Never**</span><span class="sxs-lookup"><span data-stu-id="f287a-119">**Never**</span></span> |<span data-ttu-id="f287a-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span> |
| <span data-ttu-id="f287a-121">**Always**</span><span class="sxs-lookup"><span data-stu-id="f287a-121">**Always**</span></span> |<span data-ttu-id="f287a-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span></span> |
| <span data-ttu-id="f287a-123">**Machine Only**</span><span class="sxs-lookup"><span data-stu-id="f287a-123">**Machine Only**</span></span> |<span data-ttu-id="f287a-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span></span> <span data-ttu-id="f287a-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span> |

## <a name="to-assign-a-time-sheet-administrator"></a><span data-ttu-id="f287a-126">To assign a time sheet administrator</span><span class="sxs-lookup"><span data-stu-id="f287a-126">To assign a time sheet administrator</span></span>
1. <span data-ttu-id="f287a-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f287a-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f287a-128">Add a new user if the user list does not include the person who you want to be the time sheet administrator.</span><span class="sxs-lookup"><span data-stu-id="f287a-128">Add a new user if the user list does not include the person who you want to be the time sheet administrator.</span></span> <span data-ttu-id="f287a-129">For more information, see [Manage Users and Permissions](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="f287a-129">For more information, see [Manage Users and Permissions](ui-how-users-permissions.md).</span></span>
3. <span data-ttu-id="f287a-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.** check box.</span><span class="sxs-lookup"><span data-stu-id="f287a-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.** check box.</span></span>  

> [!TIP]  
>   <span data-ttu-id="f287a-131">It is recommended that you designate only one user to be the time sheet administrator for a company.</span><span class="sxs-lookup"><span data-stu-id="f287a-131">It is recommended that you designate only one user to be the time sheet administrator for a company.</span></span> <span data-ttu-id="f287a-132">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span><span class="sxs-lookup"><span data-stu-id="f287a-132">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span></span>  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a><span data-ttu-id="f287a-133">To assign a time sheets owner and approver</span><span class="sxs-lookup"><span data-stu-id="f287a-133">To assign a time sheets owner and approver</span></span>
1. <span data-ttu-id="f287a-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f287a-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resources**, and then choose the related link.</span></span>
2. <span data-ttu-id="f287a-135">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span><span class="sxs-lookup"><span data-stu-id="f287a-135">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span></span>  
3. <span data-ttu-id="f287a-136">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-136">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span></span> <span data-ttu-id="f287a-137">The owner can enter time usage on a time sheet and submit it for approval.</span><span class="sxs-lookup"><span data-stu-id="f287a-137">The owner can enter time usage on a time sheet and submit it for approval.</span></span> <span data-ttu-id="f287a-138">In general, when the resource is a person, that person is also the owner.</span><span class="sxs-lookup"><span data-stu-id="f287a-138">In general, when the resource is a person, that person is also the owner.</span></span>  
4. <span data-ttu-id="f287a-139">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-139">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span></span> <span data-ttu-id="f287a-140">The approver can approve, reject, or reopen a time sheet.</span><span class="sxs-lookup"><span data-stu-id="f287a-140">The approver can approve, reject, or reopen a time sheet.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="f287a-141">You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span><span class="sxs-lookup"><span data-stu-id="f287a-141">You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span></span>

## <a name="see-also"></a><span data-ttu-id="f287a-142">See Also</span><span class="sxs-lookup"><span data-stu-id="f287a-142">See Also</span></span>
[<span data-ttu-id="f287a-143">Setting Up Project Management</span><span class="sxs-lookup"><span data-stu-id="f287a-143">Setting Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="f287a-144">Project Management</span><span class="sxs-lookup"><span data-stu-id="f287a-144">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="f287a-145">Finance</span><span class="sxs-lookup"><span data-stu-id="f287a-145">Finance</span></span>](finance.md)  
<span data-ttu-id="f287a-146">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="f287a-146">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="f287a-147">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="f287a-147">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="f287a-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f287a-148">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

