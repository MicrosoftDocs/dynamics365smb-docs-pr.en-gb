---
title: How to Export and Import Workflows | Microsoft Docs
description: To transfer workflows to other Business Central databases, for example to save time when creating new workflows, you can export and import workflows.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 4d11bc57066c0124bcb004894ed6b2c9dc4b812e
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754774"
---
# <a name="export-and-import-workflows"></a><span data-ttu-id="05215-103">Export and Import Workflows</span><span class="sxs-lookup"><span data-stu-id="05215-103">Export and Import Workflows</span></span>
<span data-ttu-id="05215-104">To transfer workflows to other [!INCLUDE[prod_short](includes/prod_short.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span><span class="sxs-lookup"><span data-stu-id="05215-104">To transfer workflows to other [!INCLUDE[prod_short](includes/prod_short.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="05215-105">Another way to quickly create workflows is to create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="05215-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="05215-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="05215-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="05215-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="05215-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="05215-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="05215-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="05215-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="05215-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="05215-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="05215-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="05215-111">To export a workflow</span><span class="sxs-lookup"><span data-stu-id="05215-111">To export a workflow</span></span>  
1.  <span data-ttu-id="05215-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="05215-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="05215-113">Select a workflow, and then choose the **Export to File** action.</span><span class="sxs-lookup"><span data-stu-id="05215-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="05215-114">On the **Export File** page, choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="05215-114">On the **Export File** page, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="05215-115">On the **Export** page, select a file location, and then choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="05215-115">On the **Export** page, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="05215-116">To import a workflow</span><span class="sxs-lookup"><span data-stu-id="05215-116">To import a workflow</span></span>  
1.  <span data-ttu-id="05215-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="05215-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="05215-118">Choose the **Import from File** action.</span><span class="sxs-lookup"><span data-stu-id="05215-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="05215-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="05215-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="05215-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span><span class="sxs-lookup"><span data-stu-id="05215-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="05215-121">See Also</span><span class="sxs-lookup"><span data-stu-id="05215-121">See Also</span></span>  
 <span data-ttu-id="05215-122">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="05215-122">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="05215-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="05215-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="05215-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="05215-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="05215-125">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="05215-125">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="05215-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="05215-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="05215-127">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="05215-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="05215-128">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="05215-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="05215-129">Workflow</span><span class="sxs-lookup"><span data-stu-id="05215-129">Workflow</span></span>](across-workflow.md)   
