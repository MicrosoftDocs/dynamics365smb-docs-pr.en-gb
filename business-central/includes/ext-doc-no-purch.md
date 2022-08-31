---
author: edupont04
ms.topic: include
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: f1c6ead7a776d11ccc8917944c3752ec6ac43c66
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2022
ms.locfileid: "8132661"
---
On purchase documents and journals, you can specify a document number that refers to the vendor's numbering system. Use this field to record the number that the vendor assigned to the order, invoice, or credit memo. You can then use the number later if, for some reason, you need to search for the posted entry using this number.

The **Ext. Doc. No. Mandatory** field in the **Purchases & Payables Setup** page specifies whether it is mandatory to enter an external document number in the following situations:

* In the **Vendor Invoice No.** field, **Vendor Order No.** field, or the **Vendor Cr. Memo No.** field on a purchase header

* In the **External Document No.** field on a general journal line, where the **Document Type** field is set to *Invoice*, *Credit Memo*, or *Finance Charge Memo*, and the **Account Type** field is set to *Vendor*.

If you select this field, it will not be possible to post an invoice, a credit memo, or the type of general journal line described above without an external document number.

The external document number is included in posted documents where you can search by the relevant number. You can also search using the external document number when navigating on vendor ledger entries.

A different way to handle external document numbers is to use the **Your Reference** field. If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields. But the field is not available on journal lines.
