---
title: Create and Manage Catalogue Items
description: Describes how to trade in items that are in your suppliers list of items but not in your own list of items.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.search.forms: 5725, 5726, 5732
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1051b36f70eeb5d86aef04e7faf200660117232d
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2022
ms.locfileid: "8516168"
---
# <a name="work-with-catalog-items"></a>Work with Catalogue Items
You can offer certain items to your customers for their convenience, which you do not want to manage in your system until you start selling them. When you want to start managing such items in your system, you can convert them to normal item cards in two ways.

* From a catalogue item card, create a new item card based on a template.
* From a sales order line of type **Item** with an empty **No** field, select a catalogue item. An item card is then automatically created for the catalogue item.

> [!NOTE]  
> You cannot select a catalogue item from the **Sales Invoice** page.<br /><br />
> You can select a catalogue item from the **Sales Quote** page, but the catalogue item will not be converted to a normal item when you use the **Make Order** function.

A catalogue item typically has the item number of the supplier who supplies it. To enable conversion of a catalogue item card to a normal item card, you must first set up how supplier item numbering is converted to your own item numbering.   

> [!Important]
> Catalogue items are not to be mistaken with non-inventory items, which are regular items that are given the type **Non-Inventory** to keep them out of availability and costing calculations, for example, because they are only used internally and have a low cost. For more information, see [About Item Types](inventory-about-item-types.md).

## <a name="to-create-a-catalog-item"></a>To create a catalogue item
Catalogue item cards have much less information than normal item cards because you only use them to offer on quotes and in other ways. For that reason, they must be converted to normal item cards before you can post sales transactions for them.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Items**, and then choose the related link.
2. Choose the **New** action.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-how-catalog-item-numbers-are-converted-to-your-own-numbering"></a>To set up how catalogue item numbers are converted to your own numbering
To enable conversion of a catalogue item card to a normal item card, you must first set up how the supplier's item numbering is converted to your own item number format.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Item Setup**, and then choose the related link.
2. Fill in the fields as necessary.

## <a name="to-convert-a-catalog-item-to-a-normal-item"></a>To convert a catalogue item to a normal item
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Catalogue Items**, and then choose the related link.
2. Open the card for a catalogue item that you want to convert to a normal item.
3. On the **Catalogue Item Card** page, choose the **Create Item** action.

A new item card pre-filled with information from the catalogue item and a relevant item template is created. You can then fill or edit fields on the new item card as necessary. For more information, see [Register New Items](inventory-how-register-new-items.md).

## <a name="to-sell-a-catalog-item-and-convert-it-to-a-normal-item"></a>To sell a catalogue item, and convert it to a normal item
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.
2. Choose the **New** action. Fill in the fields on the **General** FastTab as for any sales order. For more information, see [Sell Products](sales-how-sell-products.md).
3. On a new sales line, in the **Type** field, select **Item**, but leave the **No.** field empty.
4. Choose the **Line** action, and then choose the **Select Catalogue Items** action.

    The catalogue item is converted to a normal item. A new item card prefilled with information from the catalogue item and a relevant item template is created.
5. On the **Catalogue Items** page, select the catalogue item that you want to sell, and then choose the **OK** button.
6. When the sales order is complete, choose the **Post** action.

You can then fill or edit fields on the new item card as necessary. For more information, see [Register New Items](inventory-how-register-new-items.md).

> [!NOTE]  
>   An item reference is automatically item between the supplier's item number and your new item number. For more information, see [Use Item References](inventory-how-use-item-cross-refs.md).

## <a name="see-also"></a>See Also
[Register New Items](inventory-how-register-new-items.md)  
[Create Special Orders](sales-how-to-create-special-orders.md)|  
[Inventory](inventory-manage-inventory.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]