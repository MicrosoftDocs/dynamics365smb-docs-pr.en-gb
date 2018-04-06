---
title: How to Print Cheques for APACS | Microsoft Docs
description: The Association for Payment Clearing Services (APACS) specification defines a standard layout for fields on cheques. The **Cheque** report uses this specification.
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
ms.openlocfilehash: 9d367b810e01926d10a6cde38ba211a9cb3623bc
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

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
    |**Last Cheque No.**|Specifies the last cheque number that was specified in the **Bank Account Card** window.|  
    |**One Cheque per Vendor per Document No.**|Select to print only one cheque per vendor for each document number.|  
    |**Reprint Cheques**|Select to reprint cancelled cheques.|  
    |**Test Print**|Select to print cheques on blank paper before printing them on cheque forms.|  
    |**Preprinted Stub**|Select to use cheque forms with preprinted stubs.|  

5.  Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.  

## <a name="see-also"></a>See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)

