---
title: Workflow | Microsoft Docs
description: You can set up and use workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/22/2020
ms.author: edupont
ms.openlocfilehash: 3336eeeb0a3560670fa2b1fb99fb64bac20d15be
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/09/2020
ms.locfileid: "3785703"
---
# <a name="workflows-in-dynamics-365-business-central"></a><span data-ttu-id="126ee-105">Workflows in Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="126ee-105">Workflows in Dynamics 365 Business Central</span></span>

<span data-ttu-id="126ee-106">You can set up and use workflows that connect business-process tasks performed by different users.</span><span class="sxs-lookup"><span data-stu-id="126ee-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="126ee-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span><span class="sxs-lookup"><span data-stu-id="126ee-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="126ee-108">Requesting and granting approval to create new records are typical workflow steps.</span><span class="sxs-lookup"><span data-stu-id="126ee-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="126ee-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="126ee-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="126ee-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="126ee-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="126ee-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="126ee-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="126ee-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span><span class="sxs-lookup"><span data-stu-id="126ee-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="126ee-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="126ee-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="126ee-114">For more information, see the list of workflow templates in the Workflow Templates page.</span><span class="sxs-lookup"><span data-stu-id="126ee-114">For more information, see the list of workflow templates in the Workflow Templates page.</span></span>  

 <span data-ttu-id="126ee-115">If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customise the application code.</span><span class="sxs-lookup"><span data-stu-id="126ee-115">If a business scenario requires a workflow event or response that is not supported, you can either use Power Automate or work with a Microsoft partner to customize the application code.</span></span> <span data-ttu-id="126ee-116">For more information, see [Using [!INCLUDE[prodshort](includes/prodshort.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="126ee-116">For more information, see [Using [!INCLUDE[prodshort](includes/prodshort.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>

<span data-ttu-id="126ee-117">Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="126ee-117">Any workflow template that you create with Power Automate is added to the list of workflow templates within [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="126ee-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="126ee-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>  

 <span data-ttu-id="126ee-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="126ee-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="126ee-120">**To**</span><span class="sxs-lookup"><span data-stu-id="126ee-120">**To**</span></span>|<span data-ttu-id="126ee-121">**See**</span><span class="sxs-lookup"><span data-stu-id="126ee-121">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="126ee-122">Set up workflow users, specify how users get notified, and create new workflows.</span><span class="sxs-lookup"><span data-stu-id="126ee-122">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="126ee-123">For new workflows for unsupported scenarios, implement the required workflow elements by customising the application code.</span><span class="sxs-lookup"><span data-stu-id="126ee-123">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="126ee-124">Setting Up Workflows</span><span class="sxs-lookup"><span data-stu-id="126ee-124">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="126ee-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span><span class="sxs-lookup"><span data-stu-id="126ee-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="126ee-126">Archive and delete workflows.</span><span class="sxs-lookup"><span data-stu-id="126ee-126">Archive and delete workflows.</span></span>|[<span data-ttu-id="126ee-127">Using Workflows</span><span class="sxs-lookup"><span data-stu-id="126ee-127">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="126ee-128">See Also</span><span class="sxs-lookup"><span data-stu-id="126ee-128">See Also</span></span>

[<span data-ttu-id="126ee-129">Sales</span><span class="sxs-lookup"><span data-stu-id="126ee-129">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="126ee-130">Purchasing</span><span class="sxs-lookup"><span data-stu-id="126ee-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="126ee-131">Managing Projects</span><span class="sxs-lookup"><span data-stu-id="126ee-131">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="126ee-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="126ee-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
