---
title: How to Block Items from Sales or Purchasing
description: You can block items from being entered on lines in sales or purchase documents, as well as from being posted in a transaction.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/16/2021
ms.author: edupont
ms.openlocfilehash: 744d19675fe3ae95bcbaa56d6e8555ac734180e6
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6441175"
---
# <a name="block-items-from-sales-or-purchasing"></a>Block Items from Sales or Purchasing
You can block an item from being entered on lines in sales or purchase documents, and you can block it from being posted in any transaction. For example, this is useful when an item has a known defect. If someone chooses a blocked item on a sales or purchase document a message will inform them that the item is blocked.

The following table describes what occurs when items are blocked.  

|Option|Description|  
|--------------------|------------|  
|**Sales Blocked**|You cannot enter the item in a sales document or in a sales item journal.|  
|**Purchasing Blocked**|You cannot enter the item in a purchase document, in a purchase item journal, or in purchase planning processes.|  
|**Blocked**|You cannot use the item for any item transaction.|  

> [!NOTE]
> Blocked items can be returned. This means that none of the above settings apply when the item is used on return orders and credit memos.

When you use the **Copy from Document** function to create new documents based on existing documents, you are notified if any items on the source document lines are blocked. The blocked document lines are excluded from the new document, and a notification shows an overview of all document lines that are blocked in the source document.

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a>To block an item from being entered on sales lines  
1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.  
2.  Select the item that you want to block, and then select the **Sales Blocked** check box.  

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a>To block an item from being entered on purchase lines  
1.  Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.  
2.  Select the item that you want to block, and then select the **Purchasing Blocked** check box.  

## <a name="to-block-an-item-from-being-posted"></a>To block an item from being posted
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.
2. Select the item that you want to block, and then select the **Blocked** check box.

## <a name="see-also"></a>See Also  
[Register New Items](inventory-how-register-new-items.md)  
[Stock](inventory-manage-inventory.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]