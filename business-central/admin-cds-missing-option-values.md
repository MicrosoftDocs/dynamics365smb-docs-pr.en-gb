---
title: Handling Missing Option Values
description: Learn how to prevent full synchronisation from failing because the options differ in mapped fields.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 02/03/2020
ms.openlocfilehash: 5f914904aaa1ec568b396a830ebc18a0fe4e40c1
ms.sourcegitcommit: 79d6d270325f1cc88bd4e9a273f9ff859ceadcbc
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/13/2020
ms.locfileid: "3693031"
---
# <a name="handling-missing-option-values"></a><span data-ttu-id="0aded-103">Handling Missing Option Values</span><span class="sxs-lookup"><span data-stu-id="0aded-103">Handling Missing Option Values</span></span>
[!INCLUDE[d365fin](includes/cds_long_md.md)] <span data-ttu-id="0aded-104">contains only three option set fields that contain option values that you can map to [!INCLUDE[d365fin](includes/d365fin_md.md)] fields of Option type</span><span class="sxs-lookup"><span data-stu-id="0aded-104">contains only three option set fields that contain option values that you can map to [!INCLUDE[d365fin](includes/d365fin_md.md)] fields of Option type</span></span><!-- Option type, not enum? @Onat can you vertify this? --> <span data-ttu-id="0aded-105">for automatic synchronisation.</span><span class="sxs-lookup"><span data-stu-id="0aded-105">for automatic synchronization.</span></span> <span data-ttu-id="0aded-106">During synchronisation, non-mapped options are ignored and the missing options are appended to the related [!INCLUDE[d365fin](includes/d365fin_md.md)] table and added to the **CDS Option Mapping** system table to handle manually later.</span><span class="sxs-lookup"><span data-stu-id="0aded-106">During synchronization, non-mapped options are ignored and the missing options are appended to the related [!INCLUDE[d365fin](includes/d365fin_md.md)] table and added to the **CDS Option Mapping** system table to handle manually later.</span></span> <span data-ttu-id="0aded-107">For example, by adding the missing options in either product and then updating the mapping.</span><span class="sxs-lookup"><span data-stu-id="0aded-107">For example, by adding the missing options in either product and then updating the mapping.</span></span> <span data-ttu-id="0aded-108">This section describes how that works.</span><span class="sxs-lookup"><span data-stu-id="0aded-108">This section describes how that works.</span></span>

<span data-ttu-id="0aded-109">The **Integration Table Mapping** page contains three maps for fields that contain one or more mapped option values.</span><span class="sxs-lookup"><span data-stu-id="0aded-109">The **Integration Table Mapping** page contains three maps for fields that contain one or more mapped option values.</span></span> <span data-ttu-id="0aded-110">After a full synchronisation, the **CDS Option Mapping** page contains the non-mapped options in the three fields respectively.</span><span class="sxs-lookup"><span data-stu-id="0aded-110">After a full synchronization, the **CDS Option Mapping** page contains the non-mapped options in the three fields respectively.</span></span>

