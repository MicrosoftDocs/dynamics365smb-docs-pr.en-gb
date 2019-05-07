---
title: How to Transfer General Ledger Entries to Cost Entries | Microsoft Docs
description: You can transfer general ledger entries to cost entries.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: a33fb434cc239de951d18783911c879587a3ace0
ms.sourcegitcommit: addfb47612cc2e4e98dfd7e338b6f41cde405d5c
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/16/2019
ms.locfileid: "939041"
---
# <a name="transfer-general-ledger-entries-to-cost-entries"></a>Transfer General Ledger Entries to Cost Entries
You can transfer general ledger entries to cost entries.  

Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.  

## <a name="to-prepare-the-transfer"></a>To prepare the transfer  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cost Accounting Setup**, and then choose the related link.  
2.  On the **Cost Accounting Setup** page, verify that the **Starting Date for G/L Transfer** field is set to the correct value.  
3.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.  
4.  On the **Cost Type Card** page, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.  
5.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.  
6.  For each relevant general ledger account, on the **G/L Account Card** page, verify that the **Cost Type No.** field is linked correctly to a cost type. For more information, see [Setting Up Cost Accounting](finance-set-up-cost-accounting.md).  
7.  Verify that all relevant general ledger entries have dimension values that correspond to a cost centre and a cost object.  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a>To transfer general ledger entries to cost entries  
1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer GL Entries to CA**, and then choose the related link.  
2.  Choose the **Yes** button to start the transfer. The process transfers all general ledger entries that have not already been transferred.  

    During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table. This makes it possible to trace the source of cost entries.  

## <a name="see-also"></a>See Also  
[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md)   
[Setting Up Cost Accounting](finance-set-up-cost-accounting.md)   
