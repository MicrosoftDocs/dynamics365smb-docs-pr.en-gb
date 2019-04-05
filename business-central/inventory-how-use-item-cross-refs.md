---
title: Use Item Cross-References| Microsoft Docs
description: If you set up a cross-reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.** field.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 03/12/2019
ms.author: sgroespe
ms.openlocfilehash: 09fb7c17e2fccbd3b2ad3195cffa37493ad40f61
ms.sourcegitcommit: d09f5ee0e164c7716f4ccb2ed71e2f9732a1f4f9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/19/2019
ms.locfileid: "852270"
---
# <a name="use-item-cross-references"></a>Use Item Cross References
If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.** field. The same functionality applies for customer item numbers on sales documents.

The following procedures describe how to use item cross references on the purchase side. The steps are similar for the sales side.

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a>To set up an item cross reference to a vendor's item description
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.
3. Choose the **Cross References** action.
4. On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a>To enter a vendor's item description on a purchase order
1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.
2. Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.
3. Create a purchase line for the item that you set up an item cross reference for in the previous procedure.
4. In the **Cross-Reference No.** field, select the item cross reference that you have created, and then choose the **OK** button.

The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Inventory](inventory-manage-inventory.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
