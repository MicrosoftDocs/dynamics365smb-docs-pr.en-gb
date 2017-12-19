---
title: How to Export and Import Workflows | Microsoft Docs
description: To transfer workflows to other Dynamics 365 databases, for example to save time when creating new workflows, you can export and import workflows.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: aa56764b5f3210229ad21eae6891fb201462209c
ms.openlocfilehash: 520c81b9c550b4ef29b077685541a2e7ea30d4d7
ms.contentlocale: en-gb
ms.lasthandoff: 12/14/2017

---
# <a name="how-to-export-and-import-workflows"></a><span data-ttu-id="f0aa2-103">How to: Export and Import Workflows</span><span class="sxs-lookup"><span data-stu-id="f0aa2-103">How to: Export and Import Workflows</span></span>
<span data-ttu-id="f0aa2-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="f0aa2-105">Another way to quickly create workflows is to create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="f0aa2-106">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="f0aa2-106">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="f0aa2-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="f0aa2-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="f0aa2-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="f0aa2-110">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="f0aa2-110">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="f0aa2-111">To export a workflow</span><span class="sxs-lookup"><span data-stu-id="f0aa2-111">To export a workflow</span></span>  
1.  <span data-ttu-id="f0aa2-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f0aa2-113">Select a workflow, and then choose the **Export to File** action.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="f0aa2-114">In the **Export File** window, choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-114">In the **Export File** window, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="f0aa2-115">In the **Export** window, select a file location, and then choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-115">In the **Export** window, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="f0aa2-116">To import a workflow</span><span class="sxs-lookup"><span data-stu-id="f0aa2-116">To import a workflow</span></span>  
1.  <span data-ttu-id="f0aa2-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f0aa2-118">Choose the **Import from File** action.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="f0aa2-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="f0aa2-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span><span class="sxs-lookup"><span data-stu-id="f0aa2-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f0aa2-121">See Also</span><span class="sxs-lookup"><span data-stu-id="f0aa2-121">See Also</span></span>  
 <span data-ttu-id="f0aa2-122">[How to: Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-122">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="f0aa2-123">[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-123">[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="f0aa2-124">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-124">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="f0aa2-125">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-125">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="f0aa2-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="f0aa2-127">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="f0aa2-128">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="f0aa2-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="f0aa2-129">Workflow</span><span class="sxs-lookup"><span data-stu-id="f0aa2-129">Workflow</span></span>](across-workflow.md)   

