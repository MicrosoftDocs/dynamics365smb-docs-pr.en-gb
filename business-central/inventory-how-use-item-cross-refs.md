---
title: Use Item References
description: Set up references between the descriptions that you and your supplier use for an item to insert the supplier's item description on purchase documents.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item reference, cross reference, inventory
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: 4eed6fce594b0b6835020fcdddb7275489b4d160
ms.sourcegitcommit: 6ad0a834fc225cc27dfdbee4a83cf06bbbcbc1c9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2021
ms.locfileid: "7588608"
---
# <a name="use-item-references"></a>Use Item References
If you set up a reference between the item description that you use for an item and the description that the supplier of that item uses, then the supplier's item description is automatically inserted on purchase documents for the supplier when you fill in the **Item Reference No.** field. The same functionality applies for customer item numbers on sales documents.

The following procedures describe how to use item references on the purchase side. The steps are similar for the sales side.

> [!NOTE]
> Not all companies use item references, so to minimise clutter on pages we've hidden the related fields and actions. If you decide to use them, you can turn on the **Use Item References** toggle on the **Stock Setup** page. After you enable item references, the fields and actions are available on the Item Card, Supplier Card, and Customer Card pages, and from sales and purchase documents.

## <a name="to-start-using-item-references"></a>To start using item references
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Stock Setup**, and then choose the related link.
2. Turn on the **Use Item References** toggle.

## <a name="to-set-up-an-item-reference-to-a-vendors-item-description"></a>To set up an item reference to a supplier's item description

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. Open the card for an item for which you want to create a reference to the item description that the supplier uses for that item.
3. Choose the **Item References** action.

     If you cannot find the **Item References** action, choose to view more options, and then find it under **Related** > **Item**.
  
4. On a new line on the **Item Reference Entries** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a>To enter a supplier's item description on a purchase order

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.
2. Create a purchase order for the supplier that you set up an item reference for in the previous procedure.
3. Create a purchase line for the item that you set up an item reference for in the previous procedure.
4. In the **Item Reference No.** field, select the item reference that you have created, and then choose the **OK** button.

The **Description** field on the line is overwritten with the supplier's item description, as set up on the item reference entry.

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Stock](inventory-manage-inventory.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]