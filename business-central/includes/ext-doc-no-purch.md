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
<span data-ttu-id="5c8ab-101">On purchase documents and journals, you can specify a document number that refers to the supplier's numbering system.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-101">On purchase documents and journals, you can specify a document number that refers to the vendor's numbering system.</span></span> <span data-ttu-id="5c8ab-102">Use this field to record the number that the supplier assigned to the order, invoice, or credit memo.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-102">Use this field to record the number that the vendor assigned to the order, invoice, or credit memo.</span></span> <span data-ttu-id="5c8ab-103">You can then use the number later if, for some reason, you need to search for the posted entry using this number.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-103">You can then use the number later if, for some reason, you need to search for the posted entry using this number.</span></span>

<span data-ttu-id="5c8ab-104">The **Ext. Doc. No. Mandatory** field in the **Purchases & Payables Setup** page specifies whether it is mandatory to enter an external document number in the following situations:</span><span class="sxs-lookup"><span data-stu-id="5c8ab-104">The **Ext. Doc. No. Mandatory** field in the **Purchases & Payables Setup** page specifies whether it is mandatory to enter an external document number in the following situations:</span></span>

* <span data-ttu-id="5c8ab-105">In the **Supplier Invoice No.** field, **Supplier Order No.**</span><span class="sxs-lookup"><span data-stu-id="5c8ab-105">In the **Vendor Invoice No.** field, **Vendor Order No.**</span></span> <span data-ttu-id="5c8ab-106">field, or the **Supplier Cr. Memo No.**</span><span class="sxs-lookup"><span data-stu-id="5c8ab-106">field, or the **Vendor Cr. Memo No.**</span></span> <span data-ttu-id="5c8ab-107">field on a purchase header</span><span class="sxs-lookup"><span data-stu-id="5c8ab-107">field on a purchase header</span></span>

* <span data-ttu-id="5c8ab-108">In the **External Document No.** field on a general journal line, where the **Document Type** field is set to *Invoice*, *Credit Memo*, or *Finance Charge Memo*, and the **Account Type** field is set to *Supplier*.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-108">In the **External Document No.** field on a general journal line, where the **Document Type** field is set to *Invoice*, *Credit Memo*, or *Finance Charge Memo*, and the **Account Type** field is set to *Vendor*.</span></span>

<span data-ttu-id="5c8ab-109">If you select this field, it will not be possible to post an invoice, a credit memo, or the type of general journal line described above without an external document number.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-109">If you select this field, it will not be possible to post an invoice, a credit memo, or the type of general journal line described above without an external document number.</span></span>

<span data-ttu-id="5c8ab-110">The external document number is included in posted documents where you can search by the relevant number.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-110">The external document number is included in posted documents where you can search by the relevant number.</span></span> <span data-ttu-id="5c8ab-111">You can also search using the external document number when navigating on supplier ledger entries.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-111">You can also search using the external document number when navigating on vendor ledger entries.</span></span>

<span data-ttu-id="5c8ab-112">A different way to handle external document numbers is to use the **Your Reference** field.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-112">A different way to handle external document numbers is to use the **Your Reference** field.</span></span> <span data-ttu-id="5c8ab-113">If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-113">If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields.</span></span> <span data-ttu-id="5c8ab-114">But the field is not available on journal lines.</span><span class="sxs-lookup"><span data-stu-id="5c8ab-114">But the field is not available on journal lines.</span></span>
