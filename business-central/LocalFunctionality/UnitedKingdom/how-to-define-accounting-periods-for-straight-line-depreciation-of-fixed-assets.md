---
title: Straight-Line Depreciation of Fixed Assets in the UK | Microsoft Docs
description: Define 13 accounting periods to calculate straight-line depreciation in the UK version. You must calculate depreciation daily and distribute across the relevant periods.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.search.keywords: write down
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: ec19e1666e556ac6dd12e2fd9a8c1fe227600b7b
ms.sourcegitcommit: 41876b559872fe7adbfa5b59a6e1a71dc907fb15
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/14/2021
ms.locfileid: "7920948"
---
# <a name="define-accounting-periods-for-straight-line-depreciation-of-fixed-assets"></a>Define Accounting Periods for Straight-Line Depreciation of Fixed Assets
You can define 13 accounting periods to calculate straight line depreciation. You must calculate depreciation daily and distribute across the relevant periods. You can also define these accounting periods in the **FA - Projected Value** report.  

> [!NOTE]  
>  To calculate depreciation using both the old (360 days) and the new methods (365 or 366 days), create separate depreciation books; one for the old method, and one for the new method. Attach these books to the relevant assets.  

### <a name="to-define-accounting-periods-to-calculate-straight-line-depreciation"></a>To define accounting periods to calculate straight line depreciation  

1.  Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Depreciation Books**, and then choose the related link.  
2.  To open a new **Depreciation Book Card** page, choose the **New** action.  
3.  On the **General** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
5.  Choose the **OK** button.  

## <a name="to-define-accounting-periods-in-the-fa---projected-value-report"></a>To define accounting periods in the FA - Projected Value report  

1.  Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA - Projected Value**, and then choose the related link.  
2.  On the **Options** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3.  Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.  

> [!NOTE]
> You can turn on the **Use Accounting Period** toggle if you want the periods between start date and ending date to correspond to the accounting periods you have specified on the **Accounting Periods** page. The **Number of Days** field will be cleared and made read-only on the FA - Projected Value report. If you do not turn on the toggle, the projected value amounts will be calculated based on a 360 day year.

## <a name="see-also"></a>See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)   
[Set Up Fixed Asset Depreciation](../../fa-how-setup-depreciation.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]