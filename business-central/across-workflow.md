---
title: Workflow | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d8dac033ad2f4573d8a7f0047c44ac04eb8e6eb0
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773418"
---
# <a name="workflows-in-dynamics-365-business-central"></a><span data-ttu-id="b7776-105">Workflows in Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="b7776-105">Workflows in Dynamics 365 Business Central</span></span>

<span data-ttu-id="b7776-106">You can set up and use workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="b7776-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="b7776-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="b7776-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="b7776-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="b7776-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="b7776-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="b7776-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="b7776-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="b7776-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="b7776-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="b7776-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="b7776-112">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span><span class="sxs-lookup"><span data-stu-id="b7776-112">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="b7776-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="b7776-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="b7776-114">For more information, see the list of workflow templates in the Workflow Templates page.</span><span class="sxs-lookup"><span data-stu-id="b7776-114">For more information, see the list of workflow templates in the Workflow Templates page.</span></span>  

 <span data-ttu-id="b7776-115">If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customise the application code.</span><span class="sxs-lookup"><span data-stu-id="b7776-115">If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customize the application code.</span></span> <span data-ttu-id="b7776-116">For more information, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="b7776-116">For more information, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>

<span data-ttu-id="b7776-117">Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b7776-117">Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b7776-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="b7776-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>  

 <span data-ttu-id="b7776-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="b7776-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="b7776-120">**To**</span><span class="sxs-lookup"><span data-stu-id="b7776-120">**To**</span></span>|<span data-ttu-id="b7776-121">**See**</span><span class="sxs-lookup"><span data-stu-id="b7776-121">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b7776-122">Set up workflow users, specify how users get notified, and create new workflows.</span><span class="sxs-lookup"><span data-stu-id="b7776-122">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="b7776-123">For new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="b7776-123">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="b7776-124">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="b7776-124">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="b7776-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span><span class="sxs-lookup"><span data-stu-id="b7776-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="b7776-126">Archive and delete workflows.</span><span class="sxs-lookup"><span data-stu-id="b7776-126">Archive and delete workflows.</span></span>|[<span data-ttu-id="b7776-127">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="b7776-127">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="b7776-128">See Also</span><span class="sxs-lookup"><span data-stu-id="b7776-128">See Also</span></span>

[<span data-ttu-id="b7776-129">Sales</span><span class="sxs-lookup"><span data-stu-id="b7776-129">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="b7776-130">Purchasing</span><span class="sxs-lookup"><span data-stu-id="b7776-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="b7776-131">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="b7776-131">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="b7776-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b7776-132">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]