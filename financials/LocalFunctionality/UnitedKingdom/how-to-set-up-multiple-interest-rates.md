---
title: How to Set Up Multiple Interest Rates | Microsoft Docs
description: You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 7f5810d59f3a1d2dc88814f92fdc3373c3870878
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-multiple-interest-rates"></a>Set Up Multiple Interest Rates
You can calculate finance charges with multiple interest rates for a specific period. The interest calculation is similar for all financial charges, with variation only in the rate of interest for a specific period.  

For example, you can charge customers accordingly if they pay late.  

## <a name="to-set-up-multiple-interest-rates"></a>To set up multiple interest rates  

1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.  
2.  In the **Finance Charge Terms** window, select the required finance term, and then, on the **Navigate** tab, choose **Interest Rates**.  
3.  Fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Start Date**|Enter the start date for each finance charge interest rate code.|  
    |**Interest Rate**|Enter the percentage that must be used to calculate interest.|  
    |**Interest Period (Days)**|Enter the period for each finance charge interest rate.|  

4.  Choose the **OK** button.  
5.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.  
6.  In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.  
7.  In the **Reminder Levels** window, select the **Calculate Interest** field.  

 When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period. The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount. The opening entry on the memo is displayed in bold. The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.  

## <a name="see-also"></a>See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  
[Collect Outstanding Balances](../../receivables-collect-outstanding-balances.md)   

