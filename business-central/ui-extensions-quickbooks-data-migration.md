---
title: Using the QuickBooks Migration Extension | Microsoft Docs
description: Describes how to use the extension to import customers, vendors, items, and accounts from QuickBooks Desktop to Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 583f6947acd3778710f0889736439322d9179ce6
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="the-quickbooks-data-migration-extension"></a><span data-ttu-id="04e6a-103">The QuickBooks Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="04e6a-103">The QuickBooks Data Migration Extension</span></span>
<span data-ttu-id="04e6a-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="04e6a-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="04e6a-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="04e6a-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
<span data-ttu-id="04e6a-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="04e6a-106">For more information, see [Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md).</span></span>

## <a name="exporting-data-from-quickbooks-desktop"></a><span data-ttu-id="04e6a-107">Exporting Data from QuickBooks Desktop</span><span class="sxs-lookup"><span data-stu-id="04e6a-107">Exporting Data from QuickBooks Desktop</span></span>
<span data-ttu-id="04e6a-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span><span class="sxs-lookup"><span data-stu-id="04e6a-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span></span> <span data-ttu-id="04e6a-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="04e6a-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="04e6a-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="04e6a-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span></span>  
<span data-ttu-id="04e6a-111">In QuickBooks, the File menu includes a utility to export lists.</span><span class="sxs-lookup"><span data-stu-id="04e6a-111">In QuickBooks, the File menu includes a utility to export lists.</span></span> <span data-ttu-id="04e6a-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span><span class="sxs-lookup"><span data-stu-id="04e6a-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span></span>

* <span data-ttu-id="04e6a-113">Customer List</span><span class="sxs-lookup"><span data-stu-id="04e6a-113">Customer List</span></span>  
* <span data-ttu-id="04e6a-114">Vendor List</span><span class="sxs-lookup"><span data-stu-id="04e6a-114">Vendor List</span></span>  
* <span data-ttu-id="04e6a-115">Item List</span><span class="sxs-lookup"><span data-stu-id="04e6a-115">Item List</span></span>  
* <span data-ttu-id="04e6a-116">Account List</span><span class="sxs-lookup"><span data-stu-id="04e6a-116">Account List</span></span>  

<span data-ttu-id="04e6a-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="04e6a-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="finding-the-quickbooks-data-migration-extension"></a><span data-ttu-id="04e6a-118">Finding the QuickBooks Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="04e6a-118">Finding the QuickBooks Data Migration Extension</span></span>
<span data-ttu-id="04e6a-119">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="04e6a-119">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span></span> <span data-ttu-id="04e6a-120">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="04e6a-120">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Assisted Setup**, and then choose the related link.</span></span> <span data-ttu-id="04e6a-121">Choose **Migrate business data**, and then follow the steps in the guide.</span><span class="sxs-lookup"><span data-stu-id="04e6a-121">Choose **Migrate business data**, and then follow the steps in the guide.</span></span>  

## <a name="see-also"></a><span data-ttu-id="04e6a-122">See Also</span><span class="sxs-lookup"><span data-stu-id="04e6a-122">See Also</span></span>
[<span data-ttu-id="04e6a-123">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="04e6a-123">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="04e6a-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="04e6a-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  