|         <span data-ttu-id="0aded-111">Record</span><span class="sxs-lookup"><span data-stu-id="0aded-111">Record</span></span>             | <span data-ttu-id="0aded-112">Option Value</span><span class="sxs-lookup"><span data-stu-id="0aded-112">Option Value</span></span> | <span data-ttu-id="0aded-113">Option Value Caption</span><span class="sxs-lookup"><span data-stu-id="0aded-113">Option Value Caption</span></span> |
|----------------------------|--------------|----------------------|
| <span data-ttu-id="0aded-114">Payment Terms: NET30</span><span class="sxs-lookup"><span data-stu-id="0aded-114">Payment Terms: NET30</span></span>       | <span data-ttu-id="0aded-115">1</span><span class="sxs-lookup"><span data-stu-id="0aded-115">1</span></span>            | <span data-ttu-id="0aded-116">Net 30</span><span class="sxs-lookup"><span data-stu-id="0aded-116">Net 30</span></span>               |
| <span data-ttu-id="0aded-117">Payment Terms: 2%10NET30</span><span class="sxs-lookup"><span data-stu-id="0aded-117">Payment Terms: 2%10NET30</span></span>   | <span data-ttu-id="0aded-118">2</span><span class="sxs-lookup"><span data-stu-id="0aded-118">2</span></span>            | <span data-ttu-id="0aded-119">2% 10; Net 30</span><span class="sxs-lookup"><span data-stu-id="0aded-119">2% 10; Net 30</span></span>        |
| <span data-ttu-id="0aded-120">Payment Terms: NET45</span><span class="sxs-lookup"><span data-stu-id="0aded-120">Payment Terms: NET45</span></span>       | <span data-ttu-id="0aded-121">3</span><span class="sxs-lookup"><span data-stu-id="0aded-121">3</span></span>            | <span data-ttu-id="0aded-122">Net 45</span><span class="sxs-lookup"><span data-stu-id="0aded-122">Net 45</span></span>               |
| <span data-ttu-id="0aded-123">Payment Terms: NET60</span><span class="sxs-lookup"><span data-stu-id="0aded-123">Payment Terms: NET60</span></span>       | <span data-ttu-id="0aded-124">4</span><span class="sxs-lookup"><span data-stu-id="0aded-124">4</span></span>            | <span data-ttu-id="0aded-125">Net 60</span><span class="sxs-lookup"><span data-stu-id="0aded-125">Net 60</span></span>               |
| <span data-ttu-id="0aded-126">Shipment Method: FOB</span><span class="sxs-lookup"><span data-stu-id="0aded-126">Shipment Method: FOB</span></span>       | <span data-ttu-id="0aded-127">1</span><span class="sxs-lookup"><span data-stu-id="0aded-127">1</span></span>            | <span data-ttu-id="0aded-128">FOB</span><span class="sxs-lookup"><span data-stu-id="0aded-128">FOB</span></span>                  |
| <span data-ttu-id="0aded-129">Shipment Method: NOCHARGE</span><span class="sxs-lookup"><span data-stu-id="0aded-129">Shipment Method: NOCHARGE</span></span>  | <span data-ttu-id="0aded-130">2</span><span class="sxs-lookup"><span data-stu-id="0aded-130">2</span></span>            | <span data-ttu-id="0aded-131">No Charge</span><span class="sxs-lookup"><span data-stu-id="0aded-131">No Charge</span></span>            |
| <span data-ttu-id="0aded-132">Shipping Agent: AIRBORNE</span><span class="sxs-lookup"><span data-stu-id="0aded-132">Shipping Agent: AIRBORNE</span></span>   | <span data-ttu-id="0aded-133">1</span><span class="sxs-lookup"><span data-stu-id="0aded-133">1</span></span>            | <span data-ttu-id="0aded-134">Airborne</span><span class="sxs-lookup"><span data-stu-id="0aded-134">Airborne</span></span>             |
| <span data-ttu-id="0aded-135">Shipping Agent: DHL</span><span class="sxs-lookup"><span data-stu-id="0aded-135">Shipping Agent: DHL</span></span>        | <span data-ttu-id="0aded-136">2</span><span class="sxs-lookup"><span data-stu-id="0aded-136">2</span></span>            | <span data-ttu-id="0aded-137">DHL</span><span class="sxs-lookup"><span data-stu-id="0aded-137">DHL</span></span>                  |
| <span data-ttu-id="0aded-138">Shipping Agent: FEDEX</span><span class="sxs-lookup"><span data-stu-id="0aded-138">Shipping Agent: FEDEX</span></span>      | <span data-ttu-id="0aded-139">3</span><span class="sxs-lookup"><span data-stu-id="0aded-139">3</span></span>            | <span data-ttu-id="0aded-140">FedEx</span><span class="sxs-lookup"><span data-stu-id="0aded-140">FedEx</span></span>                |
| <span data-ttu-id="0aded-141">Shipping Agent: UPS</span><span class="sxs-lookup"><span data-stu-id="0aded-141">Shipping Agent: UPS</span></span>        | <span data-ttu-id="0aded-142">4</span><span class="sxs-lookup"><span data-stu-id="0aded-142">4</span></span>            | <span data-ttu-id="0aded-143">UPS</span><span class="sxs-lookup"><span data-stu-id="0aded-143">UPS</span></span>                  |
| <span data-ttu-id="0aded-144">Shipping Agent: POSTALMAIL</span><span class="sxs-lookup"><span data-stu-id="0aded-144">Shipping Agent: POSTALMAIL</span></span> | <span data-ttu-id="0aded-145">5</span><span class="sxs-lookup"><span data-stu-id="0aded-145">5</span></span>            | <span data-ttu-id="0aded-146">Postal Mail</span><span class="sxs-lookup"><span data-stu-id="0aded-146">Postal Mail</span></span>          |
| <span data-ttu-id="0aded-147">Shipping Agent: FULLLOAD</span><span class="sxs-lookup"><span data-stu-id="0aded-147">Shipping Agent: FULLLOAD</span></span>   | <span data-ttu-id="0aded-148">6</span><span class="sxs-lookup"><span data-stu-id="0aded-148">6</span></span>            | <span data-ttu-id="0aded-149">Full Load</span><span class="sxs-lookup"><span data-stu-id="0aded-149">Full Load</span></span>            |
| <span data-ttu-id="0aded-150">Shipping Agent: WILLCALL</span><span class="sxs-lookup"><span data-stu-id="0aded-150">Shipping Agent: WILLCALL</span></span>   | <span data-ttu-id="0aded-151">7</span><span class="sxs-lookup"><span data-stu-id="0aded-151">7</span></span>            | <span data-ttu-id="0aded-152">Will Call</span><span class="sxs-lookup"><span data-stu-id="0aded-152">Will Call</span></span>            |

