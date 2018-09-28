---
title: WIP Methods for Calculating and Recording Job Progress| Microsoft Docs
description: Describes the different work in process (WIP) methods you can use to post, monitor, and calculate financial information for ongoing jobs that are in progress.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: work in process, work in progress, calculate project WIP
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 85724fd6f43c684007dd22b34665438bf22bf99a
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="understanding-wip-methods"></a>Understanding WIP Methods
[!INCLUDE[d365fin](includes/d365fin_md.md)] supports the following methods of calculating and recording the value of work in process.

| WIP Method | Calculation Formula | Calculation Description |
| --- | --- | --- |
| Cost Value |Recognised Revenue = Billable Invoiced Price<br /><br /> Estimated Total Costs = Billable Total Price x Budget Cost Ratio<br /><br /> WIP Costs = (Percentage of Completion -Invoiced %) x Estimated Total Costs<br /><br /> Percentage of Completion = Usage Total Costs / Budget Total Costs<br /> Invoiced % = Billable Invoiced Price<br /><br /> Billable Total Price Recognised Costs = Usage Total Costs - WIP |Cost value calculations start by calculating the value of what has been provided by taking a proportion of the estimated total costs based on percentage of completion. Invoiced costs are subtracted by taking a proportion of the estimated total costs based on the invoiced percentage.<br /><br /> This calculation requires that the billable total price, budget total price, and budget total costs be correctly entered for the whole job. |
| Cost of Sales |Recognised Revenue = Billable Invoiced Price<br /><br /> Recognised Costs = Budget Total Cost x Invoiced Percentage<br /><br /> Invoiced % = Billable Invoiced Price / Billable Total Price<br /><br /> (Invoiced % exists as column on job task lines)<br /><br /> WIP Costs = Usage Total Costs – Recognized Costs |Cost of sales calculations begin by calculating the recognised costs. Costs are recognised proportionally based on budget total costs.<br /><br /> This calculation requires that the billable total price and budget total costs be correctly entered for the whole job. |
| Sales Value |Recognised Costs = Usage Total Costs<br /><br /> Recognised Revenue = Usage Total Price x Expected invoicing ratio<br /><br /> Cost Recovery % = Billable Total Price / Budget Total Price<br /><br /> WIP Sales = Recognised Sales - Billable Invoiced Price |Sales value calculations recognise revenue proportionally based on usage total costs and the expected cost recovery ratio.<br /><br /> This calculation requires that the billable total price and budget total price be correctly entered for the whole job. |
| Percentage of Completion |Recognised Costs = Usage Total Costs<br /><br /> Recognised Revenue = Billable Total Price x Percentage of Completion<br /><br /> Percentage of Completion = Usage Total Costs / Budget Total Costs<br /> (Referred to as "Cost Completion %" on job task lines)<br /><br /> WIP Sales = Recognised Sales - Billable Invoiced Price |Percentage of completion calculations recognise revenue proportionally based on the percentage of completion, that is, usage total costs vs. budget costs.<br /><br /> This calculation requires that the billable total price and budget total costs be correctly entered for the whole job. |
| Completed Contract |WIP Amount = WIP Cost Amount = Usage (Total Cost)<br /><br /> WIP Sales Amount = Billable (Invoiced Price) |Completed contract does not recognise revenue and costs until the job is complete. You may want to do this when there is high uncertainty around the estimates of costs and revenue for the job.<br /><br /> All usage is posted to the WIP Costs account (asset) and all invoiced sales are posted to the WIP Invoiced Sales account (liability) until the job is complete. |

## <a name="see-also"></a>See Also
[Project Management](projects-manage-projects.md)  
[Finance](finance.md)  
[Purchasing](purchasing-manage-purchasing.md)         
[Sales](sales-manage-sales.md)      
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

