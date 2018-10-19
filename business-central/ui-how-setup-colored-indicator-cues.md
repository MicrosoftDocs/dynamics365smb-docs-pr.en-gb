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
# <a name="set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="e4cef-103">Set Up a Coloured Indicator on Cues</span><span class="sxs-lookup"><span data-stu-id="e4cef-103">Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="e4cef-104">You can set up Cues that appear on the Role Centre to include an indicator that changes colour based on the data values in the Cues.</span><span class="sxs-lookup"><span data-stu-id="e4cef-104">You can set up Cues that appear on the Role Center to include an indicator that changes color based on the data values in the Cues.</span></span>

<span data-ttu-id="e4cef-105">The indicator appears as a coloured bar along the top border of the Cue tile.</span><span class="sxs-lookup"><span data-stu-id="e4cef-105">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="e4cef-106">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span><span class="sxs-lookup"><span data-stu-id="e4cef-106">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="e4cef-107">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span><span class="sxs-lookup"><span data-stu-id="e4cef-107">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="e4cef-108">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span><span class="sxs-lookup"><span data-stu-id="e4cef-108">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="e4cef-109">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different colour (or style).</span><span class="sxs-lookup"><span data-stu-id="e4cef-109">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="e4cef-110">To set up coloured indicators on Cues</span><span class="sxs-lookup"><span data-stu-id="e4cef-110">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="e4cef-111">Under **Activities** on your Role Centre, choose **Set Up Cues**.</span><span class="sxs-lookup"><span data-stu-id="e4cef-111">Under **Activities** on your Role Center, choose **Set Up Cues**.</span></span>  
   <span data-ttu-id="e4cef-112">The **Cue Setup** window appears.</span><span class="sxs-lookup"><span data-stu-id="e4cef-112">The **Cue Setup** window appears.</span></span> <span data-ttu-id="e4cef-113">The window lists the indicators that are currently setup up on Cues.</span><span class="sxs-lookup"><span data-stu-id="e4cef-113">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="e4cef-114">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span><span class="sxs-lookup"><span data-stu-id="e4cef-114">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="e4cef-115">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span><span class="sxs-lookup"><span data-stu-id="e4cef-115">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

| <span data-ttu-id="e4cef-116">Option</span><span class="sxs-lookup"><span data-stu-id="e4cef-116">Option</span></span> | <span data-ttu-id="e4cef-117">Colour</span><span class="sxs-lookup"><span data-stu-id="e4cef-117">Color</span></span> |
| --- | --- |
| <span data-ttu-id="e4cef-118">**None**</span><span class="sxs-lookup"><span data-stu-id="e4cef-118">**None**</span></span> |<span data-ttu-id="e4cef-119">No colour (same colour as the Cue tile)</span><span class="sxs-lookup"><span data-stu-id="e4cef-119">No color (same color as the Cue tile)</span></span>|
| <span data-ttu-id="e4cef-120">**Favorable**</span><span class="sxs-lookup"><span data-stu-id="e4cef-120">**Favorable**</span></span> |<span data-ttu-id="e4cef-121">Green</span><span class="sxs-lookup"><span data-stu-id="e4cef-121">Green</span></span> |
| <span data-ttu-id="e4cef-122">**Unfavorable**</span><span class="sxs-lookup"><span data-stu-id="e4cef-122">**Unfavorable**</span></span> |<span data-ttu-id="e4cef-123">Red</span><span class="sxs-lookup"><span data-stu-id="e4cef-123">Red</span></span> |
| <span data-ttu-id="e4cef-124">**Ambiguous**</span><span class="sxs-lookup"><span data-stu-id="e4cef-124">**Ambiguous**</span></span> |<span data-ttu-id="e4cef-125">Yellow</span><span class="sxs-lookup"><span data-stu-id="e4cef-125">Yellow</span></span> |
| <span data-ttu-id="e4cef-126">**Subordinate**</span><span class="sxs-lookup"><span data-stu-id="e4cef-126">**Subordinate**</span></span> |<span data-ttu-id="e4cef-127">Grey</span><span class="sxs-lookup"><span data-stu-id="e4cef-127">Gray</span></span> |

## <a name="see-also"></a><span data-ttu-id="e4cef-128">See Also</span><span class="sxs-lookup"><span data-stu-id="e4cef-128">See Also</span></span>
<span data-ttu-id="e4cef-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e4cef-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

