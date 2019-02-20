---
title: Using the QuickBooks Payroll File Import Extension | Microsoft Docs
description: This topic describes how to use the extension to import salary and wage transactions from QuickBooks.
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 01/09/2019
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 79729b42b660399893aebe1116c80ef3b3209042
ms.openlocfilehash: ac68f8a4d67224ad55b1c34ff9b2e4ffa2c372aa
ms.contentlocale: en-gb
ms.lasthandoff: 01/15/2019

---
# <a name="the-quickbooks-payroll-file-import-extension"></a>The QuickBooks Payroll File Import Extension
Use the QuickBooks Payroll File Import extension to import payroll transactions from QuickBooks to general ledger accounts in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For example, this is useful when you are transitioning from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)], or if you outsource your payroll but also want to keep track of it in [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="steps-to-import-payroll-data"></a>Steps to Import Payroll Data
The first step is for you, or maybe your accountant, to use the export features in QuickBooks to export the payroll data to an .IIF file. The second step is to open the **General Journals** page in [!INCLUDE[d365fin](includes/d365fin_md.md)] and use the **Import Payroll Transactions** action to import the file. During the import process you map the general ledger accounts from QuickBooks to corresponding accounts in [!INCLUDE[d365fin](includes/d365fin_md.md)]. The final step is to post the payroll transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] according to the account mapping. 

For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).

## <a name="see-also"></a>See Also
[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)    
[Finance](finance.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

