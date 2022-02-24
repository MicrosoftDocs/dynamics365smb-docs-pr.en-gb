---
title: How to Print Cheques for APACS | Microsoft Docs
description: The Association for Payment Clearing Services (APACS) specification defines a standard layout for fields on cheques. The Cheque report uses this specification.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 0fbcef4407d0c5886b08a693a5803d64d426f82c
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878795"
---
# <a name="print-checks-for-apacs"></a>Print Cheques for APACS
The Association for Payment Clearing Services (APACS) specification defines a standard layout for fields on cheques. The **Cheque** report uses this specification.  

## <a name="to-print-checks-for-apacs"></a>To print cheques for APACS  

1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.  
2.  To preview the cheque, choose the **Preview Cheque** action.  
3.  To print the cheque, choose the **Print Cheque** action.  

4.  On the **Options** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Bank Account**|Specifies bank account code.|  
    |**Last Cheque No.**|Specifies the last cheque number that was specified on the **Bank Account Card** page.|  
    |**One Cheque per Vendor per Document No.**|Select to print only one cheque per vendor for each document number.|  
    |**Reprint Cheques**|Select to reprint cancelled cheques.|  
    |**Test Print**|Select to print cheques on blank paper before printing them on cheque forms.|  
    |**Preprinted Stub**|Select to use cheque forms with preprinted stubs.|  

5.  Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.  

## <a name="see-also"></a>See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)
