---
title: Use Item References
description: Set up references between the descriptions, unit of measurements, and variants that you and your supplier or customer use for an item.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item reference, cross reference, inventory
ms.date: 10/27/2021
ms.author: edupont
ms.openlocfilehash: 180b07e9970d9387988bae4db7655fca73d5f4fd
ms.sourcegitcommit: 400554d3a8aa83d442f134c55da49e2e67168308
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/27/2021
ms.locfileid: "7701495"
---
# <a name="use-item-references"></a>Use Item References

If you buy or sell items that you and your supplier or customer use different terms for, then you can set up a reference between your terms for the items and the terms that the customer or supplier of that item uses. This way, the supplier's or customer's item description, unit of measurement, or variant code is automatically inserted on the relevant documents when you fill in the **Item Reference No.** field.  

> [!NOTE]
> [!INCLUDE [2021_releasewave2](includes/2021_releasewave2.md)]
>
> Not all companies use item references. To minimise clutter on pages, we've hidden the related fields and actions by default. If you decide to use them, select the **Use Item References** field on the **Stock Setup** page. After you turn on item references, the fields and actions are available on the Item Card, Supplier Card, and Customer Card pages, and from sales and purchase documents.
>
> In versions earlier than 2021 release wave 2, your administrator can turn on the *Write longer item references* feature in the [Feature Management](https://businesscentral.dynamics.com/?page=2610) page (link requires that you have a [!INCLUDE [prod_short](includes/prod_short.md)] tenant). How you use references doesn't change, but the names of things like pages and buttons will. For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.

## <a name="to-start-using-item-references"></a>To start using item references

[!INCLUDE [2021_releasewave2](includes/2021_releasewave2.md)]

1. Choose the :::image type="icon" source="media/ui-search/search_small.png" border="false"::: icon, enter **Stock Setup**, and then choose the related link.
2. Select the **Use Item References** field.

## <a name="to-set-up-an-item-reference"></a>To set up an item reference

1. Choose the :::image type="icon" source="media/ui-search/search_small.png" border="false"::: icon, enter **Items**, and then choose the related link.
2. Open the card for an item for which you want to create a reference.
3. Choose the **Item References** action.

     If you cannot find the **Item References** action, choose to view more options, and then find it under **Related** > **Item**.
  
4. On a new line on the **Item Reference Entries** page, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

The following procedure describes how you specify the item reference on a purchase order. Similar steps apply to sales documents and other purchase documents.  

## <a name="to-enter-a-vendors-item-description-on-a-document"></a>To enter a supplier's item description on a document

1. Choose the :::image type="icon" source="media/ui-search/search_small.png" border="false"::: icon, enter **Purchase Orders**, and then choose the related link.
2. Create a purchase order for the supplier that you set up an item reference for in the previous procedure.
3. Create a purchase line for the item that you set up an item reference for in the previous procedure.
4. In the **Item Reference No.** field, select the relevant item reference, and then choose the **OK** button.

The **Description** field on the line is overwritten with the supplier's item description, as set up on the item reference entry. If the item reference includes a variant code or a unit of measurement, these values are also copied to the document.  

## <a name="see-also"></a>See Also

[Register New Items](inventory-how-register-new-items.md)  
[Stock](inventory-manage-inventory.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]