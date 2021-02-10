---
title: Create New Value Entries for Items in the Inventory| Microsoft Docs
description: Describes how to appreciate or depreciate the value entries of one or more items in the inventory by posting their current, calculated value.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 2bcd09876f18bb948e060b06199d3d36facaa83f
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4750062"
---
# <a name="revalue-inventory"></a><span data-ttu-id="0c724-103">Revalue Inventory</span><span class="sxs-lookup"><span data-stu-id="0c724-103">Revalue Inventory</span></span>
<span data-ttu-id="0c724-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span><span class="sxs-lookup"><span data-stu-id="0c724-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="0c724-105">To revalue inventory</span><span class="sxs-lookup"><span data-stu-id="0c724-105">To revalue inventory</span></span>
1. <span data-ttu-id="0c724-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0c724-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="0c724-107">Choose the **Calculate Inventory Value** action.</span><span class="sxs-lookup"><span data-stu-id="0c724-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="0c724-108">On the **Calculate Inventory Value** page, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="0c724-108">On the **Calculate Inventory Value** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="0c724-109">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0c724-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="0c724-110">On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span><span class="sxs-lookup"><span data-stu-id="0c724-110">On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="0c724-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span><span class="sxs-lookup"><span data-stu-id="0c724-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="0c724-112">The relevant fields are automatically updated.</span><span class="sxs-lookup"><span data-stu-id="0c724-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="0c724-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span><span class="sxs-lookup"><span data-stu-id="0c724-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="0c724-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span><span class="sxs-lookup"><span data-stu-id="0c724-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="0c724-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span><span class="sxs-lookup"><span data-stu-id="0c724-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="0c724-116">New value entries are now created to reflect the revaluations that you have posted.</span><span class="sxs-lookup"><span data-stu-id="0c724-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="0c724-117">You can see the new values on the respective item cards.</span><span class="sxs-lookup"><span data-stu-id="0c724-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="0c724-118">See Also</span><span class="sxs-lookup"><span data-stu-id="0c724-118">See Also</span></span>
[<span data-ttu-id="0c724-119">Design Details: Revaluation</span><span class="sxs-lookup"><span data-stu-id="0c724-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="0c724-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="0c724-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0c724-121">Sales</span><span class="sxs-lookup"><span data-stu-id="0c724-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="0c724-122">Purchasing</span><span class="sxs-lookup"><span data-stu-id="0c724-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="0c724-123">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0c724-123">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
