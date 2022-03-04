---
title: Work with Production Families in Manufacturing
description: The main task in customizing a base calendar for your company, or one of its business partners, is to enter any changes to working and nonworking day status.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 99000790, 99000791, 99000792, 99000793
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d786da721738c6c8907232d510954d2dcba224e4
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2022
ms.locfileid: "8135010"
---
# <a name="work-with-production-families"></a>Work with Production Families

A production family is a group of individual items whose relationship is based on the similarity of their manufacturing processes. By forming production families, some items can be manufactured twice or more in one production, which will optimise material consumption.

In the **Quantity** field on the **Family** page, you enter the quantity that will be produced when the whole family has been manufactured once.

## <a name="example"></a>Example

In punching processes, four pieces of the same item can be produced from one sheet and 10 pieces of another, different, item at the same time. The punching machine will punch all 14 pieces in one step.

Forming production families reduces the scrap quantity because what would normally be leftover scrap, when producing big pieces, will be used instead to produce small items.

## <a name="to-set-up-a-production-family"></a>To set up a production family

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Families**, and then choose the related link.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-produce-based-on-a-production-family"></a>To produce based on a production family

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.
2. Create a new works order. For more information, see [Create Works orders](production-how-to-create-production-orders.md).
3. In the **Source Type** field, select **Family**.  
4. In the **Source No.** field, select the relevant production family.

## <a name="see-also"></a>See Also

[Create Production BOMs](production-how-to-create-production-boms.md)  
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Manufacturing](production-manage-manufacturing.md)
[Planning](production-planning.md)   
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]