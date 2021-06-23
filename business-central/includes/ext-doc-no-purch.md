---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: 59376b96dcd6f755040b07784ceca53e157bcf14
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116014"
---
On purchase documents and journals, you can specify a document number that refers to the supplier's numbering system. Use this field to record the number that the supplier assigned to the order, invoice, or credit memo. You can then use the number later if, for some reason, you need to search for the posted entry using this number.

The **Ext. Doc. No. Mandatory** field in the **Purchases & Payables Setup** page specifies whether it is mandatory to enter an external document number in the following situations:

* In the **Supplier Invoice No.** field, **Supplier Order No.** field, or the **Supplier Cr. Memo No.** field on a purchase header

* In the **External Document No.** field on a general journal line, where the **Document Type** field is set to *Invoice*, *Credit Memo*, or *Finance Charge Memo*, and the **Account Type** field is set to *Supplier*.

If you select this field, it will not be possible to post an invoice, a credit memo, or the type of general journal line described above without an external document number.

The external document number is included in posted documents where you can search by the relevant number. You can also search using the external document number when navigating on supplier ledger entries.

A different way to handle external document numbers is to use the **Your Reference** field. If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields. But the field is not available on journal lines.
