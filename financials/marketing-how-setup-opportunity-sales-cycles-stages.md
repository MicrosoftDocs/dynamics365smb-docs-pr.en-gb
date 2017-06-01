---
title: 'How to: Set Up Opportunity Sales Cycles and Cycle Stages | Microsoft Docs'
description: Describes how to set up opportunity sales cycles and stages in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 63d3e4689a751e8e56363efcfde1d609762a419e
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a>How to: Set Up Opportunity Sales Cycles and Cycle Stages
Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages. A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale. Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage. You can also specify whether a stage can be skipped. You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.

Implementing opportunity sales cycles involves setting up the sales cycle code, defining the different stages of the cycle, and then assigning the cycle to opportunities.

## <a name="to-set-up-an-opportunity-sales-cycle-code"></a>To set up an opportunity sales cycle code
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Sales Cycles**, and then choose the related link. The **Sales Cycles** window opens, and lists all the existing sales cycles.
2. Choose the **New** action, and fill in the fields.

Repeat these steps to set up as many sales cycles as you want. After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.

## <a name="to-define-opportunity-sales-cycle-stages"></a>To define opportunity sales cycle stages
1. In the **Sales Cycles** window, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action. The **Sales Cycle Stages** window opens.
2. Choose the **New** action to enter a new stage in the sales cycle.

Repeat these steps to set up as many stages as you want within the sales cycle.

## <a name="to-assign-stage-cycle-to-an-opportunity"></a>To assign stage cycle to an opportunity
After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field. For more information, see [How to: Create Sales Opportunities](marketing-how-create-opportunities.md).

## <a name="see-also"></a>See Also
[Processing Sales Opportunities](marketing-processing-sales-opportunities.md)  
[Sales](sales-manage-sales.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

