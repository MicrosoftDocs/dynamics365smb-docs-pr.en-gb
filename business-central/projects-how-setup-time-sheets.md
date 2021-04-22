---
title: Set Up Time Sheets and Their Approval| Microsoft Docs
description: You set up time sheets to track the time used on jobs and using resources, helping you with project management, staffing, and capacity
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff, resource
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7134f45ef41400df1e44655d7a7e580da8dcb06b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780414"
---
# <a name="set-up-time-sheets"></a><span data-ttu-id="f975c-103">Set Up Time Sheets</span><span class="sxs-lookup"><span data-stu-id="f975c-103">Set Up Time Sheets</span></span>
<span data-ttu-id="f975c-104">Time sheets in [!INCLUDE[prod_short](includes/prod_short.md)] handle time registration in weekly increments of seven days.</span><span class="sxs-lookup"><span data-stu-id="f975c-104">Time sheets in [!INCLUDE[prod_short](includes/prod_short.md)] handle time registration in weekly increments of seven days.</span></span> <span data-ttu-id="f975c-105">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span><span class="sxs-lookup"><span data-stu-id="f975c-105">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span></span> <span data-ttu-id="f975c-106">Before you can use time sheets, you must specify how you want them to be set up and configured.</span><span class="sxs-lookup"><span data-stu-id="f975c-106">Before you can use time sheets, you must specify how you want them to be set up and configured.</span></span>

<span data-ttu-id="f975c-107">After you have set up how your organisation will use time sheets, you can specify if and how time sheets are approved.</span><span class="sxs-lookup"><span data-stu-id="f975c-107">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span></span> <span data-ttu-id="f975c-108">Depending on the needs of your organisation, you can designate:</span><span class="sxs-lookup"><span data-stu-id="f975c-108">Depending on the needs of your organization, you can designate:</span></span>

* <span data-ttu-id="f975c-109">One or more users as the time sheet administrator and approver for all time sheets.</span><span class="sxs-lookup"><span data-stu-id="f975c-109">One or more users as the time sheet administrator and approver for all time sheets.</span></span>
* <span data-ttu-id="f975c-110">A time sheet approver for each resource.</span><span class="sxs-lookup"><span data-stu-id="f975c-110">A time sheet approver for each resource.</span></span>

<span data-ttu-id="f975c-111">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span><span class="sxs-lookup"><span data-stu-id="f975c-111">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span></span> <span data-ttu-id="f975c-112">For more information, see [Use Time Sheets](projects-how-use-time-sheets.md).</span><span class="sxs-lookup"><span data-stu-id="f975c-112">For more information, see [Use Time Sheets](projects-how-use-time-sheets.md).</span></span>

## <a name="to-set-up-general-information-for-time-sheets"></a><span data-ttu-id="f975c-113">To set up general information for time sheets</span><span class="sxs-lookup"><span data-stu-id="f975c-113">To set up general information for time sheets</span></span>
1. <span data-ttu-id="f975c-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f975c-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f975c-115">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="f975c-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="f975c-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span><span class="sxs-lookup"><span data-stu-id="f975c-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span></span>

| <span data-ttu-id="f975c-117">Option</span><span class="sxs-lookup"><span data-stu-id="f975c-117">Option</span></span> | <span data-ttu-id="f975c-118">Description</span><span class="sxs-lookup"><span data-stu-id="f975c-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="f975c-119">**Never**</span><span class="sxs-lookup"><span data-stu-id="f975c-119">**Never**</span></span> |<span data-ttu-id="f975c-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span> |
| <span data-ttu-id="f975c-121">**Always**</span><span class="sxs-lookup"><span data-stu-id="f975c-121">**Always**</span></span> |<span data-ttu-id="f975c-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span></span> |
| <span data-ttu-id="f975c-123">**Machine Only**</span><span class="sxs-lookup"><span data-stu-id="f975c-123">**Machine Only**</span></span> |<span data-ttu-id="f975c-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span></span> <span data-ttu-id="f975c-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span> |

## <a name="to-assign-a-time-sheet-administrator"></a><span data-ttu-id="f975c-126">To assign a time sheet administrator</span><span class="sxs-lookup"><span data-stu-id="f975c-126">To assign a time sheet administrator</span></span>
1. <span data-ttu-id="f975c-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f975c-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f975c-128">Add a new user if the user list does not include the person who you want to be the time sheet administrator.</span><span class="sxs-lookup"><span data-stu-id="f975c-128">Add a new user if the user list does not include the person who you want to be the time sheet administrator.</span></span> <span data-ttu-id="f975c-129">For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="f975c-129">For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>
3. <span data-ttu-id="f975c-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.** check box.</span><span class="sxs-lookup"><span data-stu-id="f975c-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.** check box.</span></span>  

> [!TIP]  
>   <span data-ttu-id="f975c-131">It is recommended that you designate only one user to be the time sheet administrator for a company.</span><span class="sxs-lookup"><span data-stu-id="f975c-131">It is recommended that you designate only one user to be the time sheet administrator for a company.</span></span> <span data-ttu-id="f975c-132">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span><span class="sxs-lookup"><span data-stu-id="f975c-132">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span></span>  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a><span data-ttu-id="f975c-133">To assign a time sheets owner and approver</span><span class="sxs-lookup"><span data-stu-id="f975c-133">To assign a time sheets owner and approver</span></span>
1. <span data-ttu-id="f975c-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f975c-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resources**, and then choose the related link.</span></span>
2. <span data-ttu-id="f975c-135">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span><span class="sxs-lookup"><span data-stu-id="f975c-135">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span></span>  
3. <span data-ttu-id="f975c-136">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-136">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span></span> <span data-ttu-id="f975c-137">The owner can enter time usage on a time sheet and submit it for approval.</span><span class="sxs-lookup"><span data-stu-id="f975c-137">The owner can enter time usage on a time sheet and submit it for approval.</span></span> <span data-ttu-id="f975c-138">In general, when the resource is a person, that person is also the owner.</span><span class="sxs-lookup"><span data-stu-id="f975c-138">In general, when the resource is a person, that person is also the owner.</span></span>  
4. <span data-ttu-id="f975c-139">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-139">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span></span> <span data-ttu-id="f975c-140">The approver can approve, reject, or reopen a time sheet.</span><span class="sxs-lookup"><span data-stu-id="f975c-140">The approver can approve, reject, or reopen a time sheet.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="f975c-141">You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span><span class="sxs-lookup"><span data-stu-id="f975c-141">You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span></span>

## <a name="see-also"></a><span data-ttu-id="f975c-142">See Also</span><span class="sxs-lookup"><span data-stu-id="f975c-142">See Also</span></span>
[<span data-ttu-id="f975c-143">Setting Up Project Management</span><span class="sxs-lookup"><span data-stu-id="f975c-143">Setting Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="f975c-144">Project Management</span><span class="sxs-lookup"><span data-stu-id="f975c-144">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="f975c-145">Finance</span><span class="sxs-lookup"><span data-stu-id="f975c-145">Finance</span></span>](finance.md)  
<span data-ttu-id="f975c-146">[Purchasing](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="f975c-146">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="f975c-147">[Sales](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="f975c-147">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="f975c-148">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f975c-148">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]