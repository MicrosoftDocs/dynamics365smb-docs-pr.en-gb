---
title: How to Print VAT Audit Reports | Microsoft Docs
description: All vendors must export the data required for auditing in a Content Separated Value (CSV) file format.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 323de29c489a9ef22e91d83f89d51983da40f943
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241212"
---
# <a name="print-vat-audit-reports"></a><span data-ttu-id="26581-103">Print VAT Audit Reports</span><span class="sxs-lookup"><span data-stu-id="26581-103">Print VAT Audit Reports</span></span>
<span data-ttu-id="26581-104">All vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span><span class="sxs-lookup"><span data-stu-id="26581-104">All vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span></span> <span data-ttu-id="26581-105">The following reports comply with this requirement:</span><span class="sxs-lookup"><span data-stu-id="26581-105">The following reports comply with this requirement:</span></span>  

-   <span data-ttu-id="26581-106">**VAT Audit**  report – This report is used for VAT auditing.</span><span class="sxs-lookup"><span data-stu-id="26581-106">**VAT Audit**  report – This report is used for VAT auditing.</span></span>  
-   <span data-ttu-id="26581-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span><span class="sxs-lookup"><span data-stu-id="26581-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span></span> <span data-ttu-id="26581-108">It also displays the difference in VAT amounts for the tax authorities.</span><span class="sxs-lookup"><span data-stu-id="26581-108">It also displays the difference in VAT amounts for the tax authorities.</span></span>  

## <a name="to-print-the-vat-audit-report"></a><span data-ttu-id="26581-109">To print the VAT audit report</span><span class="sxs-lookup"><span data-stu-id="26581-109">To print the VAT audit report</span></span>  

1.  <span data-ttu-id="26581-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Audit**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="26581-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Audit**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="26581-111">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="26581-111">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="26581-112">Field</span><span class="sxs-lookup"><span data-stu-id="26581-112">Field</span></span>|<span data-ttu-id="26581-113">Description</span><span class="sxs-lookup"><span data-stu-id="26581-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="26581-114">**Export Customers**</span><span class="sxs-lookup"><span data-stu-id="26581-114">**Export Customers**</span></span>|<span data-ttu-id="26581-115">Select to export the file to the **Customer** table.</span><span class="sxs-lookup"><span data-stu-id="26581-115">Select to export the file to the **Customer** table.</span></span>|  
    |<span data-ttu-id="26581-116">**Export Open Payments**</span><span class="sxs-lookup"><span data-stu-id="26581-116">**Export Open Payments**</span></span>|<span data-ttu-id="26581-117">Select to export the open credit entries.</span><span class="sxs-lookup"><span data-stu-id="26581-117">Select to export the open credit entries.</span></span>|  
    |<span data-ttu-id="26581-118">**Export Late Invoicing**</span><span class="sxs-lookup"><span data-stu-id="26581-118">**Export Late Invoicing**</span></span>|<span data-ttu-id="26581-119">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span><span class="sxs-lookup"><span data-stu-id="26581-119">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span></span>|  
    |<span data-ttu-id="26581-120">**Late Invoice Delay (Days)**</span><span class="sxs-lookup"><span data-stu-id="26581-120">**Late Invoice Delay (Days)**</span></span>|<span data-ttu-id="26581-121">Enter the number of days between the invoice issue date and the payment received date.</span><span class="sxs-lookup"><span data-stu-id="26581-121">Enter the number of days between the invoice issue date and the payment received date.</span></span> <span data-ttu-id="26581-122">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span><span class="sxs-lookup"><span data-stu-id="26581-122">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span></span>|  
    |<span data-ttu-id="26581-123">**Export Vendors**</span><span class="sxs-lookup"><span data-stu-id="26581-123">**Export Vendors**</span></span>|<span data-ttu-id="26581-124">Select to export the file to the **Vendor** table.</span><span class="sxs-lookup"><span data-stu-id="26581-124">Select to export the file to the **Vendor** table.</span></span>|  
    |<span data-ttu-id="26581-125">**Export VAT Entries**</span><span class="sxs-lookup"><span data-stu-id="26581-125">**Export VAT Entries**</span></span>|<span data-ttu-id="26581-126">Select to export the entries in the **VAT Entry** table.</span><span class="sxs-lookup"><span data-stu-id="26581-126">Select to export the entries in the **VAT Entry** table.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="26581-127">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="26581-127">You must select at least one check box in this page.</span></span>  

