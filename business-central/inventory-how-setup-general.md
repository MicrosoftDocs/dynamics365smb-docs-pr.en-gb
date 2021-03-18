---
title: Define the General Inventory Setup
description: Describes how to define the general inventory setup so that you can manage your warehouse and stock.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 10344ae85edc8a63dcff1a5a5927bf2d19045810
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5389406"
---
# <a name="set-up-general-inventory-information"></a><span data-ttu-id="bdcab-103">Set Up General Inventory Information</span><span class="sxs-lookup"><span data-stu-id="bdcab-103">Set Up General Inventory Information</span></span>

<span data-ttu-id="bdcab-104">You specify your general inventory setup on the **Inventory Setup** page.</span><span class="sxs-lookup"><span data-stu-id="bdcab-104">You specify your general inventory setup on the **Inventory Setup** page.</span></span>

## <a name="to-set-up-general-inventory-information"></a><span data-ttu-id="bdcab-105">To set up general inventory information</span><span class="sxs-lookup"><span data-stu-id="bdcab-105">To set up general inventory information</span></span>

1. <span data-ttu-id="bdcab-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bdcab-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="bdcab-107">On the **Inventory Setup** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bdcab-107">On the **Inventory Setup** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="bdcab-108">For detailed information about the costing fields, **Automatic Cost Posting**, **Expected Cost Posting to G/L**, and **Default Costing Method**, see [Reconcile Inventory Costs with the General Ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md), [Design Details: Inventory Costing](design-details-inventory-costing.md), and [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md).</span><span class="sxs-lookup"><span data-stu-id="bdcab-108">For detailed information about the costing fields, **Automatic Cost Posting**, **Expected Cost Posting to G/L**, and **Default Costing Method**, see [Reconcile Inventory Costs with the General Ledger](finance-how-to-post-inventory-costs-to-the-general-ledger.md), [Design Details: Inventory Costing](design-details-inventory-costing.md), and [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md).</span></span> <span data-ttu-id="bdcab-109">For more information about costing in general, see [Managing Inventory Costs](finance-manage-inventory-costs.md).</span><span class="sxs-lookup"><span data-stu-id="bdcab-109">For more information about costing in general, see [Managing Inventory Costs](finance-manage-inventory-costs.md).</span></span>  

<span data-ttu-id="bdcab-110">If you want to include warehouse handling time in the order promising calculation on the purchase line, you can set it up as a default for the inventory, on the **Inventory Setup** page, and for your location.</span><span class="sxs-lookup"><span data-stu-id="bdcab-110">If you want to include warehouse handling time in the order promising calculation on the purchase line, you can set it up as a default for the inventory, on the **Inventory Setup** page, and for your location.</span></span> <span data-ttu-id="bdcab-111">For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span><span class="sxs-lookup"><span data-stu-id="bdcab-111">For more information, see [Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span></span>  

> [!NOTE]
> <span data-ttu-id="bdcab-112">The **Automatic Cost Adjustment** toggle is turned on by default to ensure that inventory values are always correct in the general ledger, which in turn keeps your sales and profit statistics up to date.</span><span class="sxs-lookup"><span data-stu-id="bdcab-112">The **Automatic Cost Adjustment** toggle is turned on by default to ensure that inventory values are always correct in the general ledger, which in turn keeps your sales and profit statistics up to date.</span></span> <span data-ttu-id="bdcab-113">Cost changes from inbound entries, such as those for purchases or production output, are assigned to the related outbound entries, such as sales or transfers.</span><span class="sxs-lookup"><span data-stu-id="bdcab-113">Cost changes from inbound entries, such as those for purchases or production output, are assigned to the related outbound entries, such as sales or transfers.</span></span> <span data-ttu-id="bdcab-114">This is helpful for new [!INCLUDE[prod_short](includes/prod_short.md)] customers and small businesses with relatively low inventory transaction levels.</span><span class="sxs-lookup"><span data-stu-id="bdcab-114">This is helpful for new [!INCLUDE[prod_short](includes/prod_short.md)] customers and small businesses with relatively low inventory transaction levels.</span></span> <span data-ttu-id="bdcab-115">However, as a business grows and inventory levels increase, this can slow down system performance.</span><span class="sxs-lookup"><span data-stu-id="bdcab-115">However, as a business grows and inventory levels increase, this can slow down system performance.</span></span> <span data-ttu-id="bdcab-116">To minimise reduced performance during posting, select a time option to define how far back in time from the work date an inbound transaction can occur to potentially trigger adjustment of related outbound value entries.</span><span class="sxs-lookup"><span data-stu-id="bdcab-116">To minimize reduced performance during posting, select a time option to define how far back in time from the work date an inbound transaction can occur to potentially trigger adjustment of related outbound value entries.</span></span> <span data-ttu-id="bdcab-117">Alternatively, you can manually adjust costs at regular intervals with the Adjust Cost - Item Entries batch job.</span><span class="sxs-lookup"><span data-stu-id="bdcab-117">Alternatively, you can manually adjust costs at regular intervals with the Adjust Cost - Item Entries batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="bdcab-118">See Also</span><span class="sxs-lookup"><span data-stu-id="bdcab-118">See Also</span></span>
[<span data-ttu-id="bdcab-119">Set Up Inventory</span><span class="sxs-lookup"><span data-stu-id="bdcab-119">Set Up Inventory</span></span>](inventory-setup-inventory.md)  
<span data-ttu-id="bdcab-120">[Design Details: Costing Methods](design-details-costing-methods.md)  </span><span class="sxs-lookup"><span data-stu-id="bdcab-120">[Design Details: Costing Methods](design-details-costing-methods.md)  </span></span>  
[<span data-ttu-id="bdcab-121">Manage Inventory</span><span class="sxs-lookup"><span data-stu-id="bdcab-121">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="bdcab-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bdcab-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="bdcab-123">Change Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="bdcab-123">Change Which Features are Displayed</span></span>](ui-experiences.md)  
[<span data-ttu-id="bdcab-124">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="bdcab-124">General Business Functionality</span></span>](ui-across-business-areas.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]