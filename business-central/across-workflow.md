---
title: Workflow | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 05/09/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 75501b9402bb1c14fcfeb2fc6e61f055a2247493
ms.openlocfilehash: 128d20233d1750b2b89c3c7e2de6e497bd32b342
ms.contentlocale: en-gb
ms.lasthandoff: 05/15/2018

---
# <a name="workflow"></a><span data-ttu-id="e7a44-105">Workflow</span><span class="sxs-lookup"><span data-stu-id="e7a44-105">Workflow</span></span>
<span data-ttu-id="e7a44-106">You can set up and use workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="e7a44-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="e7a44-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="e7a44-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="e7a44-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="e7a44-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="e7a44-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="e7a44-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="e7a44-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="e7a44-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="e7a44-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="e7a44-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="e7a44-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span><span class="sxs-lookup"><span data-stu-id="e7a44-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="e7a44-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="e7a44-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="e7a44-114">For more information, see the list of workflow templates in the Workflow Templates window.</span><span class="sxs-lookup"><span data-stu-id="e7a44-114">For more information, see the list of workflow templates in the Workflow Templates window.</span></span>  

 <span data-ttu-id="e7a44-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="e7a44-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="e7a44-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span><span class="sxs-lookup"><span data-stu-id="e7a44-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span></span>

> [!NOTE]  
> <span data-ttu-id="e7a44-117">Workflows can also be initiated from Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="e7a44-117">Workflows can also be initiated from Microsoft Flow.</span></span> <span data-ttu-id="e7a44-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="e7a44-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>  

 <span data-ttu-id="e7a44-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="e7a44-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="e7a44-120">**To**</span><span class="sxs-lookup"><span data-stu-id="e7a44-120">**To**</span></span>|<span data-ttu-id="e7a44-121">**See**</span><span class="sxs-lookup"><span data-stu-id="e7a44-121">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="e7a44-122">Set up workflow users, specify how users get notified, and create new workflows.</span><span class="sxs-lookup"><span data-stu-id="e7a44-122">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="e7a44-123">For new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="e7a44-123">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="e7a44-124">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="e7a44-124">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="e7a44-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span><span class="sxs-lookup"><span data-stu-id="e7a44-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="e7a44-126">Archive and delete workflows.</span><span class="sxs-lookup"><span data-stu-id="e7a44-126">Archive and delete workflows.</span></span>|[<span data-ttu-id="e7a44-127">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="e7a44-127">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="e7a44-128">See Also</span><span class="sxs-lookup"><span data-stu-id="e7a44-128">See Also</span></span>  
[<span data-ttu-id="e7a44-129">Sales</span><span class="sxs-lookup"><span data-stu-id="e7a44-129">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="e7a44-130">Purchasing</span><span class="sxs-lookup"><span data-stu-id="e7a44-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="e7a44-131">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="e7a44-131">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="e7a44-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7a44-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

