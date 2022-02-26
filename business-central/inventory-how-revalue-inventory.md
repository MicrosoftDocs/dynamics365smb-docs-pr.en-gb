---
title: Create New Value Entries for Items in the Stock| Microsoft Docs
description: Describes how to appreciate or depreciate the value entries of one or more items in inventory by posting their current, calculated value.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.search.forms: 5803,
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b07aba72be831dd68eea3475f3ee591a7c319051
ms.sourcegitcommit: 189bf08d7ddf6c8b7ef2c09058c6847aa6e590d3
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/31/2022
ms.locfileid: "8059603"
---
# <a name="revalue-inventory"></a>Revalue Inventory
If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.

## <a name="to-revalue-inventory"></a>To revalue inventory
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Revaluation Journal**, and then choose the related link.
2. Choose the **Calculate Inventory Value** action.
3. On the **Calculate Inventory Value** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choose the **OK** button.
5. On each line on the **Revaluation Journal** page, in the **Unit Cost (Revalued)** field, enter the new unit cost. Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.

    The relevant fields are automatically updated. Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry. It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.
6. When you have completed all lines in the revaluation journal, choose the **Post** action.

New value entries are now created to reflect the revaluations that you have posted. You can see the new values on the respective item cards.

## <a name="see-also"></a>See Also
[Design Details: Revaluation](design-details-revaluation.md)  
[Inventory](inventory-manage-inventory.md)  
[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]