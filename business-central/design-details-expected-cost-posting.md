---
title: Design Details - Expected Cost Posting | Microsoft Docs
description: Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 181b0168dc73aba7bb4d09b7cda7a2ce7028e142
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215285"
---
# <a name="design-details-expected-cost-posting"></a>Design Details: Expected Cost Posting
Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.  

 You can post expected cost to stock and to the general ledger. When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost. This expected cost affects the stock value, but is not posted to the general ledger unless you set up the system up to do so.  

> [!NOTE]  
>  Expected costs are only managed for item transactions. Expected costs are not for immaterial transaction nature codes, such as capacity and item charges.  

 If only the quantity part of an stock increase has been posted, then the stock value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box on the **Stock Setup** page. In that case, the expected cost is posted to interim accounts at the time of receipt. After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the stock account.  

 To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.  

## <a name="example"></a>Example  
 The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected on the **Stock Setup** page.  

 You post a purchase order as received. The expected cost is LCY 95.00.  

 **Value Entries**  

|Posting Date|Entry Type|Cost Amount (Expected)|Expected Cost Posted to G/L|Expected Cost|Item Ledger Entry No.|Entry No.|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|01-01-20|Direct Cost|95.00|95.00|Yes|1|1|  

 **Relation Entries in the G/L – Item Ledger Relation Table**  

|G/L Entry No.|Value Entry No.|G/L Register No.|  
|--------------------|---------------------|-----------------------|  
|1|1|1|  
|2|1|1|  

 **General Ledger Entries**  

|Posting Date|G/L Account|Account No. (En-US Demo)|Amount|Entry No.|  
|------------------|------------------|---------------------------------|------------|---------------|  
|01-01-20|Stock Accrual Account (Interim)|5530|-95.00|2|  
|01-01-20|Stock Account (Interim)|2131|95.00|1|  

 At a later date, you post the purchase order as invoiced. The invoiced cost is LCY 100.00.  

 **Value Entries**  

|Posting Date|Cost Amount (Actual)|Cost Amount (Expected)|Cost Posted to G/L|Expected Cost|Item Ledger Entry No.|Entry No.|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|01-15-20|100.00|-95.00|100.00|No|1|2|  

 **Relation Entries in the G/L – Item Ledger Relation Table**  

|G/L Entry No.|Value Entry No.|G/L Register No.|  
|--------------------|---------------------|-----------------------|  
|3|2|2|  
|4|2|2|  
|5|2|2|  
|6|2|2|  

 **General Ledger Entries**  

|Posting Date|G/L Account|Account No. (En-US Demo)|Amount|Entry No.|  
|------------------|------------------|---------------------------------|------------|---------------|  
|01-15-20|Stock Accrual Account (Interim)|5530|95.00|4|  
|01-15-20|Stock Account (Interim)|2131|-95.00|3|  
|01-15-20|Direct Cost Applied Account|7291|-100|6|  
|01-15-20|Stock Account|2130|100|5|  

## <a name="see-also"></a>See Also
 [Design Details: Stock Costing](design-details-inventory-costing.md)   
 [Design Details: Cost Adjustment](design-details-cost-adjustment.md)   
 [Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md)   
 [Design Details: Stock Posting](design-details-inventory-posting.md)   
 [Design Details: Variance](design-details-variance.md)  
 [Managing Stock Costs](finance-manage-inventory-costs.md)  
 [Finance](finance.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]