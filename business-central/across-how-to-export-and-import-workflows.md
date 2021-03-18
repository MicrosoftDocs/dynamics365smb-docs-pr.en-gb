---
title: How to Export and Import Workflows | Microsoft Docs
description: To transfer workflows to other Business Central databases, for example to save time when creating new workflows, you can export and import workflows.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 6f47b137a2915f790b510c0fd66944a4fe7814ca
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5384431"
---
# <a name="export-and-import-workflows"></a><span data-ttu-id="a6fa3-103">Export and Import Workflows</span><span class="sxs-lookup"><span data-stu-id="a6fa3-103">Export and Import Workflows</span></span>
<span data-ttu-id="a6fa3-104">To transfer workflows to other [!INCLUDE[prod_short](includes/prod_short.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-104">To transfer workflows to other [!INCLUDE[prod_short](includes/prod_short.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="a6fa3-105">Another way to quickly create workflows is to create workflows from workflow templates.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="a6fa3-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="a6fa3-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="a6fa3-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="a6fa3-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="a6fa3-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="a6fa3-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="a6fa3-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="a6fa3-111">To export a workflow</span><span class="sxs-lookup"><span data-stu-id="a6fa3-111">To export a workflow</span></span>  
1.  <span data-ttu-id="a6fa3-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a6fa3-113">Select a workflow, and then choose the **Export to File** action.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="a6fa3-114">On the **Export File** page, choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-114">On the **Export File** page, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="a6fa3-115">On the **Export** page, select a file location, and then choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-115">On the **Export** page, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="a6fa3-116">To import a workflow</span><span class="sxs-lookup"><span data-stu-id="a6fa3-116">To import a workflow</span></span>  
1.  <span data-ttu-id="a6fa3-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a6fa3-118">Choose the **Import from File** action.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="a6fa3-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="a6fa3-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span><span class="sxs-lookup"><span data-stu-id="a6fa3-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a6fa3-121">See Also</span><span class="sxs-lookup"><span data-stu-id="a6fa3-121">See Also</span></span>  
 <span data-ttu-id="a6fa3-122">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-122">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="a6fa3-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="a6fa3-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="a6fa3-125">[Delete Workflows](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-125">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="a6fa3-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="a6fa3-127">[Setting Up Workflows](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="a6fa3-128">[Using Workflows](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="a6fa3-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="a6fa3-129">Workflow</span><span class="sxs-lookup"><span data-stu-id="a6fa3-129">Workflow</span></span>](across-workflow.md)   


[!INCLUDE[footer-include](includes/footer-banner.md)]