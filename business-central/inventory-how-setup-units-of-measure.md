---
title: How to Set Up Item Units of Measurement | Microsoft Docs
description: You can set up multiple units of measurement for an item so that you can assign units of measurement to the item.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: UOM
ms.date: 10/16/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Set Up Units of Measurement

As part of setting up your [!INCLUDE [prod_short](includes/prod_short.md)], you set up general units of measurement in the **Units of Measurement** page. Then, when you register new items, you specify the base unit of measurement on the **Item Card**. But you can also add units of measurement later.  

You can set up multiple units of measurement for an item so that you can assign units of measurement to the item for the following purposes:

- Assign a base unit of measurement on the item's item card to define how it is stored in inventory and to serve as the conversion basis for alternate units of measurement.
- Assign alternate units of measurement to purchase, production, or sales documents to specify how many units of the base unit of measurement you handle at a time in those processes. For example, you may buy the item on pallets and only use single pieces in your production.

If an item is stocked in one unit of measurement but produced in another, a production order is created that uses a manufacturing batch unit of measurement to calculate the correct quantity of the components during the **Refresh Production Order** batch job. An example of a manufacturing batch unit of measurement calculation is when a manufactured item is stocked in pieces but produced in tons. For more information, see [Work with Manufacturing Batch Units of Measurement](production-how-to-use-the-manufacturing-batch-unit-of-measure.md).  

Another tool that makes it easier to work with multiple units of measurement for items is the ability to specify a rounding precision for base units of measurement. Specifying a rounding precision provides guidance on what someone should enter for a given business process, and helps reduce rounding issues. When you use alternate units of measurement, the value in the **Qty. per Unit of Measurement** field helps calculate the quantity in the base unit of measurement, which can lead to rounding issues. For example, imagine you're receiving one box that contains six items. When the box arrives at your warehouse, you discover that one of the six items is missing. You decide not to post the receipt of one box, but instead change the quantity received to five of six pieces. That would lead to a receipt of 4.99998 pieces, rather than five. On the **Item Units of Measurement** page, the **Quantity Rounding Precision** field lets you specify a value that will convert the quantity to a number that is easier to understand. Continuing with the example, we would enter **1** in the field to round up to an even five pieces.

## To set up units of measurement

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Units of Measurement**, and then choose the related link.  
2. Choose the **New** action. A new empty line is inserted.  
3. Fill in the fields. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  
4. If you know that your organisation will sell items with this unit of measurement to customers in other countries/regions, you can add translations.  
    1. Select the code for which you want to set up translations, and then choose the **Translations** action.
    2. In the **Language Code** field, select the drop-down arrow to see a list of available language codes. Select the language code for which you want to enter a translation, and then choose the OK button to copy the code to the field.
    3. In the **Description** field, enter the appropriate text.
5. Repeat the previous steps for any additional units of measurement that you want to add.  

When you register a new item, you can choose the base unit of measurement from the list of units of measurement that you have now set up. You can also set up multiple units of measurement for an item.  

## To set up multiple item units of measurement

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. Open the card of the item for which you want to set up alternate units of measurement.
3. Choose the **Units of Measurement** action. The **Item Units of Measurement** page opens.
4. If the **Base Unit of Measurement** field on the item card is filled, then that unit of measurement is already set up.
5. Choose the **New** action. A new empty line is inserted.
6. In the **Code** field, enter the name of the unit of measurement. Alternatively, choose the field to select from the unit of measurement codes that are in the database.
7. In the **Qty. per Unit of Measurement** field, enter how many units of the base unit of measurement the new unit of measurement contains.
8. Optionally, in the **Height**, **Width**, **Length**, and **Weight** fields, specify precise information about the size of one unit of measurement so that the [!INCLUDE [prod_short](includes/prod_short.md)] can calculate how many of each item unit can be placed in any given bin. The **Cubage** field is calculated automatically based on **Height**, **Width**, and **Length**.

    If any of these fields contain a value other than 0, then that measure is used during all processes that involve placing items in a bin: put-away, movements, receipts, shipments, picks, and adjustments. [!INCLUDE [prod_short](includes/prod_short.md)] checks the sum of each physical measure of the items being put away and the items already in the bin against the maximum size or other measure that can fit into a bin, according to the bin capacity policy on the location card for this item. In other words, you must use the same unit measure for each dimension across all item units of measurement - use kilograms or pounds for weight, for example, but be consistent.
9. Repeat steps 5 through 7 to set up all the alternate units of measurement that you want to use in different processes for this item.

    In the **Base Unit of Measurement** field at the bottom of the window, you can view or change the item's base unit of measurement. You can also change the base unit of measurement in the **Base Unit of Measurement** field on the item card. In the **Item Units of Measurement** page, the base unit of measurement must have the value **1** in the **Qty. per Unit of Measurement** field.

You can now use the alternate units of measurement on purchase, production, and sales documents. For more information, see [To enter a default unit of measurement code for sales and purchasing transactions](#to-enter-a-default-unit-of-measure-code-for-sales-and-purchasing-transactions).  

## To set up unit of measurement translations

When you sell items to foreign customers, you might want to specify the unit of measurement in the customer's language. You can do that by specifying translations for units of measurement.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Units of Measurement**, and then choose the related link.
2. Select the code for which you want to set up translations, and then choose the **Translations** action.
3. In the **Language Code** field, select the drop-down arrow to see a list of available language codes. Select the language code for which you want to enter a translation, and then choose the OK button to copy the code to the field.
4. In the **Description** field, enter the appropriate text.
5. Repeat steps 2 through 4 for the unit of measurement codes and the languages for which you want to enter translations.

## To enter a default unit of measurement code for sales and purchasing transactions

If you usually buy or sell in units different from the base unit of measurement, you can specify separate units of measurement for purchases and sales. To do this, the units of measurement must be set up on the **Item Units of Measurement** page.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. Open the relevant item card for which you want to specify a default sales or purchase unit of measurement code.
3. For sales, on the **Invoicing** FastTab, in the **Sales Unit of Measurement** field, open the **Item Units of Measurement** page.
4. For purchasing, on the **Replenishment** FastTab, in the **Purch. Unit of Measurement** field, open the **Item Units of Measurement** page.
5. Select the code you want to set up as the default unit of measurement for sales or purchasing respectively, and then choose the **OK** button.

## See also 

[Work with Manufacturing Batch Units of Measurement](production-how-to-use-the-manufacturing-batch-unit-of-measure.md)  
[Register New Items](inventory-how-register-new-items.md)  
[Managing Inventory](inventory-manage-inventory.md)  
[Managing Purchasing](purchasing-manage-purchasing.md)  
[Managing Sales](sales-manage-sales.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
