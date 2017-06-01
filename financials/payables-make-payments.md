---
title: Make Payments| Microsoft Docs
description: Make Payments
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 03/28/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: f6721c0359b4499a597b349a280afb56818a1f28
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
# <a name="make-payments"></a>Make Payments
When you make payments to vendors, you post the related payment lines in the **Payment Journal** window. You can use the **Suggest Vendor Payments** function to find payments that are due. You can also use the **Vendor - Summary Aging** report to get an overview of due payments.

From the payment journal, you can print computer cheques or record when cheques are written. If you select **Computer Cheque** in the **Bank Payment Type** field, then any lines representing cheques must be printed before the payment journal can be posted.

When the payments are posted, you can export them to a bank file for upload to your bank for processing.

After the payments are made at your bank, you must apply them to their related open vendor ledger entries. You can do this manually or by importing a bank statement file and applying the payments automatically. For more information, see [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).

The following table describes a sequence of tasks, with links to the topics that describe them.

| To | See |
| --- | --- |
| Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity. |[How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md) |
| Issue cheques for payments, either as print-outs or as computer cheques. Void cheques before or after posting. |[How to: Work With Checks](payables-how-work-checks.md) |
| Make sure that your bank only clears validated cheques and amounts by sending them a file that contains vendor, cheque, and payment information. |[How to: Export a Positive Pay file](finance-how-positive-pay.md) |
|Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America. |[How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md)|  

## <a name="see-also"></a>See Also
[Managing Payables](payables-manage-payables.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Managing Receivables](receivables-manage-receivables.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

