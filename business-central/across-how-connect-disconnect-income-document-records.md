---
title: Create Incoming Document Records From Docs
description: You can store external business documents by attaching the document files to the related incoming document records.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/25/2021
ms.author: edupont
ms.openlocfilehash: 65b0d704708232d0999cfc0e72a6380a00a4a273
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6437734"
---
# <a name="create-incoming-document-records-directly-from-documents-and-entries"></a>Create Incoming Document Records Directly from Documents and Entries
You can store external business documents in [!INCLUDE[prod_short](includes/prod_short.md)] by attaching the document files to the related incoming document records. If the document, such as a purchase invoice, did not start its existence as an incoming document record, you can still create and connect an incoming document record to it later. You can also attach incoming document files to posted purchase and sales documents and to supplier, customer, and general ledger entries by using the **Incoming Document Files** FactBox in, for example, the **Posted Purchase Invoices** and **Supplier Ledger Entries** pages.

From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files. For more information, see [Find Posted Documents without Incoming Document Records](across-how-find-posted-documents-without-income-document-records.md).

The following procedures show how to attach a file to an existing purchase invoice that was not created from an incoming document record and how to attach a file to a supplier ledger entry. Attaching a file to posted purchase or sales documents works in a similar way.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>To create and connect an incoming document record from a purchase invoice
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.
2. Select the line for a purchase invoice that you want to attach a file to, and then choose the **Create Incoming Document from File** action.
3. Alternatively, select the line for a purchase invoice that you want to attach a file to, and then choose the **Attach File** action.
4. On the **Insert File** page, select the file that represents the incoming document in question, and then choose the **Open** button.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>To create and connect an incoming document record from a supplier ledger entry
1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Supplier Ledger Entries**, and then choose the related link.
2. Select a line for a supplier ledger entry that you want to attach a file to, and then choose the **Create Incoming Document from File** action.
3. Alternatively, select a line for a supplier ledger entry that you want to attach a file to, and then choose the **Attach File** action.
4. On the **Insert File** page, select the file that represents the incoming document in question, and then choose the **Open** button.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>To remove a connection from an incoming document record to a posted document
You can remove file attachments from non-posted documents at any time by deleting the related incoming document record. If the document is posted, then you must first remove the connection from the incoming document record.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Documents**, and then choose the related link.
2. Select the line for an incoming document record connected to a posted document that you want to remove, and then choose the **Remove Reference to Record** action.

The connection to the posted document is removed. You can now proceed to connect another incoming document record to the posted document as described in this topic.

## <a name="see-also"></a>See Also
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]