<span data-ttu-id="0aded-153">The content of the **CDS Option Mapping** page is based on enum values in the **CDS Account** table.</span><span class="sxs-lookup"><span data-stu-id="0aded-153">The content of the **CDS Option Mapping** page is based on enum values in the **CDS Account** table.</span></span> <span data-ttu-id="0aded-154">In [!INCLUDE[d365fin](includes/cds_long_md.md)], the following fields on the account entity are mapped to fields on the customer and vendor records:</span><span class="sxs-lookup"><span data-stu-id="0aded-154">In [!INCLUDE[d365fin](includes/cds_long_md.md)], the following fields on the account entity are mapped to fields on the customer and vendor records:</span></span>

- <span data-ttu-id="0aded-155">**Address 1: Freight Terms** of data type Enum, where values are defined as follow:</span><span class="sxs-lookup"><span data-stu-id="0aded-155">**Address 1: Freight Terms** of data type Enum, where values are defined as follow:</span></span>

```
enum 5335 "CDS Shipment Method Code"
{
    Extensible = true;
    value(0; " ") { Caption = ' '; }
    value(1; "FOB") { Caption = 'FOB'; }
    value(2; "NoCharge") { Caption = 'No Charge'; }
}
```

- <span data-ttu-id="0aded-156">**Address 1: Shipping Method** of data type Enum, where values are defined as follows:</span><span class="sxs-lookup"><span data-stu-id="0aded-156">**Address 1: Shipping Method** of data type Enum, where values are defined as follows:</span></span>

```
enum 5336 "CDS Shipping Agent Code"
enum 5336 "CDS Shipping Agent Code"
{
    Extensible = true;
    value(0; " ") { Caption = ' '; }
    value(1; "Airborne") { Caption = 'Airborne'; }
    value(2; "DHL") { Caption = 'DHL'; }
    value(3; "FedEx") { Caption = 'FedEx'; }
    value(4; "UPS") { Caption = 'UPS'; }
    value(5; "PostalMail") { Caption = 'Postal Mail'; }
    value(6; "FullLoad") { Caption = 'Full Load'; }
    value(7; "WillCall") { Caption = 'Will Call'; }
}
```

- <span data-ttu-id="0aded-157">**Payment Terms** of data type Enum, where values are defined as follows:</span><span class="sxs-lookup"><span data-stu-id="0aded-157">**Payment Terms** of data type Enum, where values are defined as follows:</span></span>

