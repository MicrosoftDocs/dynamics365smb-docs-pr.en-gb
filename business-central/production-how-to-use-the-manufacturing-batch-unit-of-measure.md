---
title: Use the Manufacturing Batch Unit of Measurement
description: This topic gives an overview of how to work with manufacturing batch units of measurement in Business Central.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/25/2021
ms.author: edupont
ms.openlocfilehash: abf8fd20f15f02edad3f451da04729dfd2824bd4
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2022
ms.locfileid: "8514446"
---
# <a name="work-with-manufacturing-batch-units-of-measure"></a>Work with Manufacturing Batch Units of Measurement
If an item is stocked in one unit of measurement but produced in another, a works order is created that uses a manufacturing batch unit of measurement to calculate the correct quantity of the components during the **Refresh Works Order** batch job. An example of a manufacturing batch unit of measurement calculation is when a manufactured item is stocked in pieces but produced in tons.  

## <a name="to-create-a-production-bom-using-a-batch-unit-of-measure"></a>To create a production BOM using a batch unit of measurement  
1.  The manufacturing batch unit of measurement is set up as an alternative unit of measurement on the **Item Units of Measurement** page on the item to be produced. The batch unit of measurement will not replace the base unit of measurement on the item.  
2.  Create a production BOM for the item set up with the manufacturing batch unit of measurement. For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).  
3.  In the **Unit of Measurement Code** field, select the manufacturing batch unit of measurement.  
4.  For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measurement.  
5.  Open the **Item Card** for the related item.  

    On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.  
6.  Create a works order header using the item set up with the manufacturing batch unit of measurement. For more information, see [Create Works Orders](production-how-to-create-production-orders.md).  
7.  Choose the **Refresh** action, and then choose  the **OK** button.  

On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result. The application calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measurement.  

## <a name="to-calculate-a-manufacturing-batch-unit-of-measure-on-a-production-order"></a>To calculate a manufacturing batch unit of measurement on a works order  
1.  Create a works order header using the item set up with the manufacturing batch unit of measurement.  
2.  In the **Item No.** field in the Works Order line, type the same item number used in the header.  
3.  In the **Quantity** field, enter the same quantity used in the header.  
4.  In the **Unit of Measurement Code** field, select the manufacturing batch unit of measurement code.  
5.  Choose the **Refresh** action.
6.  On the **Calculate** FastTab, clear the **Lines** check box.  
7.  Choose the **OK** button.  
8.  On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result. The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measurement.  

## <a name="see-also"></a>See Also  
[Create Routings](production-how-to-create-routings.md)  
[Create Production BOMs](production-how-to-create-production-boms.md)     
[Setting Up Manufacturing](production-configure-production-processes.md)  
[Manufacturing](production-manage-manufacturing.md)    
[Planning](production-planning.md)   
[Inventory](inventory-manage-inventory.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]