---
title: Archive Sales and Purchase Documents
description: You can archive sales and purchase orders, quotes, return orders, and blanket orders, and restore the originals if needed.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 42, 49, 50, 459, 460, 5159, 5162, 5164, 5167, 6627, 6630, 6644, 9305, 9306, 9346, 9347, 9348, 9349
ms.date: 03/06/2022
ms.author: bholtorf
ms.openlocfilehash: c81248844f603f80304822c0ce089c666f9be9bc
ms.sourcegitcommit: 7b6d70798b4da283d1d3e38a05151df2209c2b72
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/12/2022
ms.locfileid: "8950336"
---
# <a name="archive-documents"></a>Archive Documents
You can archive sales and purchase orders, quotes, return orders, and blanket orders. Archiving documents lets you restore the original, if needed. You can archive a sales or purchase document several times, saving a different archived version each time.

For archived sales documents where the original still exists and isn't posted, you can use the **Restore** action to overwrite the current document with an archived version. 

For archived documents where the original is deleted, you can only reuse the content by copying the data, for example, by using the **Copy from Document** action.  

## <a name="to-set-up-automatic-document-archiving"></a>To set up automatic document archiving

You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders. When automatic archiving is turned on, a new version of the archived document is created when someone does the following things:

* Changes or deletes a document.
* Prints, downloads, or sends a document by email.
* Converts a quote to an order or invoice.
* Posts an order.

The following procedure describes how to set up automatic archiving of sales documents. The steps are similar for purchase documents.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.
2. On the **Archiving** FastTab, specify whether to turn on automatic archiving for the various types of sales documents. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

The following table describes the options for the **Archive Quotes** field.

|Option|Description|
|------|-----------|
|**Never**| Don't archive sales quotes when they're deleted.|
|**Question**|Prompt the user to choose whether to archive sales quotes when they're deleted.|
|**Always**|Archive sales quotes automatically when they're deleted.|

## <a name="to-archive-a-sales-order"></a>To archive a sales order

The following procedure describes how to archive a sales order. The steps are similar for all orders, blanket orders, return orders, and quotes.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.  
2. Open a sales order that you want to archive.  
3. Choose the **Archive Document** action.

The sales order is archived. You can view it on the **Archived Sales Orders** page.

## <a name="to-restore-a-non-posted-sales-order-from-the-archive"></a>To restore a non-posted sales order from the archive

The following procedure describes how to restore an archived sales order to the original sales order. Restoring a document is only possible when the original document hasn't been posted. The steps are similar for all orders, blanket orders, return orders, and quotes.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Order Archives**, and then choose the related link.
2. Select the archived sales order, or version of it, that you want to restore, and then choose the **Restore** action.  

The contents of the original sales order are replaced with the archived version.

## <a name="to-delete-archived-sales-orders"></a>To delete archived sales orders

The following procedure describes how to delete archived sales orders. The steps are similar for other archived sales and purchase documents.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Order Archives**, and then choose the related link.  
2. Choose the **Delete Older Versions** action, and then, on the **Delete Archived Sales Order Versions** page, select the appropriate filters.  
3. Choose the **OK** button.

## <a name="see-also"></a>See Also

[Track Document Lines](across-how-to-track-document-lines.md)  
[Sales](sales-manage-sales.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