```
enum 5334 "CDS Payment Terms Code"
{
    Extensible = true;
    value(0; " ") { Caption = ' '; }
    value(1; "Net30") { Caption = 'Net 30'; }
    value(2; "2%10Net30") { Caption = '2% 10; Net 30'; }
    value(3; "Net45") { Caption = 'Net 45'; }
    value(4; "Net60") { Caption = 'Net 60'; }
}
```

<span data-ttu-id="0aded-158">All of the [!INCLUDE[d365fin](includes/d365fin_md.md)] enums above are mapped to option sets in [!INCLUDE[d365fin](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="0aded-158">All of the [!INCLUDE[d365fin](includes/d365fin_md.md)] enums above are mapped to option sets in [!INCLUDE[d365fin](includes/cds_long_md.md)].</span></span>

### <a name="extending-option-sets-in-d365fin"></a><span data-ttu-id="0aded-159">Extending Option Sets in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="0aded-159">Extending Option Sets in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
1. <span data-ttu-id="0aded-160">Create a new AL extension.</span><span class="sxs-lookup"><span data-stu-id="0aded-160">Create a new AL extension.</span></span>

2. <span data-ttu-id="0aded-161">Add an Enum extension for the options that you want to extend.</span><span class="sxs-lookup"><span data-stu-id="0aded-161">Add an Enum extension for the options that you want to extend.</span></span> <span data-ttu-id="0aded-162">Be sure that you use the same value.</span><span class="sxs-lookup"><span data-stu-id="0aded-162">Be sure that you use the same value.</span></span> 

```
enumextension 50100 "CDS Payment Terms Code Extension" extends "CDS Payment Terms Code"
{
    value(779800001; "Cash Payment") { Caption = 'Cash Payment'; }
    value(779800002; "Transfer") { Caption = 'Transfer'; }
}
```

> [!IMPORTANT]  
> <span data-ttu-id="0aded-163">You must use the same option ID values from [!INCLUDE[d365fin](includes/cds_long_md.md)] when you extend the [!INCLUDE[d365fin](includes/d365fin_md.md)] enum.</span><span class="sxs-lookup"><span data-stu-id="0aded-163">You must use the same option ID values from [!INCLUDE[d365fin](includes/cds_long_md.md)] when you extend the [!INCLUDE[d365fin](includes/d365fin_md.md)] enum.</span></span> <span data-ttu-id="0aded-164">Otherwise synchronisation will fail.</span><span class="sxs-lookup"><span data-stu-id="0aded-164">Otherwise synchronization will fail.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="0aded-165">Do not use character "," in the Enum values and captions.</span><span class="sxs-lookup"><span data-stu-id="0aded-165">Do not use character "," in the Enum values and captions.</span></span> <span data-ttu-id="0aded-166">This is currently not supported by the [!INCLUDE[d365fin](includes/d365fin_md.md)] runtime.</span><span class="sxs-lookup"><span data-stu-id="0aded-166">This is currently not supported by the [!INCLUDE[d365fin](includes/d365fin_md.md)] runtime.</span></span>

> [!NOTE]
> <span data-ttu-id="0aded-167">The first ten characters of the new option value names and captions must be unique.</span><span class="sxs-lookup"><span data-stu-id="0aded-167">The first ten characters of the new option value names and captions must be unique.</span></span> <span data-ttu-id="0aded-168">For example, two options named "Transfer 20 working days" and "Transfer 20 calendar days" will cause an error because both have the same first 10 characters, "Transfer 2".</span><span class="sxs-lookup"><span data-stu-id="0aded-168">For example, two options named "Transfer 20 working days" and "Transfer 20 calendar days" will cause an error because both have the same first 10 characters, "Transfer 2".</span></span> <span data-ttu-id="0aded-169">Name them, for example, "TRF20 WD" and "TRF20 CD."</span><span class="sxs-lookup"><span data-stu-id="0aded-169">Name them, for example, "TRF20 WD" and "TRF20 CD."</span></span>

### <a name="update-d365fin-option-mapping"></a><span data-ttu-id="0aded-170">Update [!INCLUDE[d365fin](includes/cds_long_md.md)] Option Mapping</span><span class="sxs-lookup"><span data-stu-id="0aded-170">Update [!INCLUDE[d365fin](includes/cds_long_md.md)] Option Mapping</span></span>
<span data-ttu-id="0aded-171">Now you can recreate the mapping between [!INCLUDE[d365fin](includes/cds_long_md.md)] options and [!INCLUDE[d365fin](includes/d365fin_md.md)] records.</span><span class="sxs-lookup"><span data-stu-id="0aded-171">Now you can recreate the mapping between [!INCLUDE[d365fin](includes/cds_long_md.md)] options and [!INCLUDE[d365fin](includes/d365fin_md.md)] records.</span></span>

<span data-ttu-id="0aded-172">On the **Integration Table Mapping** page, choose the line for the **Payment Terms** map, and then choose the **Synchronise Modified Records** action.</span><span class="sxs-lookup"><span data-stu-id="0aded-172">On the **Integration Table Mapping** page, choose the line for the **Payment Terms** map, and then choose the **Synchronize Modified Records** action.</span></span> <span data-ttu-id="0aded-173">The **CDS Option Mapping** page is updated with the additional records below.</span><span class="sxs-lookup"><span data-stu-id="0aded-173">The **CDS Option Mapping** page is updated with the additional records below.</span></span>

|         <span data-ttu-id="0aded-174">Record</span><span class="sxs-lookup"><span data-stu-id="0aded-174">Record</span></span>                 | <span data-ttu-id="0aded-175">Option Value</span><span class="sxs-lookup"><span data-stu-id="0aded-175">Option Value</span></span>   | <span data-ttu-id="0aded-176">Option Value Caption</span><span class="sxs-lookup"><span data-stu-id="0aded-176">Option Value Caption</span></span> |
|--------------------------------|----------------|----------------------|
| <span data-ttu-id="0aded-177">Payment Terms: NET30</span><span class="sxs-lookup"><span data-stu-id="0aded-177">Payment Terms: NET30</span></span>           | <span data-ttu-id="0aded-178">1</span><span class="sxs-lookup"><span data-stu-id="0aded-178">1</span></span>              | <span data-ttu-id="0aded-179">Net 30</span><span class="sxs-lookup"><span data-stu-id="0aded-179">Net 30</span></span>               |
| <span data-ttu-id="0aded-180">Payment Terms: 2%10NET30</span><span class="sxs-lookup"><span data-stu-id="0aded-180">Payment Terms: 2%10NET30</span></span>       | <span data-ttu-id="0aded-181">2</span><span class="sxs-lookup"><span data-stu-id="0aded-181">2</span></span>              | <span data-ttu-id="0aded-182">2% 10; Net 30</span><span class="sxs-lookup"><span data-stu-id="0aded-182">2% 10; Net 30</span></span>        |
| <span data-ttu-id="0aded-183">Payment Terms: NET45</span><span class="sxs-lookup"><span data-stu-id="0aded-183">Payment Terms: NET45</span></span>           | <span data-ttu-id="0aded-184">3</span><span class="sxs-lookup"><span data-stu-id="0aded-184">3</span></span>              | <span data-ttu-id="0aded-185">Net 45</span><span class="sxs-lookup"><span data-stu-id="0aded-185">Net 45</span></span>               |
| <span data-ttu-id="0aded-186">Payment Terms: NET60</span><span class="sxs-lookup"><span data-stu-id="0aded-186">Payment Terms: NET60</span></span>           | <span data-ttu-id="0aded-187">4</span><span class="sxs-lookup"><span data-stu-id="0aded-187">4</span></span>              | <span data-ttu-id="0aded-188">Net 60</span><span class="sxs-lookup"><span data-stu-id="0aded-188">Net 60</span></span>               | 
| <span data-ttu-id="0aded-189">**Payment Terms: CASH PAYME**</span><span class="sxs-lookup"><span data-stu-id="0aded-189">**Payment Terms: CASH PAYME**</span></span>  | <span data-ttu-id="0aded-190">**779800001**</span><span class="sxs-lookup"><span data-stu-id="0aded-190">**779800001**</span></span>  | <span data-ttu-id="0aded-191">**Cash Payment**</span><span class="sxs-lookup"><span data-stu-id="0aded-191">**Cash Payment**</span></span>     |
| <span data-ttu-id="0aded-192">**Payment Terms: TRANSFER**</span><span class="sxs-lookup"><span data-stu-id="0aded-192">**Payment Terms: TRANSFER**</span></span>    | <span data-ttu-id="0aded-193">**779800002**</span><span class="sxs-lookup"><span data-stu-id="0aded-193">**779800002**</span></span>  | <span data-ttu-id="0aded-194">**Transfer**</span><span class="sxs-lookup"><span data-stu-id="0aded-194">**Transfer**</span></span>         |

<span data-ttu-id="0aded-195">The **Payment Terms** table in [!INCLUDE[d365fin](includes/d365fin_md.md)] will then have new records for the [!INCLUDE[d365fin](includes/cds_long_md.md)] options.</span><span class="sxs-lookup"><span data-stu-id="0aded-195">The **Payment Terms** table in [!INCLUDE[d365fin](includes/d365fin_md.md)] will then have new records for the [!INCLUDE[d365fin](includes/cds_long_md.md)] options.</span></span> <span data-ttu-id="0aded-196">In the following table new options are in bold font .</span><span class="sxs-lookup"><span data-stu-id="0aded-196">In the following table new options are in bold font .</span></span> <span data-ttu-id="0aded-197">Italic rows represent all options that can now be synchronised.</span><span class="sxs-lookup"><span data-stu-id="0aded-197">Italic rows represent all options that can now be synchronized.</span></span> <span data-ttu-id="0aded-198">Remaining rows represent options are not in use and will be ignored during synchronisation.</span><span class="sxs-lookup"><span data-stu-id="0aded-198">Remaining rows represent options are not in use and will be ignored during synchronization.</span></span> <span data-ttu-id="0aded-199">You can remove them or extend CDS options with the same names.)</span><span class="sxs-lookup"><span data-stu-id="0aded-199">You can remove them or extend CDS options with the same names.)</span></span>

