---
title: How to Set Up Cost Centres | Microsoft Docs
description: Cost centres are departments that are responsible for costs and income. The chart of cost centres is similar to the dimension information for the general ledger.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 7362518cbade8132fb07f49e7b2e9be67c4bce29
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-cost-centers"></a>Set Up Cost Centres
Cost centres are departments that are responsible for costs and income. The chart of cost centres is similar to the dimension information for the general ledger. You can set up the chart of cost centres in the following ways:  

-   Transfer dimension values in the general ledger to the chart of cost centres. You can make any necessary adjustments after the transfer.  
-   Create a new chart of cost centre that is independent of the general ledger or add a new cost centre to an existing chart of cost centre. You must create each cost centre individually.  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a>To transfer dimension values in the general ledger to the chart of cost centres  
1.  Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window. Only the values from this dimension are transferred.  
2.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centres**, and then choose the related link.  
3.  On the **Actions** tab, in the **Functions** group, choose **Get Cost Centres from Dimension** to transfer dimension values to the chart of cost centres. The function transfers the dimension values that you defined in step 1.  

    > [!NOTE]  
    >  You can set up the **Align Cost Centre Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost centres. You cannot define a synchronisation of the chart of cost centres to dimension values from the general ledger.  

The chart of cost centres now contains all specified dimension values from the general ledger and includes titles and subtotals.  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a>To create new cost centers in the Chart of Cost Centers window  
You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window. In this procedure, you set up cost centers in the **Chart of Cost Centers** window.  

1. Open the **Chart of Cost Centers** window in edit mode.  
2. In the **Code** field, enter the cost center code. All cost centres must have a code.  
3. In the **Name** field, enter the cost center name.  
4. Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost centre.  

    - For cost centers of the **Total** type, you must fill in the **Totaling** field. Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.  
    - For cost centres of the **End-Total** line type, this field is filled in automatically when you use the indent function.  
5.  Fill in the **Sorting Order** and **Cost Subtype** fields.  
6.  Choose the next empty line to create a new cost centre, and then repeat steps 2 through 5.  
7.  After you have set up all the cost centres, choose the **Indent Cost Centres** action. Choose the **Yes** button.  

> [!IMPORTANT]  
>  If you have entered definitions in the **Totalling** fields for **End-Total** cost centres before you run the indent function, then you must enter them again. The function overwrites the values in all **End-Total** fields.  

## <a name="see-also"></a>See Also  
[Accounting for Costs](finance-manage-cost-accounting.md)  
[Setting Up Cost Accounting](finance-set-up-cost-accounting.md)   
[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md)   
[About Cost Accounting](finance-about-cost-accounting.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

