---
title: Customise Visual Signals About a Cue's Activity | Microsoft Docs
description: "Set up a coloured indicator on a Cue tile to provide a personalised visual signal of the Cue’s activity."
services: project-madeira
documentationcenter: 
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 10/01/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: e4ceaeae1a37a521d2d5bd22ab711757283e6321
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-a-colored-indicator-on-cues"></a>Set Up a Coloured Indicator on Cues
You can set up Cues that appear on the Role Centre to include an indicator that changes colour based on the data values in the Cues.

The indicator appears as a coloured bar along the top border of the Cue tile. It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action. For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.

From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.

To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different colour (or style).

## <a name="to-set-up-colored-indicators-on-cues"></a>To set up coloured indicators on Cues
1. Under **Activities** on your Role Centre, choose **Set Up Cues**.  
   The **Cue Setup** window appears. The window lists the indicators that are currently setup up on Cues.
2. To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.  

The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.

| Option | Colour |
| --- | --- |
| **None** |No colour (same colour as the Cue tile)|
| **Favorable** |Green |
| **Unfavorable** |Red |
| **Ambiguous** |Yellow |
| **Subordinate** |Grey |

## <a name="see-also"></a>See Also
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

