---
title: Walkthrough - Making Cash Flow Forecasts by Using Account Schedules
description: Learn how you can use account schedules to make cash flow forecasts.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 48a176c4c363c4a33ae336d754be71c9f7dd0aeb
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772111"
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

- [!INCLUDE[prod_short](includes/prod_short.md)]  
- The cash flow worksheet lines are registered  

## <a name="roles"></a>Roles

This walkthrough demonstrates tasks that are performed by the following user role:  

- Controller  

## <a name="story"></a>Story

Ken is a controller at CRONUS who makes monthly cash flow forecasts. He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.  

## <a name="setting-up-a-new-account-schedule-name"></a>Setting Up a New Account Schedule Name

An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.  

### <a name="to-set-up-a-new-account-schedule-name"></a>To set up a new account schedule name  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.  
2. On the **Account Schedule Names** page, choose the **New** to create a new cash flow account schedule name.  
3. In the **Name** field, enter **Forecast**.  
4. In the **Description** field, enter **Cash Flow Forecast**.  
5. Leave the **Default Column Layout** and **Analysis View Name** fields blank.  

## <a name="setting-up-account-schedule-lines"></a>Setting Up Account Schedule Lines

After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule. Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.  

### <a name="to-set-up-account-schedule-lines"></a>To set up account schedule lines  

1. On the **Account Schedule Names** page, select the new **Forecast** account schedule name that you have created, and then choose the **Edit Account Schedule** action.  
2. On the **Account Schedule** page, enter each line as shown in the following table.  

    > [!TIP]  
    >  Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.  

    | Row No. | Description              | Totalling Type            | Totalling | Row Type   | Amount Type | Show |
    |---------|--------------------------|--------------------------|----------|------------|-------------|------|
    | R10     | Open sales orders        | Cash Flow Entry Accounts | 20       |Net Change | Net Amount  | Yes  |
    | R10     | Rentals                  | Cash Flow Entry Accounts | 30       |Net Change | Net Amount  | Yes  |
    | R10     | Financial assets         | Cash Flow Entry Accounts | 40       |Net Change | Net Amount  | Yes  |
    | R10     | Fixed assets disposal    | Cash Flow Entry Accounts | 50       |Net Change | Net Amount  | Yes  |
    | R10     | Private investments      | Cash Flow Entry Accounts | 60       |Net Change | Net Amount  | Yes  |
    | R10     | Miscellaneous receipts   | Cash Flow Entry Accounts | 70       |Net Change | Net Amount  | Yes  |
    | R10     | Open service orders      | Cash Flow Entry Accounts | 80       |Net Change | Net Amount  | Yes  |
    | R20     | Total Cash Receipts      | Formula                  | R10      |Net Change | Net Amount  | Yes  |
    | R20     | Total Cash Receipts      | Formula                  | R10      |Net Change | Net Amount  | Yes  |
    | R30     | Payables                 | Cash Flow Entry Accounts | 1010     |Net Change | Net Amount  | Yes  |
    | R30     | Open purchase orders     | Cash Flow Entry Accounts | 1020     |Net Change | Net Amount  | Yes  |
    | R30     | Personnel costs          | Cash Flow Entry Accounts | 1030     |Net Change | Net Amount  | Yes  |
    | R30     | Running costs            | Cash Flow Entry Accounts | 1040     |Net Change | Net Amount  | Yes  |
    | R30     | Finance costs            | Cash Flow Entry Accounts | 1050     |Net Change | Net Amount  | Yes  |
    | R30     | Investments              | Cash Flow Entry Accounts | 1070     |Net Change | Net Amount  | Yes  |
    | R30     | Private consumptions     | Cash Flow Entry Accounts | 1090     |Net Change | Net Amount  | Yes  |
    | R30     | VAT due                  | Cash Flow Entry Accounts | 1100     |Net Change | Net Amount  | Yes  |
    | R30     | Other expenses           | Cash Flow Entry Accounts | 1110     |Net Change | Net Amount  | Yes  |
    | R40     | Total cash disbursements | Formula                  | R30      |Net Change | Net Amount  | Yes  |
    | R50     | Surplus                  | Formula                  | R20+R40  |Net Change | Net Amount  | Yes  |
    | R60     | Cash Flow Funds          | Cash Flow Entry Accounts | 2100     |Net Change | Net Amount  | Yes  |
    | R70     | Total Cash Flow          | Formula                  | R50+R60  |Net Change | Net Amount  | Yes  |

    > [!NOTE]
    > The row number R10 is used to capture the account totals for receivables. The row number R20 is used to calculate the sum of all cash receipts. The row number R30 is used to capture the account totals for payables. The row number R40 is used to calculate the sum of all cash disbursements. The row number R50 is used to capture the sum of cash surplus. The row number R60 is used to capture the liquid funds. The row number R70 is used to calculate the forecasted cash flow.

## <a name="setting-up-a-new-column-layout"></a>Setting Up a New Column Layout

Before Ken can print the cash flow forecast, he needs to create the column layout for the numerical information. In the columns, he defines the information that he wants to use from the lines.

- The first column has the number *C10* with the title **Amount** and contains the net change.  
- The second column has the number *C20* with the title **Balance at Date** and contains the transactions for the period.  
- The third column has the number *C30* with the title **Entire Year** and contains the net change in the balances for the entire fiscal year.  
- Finally, he assigns the column layout as the default column layout for the account schedule **Forecast**.  

## <a name="to-set-up-a-new-column-layout"></a>To set up a new column layout

1. In the **Account Schedule Names** window, select the new **Forecast** account schedule name that you have created. On the **Home** tab, in the **Process** group, choose **Edit Column Layout Setup**.

    > [!TIP]
    > You can find the same action in the **Account Schedule** page if you are still editing the **Forecast** account schedule there.

2. Create a new column layout with the name **Cash Flow**.

3. Choose the OK button.

4. Enter each line exactly as shown in the following table.

    |Column No.|Column Header|Column Type|Ledger Entry Type|Amount Type|Show|  
    |----------|-------------|-----------|-----------------|-----------|----|
    |C10|Amount|Net Change|Entries|Net Amount|Always|  
    |C20|Amount until Date|Balance at Date|Entries|Net Amount|Always|  
    |C30|Entire Fiscal Year|Entire Fiscal Year|Entries|Net Amount|Always|

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a>Assigning the Column Layout to the Account Schedule Name

Ken is now ready to assign the column layout to the account schedule name.  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a>To assign the column layout to the account schedule name  

1. In the **Account Schedule** page where you're working with the **Forecast** account schedule, choose the **Edit Column Layout Setup** action.  
2. In the **Column Layout Name** field, choose the column layout **Cash Flow** to assign as the default column layout.  

### <a name="to-view-and-print-the-cash-flow-forecast"></a>To view and print the cash flow forecast

1. On the **Account Schedule Names** page, choose the **Overview** action to view the cash flow forecast.  
2. On the **Acc. Schedule Overview** page, you can select an amount and then view the cash flow forecast entries that make up the amount. In addition, you can view the formula that is used to calculate the amount. You can also filter the amounts by date and dimension.  
3. Choose the **Print** action to print the cash flow forecast.  

## <a name="see-also"></a>See Also

[Work with Account Schedules](bi-how-work-account-schedule.md)  
[Analysing Cash Flow in Your Company](finance-analyze-cash-flow.md)  
[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]