---
title: How to Restrict and Allow Usage of a Record | Microsoft Docs
description: If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: bbb22a00e878e8c4d75cb5fcdbcc27a28d9d22a4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783998"
---
# <a name="restrict-and-allow-usage-of-a-record"></a><span data-ttu-id="fb260-103">Restrict and Allow Usage of a Record</span><span class="sxs-lookup"><span data-stu-id="fb260-103">Restrict and Allow Usage of a Record</span></span>
<span data-ttu-id="fb260-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span><span class="sxs-lookup"><span data-stu-id="fb260-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span></span> <span data-ttu-id="fb260-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span><span class="sxs-lookup"><span data-stu-id="fb260-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="fb260-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span><span class="sxs-lookup"><span data-stu-id="fb260-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="fb260-107">Two responses exist in the generic version of [!INCLUDE[prod_short](includes/prod_short.md)] for this purpose: **Restrict usage of a record.**</span><span class="sxs-lookup"><span data-stu-id="fb260-107">Two responses exist in the generic version of [!INCLUDE[prod_short](includes/prod_short.md)] for this purpose: **Restrict usage of a record.**</span></span> <span data-ttu-id="fb260-108">and **Allow usage of a record.**.</span><span class="sxs-lookup"><span data-stu-id="fb260-108">and **Allow usage of a record.**.</span></span>

> [!NOTE]  
>  <span data-ttu-id="fb260-109">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span><span class="sxs-lookup"><span data-stu-id="fb260-109">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span></span> <span data-ttu-id="fb260-110">To support other restrictions, a Microsoft partner must customise the application code.</span><span class="sxs-lookup"><span data-stu-id="fb260-110">To support other restrictions, a Microsoft partner must customize the application code.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fb260-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span><span class="sxs-lookup"><span data-stu-id="fb260-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span></span>

<span data-ttu-id="fb260-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span><span class="sxs-lookup"><span data-stu-id="fb260-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span></span> <span data-ttu-id="fb260-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span><span class="sxs-lookup"><span data-stu-id="fb260-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span></span>  

## <a name="to-create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a><span data-ttu-id="fb260-114">To create a workflow step that restricts posting of unapproved purchase orders</span><span class="sxs-lookup"><span data-stu-id="fb260-114">To create a workflow step that restricts posting of unapproved purchase orders</span></span>  
1. <span data-ttu-id="fb260-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="fb260-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb260-116">On the **Workflows** page, create a new workflow named Purchase Order Approval Workflow.</span><span class="sxs-lookup"><span data-stu-id="fb260-116">On the **Workflows** page, create a new workflow named Purchase Order Approval Workflow.</span></span> <span data-ttu-id="fb260-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="fb260-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  
3. <span data-ttu-id="fb260-118">Choose the **Copy From Workflow Template** action.</span><span class="sxs-lookup"><span data-stu-id="fb260-118">Choose the **Copy From Workflow Template** action.</span></span>  
4. <span data-ttu-id="fb260-119">Choose the **Source Workflow Code** field, and then, on the **Workflow Templates** page, choose the Purchase Invoice Approval Workflow workflow template.</span><span class="sxs-lookup"><span data-stu-id="fb260-119">Choose the **Source Workflow Code** field, and then, on the **Workflow Templates** page, choose the Purchase Invoice Approval Workflow workflow template.</span></span>  

     <span data-ttu-id="fb260-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span><span class="sxs-lookup"><span data-stu-id="fb260-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span></span> <span data-ttu-id="fb260-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span><span class="sxs-lookup"><span data-stu-id="fb260-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span></span>  
5. <span data-ttu-id="fb260-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span><span class="sxs-lookup"><span data-stu-id="fb260-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span></span>  
6. <span data-ttu-id="fb260-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span><span class="sxs-lookup"><span data-stu-id="fb260-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fb260-124">See Also</span><span class="sxs-lookup"><span data-stu-id="fb260-124">See Also</span></span>  
<span data-ttu-id="fb260-125">[Create Workflows](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="fb260-125">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
[<span data-ttu-id="fb260-126">Workflow</span><span class="sxs-lookup"><span data-stu-id="fb260-126">Workflow</span></span>](across-workflow.md)   


[!INCLUDE[footer-include](includes/footer-banner.md)]