---
title: Design Details - Accounts in the General Ledger | Microsoft Docs
description: To reconcile stock and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 41b94d44ba374ecbcad64a2b1da100fcf3e1a2ab
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215585"
---
# <a name="design-details-accounts-in-the-general-ledger"></a>Design Details: Accounts in the General Ledger
To reconcile stock and capacity ledger entries with the general ledger, the related value entries are posted to different accounts in the general ledger. For more information, see [Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md).  

## <a name="from-the-inventory-ledger"></a>From the Stock Ledger  
The following table shows the relationship between different types of stock value entries and the accounts and balancing accounts in the general ledger.  

|**Item Ledger Entry Type**|**Value Entry Ttype**|**Variance Type**|**Expected Cost**|**Account**|**Balancing Account**|  
|--------------------------------|--------------------------|-----------------------|-----------------------|-----------------|---------------------------|  
|Purchase|Direct Cost||Yes|Stock (Interim)|Invt. Accrual Acc. (Interim)|  
|Purchase|Direct Cost||No|Stock|Direct Cost Applied|  
|Purchase|Indirect Cost||No|Stock|Overhead Applied|  
|Purchase|Variance|Purchase|No|Stock|Purchase Variance|  
|Purchase|Revaluation||No|Stock|Stock Adjmt.|  
|Purchase|Rounding||No|Stock|Stock Adjmt.|  
|Sale|Direct Cost||Yes|Stock (Interim)|COGS (Interim)|  
|Sale|Direct Cost||No|Stock|COGS|  
|Sale|Revaluation||No|Stock|Stock Adjmt.|  
|Sale|Rounding||No|Stock|Stock Adjmt.|  
|Positive Adjmt.,Negative Adjmt., Transfer|Direct Cost||No|Stock|Stock Adjmt.|  
|Positive Adjmt.,Negative Adjmt., Transfer|Revaluation||No|Stock|Stock Adjmt.|  
|Positive Adjmt.,Negative Adjmt., Transfer|Rounding||No|Stock|Stock Adjmt.|  
|(Production) Consumption|Direct Cost||No|Stock|WIP|  
|(Production) Consumption|Revaluation||No|Stock|Stock Adjmt.|  
|(Production) Consumption|Rounding||No|Stock|Stock Adjmt.|  
|Assembly Consumption|Direct Cost||No|Stock|Stock Adjmt.|  
|Assembly Consumption|Direct Cost||No|Direct Cost Applied|Stock Adjmt.|  
|Assembly Consumption|Indirect Cost||No|Overhead Applied|Stock Adjmt.|  
|(Production) Output|Direct Cost||Yes|Stock (Interim)|WIP|  
|(Production) Output|Direct Cost||No|Stock|WIP|  
|(Production) Output|Indirect Cost||No|Stock|Overhead Applied|  
|(Production) Output|Variance|Material|No|Stock|Material Variance|  
|(Production) Output|Variance|Capacity|No|Stock|Capacity Variance|  
|(Production) Output|Variance|Subcontracted|No|Stock|Subcontracted Variance|  
|(Production) Output|Variance|Capacity Overhead|No|Stock|Cap. Overhead Variance|  
|(Production) Output|Variance|Manufacturing Overhead|No|Stock|Mfg. Overhead Variance|  
|(Production) Output|Revaluation||No|Stock|Stock Adjmt.|  
|(Production) Output|Rounding||No|Stock|Stock Adjmt.|  
|Assembly Output|Direct Cost||No|Stock|Stock Adjmt.|  
|Assembly Output|Revaluation||No|Stock|Stock Adjmt.|  
|Assembly Output|Indirect Cost||No|Stock|Overhead Applied|  
|Assembly Output|Variance|Material|No|Stock|Material Variance|  
|Assembly Output|Variance|Capacity|No|Stock|Capacity Variance|  
|Assembly Output|Variance|Capacity Overhead|No|Stock|Cap. Overhead Variance|  
|Assembly Output|Variance|Manufacturing Overhead|No|Stock|Mfg. Overhead Variance|  
|Assembly Output|Rounding||No|Stock|Stock Adjmt.|  

## <a name="from-the-capacity-ledger"></a>From the Capacity Ledger  
 The following table shows the relationship between different types of capacity value entries and the accounts and balancing accounts in the general ledger. Capacity ledger entries represent labour time consumed in assembly or production work.  

|**Work Type**|**Capacity Ledger Entry Type**|**Value Entry Type**|**Account**|**Balancing Account**|  
|-------------------|------------------------------------|--------------------------|-----------------|---------------------------|  
|Assembly|Resource|Direct Cost|Direct Cost Applied|Stock Adjmt.|  
|Assembly|Resource|Indirect Cost|Overhead Applied|Stock Adjmt.|  
|Production|Machine Centre/Work Centre|Direct Cost|WIP Account|Direct Cost Applied|  
|Production|Machine Centre/Work Centre|Indirect Cost|WIP Account|Overhead Applied|  

## <a name="assembly-costs-are-always-actual"></a>Assembly Costs are Always Actual  
 As shown in the table above, assembly postings are not represented in interim accounts. This is because the concept of work in progress (WIP) does not apply in assembly output posting, unlike in production output posting. Assembly costs are only posted as actual cost, never as expected cost.  

 For more information, see [Design Details: Assembly Order Posting](design-details-assembly-order-posting.md).  

## <a name="calculating-the-amount-to-post-to-the-general-ledger"></a>Calculating the Amount to Post to the General Ledger  
 The following fields in the **Value Entry** table are used to calculate the expected cost amount that is posted to the general ledger:  

-   Cost Amount (Actual)  
-   Cost Posted to G/L  
-   Cost Amount (Expected)  
-   Expected Cost Posted to G/L  

The following table shows how the amounts to post to the general ledger are calculated for the two different cost types.  

|Cost Type|Calculation|  
|---------------|-----------------|  
|Actual Cost|Cost Amount (Actual) – Cost Posted to G/L|  
|Expected Cost|Cost Amount (Expected) –  Expected Cost Posted to G/L|  

## <a name="see-also"></a>See Also  
 [Design Details: Stock Costing](design-details-inventory-costing.md)   
 [Design Details: Stock Posting](design-details-inventory-posting.md)   
 [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md)  
 [Managing Stock Costs](finance-manage-inventory-costs.md)  
 [Finance](finance.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]