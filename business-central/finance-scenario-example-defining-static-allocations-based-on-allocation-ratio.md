---
title: Defining Static Allocations Based on Allocation Ratio | Microsoft Docs
description: Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: finance-define-and-allocate-costs
ms.openlocfilehash: bd17923913355f883d14beb24136e97a839116e3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1243395"
---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a><span data-ttu-id="7180b-103">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span><span class="sxs-lookup"><span data-stu-id="7180b-103">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>
<span data-ttu-id="7180b-104">Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="7180b-104">Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.</span></span>  

<span data-ttu-id="7180b-105">This topic describes how to define three new allocation target cost objects for the allocation source PROD cost centre using the established allocation ratio 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="7180b-105">This topic describes how to define three new allocation target cost objects for the allocation source PROD cost center using the established allocation ratio 5:2:4.</span></span> <span data-ttu-id="7180b-106">The three target cost objects are ACCESSO, PAINT, and FITTINGS.</span><span class="sxs-lookup"><span data-stu-id="7180b-106">The three target cost objects are ACCESSO, PAINT, and FITTINGS.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="7180b-107">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7180b-107">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a><span data-ttu-id="7180b-108">To define the allocation source PROD cost centre on the General FastTab</span><span class="sxs-lookup"><span data-stu-id="7180b-108">To define the allocation source PROD cost center on the General FastTab</span></span>  

1.  <span data-ttu-id="7180b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocation**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7180b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Allocation**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7180b-110">On the **Cost Allocation** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="7180b-110">On the **Cost Allocation** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="7180b-111">In the **ID** field, press Enter or enter an ID.</span><span class="sxs-lookup"><span data-stu-id="7180b-111">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="7180b-112">In the **Level** field, enter **1**.</span><span class="sxs-lookup"><span data-stu-id="7180b-112">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="7180b-113">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span><span class="sxs-lookup"><span data-stu-id="7180b-113">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="7180b-114">In the **Cost Center Code** field, enter **PROD**.</span><span class="sxs-lookup"><span data-stu-id="7180b-114">In the **Cost Center Code** field, enter **PROD**.</span></span>  
7.  <span data-ttu-id="7180b-115">In the **Credit to Cost Type** field, enter the cost type **9903**.</span><span class="sxs-lookup"><span data-stu-id="7180b-115">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a><span data-ttu-id="7180b-116">To define the allocation target cost objects on the Lines FastTab</span><span class="sxs-lookup"><span data-stu-id="7180b-116">To define the allocation target cost objects on the Lines FastTab</span></span>  

1.  <span data-ttu-id="7180b-117">On the first line, in the **Target Cost Type** field, enter **9903**.</span><span class="sxs-lookup"><span data-stu-id="7180b-117">On the first line, in the **Target Cost Type** field, enter **9903**.</span></span>  
2.  <span data-ttu-id="7180b-118">On the first line, in the **Target Cost Object** field, select **ACCESSO**.</span><span class="sxs-lookup"><span data-stu-id="7180b-118">On the first line, in the **Target Cost Object** field, select **ACCESSO**.</span></span>  
3.  <span data-ttu-id="7180b-119">On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="7180b-119">On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
4.  <span data-ttu-id="7180b-120">On the first line, in the **Base** field, select **Static** to use the static allocation method.</span><span class="sxs-lookup"><span data-stu-id="7180b-120">On the first line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
5.  <span data-ttu-id="7180b-121">On the first line, in the **Share** field, enter the allocation ratio **5**.</span><span class="sxs-lookup"><span data-stu-id="7180b-121">On the first line, in the **Share** field, enter the allocation ratio **5**.</span></span>  
6.  <span data-ttu-id="7180b-122">On the second line, in the **Target Cost Type** field, enter **9903**.</span><span class="sxs-lookup"><span data-stu-id="7180b-122">On the second line, in the **Target Cost Type** field, enter **9903**.</span></span>  
7.  <span data-ttu-id="7180b-123">On the second line, in the **Target Cost Object** field, select **PAINT**.</span><span class="sxs-lookup"><span data-stu-id="7180b-123">On the second line, in the **Target Cost Object** field, select **PAINT**.</span></span>  
8.  <span data-ttu-id="7180b-124">On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="7180b-124">On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
9. <span data-ttu-id="7180b-125">On the second line, in the **Base** field, select **Static** to use the static allocation method.</span><span class="sxs-lookup"><span data-stu-id="7180b-125">On the second line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
10. <span data-ttu-id="7180b-126">On the second line, in the **Share** field, enter the allocation ratio **2**.</span><span class="sxs-lookup"><span data-stu-id="7180b-126">On the second line, in the **Share** field, enter the allocation ratio **2**.</span></span>  
11. <span data-ttu-id="7180b-127">On the third line, in the **Target Cost Type** field, enter **9903**.</span><span class="sxs-lookup"><span data-stu-id="7180b-127">On the third line, in the **Target Cost Type** field, enter **9903**.</span></span>  
12. <span data-ttu-id="7180b-128">On the third line, in the **Target Cost Object** field, select **FITTINGS**.</span><span class="sxs-lookup"><span data-stu-id="7180b-128">On the third line, in the **Target Cost Object** field, select **FITTINGS**.</span></span>  
13. <span data-ttu-id="7180b-129">On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span><span class="sxs-lookup"><span data-stu-id="7180b-129">On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
14. <span data-ttu-id="7180b-130">On the third line, in the **Base** field, select **Static** to use the static allocation method.</span><span class="sxs-lookup"><span data-stu-id="7180b-130">On the third line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
15. <span data-ttu-id="7180b-131">On the third line, in the **Share** field, enter the allocation ratio **4**.</span><span class="sxs-lookup"><span data-stu-id="7180b-131">On the third line, in the **Share** field, enter the allocation ratio **4**.</span></span>  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="7180b-132">automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.</span><span class="sxs-lookup"><span data-stu-id="7180b-132">automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7180b-133">See Also</span><span class="sxs-lookup"><span data-stu-id="7180b-133">See Also</span></span>  
[<span data-ttu-id="7180b-134">Defining and Allocating Costs</span><span class="sxs-lookup"><span data-stu-id="7180b-134">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)   
