---
title: Specify Coloured Indicators to Customise Visual Signals About a Cue's Activity | Microsoft Docs
description: "Set up a coloured indicator on a Cue tile to provide a personalised visual signal of the Cue’s activity."
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 0cb10770954f485d9c0a3474615e6c69411de321
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a>How to: Set Up a Coloured Indicator on Cues
You can set up Cues that appear on the **Home** page to include an indicator that changes colour based on the data values in the Cues.

The indicator appears as a coloured bar along the top border of the Cue tile. It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action. For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.

From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.

To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different colour (or style).

## <a name="to-set-up-colored-indicators-on-cues"></a>To set up coloured indicators on Cues
1. Under **Activities** on your **Home** page, choose **Set Up Cues**.  
   The **Cue Setup** window appears. The window lists the indicators that are currently setup up on Cues.
2. To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.  

The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.

| Option | Colour |
| --- | --- |
| **None** |No colour (same colour as the Cue tile |
| **Favorable** |Green |
| **Unfavorable** |Red |
| **Ambiguous** |Yellow |
| **Subordinate** |Grey |

## <a name="see-also"></a>See Also
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

