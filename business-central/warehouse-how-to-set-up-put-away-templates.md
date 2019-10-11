---
title: How to Set Up Put-away Templates | Microsoft Docs
description: With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 9d984ff5646fd467bf5c30ee3bebf4c377e38365
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2310139"
---
# <a name="set-up-put-away-templates"></a><span data-ttu-id="7bbb7-103">Set Up Put-away Templates</span><span class="sxs-lookup"><span data-stu-id="7bbb7-103">Set Up Put-away Templates</span></span>
<span data-ttu-id="7bbb7-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="7bbb7-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="7bbb7-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="7bbb7-107">To set up put-away templates</span><span class="sxs-lookup"><span data-stu-id="7bbb7-107">To set up put-away templates</span></span>  
1.  <span data-ttu-id="7bbb7-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7bbb7-109">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-109">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="7bbb7-110">Enter a code that is the unique identifier of the template you are about to create.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4.  <span data-ttu-id="7bbb7-111">Enter a short description, if you wish.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-111">Enter a short description, if you wish.</span></span>  
5.  <span data-ttu-id="7bbb7-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>  
6.  <span data-ttu-id="7bbb7-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="7bbb7-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7.  <span data-ttu-id="7bbb7-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8.  <span data-ttu-id="7bbb7-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="7bbb7-117">You can create various put-away templates and then apply them as you see fit.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-117">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="7bbb7-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="7bbb7-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span><span class="sxs-lookup"><span data-stu-id="7bbb7-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7bbb7-120">See Also</span><span class="sxs-lookup"><span data-stu-id="7bbb7-120">See Also</span></span>  
[<span data-ttu-id="7bbb7-121">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="7bbb7-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="7bbb7-122">Inventory</span><span class="sxs-lookup"><span data-stu-id="7bbb7-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="7bbb7-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="7bbb7-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="7bbb7-124">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="7bbb7-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="7bbb7-125">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="7bbb7-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="7bbb7-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7bbb7-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
