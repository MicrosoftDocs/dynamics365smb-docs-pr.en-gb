---
title: Walkthrough - Making Cash Flow Forecasts by Using Account Schedules | Microsoft Docs
description: This walkthrough describes how you can use account schedules to make cash flow forecasts. Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts. In the account schedules, you can set up subtotals for cash flow receipts and disbursements. These subtotals can be included in new totals that can then be used in making cash flow forecasts.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: a210792a187bde0217917659f118c58a6a135df2
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4756548"
---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a>Walkthrough: Making Cash Flow Forecasts by Using Account Schedules
This walkthrough describes how you can use account schedules to make cash flow forecasts. Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts. In the account schedules, you can set up subtotals for cash flow receipts and disbursements. These subtotals can be included in new totals that can then be used in making cash flow forecasts.  

## <a name="about-this-walkthrough"></a>About This Walkthrough  
This walkthrough describes the following tasks:  

- Setting up a new cash flow account schedule name.  
- Setting up account schedule lines.  
- Setting up a new column layout.  
- Assigning a column layout to an account schedule.  
- Viewing and printing the cash flow forecast.  

### <a name="prerequisites"></a>Prerequisites  
To complete this walkthrough, you will need:  

- [!INCLUDE[prod_short](includes/prod_short.md)] installed.  
- The cash flow worksheet lines are registered.  

## <a name="roles"></a>Roles  
This walkthrough demonstrates tasks that are performed by the following user role:  

- Controller  

## <a name="story"></a>Story  
Ken is a controller at CRONUS who makes monthly cash flow forecasts. He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.  

## <a name="setting-up-a-new-account-schedule-name"></a>Setting Up a New Account Schedule Name  
An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.  

### <a name="to-set-up-a-new-account-schedule-name"></a>To set up a new account schedule name  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.  
2.  On the **Account Schedule Names** page, choose the **New** to create a new cash flow account schedule name.  
3.  In the **Name** field, enter **Forecast**.  
4.  In the **Description** field, enter **Cash Flow Forecast**.  
5.  Leave the **Default Column Layout** and **Analysis View Name** fields blank.  

## <a name="setting-up-account-schedule-lines"></a>Setting Up Account Schedule Lines  
After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule. Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.  

### <a name="to-set-up-account-schedule-lines"></a>To set up account schedule lines  

1.  On the **Account Schedule Names** page, select the new **Forecast** account schedule name that you have created, and then choose the **Edit Account Schedule** action.  
2.  On the **Account Schedule** page, enter each line exactly as shown in the following table.  

    > [!NOTE]  
    >  Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.  

    |Row No.|Description|Totalling Type|Totalling|Row Type|Amount Type|Show|  
    |-------|-----------|-------------|--------|--------|-----------|----|
    |C10|Amount|Net Change|Entries|Net Amount|Always|  
    |C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|  
    |C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|  

4.  Choose the **OK** button.  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a>Assigning the Column Layout to the Account Schedule Name  
Ken is now ready to assign the column layout to the account schedule name.  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a>To assign the column layout to the account schedule name  

1.  On the **Account Schedule Names** page, select **Forecast** in the **Name** field.  
2.  In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.  

### <a name="to-view-and-print-the-cash-flow-forecast"></a>To view and print the cash flow forecast  
1.  On the **Account Schedule Names** page, choose the **Overview** action to view the cash flow forecast.  
2.  On the **Acc. Schedule Overview** page, you can select an amount and then view the cash flow forecast entries that make up the amount. In addition, you can view the formula that is used to calculate the amount. You can also filter the amounts by date and dimension.  
3.  Choose the **Print** action to print the cash flow forecast.  

## <a name="see-also"></a>See Also  
 [Work with Account Schedules](bi-how-work-account-schedule.md)   
 [Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md)  
 [Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)