| <span data-ttu-id="0aded-200">Code</span><span class="sxs-lookup"><span data-stu-id="0aded-200">Code</span></span>       | <span data-ttu-id="0aded-201">Due Date Calculation</span><span class="sxs-lookup"><span data-stu-id="0aded-201">Due Date Calculation</span></span> | <span data-ttu-id="0aded-202">Discount Date Calculation</span><span class="sxs-lookup"><span data-stu-id="0aded-202">Discount Date Calculation</span></span> | <span data-ttu-id="0aded-203">Discount %</span><span class="sxs-lookup"><span data-stu-id="0aded-203">Discount %</span></span> | <span data-ttu-id="0aded-204">Calc. Pmt. Disc. on Cr. Memos</span><span class="sxs-lookup"><span data-stu-id="0aded-204">Calc. Pmt. Disc. on Cr. Memos</span></span> | <span data-ttu-id="0aded-205">Description</span><span class="sxs-lookup"><span data-stu-id="0aded-205">Description</span></span>       |
|------------|----------------------|---------------------------|------------|-------------------------------|-------------------|
| <span data-ttu-id="0aded-206">10 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-206">10 DAYS</span></span>    | <span data-ttu-id="0aded-207">10D</span><span class="sxs-lookup"><span data-stu-id="0aded-207">10D</span></span>                  |                           | <span data-ttu-id="0aded-208">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-208">0.</span></span>         | <span data-ttu-id="0aded-209">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-209">FALSE</span></span>                         | <span data-ttu-id="0aded-210">Net 10 days</span><span class="sxs-lookup"><span data-stu-id="0aded-210">Net 10 days</span></span>       |
| <span data-ttu-id="0aded-211">14 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-211">14 DAYS</span></span>    | <span data-ttu-id="0aded-212">14D</span><span class="sxs-lookup"><span data-stu-id="0aded-212">14D</span></span>                  |                           | <span data-ttu-id="0aded-213">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-213">0.</span></span>         | <span data-ttu-id="0aded-214">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-214">FALSE</span></span>                         | <span data-ttu-id="0aded-215">Net 14 days</span><span class="sxs-lookup"><span data-stu-id="0aded-215">Net 14 days</span></span>       |
| <span data-ttu-id="0aded-216">15 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-216">15 DAYS</span></span>    | <span data-ttu-id="0aded-217">15D</span><span class="sxs-lookup"><span data-stu-id="0aded-217">15D</span></span>                  |                           | <span data-ttu-id="0aded-218">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-218">0.</span></span>         | <span data-ttu-id="0aded-219">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-219">FALSE</span></span>                         | <span data-ttu-id="0aded-220">Net 15 days</span><span class="sxs-lookup"><span data-stu-id="0aded-220">Net 15 days</span></span>       |
| <span data-ttu-id="0aded-221">1M(8D)</span><span class="sxs-lookup"><span data-stu-id="0aded-221">1M(8D)</span></span>     | <span data-ttu-id="0aded-222">1M</span><span class="sxs-lookup"><span data-stu-id="0aded-222">1M</span></span>                   | <span data-ttu-id="0aded-223">8D</span><span class="sxs-lookup"><span data-stu-id="0aded-223">8D</span></span>                        | <span data-ttu-id="0aded-224">2.</span><span class="sxs-lookup"><span data-stu-id="0aded-224">2.</span></span>         | <span data-ttu-id="0aded-225">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-225">FALSE</span></span>                         | <span data-ttu-id="0aded-226">1 Month/2% 8 days</span><span class="sxs-lookup"><span data-stu-id="0aded-226">1 Month/2% 8 days</span></span> |
| <span data-ttu-id="0aded-227">2 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-227">2 DAYS</span></span>     | <span data-ttu-id="0aded-228">2D</span><span class="sxs-lookup"><span data-stu-id="0aded-228">2D</span></span>                   |                           | <span data-ttu-id="0aded-229">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-229">0.</span></span>         | <span data-ttu-id="0aded-230">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-230">FALSE</span></span>                         | <span data-ttu-id="0aded-231">Net 2 days</span><span class="sxs-lookup"><span data-stu-id="0aded-231">Net 2 days</span></span>        |
| <span data-ttu-id="0aded-232">*2%10NET30*</span><span class="sxs-lookup"><span data-stu-id="0aded-232">*2%10NET30*</span></span> |                      |                           | <span data-ttu-id="0aded-233">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-233">0.</span></span>         | <span data-ttu-id="0aded-234">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-234">FALSE</span></span>                         |                   |
| <span data-ttu-id="0aded-235">21 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-235">21 DAYS</span></span>    | <span data-ttu-id="0aded-236">21D</span><span class="sxs-lookup"><span data-stu-id="0aded-236">21D</span></span>                  |                           | <span data-ttu-id="0aded-237">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-237">0.</span></span>         | <span data-ttu-id="0aded-238">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-238">FALSE</span></span>                         | <span data-ttu-id="0aded-239">Net 21 days</span><span class="sxs-lookup"><span data-stu-id="0aded-239">Net 21 days</span></span>       |
| <span data-ttu-id="0aded-240">30 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-240">30 DAYS</span></span>    | <span data-ttu-id="0aded-241">30D</span><span class="sxs-lookup"><span data-stu-id="0aded-241">30D</span></span>                  |                           | <span data-ttu-id="0aded-242">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-242">0.</span></span>         | <span data-ttu-id="0aded-243">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-243">FALSE</span></span>                         | <span data-ttu-id="0aded-244">Net 30 days</span><span class="sxs-lookup"><span data-stu-id="0aded-244">Net 30 days</span></span>       |
| <span data-ttu-id="0aded-245">60 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-245">60 DAYS</span></span>    | <span data-ttu-id="0aded-246">60D</span><span class="sxs-lookup"><span data-stu-id="0aded-246">60D</span></span>                  |                           | <span data-ttu-id="0aded-247">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-247">0.</span></span>         | <span data-ttu-id="0aded-248">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-248">FALSE</span></span>                         | <span data-ttu-id="0aded-249">Net 60 days</span><span class="sxs-lookup"><span data-stu-id="0aded-249">Net 60 days</span></span>       |
| <span data-ttu-id="0aded-250">7 DAYS</span><span class="sxs-lookup"><span data-stu-id="0aded-250">7 DAYS</span></span>     | <span data-ttu-id="0aded-251">7D</span><span class="sxs-lookup"><span data-stu-id="0aded-251">7D</span></span>                   |                           | <span data-ttu-id="0aded-252">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-252">0.</span></span>         | <span data-ttu-id="0aded-253">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-253">FALSE</span></span>                         | <span data-ttu-id="0aded-254">Net 7 days</span><span class="sxs-lookup"><span data-stu-id="0aded-254">Net 7 days</span></span>        |
| <span data-ttu-id="0aded-255">***CASH PAYME***</span><span class="sxs-lookup"><span data-stu-id="0aded-255">***CASH PAYME***</span></span> |                      |                           | <span data-ttu-id="0aded-256">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-256">0.</span></span>         | <span data-ttu-id="0aded-257">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-257">FALSE</span></span>                         |                   |
| <span data-ttu-id="0aded-258">CM</span><span class="sxs-lookup"><span data-stu-id="0aded-258">CM</span></span>         | <span data-ttu-id="0aded-259">CM</span><span class="sxs-lookup"><span data-stu-id="0aded-259">CM</span></span>                   |                           | <span data-ttu-id="0aded-260">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-260">0.</span></span>         | <span data-ttu-id="0aded-261">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-261">FALSE</span></span>                         | <span data-ttu-id="0aded-262">Current Month</span><span class="sxs-lookup"><span data-stu-id="0aded-262">Current Month</span></span>     |
| <span data-ttu-id="0aded-263">COD</span><span class="sxs-lookup"><span data-stu-id="0aded-263">COD</span></span>        | <span data-ttu-id="0aded-264">0D</span><span class="sxs-lookup"><span data-stu-id="0aded-264">0D</span></span>                   |                           | <span data-ttu-id="0aded-265">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-265">0.</span></span>         | <span data-ttu-id="0aded-266">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-266">FALSE</span></span>                         | <span data-ttu-id="0aded-267">Cash on delivery</span><span class="sxs-lookup"><span data-stu-id="0aded-267">Cash on delivery</span></span>  |
| <span data-ttu-id="0aded-268">*NET30*</span><span class="sxs-lookup"><span data-stu-id="0aded-268">*NET30*</span></span>      |                      |                           | <span data-ttu-id="0aded-269">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-269">0.</span></span>         | <span data-ttu-id="0aded-270">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-270">FALSE</span></span>                         |                   |
| <span data-ttu-id="0aded-271">*NET45*</span><span class="sxs-lookup"><span data-stu-id="0aded-271">*NET45*</span></span>      |                      |                           | <span data-ttu-id="0aded-272">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-272">0.</span></span>         | <span data-ttu-id="0aded-273">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-273">FALSE</span></span>                         |                   |
| <span data-ttu-id="0aded-274">*NET60*</span><span class="sxs-lookup"><span data-stu-id="0aded-274">*NET60*</span></span>      |                      |                           | <span data-ttu-id="0aded-275">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-275">0.</span></span>         | <span data-ttu-id="0aded-276">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-276">FALSE</span></span>                         |                   |
| <span data-ttu-id="0aded-277">***TRANSFER***</span><span class="sxs-lookup"><span data-stu-id="0aded-277">***TRANSFER***</span></span> |                      |                           | <span data-ttu-id="0aded-278">0.</span><span class="sxs-lookup"><span data-stu-id="0aded-278">0.</span></span>         | <span data-ttu-id="0aded-279">FALSE</span><span class="sxs-lookup"><span data-stu-id="0aded-279">FALSE</span></span>                         |                   |

## <a name="see-also"></a><span data-ttu-id="0aded-280">See Also</span><span class="sxs-lookup"><span data-stu-id="0aded-280">See Also</span></span>