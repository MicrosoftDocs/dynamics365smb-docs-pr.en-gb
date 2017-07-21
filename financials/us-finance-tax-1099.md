---
title: Reporting 1099 Transactions in the US | Microsoft Docs
description: The IRS requires the 1099 tax form for payments to vendors and you can specify a purchase document is 1099 liable and specify the 1099 code for the vendor.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: local
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: c20c52927aa979e56aeef7975fbcee1564ca4dd7
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="reporting-transactions-as-1099-liable-in-the-us"></a>Reporting Transactions as 1099 Liable in the US

The Internal Revenue Service (IRS) requires one or more versions of the 1099 tax form for payments to vendors. Copies of these forms must be sent to vendors annually on or before the last day of January. On your purchase documents, you can specify that the document is 1099 liable, and you can specify the 1099 code for the vendor.  

## <a name="1099-codes"></a>1099 codes
In [!INCLUDE[d365fin](includes/d365fin_md.md)], the most common 1099 codes are already set up for you so you are ready to generate the required reports. The codes are defined in the **IRS 1099 Form Box** window where you can also add new 1099 codes. For each tax liable vendor, you can then specify the relevant 1099 code on the **Payments** FastTab on the Vendor card.  

With the **Vendor 1099 Information** report, you can review 1099 transactions paid during a specified period. At the end of the year, you can print 1099 transactions on preprinted forms.  

## <a name="printing-1099-tax-forms"></a>Printing 1099 tax forms
From the **IRS 1099 Form Box** window, you can access the following tax forms:  

* Vendor 1099 Div  

  Prints the federal form 1099-DIV for dividends and distribution. You can print all or specific 1099-DIV forms. The report uses the codes that apply to the DIV form amount boxes from the **IRS 1099 Form-Box** window.  
* Vendor 1099 Int  

  Prints the federal form 1099-INT for interest income. You can print all or specific 1099-INT forms. The report uses the codes that apply to the INT form amount boxes from the **IRS 1099 Form-Box** window.  
* Vendor 1099 Misc - Miscellaneous income  

  Prints the federal form 1099-MISC for miscellaneous income. You can print all or specific 1099-MISC forms. The report uses the codes that apply to the MISC form amount boxes from the **IRS 1099 Form-Box** window.  

Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.
It may be helpful to run the **Vendor 1099 Information** report to review the data before printing the forms.

## <a name="submitting-1099-tax-forms-electronically"></a>Submitting 1099 tax forms electronically
To submit the 1099 tax forms electronically, use the **Vendor 1099 Magnetic Media** report. Specifies the 1099 forms that can be exported. The form information exported by this report is the same as the reports that print 1099 forms that are described in the previous section.  

The report uses the codes that apply to the form amount boxes from the **IRS 1099 Form-Box** window. The codes are mapped to the form boxes in the file layouts of this report, therefore the table data and report version for a particular tax year must be in agreement. If any custom codes are added to the table these must be mapped to the form boxes inside this object.  

Regulatory changes affecting this report and the table data are generally handled in end-of-year updates.
It may be helpful to run the **Vendor 1099 Information** report to review the data before generating the electronic file.  

## <a name="see-also"></a>See Also
[How to: Register New Vendors](purchasing-how-register-new-vendors.md)  
[How to: Record Purchase](purchasing-how-record-purchases.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

