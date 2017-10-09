---
title: Using the QuickBooks Migration Extension | Microsoft Docs
description: Describes how to use the extension to import customers, vendors, items, and accounts from QuickBooks Desktop to Dynamics 365 for Financials.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 4775c945a7721b8f4e52a187840a585396611e47
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-365-for-financials"></a><span data-ttu-id="73fea-103">The QuickBooks Data Migration Extension for Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="73fea-103">The QuickBooks Data Migration Extension for Dynamics 365 for Financials</span></span>
<span data-ttu-id="73fea-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks Desktop to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="73fea-104">This extension makes it easy to migrate customers, vendors, items, and accounts from QuickBooks Desktop to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="73fea-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="73fea-105">If your business uses QuickBooks today, you can export the relevant information and then open an assisted setup guide to upload the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
<span data-ttu-id="73fea-106">For more information, see [Importing Business Data from Other Finance Systems](upload-data.md).</span><span class="sxs-lookup"><span data-stu-id="73fea-106">For more information, see [Importing Business Data from Other Finance Systems](upload-data.md).</span></span>

## <a name="exporting-data-from-quickbooks-desktop"></a><span data-ttu-id="73fea-107">Exporting Data from QuickBooks Desktop</span><span class="sxs-lookup"><span data-stu-id="73fea-107">Exporting Data from QuickBooks Desktop</span></span>
<span data-ttu-id="73fea-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span><span class="sxs-lookup"><span data-stu-id="73fea-108">You must have exported some or all of your existing customers, vendors, inventory items, and accounts to an Intuit Interchange Format (IIF) file.</span></span> <span data-ttu-id="73fea-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="73fea-109">The QuickBooks Data Migration extension includes a default mapping of QuickBooks data so that you can use your existing data to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="73fea-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="73fea-110">The default mapping will be sufficient in the vast majority of cases, but you can change the mapping in the assisted setup guide.</span></span>  
<span data-ttu-id="73fea-111">In QuickBooks, the File menu includes a utility to export lists.</span><span class="sxs-lookup"><span data-stu-id="73fea-111">In QuickBooks, the File menu includes a utility to export lists.</span></span> <span data-ttu-id="73fea-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span><span class="sxs-lookup"><span data-stu-id="73fea-112">For the purposes of [!INCLUDE[d365fin](includes/d365fin_md.md)], you can export the following lists:</span></span>

* <span data-ttu-id="73fea-113">Customer List</span><span class="sxs-lookup"><span data-stu-id="73fea-113">Customer List</span></span>  
* <span data-ttu-id="73fea-114">Vendor List</span><span class="sxs-lookup"><span data-stu-id="73fea-114">Vendor List</span></span>  
* <span data-ttu-id="73fea-115">Item List</span><span class="sxs-lookup"><span data-stu-id="73fea-115">Item List</span></span>  
* <span data-ttu-id="73fea-116">Account List</span><span class="sxs-lookup"><span data-stu-id="73fea-116">Account List</span></span>  

<span data-ttu-id="73fea-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="73fea-117">The exported data is saved as an IIF file that you can then upload to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="finding-the-quickbooks-data-migration-extension"></a><span data-ttu-id="73fea-118">Finding the QuickBooks Data Migration Extension</span><span class="sxs-lookup"><span data-stu-id="73fea-118">Finding the QuickBooks Data Migration Extension</span></span>
<span data-ttu-id="73fea-119">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="73fea-119">The QuickBooks Data Migration extension is installed and ready to go as an integrated part of the Data Migration assisted setup guide.</span></span> <span data-ttu-id="73fea-120">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="73fea-120">If you are ready to get started now, and have exported your data from QuickBooks, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose the related link.</span></span> <span data-ttu-id="73fea-121">Choose **Migrate business data**, and then follow the steps in the guide.</span><span class="sxs-lookup"><span data-stu-id="73fea-121">Choose **Migrate business data**, and then follow the steps in the guide.</span></span>  

## <a name="see-also"></a><span data-ttu-id="73fea-122">See Also</span><span class="sxs-lookup"><span data-stu-id="73fea-122">See Also</span></span>
[<span data-ttu-id="73fea-123">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="73fea-123">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="73fea-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="73fea-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  

