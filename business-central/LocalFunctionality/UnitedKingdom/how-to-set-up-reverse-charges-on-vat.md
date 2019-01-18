---
title: How to Set Up Reverse Charges on VAT | Microsoft Docs
description: Learn how you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC).
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: d173d41202a9bf874d6cbc074892d492979323b6
ms.contentlocale: en-gb
ms.lasthandoff: 11/22/2018

---
# <a name="set-up-multiple-interest-rates"></a>Set Up Multiple Interest Rates
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud. This feature is supplemented by the **Reverse Charge Sales List** report. The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units. These goods will apply to reverse charges.

> [!IMPORTANT]  
>  Legislative information may be subject to change by HM Revenue & Customs (HMRC). For more information, see the [HMRC website](https://www.hmrc.gov.uk/index.htm).  

## <a name="to-reverse-charges-on-vat"></a>To reverse charges on VAT  

1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Business Posting Groups**, and then choose the related link.  
2.  Create a new VAT business posting group. Set up the needed VAT product posting groups.  
3.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.  
4.  On the **Reverse Charge** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
5.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.  
6.  On the **Reverse Charge** FastTab, fill in the fields as necessary.
7.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup** and then choose the related link.  
6.  On the **Reverse Charge** FastTab, fill in the fields as necessary.
9. To set up items subject to reverse charge, select the item, and open the **Item Card** page.  
10. On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.  

## <a name="reverse-charge-sales-list"></a>Reverse Charge Sales List
This report displays sales of goods which are subject to reverse charge. The report is based on information in the VAT Entry table. You use this to report to the customs and tax authorities the reverse charge sales.  

Examples of goods subject to reverse charge:  

-   Mobile telephones.  
-   Computer chips  

Consult the [HMRC website](http:\\www.hmrc.gov.uk) for the list of goods subject to reverse charge.  

## <a name="see-also"></a>See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  

