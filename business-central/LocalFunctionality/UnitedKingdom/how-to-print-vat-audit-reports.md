---
title: How to Print VAT Audit Reports | Microsoft Docs
description: All vendors must export the data required for auditing in a Content Separated Value (CSV) file format.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 0ee001f24f5a4d5d326a3db94076fcfeb6318e45
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881283"
---
# <a name="print-vat-audit-reports"></a><span data-ttu-id="01097-103">Print VAT Audit Reports</span><span class="sxs-lookup"><span data-stu-id="01097-103">Print VAT Audit Reports</span></span>
<span data-ttu-id="01097-104">All vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span><span class="sxs-lookup"><span data-stu-id="01097-104">All vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span></span> <span data-ttu-id="01097-105">The following reports comply with this requirement:</span><span class="sxs-lookup"><span data-stu-id="01097-105">The following reports comply with this requirement:</span></span>  

-   <span data-ttu-id="01097-106">**VAT Audit**  report – This report is used for VAT auditing.</span><span class="sxs-lookup"><span data-stu-id="01097-106">**VAT Audit**  report – This report is used for VAT auditing.</span></span>  
-   <span data-ttu-id="01097-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span><span class="sxs-lookup"><span data-stu-id="01097-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span></span> <span data-ttu-id="01097-108">It also displays the difference in VAT amounts for the tax authorities.</span><span class="sxs-lookup"><span data-stu-id="01097-108">It also displays the difference in VAT amounts for the tax authorities.</span></span>  

## <a name="to-print-the-vat-audit-report"></a><span data-ttu-id="01097-109">To print the VAT audit report</span><span class="sxs-lookup"><span data-stu-id="01097-109">To print the VAT audit report</span></span>  

1.  <span data-ttu-id="01097-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Audit**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="01097-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Audit**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="01097-111">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="01097-111">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="01097-112">Field</span><span class="sxs-lookup"><span data-stu-id="01097-112">Field</span></span>|<span data-ttu-id="01097-113">Description</span><span class="sxs-lookup"><span data-stu-id="01097-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="01097-114">**Export Customers**</span><span class="sxs-lookup"><span data-stu-id="01097-114">**Export Customers**</span></span>|<span data-ttu-id="01097-115">Select to export the file to the **Customer** table.</span><span class="sxs-lookup"><span data-stu-id="01097-115">Select to export the file to the **Customer** table.</span></span>|  
    |<span data-ttu-id="01097-116">**Export Open Payments**</span><span class="sxs-lookup"><span data-stu-id="01097-116">**Export Open Payments**</span></span>|<span data-ttu-id="01097-117">Select to export the open credit entries.</span><span class="sxs-lookup"><span data-stu-id="01097-117">Select to export the open credit entries.</span></span>|  
    |<span data-ttu-id="01097-118">**Export Late Invoicing**</span><span class="sxs-lookup"><span data-stu-id="01097-118">**Export Late Invoicing**</span></span>|<span data-ttu-id="01097-119">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span><span class="sxs-lookup"><span data-stu-id="01097-119">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span></span>|  
    |<span data-ttu-id="01097-120">**Late Invoice Delay (Days)**</span><span class="sxs-lookup"><span data-stu-id="01097-120">**Late Invoice Delay (Days)**</span></span>|<span data-ttu-id="01097-121">Enter the number of days between the invoice issue date and the payment received date.</span><span class="sxs-lookup"><span data-stu-id="01097-121">Enter the number of days between the invoice issue date and the payment received date.</span></span> <span data-ttu-id="01097-122">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span><span class="sxs-lookup"><span data-stu-id="01097-122">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span></span>|  
    |<span data-ttu-id="01097-123">**Export Vendors**</span><span class="sxs-lookup"><span data-stu-id="01097-123">**Export Vendors**</span></span>|<span data-ttu-id="01097-124">Select to export the file to the **Vendor** table.</span><span class="sxs-lookup"><span data-stu-id="01097-124">Select to export the file to the **Vendor** table.</span></span>|  
    |<span data-ttu-id="01097-125">**Export VAT Entries**</span><span class="sxs-lookup"><span data-stu-id="01097-125">**Export VAT Entries**</span></span>|<span data-ttu-id="01097-126">Select to export the entries in the **VAT Entry** table.</span><span class="sxs-lookup"><span data-stu-id="01097-126">Select to export the entries in the **VAT Entry** table.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="01097-127">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="01097-127">You must select at least one check box in this page.</span></span>  

