---
title: Setting Up the Chart of Accounts| Microsoft Docs
description: You change the default accounts in the chart of accounts (COA), and you can add new accounts.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: ceb01999525139cabc7c31e2304f738dcc9267f8
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a>Setting Up or Changing the Chart of Accounts
The chart of accounts shows the ledger accounts that store your financial data. [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] includes a standard chart of accounts that is ready to support your business.
However, you can change the default accounts, and you can add new accounts.  

## <a name="adding-or-changing-accounts"></a>Adding or Changing Accounts
From the chart of accounts, you can open each G/L account and add or change settings.

> [!NOTE]  
>   You can delete a general ledger account. However, before you delete it, the following must be true:  

* The balance on the account must be zero.  
* The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.  
* If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.  

## <a name="see-also"></a>See Also
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Managing Bank Accounts](bank-manage-bank-accounts.md)  
[Working with Dimensions](finance-dimensions.md)  
[Importing from Other Finance Systems](upload-data.md)  
[How to: Work With GIFI Codes in Canada](ca-finance-work-gifi-codes.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]
