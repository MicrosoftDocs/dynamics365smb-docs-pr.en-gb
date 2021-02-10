---
title: Using the QuickBooks Payroll File Import Extension | Microsoft Docs
description: This topic describes how to use the extension to import salary and wage transactions from QuickBooks.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: eae93ea8cf81a2fad6af2c3810f94d5292eef93f
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4757099"
---
# <a name="the-quickbooks-payroll-file-import-extension"></a>The QuickBooks Payroll File Import Extension
Use the QuickBooks Payroll File Import extension to import payroll transactions from QuickBooks to general ledger accounts in [!INCLUDE[prod_short](includes/prod_short.md)]. For example, this is useful when you are transitioning from QuickBooks to [!INCLUDE[prod_short](includes/prod_short.md)], or if you outsource your payroll but also want to keep track of it in [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="steps-to-import-payroll-data"></a>Steps to Import Payroll Data
The first step is for you, or maybe your accountant, to use the export features in QuickBooks to export the payroll data to an .IIF file. The second step is to open the **General Journals** page in [!INCLUDE[prod_short](includes/prod_short.md)] and use the **Import Payroll Transactions** action to import the file. During the import process you map the general ledger accounts from QuickBooks to corresponding accounts in [!INCLUDE[prod_short](includes/prod_short.md)]. The final step is to post the payroll transactions in [!INCLUDE[prod_short](includes/prod_short.md)] according to the account mapping. 

For more information, see [Import Payroll Transactions](finance-how-import-payroll-transactions.md).

## <a name="see-also"></a>See Also
[Customising [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)    
[Finance](finance.md)    
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)
