---
title: Understanding the General Ledger and COA
description: Describes general ledger, chart of accounts, and account categories. Use the General Ledger Setup page to specify handling accounting issues in your company.
author: edupont04
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.search.form: 18, 20, 37, 65, 99, 312, 314, 313, 395, 552, 569, 570, 634, 790, 791, 1158
ms.date: 08/23/2022
ms.author: edupont
ms.openlocfilehash: 29f66fae0413bb0f8a757cfceedce8e0504e8686
ms.sourcegitcommit: 38b1272947f64a473de910fe81ad97db5213e6c3
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/29/2022
ms.locfileid: "9362283"
---
# <a name="understanding-the-general-ledger-and-the-chart-of-accounts"></a>Understanding the General Ledger and the Chart of Accounts

The general ledger stores your financial data. The chart of accounts shows the accounts that general ledger entries are posted to. [!INCLUDE[prod_short](includes/prod_short.md)] includes a standard chart of accounts that is ready to support your business.

## <a name="general-ledger-setup-and-general-posting-setup"></a>General ledger setup and general posting setup

The setup of the general ledger is at the core of financial processes because it defines how you post data. Two pages play an important part in configuring your finance processes:  

* The **General Ledger Setup** page

  On the **General Ledger Setup** page, you specify how to handle certain accounting issues in your company, such as:  

  * Invoice rounding details  
  * Address formats  
  * Financial reporting  

  > [!TIP]
  > The **General Ledger Setup** page includes generic fields and fields that are particular to your country or region. If you are not sure of the meaning of a field, we suggest you work with your accountant to determine whether it is of relevance to your organisation. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

    Open the page [here](https://businesscentral.dynamics.com/?page=118)
* The **General Posting Setup** page

    Similarly, on the **General Posting Setup** page, you specify how you want to set up combinations of general business and general product posting groups. Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts. You fill in a line for each combination of business posting group and product posting group. But you can also open each line in its own posting setup card. For more information, see [Posting Group Setups](finance-posting-groups.md).  

    > [!TIP]
    > If you cannot see the fields that you are looking for in the **General Posting Setup** page, then use the horizontal scroll bar at the bottom of the page to scroll to the right.  

    Open the page [here](https://businesscentral.dynamics.com/?page=314)

## <a name="the-chart-of-accounts"></a>The chart of accounts

The chart of accounts shows all general ledger accounts. From the chart of accounts, you can do things like:  

* View reports that show general ledger entries and balances.  
* Close your income statement.  
* Open the general ledger (G/L) account card to add or change settings.  
* See a list of posting groups that post to that account.
* View separate debit and credit balances for a single account  

You can add, change, or delete general ledger accounts. However, to prevent discrepancies, you can't delete a general ledger account if its data is used in the chart of accounts. To prevent mistakes in sensitive periods, you can also block deletion of accounts. For more information, see [Deleting accounts](finance-setup-chart-accounts.md#delete-accounts).  

## <a name="account-categories"></a>Account categories

You can personalise the structure of your financial statements by mapping general ledger accounts to account categories.  

The **G/L Account Categories** page shows your categories and subcategories, and the general ledger accounts that are assigned to them. You can create new subcategories and assign those categories to existing accounts.  

You create a category group by indenting other subcategories under a line on the **G/L Account Categories** page. Category groups make it easy to get an overview, because each grouping shows a total balance. For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.  

You can specify whether the accounts in each subcategory must be included in specific types of reports. The account categories help define the layout of your financial statements.  

### <a name="example"></a>Example

For example, the default balance statement has a subcategory for *Cash* under *Current Assets*. You want the balance statement consider petty cash and checking, so you take the following steps:  

1. Add two new subcategories:

    * One for petty cash  
    * One for your current account  
2. Specify another report definition **Cash Accounts** for these subcategories.  
3. Indent them under the **Cash** subcategory.  

The next time you generate account schedules, your balance statement will show the following lines:

* Total balance for cash.
* Lines with balances for petty cash and the current account.  

> [!NOTE]
> If you create a G/L account without assigning an account category, when you assign the account to a posting group [!INCLUDE[prod_short](includes/prod_short.md)] automatically assigns the account category from the G/L account immediately above the account in your chart of accounts. However, to include the new account in your financial reports, you must choose the **Generate Financial Reports** action on the **General Ledger Account Categories** page. Alternatively, you can open the G/L Account Card page, specify the account category, and then regenerate your financial report.

## <a name="get-a-quick-overview"></a>Get a quick overview

The **Chart of Accounts** page displays accounts in a hierarchical list that offers fast access to the key information for each account. However, the list is static. If you have many accounts you might have to scroll to view different accounts. If you just want a quick overview of the basics, such as net changes and balances, the **Chart of Accounts Overview** page is a useful alternative. The column layout on the page is now the same as you’ll find on the **Chart of Accounts** page (though with fewer columns), so you won’t have to reorient yourself. You can expand or collapse the hierarchical levels to condense the view. To make it easy to switch between the pages, the **Chart of Accounts Overview** page is available from the **Chart of Accounts** page.

## <a name="access-to-create-and-edit-accounts-and-account-categories"></a>Access to create and edit accounts and account categories

In a small organisation, such as the CRONUS demonstration company, most users can edit the chart of accounts. Except users with a TEAM MEMBER licence. However, larger organisations typically use roles and permissions to limit access to editing the chart of accounts. If you're an administrator, or you have the **Business Manager** or **Accountant** role, you can control user permissions to give the right people access to the relevant tables. For more information, see [To get an overview of a user's permissions](ui-define-granular-permissions.md#to-get-an-overview-of-a-users-permissions).  

## <a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/business-central-configure-general-ledger-setup/)

## <a name="see-also"></a>See also 

[Finance](finance.md)  
[Set Up or Changing the Chart of Accounts](finance-setup-chart-accounts.md)  
[Business Intelligence](bi.md)  
[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
