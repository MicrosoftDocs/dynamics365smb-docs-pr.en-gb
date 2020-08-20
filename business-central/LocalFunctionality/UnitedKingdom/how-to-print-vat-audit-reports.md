---
title: Print VAT Audit Reports
description: Learn how Business Central supports the British requirements for VAT audits.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 08/10/2020
ms.author: edupont
ms.openlocfilehash: 3755d88ebe538858710b0cfafb8a15c7e56e9baa
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676625"
---
# <a name="print-vat-audit-reports-in-the-british-version"></a><span data-ttu-id="cc91d-103">Print VAT Audit Reports in the British Version</span><span class="sxs-lookup"><span data-stu-id="cc91d-103">Print VAT Audit Reports in the British Version</span></span>

<span data-ttu-id="cc91d-104">In the United Kingdom, all vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span><span class="sxs-lookup"><span data-stu-id="cc91d-104">In the United Kingdom, all vendors must export the data required for auditing in a Content Separated Value (CSV) file format.</span></span> <span data-ttu-id="cc91d-105">The following reports in the British version of [!INCLUDE [prodshort](../../includes/prodshort.md)] comply with this requirement:</span><span class="sxs-lookup"><span data-stu-id="cc91d-105">The following reports in the British version of [!INCLUDE [prodshort](../../includes/prodshort.md)] comply with this requirement:</span></span>  

- <span data-ttu-id="cc91d-106">**VAT Audit**  report – This report is used for VAT auditing.</span><span class="sxs-lookup"><span data-stu-id="cc91d-106">**VAT Audit**  report – This report is used for VAT auditing.</span></span>  
- <span data-ttu-id="cc91d-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span><span class="sxs-lookup"><span data-stu-id="cc91d-107">**VAT Entry Exception** report - This report details the differences between the calculated VAT and the changes that occur because of rounding, VAT tolerance percentage, and discounts.</span></span> <span data-ttu-id="cc91d-108">It also displays the difference in VAT amounts for the tax authorities.</span><span class="sxs-lookup"><span data-stu-id="cc91d-108">It also displays the difference in VAT amounts for the tax authorities.</span></span>  

## <a name="to-print-the-vat-audit-report"></a><span data-ttu-id="cc91d-109">To print the VAT audit report</span><span class="sxs-lookup"><span data-stu-id="cc91d-109">To print the VAT audit report</span></span>  

