---
title: How to Set Up Put-away Templates | Microsoft Docs
description: With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 6b6064bbad133ca521e5cb44667b9ead1368c1e0
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382352"
---
# <a name="set-up-put-away-templates"></a><span data-ttu-id="906e4-103">Set Up Put-away Templates</span><span class="sxs-lookup"><span data-stu-id="906e4-103">Set Up Put-away Templates</span></span>

<span data-ttu-id="906e4-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span><span class="sxs-lookup"><span data-stu-id="906e4-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="906e4-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span><span class="sxs-lookup"><span data-stu-id="906e4-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="906e4-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span><span class="sxs-lookup"><span data-stu-id="906e4-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="906e4-107">To set up put-away templates</span><span class="sxs-lookup"><span data-stu-id="906e4-107">To set up put-away templates</span></span>

1. <span data-ttu-id="906e4-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="906e4-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="906e4-109">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="906e4-109">Choose the **New** action.</span></span>  
3. <span data-ttu-id="906e4-110">Enter a code that is the unique identifier of the template you are about to create.</span><span class="sxs-lookup"><span data-stu-id="906e4-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4. <span data-ttu-id="906e4-111">Enter a short description, if you wish.</span><span class="sxs-lookup"><span data-stu-id="906e4-111">Enter a short description, if you wish.</span></span>  
5. <span data-ttu-id="906e4-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span><span class="sxs-lookup"><span data-stu-id="906e4-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>

    <span data-ttu-id="906e4-113">For example, if want the default put-away method to be based on fixed bins, then choose the **Find Fixed Bin** field.</span><span class="sxs-lookup"><span data-stu-id="906e4-113">For example, if want the default put-away method to be based on fixed bins, then choose the **Find Fixed Bin** field.</span></span> [!INCLUDE[tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="906e4-114">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span><span class="sxs-lookup"><span data-stu-id="906e4-114">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="906e4-115">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span><span class="sxs-lookup"><span data-stu-id="906e4-115">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7. <span data-ttu-id="906e4-116">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span><span class="sxs-lookup"><span data-stu-id="906e4-116">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8. <span data-ttu-id="906e4-117">On the last line in the put-away template, select the **Find Floating Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="906e4-117">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="906e4-118">You can create various put-away templates and then apply them as you see fit.</span><span class="sxs-lookup"><span data-stu-id="906e4-118">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="906e4-119">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span><span class="sxs-lookup"><span data-stu-id="906e4-119">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="906e4-120">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span><span class="sxs-lookup"><span data-stu-id="906e4-120">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="906e4-121">See Also</span><span class="sxs-lookup"><span data-stu-id="906e4-121">See Also</span></span>

[<span data-ttu-id="906e4-122">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="906e4-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="906e4-123">Inventory</span><span class="sxs-lookup"><span data-stu-id="906e4-123">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="906e4-124">Setting Up Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="906e4-124">Setting Up Warehouse Management</span></span>](warehouse-setup-warehouse.md)  
[<span data-ttu-id="906e4-125">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="906e4-125">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="906e4-126">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="906e4-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="906e4-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="906e4-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]