3.  <span data-ttu-id="01097-128">To export the file, choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="01097-128">To export the file, choose the **OK** button.</span></span>  

    <span data-ttu-id="01097-129">The VAT audit information is exported.</span><span class="sxs-lookup"><span data-stu-id="01097-129">The VAT audit information is exported.</span></span> <span data-ttu-id="01097-130">You can save the data to a file, or open the file in the appropriate program.</span><span class="sxs-lookup"><span data-stu-id="01097-130">You can save the data to a file, or open the file in the appropriate program.</span></span>  

## <a name="to-print-the-vat-entry-exception-report"></a><span data-ttu-id="01097-131">To print the VAT entry exception report</span><span class="sxs-lookup"><span data-stu-id="01097-131">To print the VAT entry exception report</span></span>  

1.  <span data-ttu-id="01097-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Entry Exception Report**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="01097-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Entry Exception Report**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="01097-133">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="01097-133">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="01097-134">Field</span><span class="sxs-lookup"><span data-stu-id="01097-134">Field</span></span>|<span data-ttu-id="01097-135">Description</span><span class="sxs-lookup"><span data-stu-id="01097-135">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="01097-136">**VAT Base Discount**</span><span class="sxs-lookup"><span data-stu-id="01097-136">**VAT Base Discount**</span></span>|<span data-ttu-id="01097-137">Select if you want to enter a value in the **VAT Base Discount %** field.</span><span class="sxs-lookup"><span data-stu-id="01097-137">Select if you want to enter a value in the **VAT Base Discount %** field.</span></span>|  
    |<span data-ttu-id="01097-138">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="01097-138">**Manual VAT Difference**</span></span>|<span data-ttu-id="01097-139">Select if you want to enter a value in the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="01097-139">Select if you want to enter a value in the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="01097-140">**VAT Calculation Types**</span><span class="sxs-lookup"><span data-stu-id="01097-140">**VAT Calculation Types**</span></span>|<span data-ttu-id="01097-141">Select to determine the VAT calculation type.</span><span class="sxs-lookup"><span data-stu-id="01097-141">Select to determine the VAT calculation type.</span></span>|  
    |<span data-ttu-id="01097-142">**VAT Rate**</span><span class="sxs-lookup"><span data-stu-id="01097-142">**VAT Rate**</span></span>|<span data-ttu-id="01097-143">Select to determine the VAT rate for a particular journal line.</span><span class="sxs-lookup"><span data-stu-id="01097-143">Select to determine the VAT rate for a particular journal line.</span></span>|  
    |<span data-ttu-id="01097-144">**VAT Base Discount %**</span><span class="sxs-lookup"><span data-stu-id="01097-144">**VAT Base Discount %**</span></span>|<span data-ttu-id="01097-145">Enter a value in this field if you have selected the **VAT Base Discount** field.</span><span class="sxs-lookup"><span data-stu-id="01097-145">Enter a value in this field if you have selected the **VAT Base Discount** field.</span></span>|  
    |<span data-ttu-id="01097-146">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="01097-146">**Manual VAT Difference**</span></span>|<span data-ttu-id="01097-147">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="01097-147">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="01097-148">**VAT Rate % Difference**</span><span class="sxs-lookup"><span data-stu-id="01097-148">**VAT Rate % Difference**</span></span>|<span data-ttu-id="01097-149">Specify the maximum VAT rate difference.</span><span class="sxs-lookup"><span data-stu-id="01097-149">Specify the maximum VAT rate difference.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="01097-150">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="01097-150">You must select at least one check box in this page.</span></span>  

3.  <span data-ttu-id="01097-151">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span><span class="sxs-lookup"><span data-stu-id="01097-151">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span>  

## <a name="see-also"></a><span data-ttu-id="01097-152">See Also</span><span class="sxs-lookup"><span data-stu-id="01097-152">See Also</span></span>  
[<span data-ttu-id="01097-153">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="01097-153">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)
