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
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 2d309940d177491ce24f49884f388a5c233147fa
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3188283"
---
# <a name="export-and-import-workflows"></a><span data-ttu-id="fad89-103">Export and Import Workflows</span><span class="sxs-lookup"><span data-stu-id="fad89-103">Export and Import Workflows</span></span>
<span data-ttu-id="fad89-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span><span class="sxs-lookup"><span data-stu-id="fad89-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="fad89-105">Another way to quickly create workflows is to create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="fad89-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="fad89-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="fad89-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="fad89-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="fad89-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="fad89-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="fad89-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="fad89-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="fad89-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="fad89-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="fad89-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="fad89-111">To export a workflow</span><span class="sxs-lookup"><span data-stu-id="fad89-111">To export a workflow</span></span>  
1.  <span data-ttu-id="fad89-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fad89-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fad89-113">Select a workflow, and then choose the **Export to File** action.</span><span class="sxs-lookup"><span data-stu-id="fad89-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="fad89-114">On the **Export File** page, choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="fad89-114">On the **Export File** page, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="fad89-115">On the **Export** page, select a file location, and then choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="fad89-115">On the **Export** page, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="fad89-116">To import a workflow</span><span class="sxs-lookup"><span data-stu-id="fad89-116">To import a workflow</span></span>  
1.  <span data-ttu-id="fad89-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fad89-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fad89-118">Choose the **Import from File** action.</span><span class="sxs-lookup"><span data-stu-id="fad89-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="fad89-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="fad89-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="fad89-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span><span class="sxs-lookup"><span data-stu-id="fad89-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fad89-121">See Also</span><span class="sxs-lookup"><span data-stu-id="fad89-121">See Also</span></span>  
 <span data-ttu-id="fad89-122">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-122">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="fad89-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="fad89-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="fad89-125">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-125">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="fad89-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="fad89-127">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="fad89-128">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="fad89-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="fad89-129">Workflow</span><span class="sxs-lookup"><span data-stu-id="fad89-129">Workflow</span></span>](across-workflow.md)   