3.  <span data-ttu-id="26581-128">To export the file, choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="26581-128">To export the file, choose the **OK** button.</span></span>  

    <span data-ttu-id="26581-129">The VAT audit information is exported.</span><span class="sxs-lookup"><span data-stu-id="26581-129">The VAT audit information is exported.</span></span> <span data-ttu-id="26581-130">You can save the data to a file, or open the file in the appropriate program.</span><span class="sxs-lookup"><span data-stu-id="26581-130">You can save the data to a file, or open the file in the appropriate program.</span></span>  

## <a name="to-print-the-vat-entry-exception-report"></a><span data-ttu-id="26581-131">To print the VAT entry exception report</span><span class="sxs-lookup"><span data-stu-id="26581-131">To print the VAT entry exception report</span></span>  

1.  <span data-ttu-id="26581-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Entry Exception Report**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="26581-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Entry Exception Report**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="26581-133">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="26581-133">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="26581-134">Field</span><span class="sxs-lookup"><span data-stu-id="26581-134">Field</span></span>|<span data-ttu-id="26581-135">Description</span><span class="sxs-lookup"><span data-stu-id="26581-135">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="26581-136">**VAT Base Discount**</span><span class="sxs-lookup"><span data-stu-id="26581-136">**VAT Base Discount**</span></span>|<span data-ttu-id="26581-137">Select if you want to enter a value in the **VAT Base Discount %** field.</span><span class="sxs-lookup"><span data-stu-id="26581-137">Select if you want to enter a value in the **VAT Base Discount %** field.</span></span>|  
    |<span data-ttu-id="26581-138">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="26581-138">**Manual VAT Difference**</span></span>|<span data-ttu-id="26581-139">Select if you want to enter a value in the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="26581-139">Select if you want to enter a value in the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="26581-140">**VAT Calculation Types**</span><span class="sxs-lookup"><span data-stu-id="26581-140">**VAT Calculation Types**</span></span>|<span data-ttu-id="26581-141">Select to determine the VAT calculation type.</span><span class="sxs-lookup"><span data-stu-id="26581-141">Select to determine the VAT calculation type.</span></span>|  
    |<span data-ttu-id="26581-142">**VAT Rate**</span><span class="sxs-lookup"><span data-stu-id="26581-142">**VAT Rate**</span></span>|<span data-ttu-id="26581-143">Select to determine the VAT rate for a particular journal line.</span><span class="sxs-lookup"><span data-stu-id="26581-143">Select to determine the VAT rate for a particular journal line.</span></span>|  
    |<span data-ttu-id="26581-144">**VAT Base Discount %**</span><span class="sxs-lookup"><span data-stu-id="26581-144">**VAT Base Discount %**</span></span>|<span data-ttu-id="26581-145">Enter a value in this field if you have selected the **VAT Base Discount** field.</span><span class="sxs-lookup"><span data-stu-id="26581-145">Enter a value in this field if you have selected the **VAT Base Discount** field.</span></span>|  
    |<span data-ttu-id="26581-146">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="26581-146">**Manual VAT Difference**</span></span>|<span data-ttu-id="26581-147">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="26581-147">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="26581-148">**VAT Rate % Difference**</span><span class="sxs-lookup"><span data-stu-id="26581-148">**VAT Rate % Difference**</span></span>|<span data-ttu-id="26581-149">Specify the maximum VAT rate difference.</span><span class="sxs-lookup"><span data-stu-id="26581-149">Specify the maximum VAT rate difference.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="26581-150">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="26581-150">You must select at least one check box in this page.</span></span>  

3.  <span data-ttu-id="26581-151">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span><span class="sxs-lookup"><span data-stu-id="26581-151">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span>  

## <a name="see-also"></a><span data-ttu-id="26581-152">See Also</span><span class="sxs-lookup"><span data-stu-id="26581-152">See Also</span></span>  
[<span data-ttu-id="26581-153">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="26581-153">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)
