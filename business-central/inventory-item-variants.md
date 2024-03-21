---
title: Manage Product Variants
description: 'Learn how you can record products that are almost identical but vary in colour, size, or material as item variants.'
author: brentholtorf
ms.topic: conceptual
ms.search.keywords: 'item, variant, finished good, component, raw material, assembly item, item substitution'
ms.search.form: '30, 5717, 31, 32, 346, 9091, 5718, 5716, 5720, 1384, 1383, 35, 5404, 1378, 5719'
ms.date: 09/26/2022
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="manage-product-variants"></a>Manage Product Variants

Item variants are a great way to keep your list of products under control. For example, you have a large number of items that are almost identical and vary only in colour. You can define each variant as a separate item. But you choose to set up one item and specify the various colours as variants of the item.  

> [!TIP]
> For a practical introduction to using variants in production, see [Walkthrough: Variants](contoso-coffee/manufacturing/variants.md) for the Contoso Coffee demo data.  

## <a name="add-variants-to-an-item"></a>Add variants to an item

If your organisation has decided to use variants, then it's easy enough to define variants for an item.  

### <a name="to-add-variants"></a>To add variants

1. Open [the **Items List** page](https://businesscentral.dynamics.com/?page=31), open the relevant item.  
2. On the **Item** card, choose the **Item** action, and then choose the **Variants** action.  
3. In the **Item Variants** page, list the variants.  

Then, when you create a sales document and add the item, you can specify the variant of the item in the **Variant Code** field. The same applies to purchase documents.  

## <a name="item-availability-by-variant"></a>Item availability by variant

[!INCLUDE [inventory_variant-availability](includes/inventory_variant-availability.md)]

## <a name="require-use-of-variants"></a>Require use of variants

Starting in 2022 release wave 2, admins can require that users specify the variant in documents and journals for items that have variants. To activate the capability, navigate to the **Inventory Setup** page, and then select the **Variant Mandatory if Exists** field. You can override this global setting for specific items.  

On item cards, the **Variant Mandatory if Exists** field has the following options:

|Field value |Description|
|---------|----|
|Default| The setting from **Inventory Setup** applies to this item.|
|No| Users aren't required to specify a variant for this item.|
|Yes| If the item has one or more variants, users must specify the relevant variant. If they don't, they'll be blocked from posting the transaction.|

> [!NOTE]
> These settings don't affect items that have no variants.

If the capability is switched on, users can't post an entry if the variant isn't specified.

## <a name="categories-attributes-and-variants"></a>Categories, attributes, and variants

[!INCLUDE[inventory_variant](includes/inventory_variant.md)]

## <a name="see-also"></a>See also

[Register New Items](inventory-how-register-new-items.md)  
[Set Up General Stock Information](inventory-how-setup-general.md)  
[Walkthrough: Variants](contoso-coffee/manufacturing/variants.md)  
