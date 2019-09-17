---
title: Posting Sales Documents | Microsoft Docs
description: Learn about the different posting functions to post sales documents, and how you can update posted documents.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 08/27/2019
ms.author: sgroespe
ms.openlocfilehash: a2eb27a541033b755b9ab9d4ea9156bf7de9cab4
ms.sourcegitcommit: f46793abdb3efd8384c10eb7992e076383251f2c
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/27/2019
ms.locfileid: "1921437"
---
# <a name="posting-sales"></a><span data-ttu-id="2b8ac-103">Posting Sales</span><span class="sxs-lookup"><span data-stu-id="2b8ac-103">Posting Sales</span></span>
<span data-ttu-id="2b8ac-104">Under the **Posting** menu in a sales document, you can choose between the following posting functions:</span><span class="sxs-lookup"><span data-stu-id="2b8ac-104">Under the **Posting** menu in a sales document, you can choose between the following posting functions:</span></span>

* <span data-ttu-id="2b8ac-105">**Post**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-105">**Post**</span></span>
* <span data-ttu-id="2b8ac-106">**Post and New**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-106">**Post and New**</span></span>
* <span data-ttu-id="2b8ac-107">**Post and Send**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-107">**Post and Send**</span></span>
* <span data-ttu-id="2b8ac-108">**Preview Posting**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-108">**Preview Posting**</span></span>
* <span data-ttu-id="2b8ac-109">**Draft Invoice**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-109">**Draft Invoice**</span></span>
* <span data-ttu-id="2b8ac-110">**Pro Forma Invoice**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-110">**Pro Forma Invoice**</span></span>
* <span data-ttu-id="2b8ac-111">**Test Report**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-111">**Test Report**</span></span>

<span data-ttu-id="2b8ac-112">When you have completed all the lines and entered all the information on the sales order, you can post it.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-112">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="2b8ac-113">This creates a shipment and an invoice.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-113">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="2b8ac-114">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-114">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="2b8ac-115">For each sales order, a sales entry is created in the **G/L Entry** table.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-115">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="2b8ac-116">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-116">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="2b8ac-117">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-117">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="2b8ac-118">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-118">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field on the **Sales & Receivables Setup** page.</span></span>

<span data-ttu-id="2b8ac-119">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span><span class="sxs-lookup"><span data-stu-id="2b8ac-119">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="2b8ac-120">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-120">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="2b8ac-121">When you post an order, you can create both a shipment and an invoice.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-121">When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="2b8ac-122">These can be done at the same time or independently.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-122">These can be done at the same time or independently.</span></span> <span data-ttu-id="2b8ac-123">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-123">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="2b8ac-124">Note that you cannot create an invoice for something that is not shipped.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-124">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="2b8ac-125">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-125">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span>

<span data-ttu-id="2b8ac-126">When the posting is completed, the posted sales lines are removed from the order.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-126">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="2b8ac-127">A message tells you when the posting is completed.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-127">A message tells you when the posting is completed.</span></span> <span data-ttu-id="2b8ac-128">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-128">After this, you will be able to see the posted entries in the various pages that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** pages.</span></span>  

<span data-ttu-id="2b8ac-129">You can edit certain fields on posted sales documents, such as the **Package Tracking No.**</span><span class="sxs-lookup"><span data-stu-id="2b8ac-129">You can edit certain fields on posted sales documents, such as the **Package Tracking No.**</span></span> <span data-ttu-id="2b8ac-130">field.</span><span class="sxs-lookup"><span data-stu-id="2b8ac-130">field.</span></span> <span data-ttu-id="2b8ac-131">For more information, see [Edit Posted Documents](across-edit-posted-document.md).</span><span class="sxs-lookup"><span data-stu-id="2b8ac-131">For more information, see [Edit Posted Documents](across-edit-posted-document.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="2b8ac-132">See Also</span><span class="sxs-lookup"><span data-stu-id="2b8ac-132">See Also</span></span>
[<span data-ttu-id="2b8ac-133">Sales</span><span class="sxs-lookup"><span data-stu-id="2b8ac-133">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="2b8ac-134">Edit Posted Documents</span><span class="sxs-lookup"><span data-stu-id="2b8ac-134">Edit Posted Documents</span></span>](across-edit-posted-document.md)  
[<span data-ttu-id="2b8ac-135">Send Documents by Email</span><span class="sxs-lookup"><span data-stu-id="2b8ac-135">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="2b8ac-136">Correct or Cancel Unpaid Sales Invoices</span><span class="sxs-lookup"><span data-stu-id="2b8ac-136">Correct or Cancel Unpaid Sales Invoices</span></span>](sales-how-correct-cancel-sales-invoice.md)  
[<span data-ttu-id="2b8ac-137">Using Tell Me to Find Features and Information</span><span class="sxs-lookup"><span data-stu-id="2b8ac-137">Using Tell Me to Find Features and Information</span></span>](ui-search.md)  
<span data-ttu-id="2b8ac-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2b8ac-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
