---
title: Print VAT Audit Reports
description: Learn how Business Central supports the British requirements for VAT audits.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: ccd98b18b59f101634e68ba0cccc34d407c971e2
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5383420"
---
# <a name="print-vat-audit-reports-in-the-british-version"></a><span data-ttu-id="8be49-103">Print VAT Audit Reports in the British Version</span><span class="sxs-lookup"><span data-stu-id="8be49-103">Print VAT Audit Reports in the British Version</span></span>

<span data-ttu-id="8be49-104">In the United Kingdom, all vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span><span class="sxs-lookup"><span data-stu-id="8be49-104">In the United Kingdom, all vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span></span> <span data-ttu-id="8be49-105">The following reports in the British version of [!INCLUDE [prod_short](../../includes/prod_short.md)] comply with this requirement:</span><span class="sxs-lookup"><span data-stu-id="8be49-105">The following reports in the British version of [!INCLUDE [prod_short](../../includes/prod_short.md)] comply with this requirement:</span></span>  

- <span data-ttu-id="8be49-106">**VAT Audit**  report – This report is used for VAT auditing.</span><span class="sxs-lookup"><span data-stu-id="8be49-106">**VAT Audit**  report – This report is used for VAT auditing.</span></span>  
- <span data-ttu-id="8be49-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span><span class="sxs-lookup"><span data-stu-id="8be49-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span></span> <span data-ttu-id="8be49-108">It also displays the difference in VAT amounts for the tax authorities.</span><span class="sxs-lookup"><span data-stu-id="8be49-108">It also displays the difference in VAT amounts for the tax authorities.</span></span>  

## <a name="to-print-the-vat-audit-report"></a><span data-ttu-id="8be49-109">To print the VAT audit report</span><span class="sxs-lookup"><span data-stu-id="8be49-109">To print the VAT audit report</span></span>  

1. <span data-ttu-id="8be49-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8be49-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8be49-111">Choose the relevant VAT statement template, and then choose OK.</span><span class="sxs-lookup"><span data-stu-id="8be49-111">Choose the relevant VAT statement template, and then choose OK.</span></span>
3. <span data-ttu-id="8be49-112">On the **VAT Statement** page, choose **VAT Audit Report**.</span><span class="sxs-lookup"><span data-stu-id="8be49-112">On the **VAT Statement** page, choose **VAT Audit Report**.</span></span>
4. <span data-ttu-id="8be49-113">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="8be49-113">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="8be49-114">Field</span><span class="sxs-lookup"><span data-stu-id="8be49-114">Field</span></span>|<span data-ttu-id="8be49-115">Description</span><span class="sxs-lookup"><span data-stu-id="8be49-115">Description</span></span>|  
    |-----|-----------|  
    |<span data-ttu-id="8be49-116">**Export Customers**</span><span class="sxs-lookup"><span data-stu-id="8be49-116">**Export Customers**</span></span>|<span data-ttu-id="8be49-117">Select to export the file to the **Customer** table.</span><span class="sxs-lookup"><span data-stu-id="8be49-117">Select to export the file to the **Customer** table.</span></span>|  
    |<span data-ttu-id="8be49-118">**Export Open Payments**</span><span class="sxs-lookup"><span data-stu-id="8be49-118">**Export Open Payments**</span></span>|<span data-ttu-id="8be49-119">Select to export the open credit entries.</span><span class="sxs-lookup"><span data-stu-id="8be49-119">Select to export the open credit entries.</span></span>|  
    |<span data-ttu-id="8be49-120">**Export Late Invoicing**</span><span class="sxs-lookup"><span data-stu-id="8be49-120">**Export Late Invoicing**</span></span>|<span data-ttu-id="8be49-121">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span><span class="sxs-lookup"><span data-stu-id="8be49-121">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span></span>|  
    |<span data-ttu-id="8be49-122">**Late Invoice Delay (Days)**</span><span class="sxs-lookup"><span data-stu-id="8be49-122">**Late Invoice Delay (Days)**</span></span>|<span data-ttu-id="8be49-123">Enter the number of days between the invoice issue date and the payment received date.</span><span class="sxs-lookup"><span data-stu-id="8be49-123">Enter the number of days between the invoice issue date and the payment received date.</span></span> <span data-ttu-id="8be49-124">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span><span class="sxs-lookup"><span data-stu-id="8be49-124">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span></span>|  
    |<span data-ttu-id="8be49-125">**Export Vendors**</span><span class="sxs-lookup"><span data-stu-id="8be49-125">**Export Vendors**</span></span>|<span data-ttu-id="8be49-126">Select to export the file to the **Vendor** table.</span><span class="sxs-lookup"><span data-stu-id="8be49-126">Select to export the file to the **Vendor** table.</span></span>|  
    |<span data-ttu-id="8be49-127">**Export VAT Entries**</span><span class="sxs-lookup"><span data-stu-id="8be49-127">**Export VAT Entries**</span></span>|<span data-ttu-id="8be49-128">Select to export the entries in the **VAT Entry** table.</span><span class="sxs-lookup"><span data-stu-id="8be49-128">Select to export the entries in the **VAT Entry** table.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="8be49-129">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="8be49-129">You must select at least one check box in this page.</span></span>  

