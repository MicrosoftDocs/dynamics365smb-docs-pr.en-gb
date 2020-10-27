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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 1bd492b10e10f60fe853e7a50ecc25c17aa8a880
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3923093"
---
# <a name="print-checks-for-apacs"></a>Print Cheques for APACS
The Association for Payment Clearing Services (APACS) specification defines a standard layout for fields on cheques. The **Cheque** report uses this specification.  

## <a name="to-print-checks-for-apacs"></a>To print cheques for APACS  

1.  Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals** , and then choose the related link.  
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