1. <span data-ttu-id="cc91d-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc91d-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cc91d-111">Choose the relevant VAT statement template, and then choose OK.</span><span class="sxs-lookup"><span data-stu-id="cc91d-111">Choose the relevant VAT statement template, and then choose OK.</span></span>
3. <span data-ttu-id="cc91d-112">On the **VAT Statement** page, choose **VAT Audit Report**.</span><span class="sxs-lookup"><span data-stu-id="cc91d-112">On the **VAT Statement** page, choose **VAT Audit Report**.</span></span>
4. <span data-ttu-id="cc91d-113">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="cc91d-113">On the **VAT Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cc91d-114">Field</span><span class="sxs-lookup"><span data-stu-id="cc91d-114">Field</span></span>|<span data-ttu-id="cc91d-115">Description</span><span class="sxs-lookup"><span data-stu-id="cc91d-115">Description</span></span>|  
    |-----|-----------|  
    |<span data-ttu-id="cc91d-116">**Export Customers**</span><span class="sxs-lookup"><span data-stu-id="cc91d-116">**Export Customers**</span></span>|<span data-ttu-id="cc91d-117">Select to export the file to the **Customer** table.</span><span class="sxs-lookup"><span data-stu-id="cc91d-117">Select to export the file to the **Customer** table.</span></span>|  
    |<span data-ttu-id="cc91d-118">**Export Open Payments**</span><span class="sxs-lookup"><span data-stu-id="cc91d-118">**Export Open Payments**</span></span>|<span data-ttu-id="cc91d-119">Select to export the open credit entries.</span><span class="sxs-lookup"><span data-stu-id="cc91d-119">Select to export the open credit entries.</span></span>|  
    |<span data-ttu-id="cc91d-120">**Export Late Invoicing**</span><span class="sxs-lookup"><span data-stu-id="cc91d-120">**Export Late Invoicing**</span></span>|<span data-ttu-id="cc91d-121">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span><span class="sxs-lookup"><span data-stu-id="cc91d-121">Select to export customer entries that took longer to invoice than the number of days specified in the **Late Invoice Delay (Days)** field.</span></span>|  
    |<span data-ttu-id="cc91d-122">**Late Invoice Delay (Days)**</span><span class="sxs-lookup"><span data-stu-id="cc91d-122">**Late Invoice Delay (Days)**</span></span>|<span data-ttu-id="cc91d-123">Enter the number of days between the invoice issue date and the payment received date.</span><span class="sxs-lookup"><span data-stu-id="cc91d-123">Enter the number of days between the invoice issue date and the payment received date.</span></span> <span data-ttu-id="cc91d-124">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span><span class="sxs-lookup"><span data-stu-id="cc91d-124">If the **Export Late Invoicing** field is selected, entries exceeding this limit will be exported.</span></span>|  
    |<span data-ttu-id="cc91d-125">**Export Vendors**</span><span class="sxs-lookup"><span data-stu-id="cc91d-125">**Export Vendors**</span></span>|<span data-ttu-id="cc91d-126">Select to export the file to the **Vendor** table.</span><span class="sxs-lookup"><span data-stu-id="cc91d-126">Select to export the file to the **Vendor** table.</span></span>|  
    |<span data-ttu-id="cc91d-127">**Export VAT Entries**</span><span class="sxs-lookup"><span data-stu-id="cc91d-127">**Export VAT Entries**</span></span>|<span data-ttu-id="cc91d-128">Select to export the entries in the **VAT Entry** table.</span><span class="sxs-lookup"><span data-stu-id="cc91d-128">Select to export the entries in the **VAT Entry** table.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="cc91d-129">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="cc91d-129">You must select at least one check box in this page.</span></span>  

5. <span data-ttu-id="cc91d-130">To export the file, choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="cc91d-130">To export the file, choose the **OK** button.</span></span>  

    <span data-ttu-id="cc91d-131">The VAT audit information is exported.</span><span class="sxs-lookup"><span data-stu-id="cc91d-131">The VAT audit information is exported.</span></span> <span data-ttu-id="cc91d-132">You can save the data to a file, or open the file in the appropriate program.</span><span class="sxs-lookup"><span data-stu-id="cc91d-132">You can save the data to a file, or open the file in the appropriate program.</span></span>  

## <a name="to-print-the-vat-entry-exception-report"></a><span data-ttu-id="cc91d-133">To print the VAT entry exception report</span><span class="sxs-lookup"><span data-stu-id="cc91d-133">To print the VAT entry exception report</span></span>  

