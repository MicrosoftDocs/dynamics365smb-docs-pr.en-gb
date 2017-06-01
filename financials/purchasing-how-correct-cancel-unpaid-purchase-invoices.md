---
title: 'How to: Correct or Cancel Unpaid Purchase Invoices| Microsoft Docs'
description: 'How to: Correct or Cancel Unpaid Purchase Invoices'
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: fba080da79d3a9d3f816c8ddc0a02c877211bcb4
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
# <a name="how-to-correct-or-cancel-unpaid-purchase-invoices"></a>How to: Correct or Cancel Unpaid Purchase Invoices
You can correct or cancel a posted purchase invoice. This is useful if you want to correct a typing mistake, or if you want to change the purchase early in the order process.

If you have already paid for products on the posted purchase invoice, you cannot correct or cancel it from the posted purchase invoice itself. Instead, you must manually create a purchase credit memo to reverse the purchase. For more information, see [How to: Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).

In the **Posted Purchase Invoice** window, you can choose the **Correct** button or the **Cancel** button. When you correct or cancel a posted purchase invoice, the corrective purchase credit memo is applied to all general ledger and inventory ledger entries that were created when the initial purchase invoice was posted. This reverses the posted purchase invoice in your financial records and leaves the corrective posted purchase credit memo for your audit trail. In the following the use of **Correct** and **Cancel** is described.

## <a name="to-correct-a-posted-purchase-invoice"></a>To correct a posted purchase invoice
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Posted Purchase Invoices**, and then choose the related link.  
2. Select the posted purchase invoice that you want to correct.  

    **Note**: If the **Cancelled** check box is selected, then you cannot correct the posted purchase invoice because it has already been corrected or cancelled.
3. In the **Posted Purchase Invoice** window, choose **Correct**.

    A new purchase invoice with the same information is created where you can make the correction. For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md). The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.

    A purchase credit memo is automatically created and posted to void the initial posted purchase invoice.
4. Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.

## <a name="to-cancel-a-posted-purchase-invoice"></a>To cancel a posted purchase invoice
1. In the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Posted Purchase Invoices**, and then choose the related link.  
2. Select the posted purchase invoice that you want to cancel.

    **Note**: If the **Cancelled** check box is selected, then you cannot cancel the posted purchase invoice because it has already been cancelled or corrected.
3. In the **Posted Purchase Invoice** window, choose **Cancel**.

    A purchase credit memo is automatically created and posted to void the initial posted purchase invoice. The **Cancelled** field on the initial posted purchase invoice is changed to **Yes**.
4. Choose **Show Corrective Credit Memo** to view the posted purchase credit memo that voids the initial posted purchase invoice.

## <a name="see-also"></a>See Also
[Purchasing](purchasing-manage-purchasing.md)  
[How to: Record Purchases](purchasing-how-record-purchases.md)  
[Working With [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

