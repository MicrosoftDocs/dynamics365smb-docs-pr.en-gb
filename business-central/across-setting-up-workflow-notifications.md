---
title: Workflow Notifications
description: Many workflow responses are about notifying a user that an event has occurred that they must act on. For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver. On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record. For workflow steps that are about approval, each notification is tied to an approval entry.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.workload: na
ms.search.keywords: ''
ms.date: 10/14/2020
ms.author: edupont
ms.openlocfilehash: 1dd64213bc38d5d98e6369e97257e53cef04bbd0
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753032"
---
# <a name="workflow-notifications"></a><span data-ttu-id="10d18-106">Workflow Notifications</span><span class="sxs-lookup"><span data-stu-id="10d18-106">Workflow Notifications</span></span>

<span data-ttu-id="10d18-107">Set up your workflows to automatically notify users when their attention is required for a step in that workflow.</span><span class="sxs-lookup"><span data-stu-id="10d18-107">Set up your workflows to automatically notify users when their attention is required for a step in that workflow.</span></span> <span data-ttu-id="10d18-108">Many workflow responses are about notifying a user that an event has occurred that they must act on.</span><span class="sxs-lookup"><span data-stu-id="10d18-108">Many workflow responses are about notifying a user that an event has occurred that they must act on.</span></span> <span data-ttu-id="10d18-109">For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver.</span><span class="sxs-lookup"><span data-stu-id="10d18-109">For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver.</span></span> <span data-ttu-id="10d18-110">On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record.</span><span class="sxs-lookup"><span data-stu-id="10d18-110">On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record.</span></span> <span data-ttu-id="10d18-111">For workflow steps that are about approval, each notification is tied to an approval entry.</span><span class="sxs-lookup"><span data-stu-id="10d18-111">For workflow steps that are about approval, each notification is tied to an approval entry.</span></span> <span data-ttu-id="10d18-112">For more information, see [Workflow](across-workflow.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-112">For more information, see [Workflow](across-workflow.md).</span></span>  

> [!NOTE]  
> <span data-ttu-id="10d18-113">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports notifications as email and as internal notes.</span><span class="sxs-lookup"><span data-stu-id="10d18-113">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports notifications as email and as internal notes.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="10d18-114">All workflow notifications are sent through a job queue.</span><span class="sxs-lookup"><span data-stu-id="10d18-114">All workflow notifications are sent through a job queue.</span></span> <span data-ttu-id="10d18-115">Make sure that the job queue in your installation is set up to handle workflow notifications, and that the **Start Automatically From Server** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="10d18-115">Make sure that the job queue in your installation is set up to handle workflow notifications, and that the **Start Automatically From Server** check box is selected.</span></span> <span data-ttu-id="10d18-116">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-116">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

## <a name="set-up-notifications"></a><span data-ttu-id="10d18-117">Set up notifications</span><span class="sxs-lookup"><span data-stu-id="10d18-117">Set up notifications</span></span>

<span data-ttu-id="10d18-118">You set up different aspects of workflow notifications in the following places:</span><span class="sxs-lookup"><span data-stu-id="10d18-118">You set up different aspects of workflow notifications in the following places:</span></span>  

* <span data-ttu-id="10d18-119">Approver notification</span><span class="sxs-lookup"><span data-stu-id="10d18-119">Approver notification</span></span>

    <span data-ttu-id="10d18-120">For approval workflows, you set up the recipients of workflow notifications by filling a line on the **Approval User Setup** page for each user that takes part in the workflow.</span><span class="sxs-lookup"><span data-stu-id="10d18-120">For approval workflows, you set up the recipients of workflow notifications by filling a line on the **Approval User Setup** page for each user that takes part in the workflow.</span></span>  

    <span data-ttu-id="10d18-121">For example, if User 2 is specified in the **Approver ID** field on the line for User 1, then the approval request notification is sent to User 1.</span><span class="sxs-lookup"><span data-stu-id="10d18-121">For example, if User 2 is specified in the **Approver ID** field on the line for User 1, then the approval request notification is sent to User 1.</span></span> <span data-ttu-id="10d18-122">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-122">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>  
* <span data-ttu-id="10d18-123">Notification schedules</span><span class="sxs-lookup"><span data-stu-id="10d18-123">Notification schedules</span></span>

    <span data-ttu-id="10d18-124">You set up when and how users receive workflow notifications by filling the **Notification Schedule** page for each workflow user.</span><span class="sxs-lookup"><span data-stu-id="10d18-124">You set up when and how users receive workflow notifications by filling the **Notification Schedule** page for each workflow user.</span></span> <span data-ttu-id="10d18-125">For more information, see [Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-125">For more information, see [Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).</span></span>  
* <span data-ttu-id="10d18-126">Customise the email notifications</span><span class="sxs-lookup"><span data-stu-id="10d18-126">Customize the email notifications</span></span>

    <span data-ttu-id="10d18-127">If you want, you can customise the content of the email notification by modifying report 1320, Notification Email.</span><span class="sxs-lookup"><span data-stu-id="10d18-127">If you want, you can customize the content of the email notification by modifying report 1320, Notification Email.</span></span> <span data-ttu-id="10d18-128">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-128">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>  
* <span data-ttu-id="10d18-129">Response options</span><span class="sxs-lookup"><span data-stu-id="10d18-129">Response options</span></span>

    <span data-ttu-id="10d18-130">You set up specific content and rules of a workflow notification when you create the workflow in question.</span><span class="sxs-lookup"><span data-stu-id="10d18-130">You set up specific content and rules of a workflow notification when you create the workflow in question.</span></span> <span data-ttu-id="10d18-131">You do this by selecting options on the **Workflow Response Options** page for the workflow response that represents the notification.</span><span class="sxs-lookup"><span data-stu-id="10d18-131">You do this by selecting options on the **Workflow Response Options** page for the workflow response that represents the notification.</span></span> <span data-ttu-id="10d18-132">For more information, see step 9 in [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-132">For more information, see step 9 in [Create Workflows](across-how-to-create-workflows.md).</span></span>  

* <span data-ttu-id="10d18-133">Notify sender</span><span class="sxs-lookup"><span data-stu-id="10d18-133">Notify sender</span></span>

    <span data-ttu-id="10d18-134">For approval workflows, add a workflow response step to notify the sender when the request has been approved or rejected.</span><span class="sxs-lookup"><span data-stu-id="10d18-134">For approval workflows, add a workflow response step to notify the sender when the request has been approved or rejected.</span></span> <span data-ttu-id="10d18-135">For more information, see step 9 in [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="10d18-135">For more information, see step 9 in [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="10d18-136">See Also</span><span class="sxs-lookup"><span data-stu-id="10d18-136">See Also</span></span>

[<span data-ttu-id="10d18-137">Set Up Approval Users</span><span class="sxs-lookup"><span data-stu-id="10d18-137">Set Up Approval Users</span></span>](across-how-to-set-up-approval-users.md)  
[<span data-ttu-id="10d18-138">Set Up Workflow Users</span><span class="sxs-lookup"><span data-stu-id="10d18-138">Set Up Workflow Users</span></span>](across-how-to-set-up-workflow-users.md)  
[<span data-ttu-id="10d18-139">Specify When and How to Receive Notifications</span><span class="sxs-lookup"><span data-stu-id="10d18-139">Specify When and How to Receive Notifications</span></span>](across-how-to-specify-when-and-how-to-receive-notifications.md)  
[<span data-ttu-id="10d18-140">Create Workflows</span><span class="sxs-lookup"><span data-stu-id="10d18-140">Create Workflows</span></span>](across-how-to-create-workflows.md)  
[<span data-ttu-id="10d18-141">Create and Modify Custom Report Layouts</span><span class="sxs-lookup"><span data-stu-id="10d18-141">Create and Modify Custom Report Layouts</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="10d18-142">Use Job Queues to Schedule Tasks</span><span class="sxs-lookup"><span data-stu-id="10d18-142">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)  
[<span data-ttu-id="10d18-143">Set up Email</span><span class="sxs-lookup"><span data-stu-id="10d18-143">Set up Email</span></span>](admin-how-setup-email.md)  
[<span data-ttu-id="10d18-144">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span><span class="sxs-lookup"><span data-stu-id="10d18-144">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span></span>](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
[<span data-ttu-id="10d18-145">Workflow</span><span class="sxs-lookup"><span data-stu-id="10d18-145">Workflow</span></span>](across-workflow.md)  
