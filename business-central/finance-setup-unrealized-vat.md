---
title: Setting Up Unrealised Value Added Tax | Microsoft Docs
description: If you're using cash-based accounting, you can specify how to handle unrealised VAT for sales and purchases.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 09759cc8538e0870c0801df73e9c869a0cab4b34
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---

# <a name="set-up-unrealized-vat-for-cash-based-accounting"></a>Set Up Unrealised VAT for Cash-Based Accounting
If you're using cash-based accounting methods, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle unrealized VAT.

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a>To use general ledger accounts for unrealised VAT
You can choose to have VAT amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in VAT statements when the actual payment of the invoice is posted. Before you can do this, you must complete the VAT posting setup.

To use accounts for unrealised VAT, follow these steps:
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and enter **General Ledger Setup**.
2. On the **General Ledger Setup** page, on the **General** FastTab, choose **Show More**, and then choose the **Unrealized VAT** check box.
3. Close the page.
4. choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), and enter **VAT Posting Setup**.
5. On the **VAT Posting Setup** page, choose the VAT posting group, and then choose **Edit**.
6. In the **Unrealized VAT Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding VAT) and the VAT amount itself, and how to transfer VAT amounts from the unrealized VAT account to the realized account. The following table describes the options.

| Option | Description |
| --- | --- |
| Blank | Choose this option if you don't want to use the unrealised VAT feature. |
| Percentage | Payments covers both VAT and the invoice amount in proportion to the payment's percentage of the remaining invoice amount. The paid VAT amount is transferred from the unrealised VAT account to the realised VAT account. |
| First | Payments cover VAT first and then invoice amounts. In this case, the amount transferred from the unrealised VAT account to the VAT account will equal the amount of the payment until the total VAT has been paid. |
| Last | Payments cover the invoice amount first and then VAT. In this case, no amount will be transferred from the unrealised VAT account to the VAT account until the total amount of the invoice, excluding VAT, has been paid. |
| First (Fully Paid) | Payments will cover VAT first (like the _First_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid. |
| Last (Fully Paid) | Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid. |

6. In the **Sales VAT Unreal. Account** field, choose the account for unrealized sales VAT.

    > [!NOTE]  
>   The VAT amount will be posted to this account, and stay there until the customer payment is posted. The amount is then transferred to the account for sales VAT.
7. In the **Purch. VAT Unreal. Account** field, enter the general ledger account for unrealised purchase VAT.

    > [!NOTE]  
    >   The VAT amount will be posted to this account, and stay there until the customer payment is posted. The amount is then transferred to the account for purchase VAT.

## <a name="see-also"></a>See Also
[Setting Up Value Added Tax](finance-setup-vat.md)

