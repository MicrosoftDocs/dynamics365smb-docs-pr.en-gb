---
title: How to Pick for Internal Operations in Advanced Warehouse Configurations | Microsoft Docs
description: In advanced warehouse configurations where the location is set up to use picking as well as shipping, you can pick components for production and assembly activities with the **Warehouse Pick** page.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 7e4a489b49c5a97cd0df077544a51c6ba73a4a85
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="pick-for-assembly-or-production-in-advanced-warehouse-configurations"></a><span data-ttu-id="2fa10-103">Pick for Assembly or Production in Advanced Warehouse Configurations</span><span class="sxs-lookup"><span data-stu-id="2fa10-103">Pick for Assembly or Production in Advanced Warehouse Configurations</span></span>
<span data-ttu-id="2fa10-104">In advanced warehouse configurations where the location is set up to use picking as well as shipping, you can pick components for production and assembly activities with the **Warehouse Pick** page.</span><span class="sxs-lookup"><span data-stu-id="2fa10-104">In advanced warehouse configurations where the location is set up to use picking as well as shipping, you can pick components for production and assembly activities with the **Warehouse Pick** page.</span></span>  

<span data-ttu-id="2fa10-105">Alternatively, you can use the **Movement Worksheet** page to move items between bins ad hoc, meaning without reference to a source document.</span><span class="sxs-lookup"><span data-stu-id="2fa10-105">Alternatively, you can use the **Movement Worksheet** page to move items between bins ad hoc, meaning without reference to a source document.</span></span> <span data-ttu-id="2fa10-106">For more information, see [Move Items in advanced warehouse configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="2fa10-106">For more information, see [Move Items in advanced warehouse configurations](warehouse-how-to-move-items-in-advanced-warehousing.md).</span></span>  

<span data-ttu-id="2fa10-107">For information about picking items for internal operations in basic warehouse locations that are set up for picking only, see [Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span><span class="sxs-lookup"><span data-stu-id="2fa10-107">For information about picking items for internal operations in basic warehouse locations that are set up for picking only, see [Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md).</span></span>  

<span data-ttu-id="2fa10-108">You cannot create a warehouse pick document from scratch because a pick activity is always part of a workflow, either in a pull or a push scenario.</span><span class="sxs-lookup"><span data-stu-id="2fa10-108">You cannot create a warehouse pick document from scratch because a pick activity is always part of a workflow, either in a pull or a push scenario.</span></span>  

<span data-ttu-id="2fa10-109">You can create the warehouse pick document in a push fashion by selecting **Create Whse. Pick** on the source document, such as a released assembly order or warehouse shipment.</span><span class="sxs-lookup"><span data-stu-id="2fa10-109">You can create the warehouse pick document in a push fashion by selecting **Create Whse. Pick** on the source document, such as a released assembly order or warehouse shipment.</span></span> <span data-ttu-id="2fa10-110">For more information, see [Pick Items with Warehouse Picks](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span><span class="sxs-lookup"><span data-stu-id="2fa10-110">For more information, see [Pick Items with Warehouse Picks](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span></span>  

<span data-ttu-id="2fa10-111">Alternatively, you can create the warehouse pick document in a pull fashion by using the **Pick Worksheet** page to detect pick requests, both for shipment and internal operations, and then create the required warehouse pick documents.</span><span class="sxs-lookup"><span data-stu-id="2fa10-111">Alternatively, you can create the warehouse pick document in a pull fashion by using the **Pick Worksheet** page to detect pick requests, both for shipment and internal operations, and then create the required warehouse pick documents.</span></span>  

<span data-ttu-id="2fa10-112">The following procedure explains a pull scenario where you pick components for a released production order through the **Pick Worksheet** page.</span><span class="sxs-lookup"><span data-stu-id="2fa10-112">The following procedure explains a pull scenario where you pick components for a released production order through the **Pick Worksheet** page.</span></span> <span data-ttu-id="2fa10-113">The procedure also applies for an assembly order.</span><span class="sxs-lookup"><span data-stu-id="2fa10-113">The procedure also applies for an assembly order.</span></span>  

<span data-ttu-id="2fa10-114">To create pick requests, both for pull and for push scenarios, the source documents in question must be released.</span><span class="sxs-lookup"><span data-stu-id="2fa10-114">To create pick requests, both for pull and for push scenarios, the source documents in question must be released.</span></span> <span data-ttu-id="2fa10-115">Release source documents for internal operations in the following ways.</span><span class="sxs-lookup"><span data-stu-id="2fa10-115">Release source documents for internal operations in the following ways.</span></span>  

|<span data-ttu-id="2fa10-116">Source Document</span><span class="sxs-lookup"><span data-stu-id="2fa10-116">Source Document</span></span>|<span data-ttu-id="2fa10-117">Release Method</span><span class="sxs-lookup"><span data-stu-id="2fa10-117">Release Method</span></span>|  
|---------------------|--------------------|  
|<span data-ttu-id="2fa10-118">Production Order</span><span class="sxs-lookup"><span data-stu-id="2fa10-118">Production Order</span></span>|<span data-ttu-id="2fa10-119">Change order type to released production order.</span><span class="sxs-lookup"><span data-stu-id="2fa10-119">Change order type to released production order.</span></span>|  
|<span data-ttu-id="2fa10-120">Assembly Order</span><span class="sxs-lookup"><span data-stu-id="2fa10-120">Assembly Order</span></span>|<span data-ttu-id="2fa10-121">Change status to Released.</span><span class="sxs-lookup"><span data-stu-id="2fa10-121">Change status to Released.</span></span>|  

## <a name="to-pick-components-using-the-pick-worksheet"></a><span data-ttu-id="2fa10-122">To pick components using the pick worksheet</span><span class="sxs-lookup"><span data-stu-id="2fa10-122">To pick components using the pick worksheet</span></span>  
1.  <span data-ttu-id="2fa10-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Pick Worksheet**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2fa10-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Pick Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2fa10-124">Choose the **Get Warehouse Documents** action, and then select the component lines from the released production order.</span><span class="sxs-lookup"><span data-stu-id="2fa10-124">Choose the **Get Warehouse Documents** action, and then select the component lines from the released production order.</span></span>  
3.  <span data-ttu-id="2fa10-125">Inspect the lines, sort them to ensure an efficient picking round, and combine them with other worksheet lines if necessary to make best use of employee time.</span><span class="sxs-lookup"><span data-stu-id="2fa10-125">Inspect the lines, sort them to ensure an efficient picking round, and combine them with other worksheet lines if necessary to make best use of employee time.</span></span>  
4.  <span data-ttu-id="2fa10-126">Choose the **Create Pick** action.</span><span class="sxs-lookup"><span data-stu-id="2fa10-126">Choose the **Create Pick** action.</span></span>  
5.  <span data-ttu-id="2fa10-127">Define how to create the warehouse pick documents and how to sort pick lines by filling fields on the **Create Pick** page.</span><span class="sxs-lookup"><span data-stu-id="2fa10-127">Define how to create the warehouse pick documents and how to sort pick lines by filling fields on the **Create Pick** page.</span></span>  
6.  <span data-ttu-id="2fa10-128">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="2fa10-128">Choose the **OK** button.</span></span> <span data-ttu-id="2fa10-129">Warehouse pick documents are created with pick lines for each component that is required in the internal operation.</span><span class="sxs-lookup"><span data-stu-id="2fa10-129">Warehouse pick documents are created with pick lines for each component that is required in the internal operation.</span></span>  

<span data-ttu-id="2fa10-130">If the internal operation area, such as a production shop floor, is set up with a default bin for placement of components to be used in the operation, then that bin code is inserted in the Place lines on the warehouse pick document to instruct warehouse workers where to place the items.</span><span class="sxs-lookup"><span data-stu-id="2fa10-130">If the internal operation area, such as a production shop floor, is set up with a default bin for placement of components to be used in the operation, then that bin code is inserted in the Place lines on the warehouse pick document to instruct warehouse workers where to place the items.</span></span> <span data-ttu-id="2fa10-131">For more information, see the **To-Production Bin Code** or the **To-Assembly Bin Code** field.</span><span class="sxs-lookup"><span data-stu-id="2fa10-131">For more information, see the **To-Production Bin Code** or the **To-Assembly Bin Code** field.</span></span>

## <a name="filling-the-consumption-bin"></a><span data-ttu-id="2fa10-132">Filling the Consumption Bin</span><span class="sxs-lookup"><span data-stu-id="2fa10-132">Filling the Consumption Bin</span></span>
<span data-ttu-id="2fa10-133">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span><span class="sxs-lookup"><span data-stu-id="2fa10-133">This flow chart shows how the **Bin Code** field on production order component lines is filled according to your location setup.</span></span>

<span data-ttu-id="2fa10-134">![Bin flow chart](media/binflow.png "BinFlow")</span><span class="sxs-lookup"><span data-stu-id="2fa10-134">![Bin flow chart](media/binflow.png "BinFlow")</span></span>  

## <a name="see-also"></a><span data-ttu-id="2fa10-135">See Also</span><span class="sxs-lookup"><span data-stu-id="2fa10-135">See Also</span></span>
[<span data-ttu-id="2fa10-136">Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="2fa10-136">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="2fa10-137">Inventory</span><span class="sxs-lookup"><span data-stu-id="2fa10-137">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="2fa10-138">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="2fa10-138">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="2fa10-139">[Assembly Management](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="2fa10-139">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="2fa10-140">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="2fa10-140">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="2fa10-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2fa10-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