1. <span data-ttu-id="cc91d-134">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="cc91d-134">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Statements**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cc91d-135">Choose the relevant VAT statement template, and then choose OK.</span><span class="sxs-lookup"><span data-stu-id="cc91d-135">Choose the relevant VAT statement template, and then choose OK.</span></span>
3. <span data-ttu-id="cc91d-136">On the **VAT Statement** page, choose **VAT Entry Exception Report**.</span><span class="sxs-lookup"><span data-stu-id="cc91d-136">On the **VAT Statement** page, choose **VAT Entry Exception Report**.</span></span>  
4. <span data-ttu-id="cc91d-137">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="cc91d-137">On the **VAT Entry Exception Report** page, on the **Options** FastTab, fll in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="cc91d-138">Field</span><span class="sxs-lookup"><span data-stu-id="cc91d-138">Field</span></span>|<span data-ttu-id="cc91d-139">Description</span><span class="sxs-lookup"><span data-stu-id="cc91d-139">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="cc91d-140">**VAT Base Discount**</span><span class="sxs-lookup"><span data-stu-id="cc91d-140">**VAT Base Discount**</span></span>|<span data-ttu-id="cc91d-141">Select if you want to enter a value in the **VAT Base Discount %** field.</span><span class="sxs-lookup"><span data-stu-id="cc91d-141">Select if you want to enter a value in the **VAT Base Discount %** field.</span></span>|  
    |<span data-ttu-id="cc91d-142">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="cc91d-142">**Manual VAT Difference**</span></span>|<span data-ttu-id="cc91d-143">Select if you want to enter a value in the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="cc91d-143">Select if you want to enter a value in the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="cc91d-144">**VAT Calculation Types**</span><span class="sxs-lookup"><span data-stu-id="cc91d-144">**VAT Calculation Types**</span></span>|<span data-ttu-id="cc91d-145">Select to determine the VAT calculation type.</span><span class="sxs-lookup"><span data-stu-id="cc91d-145">Select to determine the VAT calculation type.</span></span>|  
    |<span data-ttu-id="cc91d-146">**VAT Rate**</span><span class="sxs-lookup"><span data-stu-id="cc91d-146">**VAT Rate**</span></span>|<span data-ttu-id="cc91d-147">Select to determine the VAT rate for a particular journal line.</span><span class="sxs-lookup"><span data-stu-id="cc91d-147">Select to determine the VAT rate for a particular journal line.</span></span>|  
    |<span data-ttu-id="cc91d-148">**VAT Base Discount %**</span><span class="sxs-lookup"><span data-stu-id="cc91d-148">**VAT Base Discount %**</span></span>|<span data-ttu-id="cc91d-149">Enter a value in this field if you have selected the **VAT Base Discount** field.</span><span class="sxs-lookup"><span data-stu-id="cc91d-149">Enter a value in this field if you have selected the **VAT Base Discount** field.</span></span>|  
    |<span data-ttu-id="cc91d-150">**Manual VAT Difference**</span><span class="sxs-lookup"><span data-stu-id="cc91d-150">**Manual VAT Difference**</span></span>|<span data-ttu-id="cc91d-151">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span><span class="sxs-lookup"><span data-stu-id="cc91d-151">Enter a value in this field if you have selected the **Manual VAT Difference** field.</span></span>|  
    |<span data-ttu-id="cc91d-152">**VAT Rate % Difference**</span><span class="sxs-lookup"><span data-stu-id="cc91d-152">**VAT Rate % Difference**</span></span>|<span data-ttu-id="cc91d-153">Specify the maximum VAT rate difference.</span><span class="sxs-lookup"><span data-stu-id="cc91d-153">Specify the maximum VAT rate difference.</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="cc91d-154">You must select at least one check box in this page.</span><span class="sxs-lookup"><span data-stu-id="cc91d-154">You must select at least one check box in this page.</span></span>  

5. <span data-ttu-id="cc91d-155">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span><span class="sxs-lookup"><span data-stu-id="cc91d-155">Choose the **Print** button to print the report or choose the **Preview** button to view it on the screen.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cc91d-156">See Also</span><span class="sxs-lookup"><span data-stu-id="cc91d-156">See Also</span></span>

[<span data-ttu-id="cc91d-157">Working with Reports, Batch Jobs, and XMLports</span><span class="sxs-lookup"><span data-stu-id="cc91d-157">Working with Reports, Batch Jobs, and XMLports</span></span>](../../ui-work-report.md)  
[<span data-ttu-id="cc91d-158">Report VAT to Tax Authorities</span><span class="sxs-lookup"><span data-stu-id="cc91d-158">Report VAT to Tax Authorities</span></span>](../../finance-how-report-vat.md)  
[<span data-ttu-id="cc91d-159">United Kingdom Local Functionality</span><span class="sxs-lookup"><span data-stu-id="cc91d-159">United Kingdom Local Functionality</span></span>](united-kingdom-local-functionality.md)
