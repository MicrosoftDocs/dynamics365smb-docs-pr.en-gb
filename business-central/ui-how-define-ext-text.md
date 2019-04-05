---
title: Add Extra Lines to Define Extended Item Descriptions | Microsoft Docs
description: You can add extra lines to extend the standard text that describes an item.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 02/26/2019
ms.author: sgroespe
ms.openlocfilehash: ecf0dab7e8c1215c6e121735fe7507ee28cc25b8
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "808823"
---
# <a name="add-extended-item-text"></a>Add Extended Item Text
You can extend a standard text for items by adding extra lines, and you can set up conditions for use of the extra lines. You do this from item cards.

## <a name="to-define-extended-text-for-an-item-description"></a>To define extended text for an item description
1. Open the card for an item that you want to add extended text to, and then choose the **Extended Text** action.
2. Fill in the **Code** and **Description** fields.
3. Choose the **New**.
4. Fill in the **Language Code** field or select the **All Language Codes** check box if you use language codes.
5. Fill in the **Starting Date** and **Ending Date** fields if you want to limit the dates on which the extended text is used.
6. In the **Text** field, write the extended text.
7. Select relevant check boxes for the document types where you want the extended text printed.
8. Close the page.

## <a name="to-add-an-extended-item-text-on-a-sales-order-line"></a>To add an extended item text on a sales order line
1. Open a sales order with a sales line for an item that has extended text defined. For more information, see [Sell Products](sales-how-sell-products.md).
2. Select the line in question, and then choose the **Insert Ext. Text** action.

## <a name="see-also"></a>See Also
[Setting Up Inventory](inventory-setup-inventory.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
