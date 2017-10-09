---
title: How to Use Item Families in Manufacturing | Microsoft Docs
description: The main task in customizing a base calendar for your company, or one of its business partners, is to enter any changes to working and nonworking day status.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/05/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 060c58991ae48ba768f5c1c0bd7442228e6bc976
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-production-families"></a><span data-ttu-id="49156-103">How to: Work with Production Families</span><span class="sxs-lookup"><span data-stu-id="49156-103">How to: Work with Production Families</span></span>
<span data-ttu-id="49156-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span><span class="sxs-lookup"><span data-stu-id="49156-104">A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes.</span></span> <span data-ttu-id="49156-105">By forming production families, some items can be manufactured twice or more in one production, which will optimise material consumption.</span><span class="sxs-lookup"><span data-stu-id="49156-105">By forming production families, some items can be manufactured twice or more in one production, which will optimize material consumption.</span></span>

<span data-ttu-id="49156-106">In the **Quantity** field in the **Family** window, you enter the quantity that will be produced when the whole family has been manufactured once.</span><span class="sxs-lookup"><span data-stu-id="49156-106">In the **Quantity** field in the **Family** window, you enter the quantity that will be produced when the whole family has been manufactured once.</span></span>

## <a name="example"></a><span data-ttu-id="49156-107">Example</span><span class="sxs-lookup"><span data-stu-id="49156-107">Example</span></span>
<span data-ttu-id="49156-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span><span class="sxs-lookup"><span data-stu-id="49156-108">In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time.</span></span> <span data-ttu-id="49156-109">The punching machine will punch all 14 pieces in one step.</span><span class="sxs-lookup"><span data-stu-id="49156-109">The punching machine will punch all 14 pieces in one step.</span></span>

<span data-ttu-id="49156-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span><span class="sxs-lookup"><span data-stu-id="49156-110">Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.</span></span>

## <a name="to-set-up-a-production-family"></a><span data-ttu-id="49156-111">To set up a production family</span><span class="sxs-lookup"><span data-stu-id="49156-111">To set up a production family</span></span>
1. <span data-ttu-id="49156-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Families**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49156-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Families**, and then choose the related link.</span></span>
2. <span data-ttu-id="49156-113">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="49156-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-familily"></a><span data-ttu-id="49156-114">To produce based on a production familily</span><span class="sxs-lookup"><span data-stu-id="49156-114">To produce based on a production familily</span></span>
1. <span data-ttu-id="49156-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="49156-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="49156-116">Create a new production order.</span><span class="sxs-lookup"><span data-stu-id="49156-116">Create a new production order.</span></span> <span data-ttu-id="49156-117">For more information, see [How to: Create Production orders](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="49156-117">For more information, see [How to: Create Production orders](production-how-to-create-production-orders.md).</span></span>
3. <span data-ttu-id="49156-118">In the **Source Type** field, select **Family**.</span><span class="sxs-lookup"><span data-stu-id="49156-118">In the **Source Type** field, select **Family**.</span></span>  
4. <span data-ttu-id="49156-119">In the **Source No.** field, select the relevant production family.</span><span class="sxs-lookup"><span data-stu-id="49156-119">In the **Source No.** field, select the relevant production family.</span></span>

## <a name="see-also"></a><span data-ttu-id="49156-120">See Also</span><span class="sxs-lookup"><span data-stu-id="49156-120">See Also</span></span>
[<span data-ttu-id="49156-121">How to: Create Production BOMs</span><span class="sxs-lookup"><span data-stu-id="49156-121">How to: Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="49156-122">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="49156-122">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="49156-123">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="49156-123">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="49156-124">[Planning](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="49156-124">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="49156-125">Inventory</span><span class="sxs-lookup"><span data-stu-id="49156-125">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="49156-126">Purchasing</span><span class="sxs-lookup"><span data-stu-id="49156-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="49156-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="49156-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

