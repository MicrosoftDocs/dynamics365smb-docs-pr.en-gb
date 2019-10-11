---
title: Importing Many Item Pictures from a ZIP File| Microsoft Docs
description: You can import multiple item pictures in one go. Simply name your picture files with names corresponding to your item numbers, compress them to a zip file, and then use the Import Item Pictures page to manage which item pictures to import.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: product, image
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: cfb80821177c0860413526b5bc529fa1bdeedf7b
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2309853"
---
# <a name="import-multiple-item-pictures"></a><span data-ttu-id="28653-104">Import Multiple Item Pictures</span><span class="sxs-lookup"><span data-stu-id="28653-104">Import Multiple Item Pictures</span></span>
<span data-ttu-id="28653-105">You can import multiple item pictures in one go.</span><span class="sxs-lookup"><span data-stu-id="28653-105">You can import multiple item pictures in one go.</span></span> <span data-ttu-id="28653-106">Simply name your picture files with names corresponding to your item numbers, compress them to a ZIP file, and then use the **Import Item Pictures** page to manage which item pictures to import.</span><span class="sxs-lookup"><span data-stu-id="28653-106">Simply name your picture files with names corresponding to your item numbers, compress them to a ZIP file, and then use the **Import Item Pictures** page to manage which item pictures to import.</span></span>

<span data-ttu-id="28653-107">All common file formats are supported.</span><span class="sxs-lookup"><span data-stu-id="28653-107">All common file formats are supported.</span></span>

## <a name="to-name-picture-files-by-the-item-names-and-prepare-the-zip-file"></a><span data-ttu-id="28653-108">To name picture files by the item names and prepare the ZIP file</span><span class="sxs-lookup"><span data-stu-id="28653-108">To name picture files by the item names and prepare the ZIP file</span></span>
1. <span data-ttu-id="28653-109">At the location where your item pictures are stored, name each files according to the number of the related item.</span><span class="sxs-lookup"><span data-stu-id="28653-109">At the location where your item pictures are stored, name each files according to the number of the related item.</span></span> <span data-ttu-id="28653-110">For example:</span><span class="sxs-lookup"><span data-stu-id="28653-110">For example:</span></span>

    |<span data-ttu-id="28653-111">Item No.</span><span class="sxs-lookup"><span data-stu-id="28653-111">Item No.</span></span>|<span data-ttu-id="28653-112">File Name</span><span class="sxs-lookup"><span data-stu-id="28653-112">File Name</span></span>|
    |-|-|
    |<span data-ttu-id="28653-113">1000</span><span class="sxs-lookup"><span data-stu-id="28653-113">1000</span></span>|<span data-ttu-id="28653-114">1000.bmp</span><span class="sxs-lookup"><span data-stu-id="28653-114">1000.bmp</span></span>|
    |<span data-ttu-id="28653-115">1001</span><span class="sxs-lookup"><span data-stu-id="28653-115">1001</span></span>|<span data-ttu-id="28653-116">1001.bmp</span><span class="sxs-lookup"><span data-stu-id="28653-116">1001.bmp</span></span>|
    |<span data-ttu-id="28653-117">1002</span><span class="sxs-lookup"><span data-stu-id="28653-117">1002</span></span>|<span data-ttu-id="28653-118">1002.bmp</span><span class="sxs-lookup"><span data-stu-id="28653-118">1002.bmp</span></span>|

2. <span data-ttu-id="28653-119">Collect all the files in a ZIP file.</span><span class="sxs-lookup"><span data-stu-id="28653-119">Collect all the files in a ZIP file.</span></span> <span data-ttu-id="28653-120">For example, in Windows Explorer, select the files, and then choose **Send to**, **Compressed (zipped) folder**.</span><span class="sxs-lookup"><span data-stu-id="28653-120">For example, in Windows Explorer, select the files, and then choose **Send to**, **Compressed (zipped) folder**.</span></span>     

## <a name="to-import-item-pictures"></a><span data-ttu-id="28653-121">To import item pictures</span><span class="sxs-lookup"><span data-stu-id="28653-121">To import item pictures</span></span>
1. <span data-ttu-id="28653-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="28653-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="28653-123">Choose the **Import Item Pictures** action.</span><span class="sxs-lookup"><span data-stu-id="28653-123">Choose the **Import Item Pictures** action.</span></span>
3. <span data-ttu-id="28653-124">In the **Select a ZIP file** field, select the relevant ZIP folder, and then choose the **Open** button.</span><span class="sxs-lookup"><span data-stu-id="28653-124">In the **Select a ZIP file** field, select the relevant ZIP folder, and then choose the **Open** button.</span></span>

    <span data-ttu-id="28653-125">A line for each item and picture is created on the **Import Item Pictures** page.</span><span class="sxs-lookup"><span data-stu-id="28653-125">A line for each item and picture is created on the **Import Item Pictures** page.</span></span>

    > [!NOTE]
    > <span data-ttu-id="28653-126">For item cards that already have a picture, the **Picture Already Exists** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="28653-126">For item cards that already have a picture, the **Picture Already Exists** check box is selected.</span></span> <span data-ttu-id="28653-127">If you do not want any existing pictures to be replaced, deselect the **Replace Pictures** check box.</span><span class="sxs-lookup"><span data-stu-id="28653-127">If you do not want any existing pictures to be replaced, deselect the **Replace Pictures** check box.</span></span> <span data-ttu-id="28653-128">If you do not want individual existing pictures to be replaced, delete the lines in question.</span><span class="sxs-lookup"><span data-stu-id="28653-128">If you do not want individual existing pictures to be replaced, delete the lines in question.</span></span>

3. <span data-ttu-id="28653-129">Choose the **Import Pictures** action.</span><span class="sxs-lookup"><span data-stu-id="28653-129">Choose the **Import Pictures** action.</span></span>

<span data-ttu-id="28653-130">The **Import Status** field is updated to show if the picture import was skipped or completed.</span><span class="sxs-lookup"><span data-stu-id="28653-130">The **Import Status** field is updated to show if the picture import was skipped or completed.</span></span>       

## <a name="see-also"></a><span data-ttu-id="28653-131">See Also</span><span class="sxs-lookup"><span data-stu-id="28653-131">See Also</span></span>
[<span data-ttu-id="28653-132">Register New Items</span><span class="sxs-lookup"><span data-stu-id="28653-132">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="28653-133">Create Number Series</span><span class="sxs-lookup"><span data-stu-id="28653-133">Create Number Series</span></span>](ui-create-number-series.md)  
[<span data-ttu-id="28653-134">Inventory</span><span class="sxs-lookup"><span data-stu-id="28653-134">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="28653-135">Purchasing</span><span class="sxs-lookup"><span data-stu-id="28653-135">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="28653-136">Sales</span><span class="sxs-lookup"><span data-stu-id="28653-136">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="28653-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="28653-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
