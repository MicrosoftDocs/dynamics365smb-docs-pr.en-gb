---
title: Print Cheques for APACS
description: The Association for Payment Clearing Services (APACS) specification defines a standard layout for fields on cheques in the UK. The Cheque report uses this specification.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.form: 256
ms.date: 04/01/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Print Cheques for APACS

The Association for Payment Clearing Services (APACS) specification defines a standard layout for fields on cheques. The **Cheque** report uses this specification.  

## To print cheques for APACS  

1.  Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.  
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

## See Also  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]