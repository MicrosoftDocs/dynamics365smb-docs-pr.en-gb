---
title: How to Set Up Reverse Charges on VAT | Microsoft Docs
description: Learn how you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC).
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: b312a1c90d4eac376a3c4d7981a3c966842f4260
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3923089"
---
# <a name="set-up-reverse-charge-vat"></a>Set Up Reverse Charge VAT
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can use reverse charge VAT accounting for a specific range of items to prevent Missing Trader Intercommunity Fund Fraud (MTIC), also known as carousel fraud. This feature is supplemented by the **Reverse Charge Sales List** report. The VAT accounting changes will affect companies trading in electronic goods and integrated circuit devices, such as mobile telephones, microprocessors, and central processing units. These goods will apply to reverse charges.

> [!IMPORTANT]  
> Legislative information may be subject to change by HM Revenue & Customs (HMRC). For more information, see the [HMRC website](https://www.gov.uk/government/organisations/hm-revenue-customs).  

## <a name="to-reverse-charges-on-vat"></a>To reverse charges on VAT  

1.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Business Posting Groups** , and then choose the related link.  
2.  Create a new VAT business posting group. Set up the needed VAT product posting groups.  
3.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup** , and then choose the related link.  
4.  On the **Reverse Charge** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
5.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup** , and then choose the related link.  
6.  On the **Reverse Charge** FastTab, fill in the fields as necessary.
7.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup** and then choose the related link.  
6.  On the **Reverse Charge** FastTab, fill in the fields as necessary.
9. To set up items subject to reverse charge, select the item, and open the **Item Card** page.  
10. On the **Invoicing** FastTab, fill in the **Reverse Charge Applies** field.  

## <a name="reverse-charge-sales-list"></a>Reverse Charge Sales List
This report displays sales of goods which are subject to reverse charge. The report is based on information in the VAT Entry table. You use this to report to the customs and tax authorities the reverse charge sales.  

Examples of goods subject to reverse charge:  

- Mobile telephones.  
- Computer chips  

Consult the [HMRC website](https://www.gov.uk/government/organisations/hm-revenue-customs) for the list of goods subject to reverse charge.  

## <a name="see-also"></a>See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  