5. <span data-ttu-id="8be49-130">To export the file, choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="8be49-130">To export the file, choose the **OK** button.</span></span>  

    <span data-ttu-id="8be49-131">The VAT audit information is exported.</span><span class="sxs-lookup"><span data-stu-id="8be49-131">The VAT audit information is exported.</span></span> <span data-ttu-id="8be49-132">You can save the data to a file, or open the file in the appropriate program.</span><span class="sxs-lookup"><span data-stu-id="8be49-132">You can save the data to a file, or open the file in the appropriate program.</span></span>  

## <a name="to-print-the-vat-entry-exception-report"></a><span data-ttu-id="8be49-133">To print the VAT entry exception report</span><span class="sxs-lookup"><span data-stu-id="8be49-133">To print the VAT entry exception report</span></span>  

1. <span data-ttu-id="8be49-134">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="8be49-134">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8be49-135">Choose the relevant VAT statement template, and then choose OK.</span><span class="sxs-lookup"><span data-stu-id="8be49-135">Choose the relevant VAT statement template, and then choose OK.</span></span>
3. <span data-ttu-id="8be49-136">On the **VAT Statement** page, choose **VAT Entry Exception Report**.</span><span class="sxs-lookup"><span data-stu-id="8be49-136">On the **VAT Statement** page, choose **VAT Entry Exception Report**.</span></span>  
4. <span data-ttu-id="8be49-137">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="8be49-137">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="8be49-138">Field</span><span class="sxs-lookup"><span data-stu-id="8be49-138">Field</span></span>|<span data-ttu-id="8be49-139">Description</span><span class="sxs-lookup"><span data-stu-id="8be49-139">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="8be49-140">**VAT Base Discount**</span><span class="sxs-lookup"><span data-stu-id="8be49-140">**VAT Base Discount**</span></span>|<span data-ttu-id="8be49-141">Select if you want to enter a value in the **VAT Base Discount %** field.</span><span class="sxs-lookup"><span data-stu-id="8be49-141">Select if you want to enter a value in the **VAT Base Discount %** field.</span></span>|  
    |<span data-ttu-id="8be49-142">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="8be49-142">**Manual VAT Difference**</span></span>|<span data-ttu-id="8be49-143">Select if you want to enter a value in the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="8be49-143">Select if you want to enter a value in the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="8be49-144">**VAT Calculation Types**</span><span class="sxs-lookup"><span data-stu-id="8be49-144">**VAT Calculation Types**</span></span>|<span data-ttu-id="8be49-145">Select to determine the VAT calculation type.</span><span class="sxs-lookup"><span data-stu-id="8be49-145">Select to determine the VAT calculation type.</span></span>|  
    |<span data-ttu-id="8be49-146">**VAT Rate**</span><span class="sxs-lookup"><span data-stu-id="8be49-146">**VAT Rate**</span></span>|<span data-ttu-id="8be49-147">Select to determine the VAT rate for a particular journal line.</span><span class="sxs-lookup"><span data-stu-id="8be49-147">Select to determine the VAT rate for a particular journal line.</span></span>|  
    |<span data-ttu-id="8be49-148">**VAT Base Discount %**</span><span class="sxs-lookup"><span data-stu-id="8be49-148">**VAT Base Discount %**</span></span>|<span data-ttu-id="8be49-149">Enter a value in this field if you have selected the **VAT Base Discount** field.</span><span class="sxs-lookup"><span data-stu-id="8be49-149">Enter a value in this field if you have selected the **VAT Base Discount** field.</span></span>|  
    |<span data-ttu-id="8be49-150">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="8be49-150">**Manual VAT Difference**</span></span>|<span data-ttu-id="8be49-151">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="8be49-151">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="8be49-152">**VAT Rate % Difference**</span><span class="sxs-lookup"><span data-stu-id="8be49-152">**VAT Rate % Difference**</span></span>|<span data-ttu-id="8be49-153">Specify the maximum VAT rate difference.</span><span class="sxs-lookup"><span data-stu-id="8be49-153">Specify the maximum VAT rate difference.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="8be49-154">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="8be49-154">You must select at least one check box in this page.</span></span>  

5. <span data-ttu-id="8be49-155">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span><span class="sxs-lookup"><span data-stu-id="8be49-155">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8be49-156">See Also</span><span class="sxs-lookup"><span data-stu-id="8be49-156">See Also</span></span>

[<span data-ttu-id="8be49-157">Working with Reports, Batch Jobs, and XMLports</span><span class="sxs-lookup"><span data-stu-id="8be49-157">Working with Reports, Batch Jobs, and XMLports</span></span>](../../ui-work-report.md)  
[<span data-ttu-id="8be49-158">Report VAT to Tax Authorities</span><span class="sxs-lookup"><span data-stu-id="8be49-158">Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
[<span data-ttu-id="8be49-159">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="8be49-159">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]