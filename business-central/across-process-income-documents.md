---
title: Process Incoming Documents| Microsoft Docs
description: To record an external document, such as a PDF,  in Business Central , you first create or complete an incoming document record.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 90bcc95fd6aaf70302caa79f6ba0a265fe92a7a9
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2308436"
---
# <a name="processing-incoming-documents"></a>Processing Incoming Documents
To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record. You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.

From PDF or image files that you receive from your trading partners, you can have an external OCR service (Optical Character Recognition) generate electronic documents that can be converted to document records in [!INCLUDE[d365fin](includes/d365fin_md.md)]. For example, when you receive an invoice in PDF format from your vendor, you can send it to the OCR service from the **Incoming Documents** page. Alternatively, you can send the file to the OCR service by email. Then, when you receive the electronic document back, a related incoming document record is created automatically. After some seconds, you receive the file back from the OCR service as an electronic invoice that can be converted to a purchase invoice for the vendor.

| To | See |
| --- | --- |
| Create incoming document records manually or automatically by taking a photo of a paper receipt, for example. |[Create Incoming Document Records](across-how-create-income-document-records.md) |
| Use an OCR service to turn PDF and image files into electronic documents that can be converted to purchase invoices in [!INCLUDE[d365fin](includes/d365fin_md.md)], for example. Train the OCR service to avoid errors next time it processes similar data. |[Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md) |
| Connect or remove incoming document records for any non-posted sales or purchase document and to any customer, vendor, or general ledger entry from the document or entry. |[Create Incoming Document Records Directly from Documents and Entries](across-how-connect-disconnect-income-document-records.md) |
| From the **Chart of Accounts** and **General Ledger Entries** pages, use a search function to find general ledger entries for posted documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files. |[Find Posted Documents without Incoming Document Records](across-how-find-posted-documents-without-income-document-records.md) |
| Get better overview by setting incoming document records to Processed to remove them from the default view. |[Manage Many Incoming Document Records](across-how-manage-many-income-document-records.md) |

## <a name="see-also"></a>See Also
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
