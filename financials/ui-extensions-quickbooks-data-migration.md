---
title: Using the QuickBooks Migration Extension | Microsoft Docs
description: Describes how to use the extension to import customers, vendors, items, and accounts from QuickBooks Desktop to Dynamics 365 for Financials.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 37d90316ea0be5489fb5abe33645de3fe0d3cf90
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-365-for-financials"></a><span data-ttu-id="95b39-103">The QuickBooks Data Migration Extension for Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="95b39-103">The QuickBooks Data Migration Extension for Dynamics 365 for Financials</span></span>
<span data-ttu-id="95b39-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="95b39-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="95b39-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="95b39-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
<span data-ttu-id="95b39-106">For more information, see [Importing Business Data from Other Finance Systems](upload-data.md).</span><span class="sxs-lookup"><span data-stu-id="95b39-106">For more information, see [Importing Business Data from Other Finance Systems](upload-data.md).</span></span>

## <a name="exporting-data-from-quickbooks"></a><span data-ttu-id="95b39-107">Exporting Data from QuickBooks</span><span class="sxs-lookup"><span data-stu-id="95b39-107">Exporting Data from QuickBooks</span></span>
<span data-ttu-id="95b39-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span><span class="sxs-lookup"><span data-stu-id="95b39-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span></span> <span data-ttu-id="95b39-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="95b39-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="95b39-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="95b39-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span></span>  
<span data-ttu-id="95b39-111">In QuickBooks, the File menu includes a utility to export lists.</span><span class="sxs-lookup"><span data-stu-id="95b39-111">In QuickBooks, the File menu includes a utility to export lists.</span></span> <span data-ttu-id="95b39-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span><span class="sxs-lookup"><span data-stu-id="95b39-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span></span>

* <span data-ttu-id="95b39-113">Customer List</span><span class="sxs-lookup"><span data-stu-id="95b39-113">Customer List</span></span>  
* <span data-ttu-id="95b39-114">Vendor List</span><span class="sxs-lookup"><span data-stu-id="95b39-114">Vendor List</span></span>  
* <span data-ttu-id="95b39-115">Item List</span><span class="sxs-lookup"><span data-stu-id="95b39-115">Item List</span></span>  
* <span data-ttu-id="95b39-116">Account List</span><span class="sxs-lookup"><span data-stu-id="95b39-116">Account List</span></span>  

<span data-ttu-id="95b39-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="95b39-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="see-also"></a><span data-ttu-id="95b39-118">See Also</span><span class="sxs-lookup"><span data-stu-id="95b39-118">See Also</span></span>
[<span data-ttu-id="95b39-119">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="95b39-119">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="95b39-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="95b39-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  

