---
title: How to Create Workflows from Workflow Templates | Microsoft Docs
description: To save time when creating new workflows, you can create workflows from workflow templates.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 407bf7cd60416a178e9ec8a5d0b154a7583e87e1
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754849"
---
# <a name="create-workflows-from-workflow-templates"></a><span data-ttu-id="80ec4-103">Create Workflows from Workflow Templates</span><span class="sxs-lookup"><span data-stu-id="80ec4-103">Create Workflows from Workflow Templates</span></span>
<span data-ttu-id="80ec4-104">To save time when creating new workflows, you can create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="80ec4-104">To save time when creating new workflows, you can create workflows from workflow templates.</span></span>  

 <span data-ttu-id="80ec4-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="80ec4-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="80ec4-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span><span class="sxs-lookup"><span data-stu-id="80ec4-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span>  

 <span data-ttu-id="80ec4-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="80ec4-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="80ec4-108">For more information, see [Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="80ec4-108">For more information, see [Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span></span>  

<span data-ttu-id="80ec4-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="80ec4-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="80ec4-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="80ec4-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="80ec4-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="80ec4-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="80ec4-112">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="80ec4-112">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-create-a-workflow-from-workflow-template"></a><span data-ttu-id="80ec4-113">To create a workflow from workflow template</span><span class="sxs-lookup"><span data-stu-id="80ec4-113">To create a workflow from workflow template</span></span>  
1.  <span data-ttu-id="80ec4-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="80ec4-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="80ec4-115">Choose the **Create Workflow from Template** action.</span><span class="sxs-lookup"><span data-stu-id="80ec4-115">Choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="80ec4-116">The **Workflow Templates** page opens.</span><span class="sxs-lookup"><span data-stu-id="80ec4-116">The **Workflow Templates** page opens.</span></span>  
3.  <span data-ttu-id="80ec4-117">Select a workflow template, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="80ec4-117">Select a workflow template, and then choose the **OK** button.</span></span>  

     <span data-ttu-id="80ec4-118">The **Workflow** page opens for a new workflow containing all the information of the selected template.</span><span class="sxs-lookup"><span data-stu-id="80ec4-118">The **Workflow** page opens for a new workflow containing all the information of the selected template.</span></span> <span data-ttu-id="80ec4-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span><span class="sxs-lookup"><span data-stu-id="80ec4-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span></span>  
4.  <span data-ttu-id="80ec4-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span><span class="sxs-lookup"><span data-stu-id="80ec4-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span></span> <span data-ttu-id="80ec4-121">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="80ec4-121">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="80ec4-122">See Also</span><span class="sxs-lookup"><span data-stu-id="80ec4-122">See Also</span></span>  
 <span data-ttu-id="80ec4-123">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-123">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="80ec4-124">[Export and Import Workflows](across-how-to-export-and-import-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-124">[Export and Import Workflows](across-how-to-export-and-import-workflows.md) </span></span>  
 <span data-ttu-id="80ec4-125">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-125">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="80ec4-126">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-126">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="80ec4-127">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-127">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="80ec4-128">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-128">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="80ec4-129">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="80ec4-129">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="80ec4-130">Workflow</span><span class="sxs-lookup"><span data-stu-id="80ec4-130">Workflow</span></span>](across-workflow.md)   
