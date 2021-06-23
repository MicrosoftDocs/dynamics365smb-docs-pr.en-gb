---
title: Posting date on value entries
description: Learn how the Adjust Cost - Item Entries batch job identifies and assigns a posting date to the value entries that the batch job is about to create.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 918a450ea40676447f872ba95eb489c7cc210211
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215110"
---
# <a name="design-details-posting-date-on-adjustment-value-entry"></a><span data-ttu-id="b7468-103">Design Details: Posting Date on Adjustment Value Entry</span><span class="sxs-lookup"><span data-stu-id="b7468-103">Design Details: Posting Date on Adjustment Value Entry</span></span>
<span data-ttu-id="b7468-104">This article provides guidance for users of the Stock Costing functionality in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b7468-104">This article provides guidance for users of the Inventory Costing functionality in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b7468-105">The specific article is providing guidance in how the **Adjust Cost - Item Entries** batch job identifies and assigns a posting date to the value entries that the batch job is about to create.</span><span class="sxs-lookup"><span data-stu-id="b7468-105">The specific article is providing guidance in how the **Adjust Cost - Item Entries** batch job identifies and assigns a posting date to the value entries that the batch job is about to create.</span></span>  

<span data-ttu-id="b7468-106">First the concept of the process is reviewed, how the batch job identifies and assigns the Posting Date to the Value Entry to be created.</span><span class="sxs-lookup"><span data-stu-id="b7468-106">First the concept of the process is reviewed, how the batch job identifies and assigns the Posting Date to the Value Entry to be created.</span></span> <span data-ttu-id="b7468-107">Thereafter there are some scenarios shared that we in the support team come across from time to time and finally there is a summary of the concepts used.</span><span class="sxs-lookup"><span data-stu-id="b7468-107">Thereafter there are some scenarios shared that we in the support team come across from time to time and finally there is a summary of the concepts used.</span></span>  

## <a name="the-concept"></a><span data-ttu-id="b7468-108">The Concept</span><span class="sxs-lookup"><span data-stu-id="b7468-108">The Concept</span></span>  
<span data-ttu-id="b7468-109">The **Adjust Cost – Item Entries** batch job assigns a posting date to the value entry it is about to create in the following steps:</span><span class="sxs-lookup"><span data-stu-id="b7468-109">The **Adjust Cost – Item Entries** batch job assigns a posting date to the value entry it is about to create in the following steps:</span></span>  

1.  <span data-ttu-id="b7468-110">Initially the Posting Date of the entry to be created is the same date as the entry it adjusts.</span><span class="sxs-lookup"><span data-stu-id="b7468-110">Initially the Posting Date of the entry to be created is the same date as the entry it adjusts.</span></span>  

2.  <span data-ttu-id="b7468-111">The Posting Date is validated against Stock Periods and/or General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-111">The Posting Date is validated against Inventory Periods and/or General Ledger Setup.</span></span>  

3.  <span data-ttu-id="b7468-112">Assignment of Posting Date; If the initial Posting Date is not within allowed posting date range the batch job will assign an allowed Posting Date from either General Ledger Setup or Stock Period.</span><span class="sxs-lookup"><span data-stu-id="b7468-112">Assignment of Posting Date; If the initial Posting Date is not within allowed posting date range the batch job will assign an allowed Posting Date from either General Ledger Setup or Inventory Period.</span></span> <span data-ttu-id="b7468-113">If both Stock Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will be assigned to the Adjustment Value Entry.</span><span class="sxs-lookup"><span data-stu-id="b7468-113">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will be assigned to the Adjustment Value Entry.</span></span>  

 <span data-ttu-id="b7468-114">Let’s review this process more in practice.</span><span class="sxs-lookup"><span data-stu-id="b7468-114">Let’s review this process more in practice.</span></span> <span data-ttu-id="b7468-115">Assume we have an Item Ledger Entry of Sale.</span><span class="sxs-lookup"><span data-stu-id="b7468-115">Assume we have an Item Ledger Entry of Sale.</span></span> <span data-ttu-id="b7468-116">The item was shipped on September 5, 2013 and it was invoiced the day after.</span><span class="sxs-lookup"><span data-stu-id="b7468-116">The item was shipped on September 5, 2013 and it was invoiced the day after.</span></span>  

<span data-ttu-id="b7468-117">![State of item ledger entries in the scenario](media/helene/TechArticleAdjustcost1.png "State of item ledger entries in the scenario")</span><span class="sxs-lookup"><span data-stu-id="b7468-117">![State of item ledger entries in the scenario](media/helene/TechArticleAdjustcost1.png "State of item ledger entries in the scenario")</span></span>  

<span data-ttu-id="b7468-118">Below, the first Value Entry (379) represents the shipment and carry the same Posting Date as the parent Item ledger Entry.</span><span class="sxs-lookup"><span data-stu-id="b7468-118">Below, the first Value Entry (379) represents the shipment and carry the same Posting Date as the parent Item ledger Entry.</span></span>  

<span data-ttu-id="b7468-119">The second Value Entry (381) represents the invoice.</span><span class="sxs-lookup"><span data-stu-id="b7468-119">The second Value Entry (381) represents the invoice.</span></span>  

 <span data-ttu-id="b7468-120">The third Value Entry (391) is an Adjustment of the invoicing Value Entry (381)</span><span class="sxs-lookup"><span data-stu-id="b7468-120">The third Value Entry (391) is an Adjustment of the invoicing Value Entry (381)</span></span>  

 <span data-ttu-id="b7468-121">![State of value entries in the scenario](media/helene/TechArticleAdjustcost2.png "State of value entries in the scenario")</span><span class="sxs-lookup"><span data-stu-id="b7468-121">![State of value entries in the scenario](media/helene/TechArticleAdjustcost2.png "State of value entries in the scenario")</span></span>  

 <span data-ttu-id="b7468-122">Step 1: Adjustment Value Entry to be created is assigned same Posting Date as the entry it adjusts, illustrated above by Value entry 391.</span><span class="sxs-lookup"><span data-stu-id="b7468-122">Step 1: Adjustment Value Entry to be created is assigned same Posting Date as the entry it adjusts, illustrated above by Value entry 391.</span></span>  

 <span data-ttu-id="b7468-123">Step 2: Validation of initial assigned Posting Date.</span><span class="sxs-lookup"><span data-stu-id="b7468-123">Step 2: Validation of initial assigned Posting Date.</span></span>  

<span data-ttu-id="b7468-124">The **Adjust Cost – Item Entries** batch job determines if the initial Posting Date of the Adjustment Value Entry is within allowed posting date range based upon Stock Periods and/or General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-124">The **Adjust Cost – Item Entries** batch job determines if the initial Posting Date of the Adjustment Value Entry is within allowed posting date range based upon Inventory Periods and/or General Ledger Setup.</span></span>  

 <span data-ttu-id="b7468-125">Let’s review the above mentioned Sale by adding setup of allowed posting date ranges.</span><span class="sxs-lookup"><span data-stu-id="b7468-125">Let’s review the above mentioned Sale by adding setup of allowed posting date ranges.</span></span>  

 <span data-ttu-id="b7468-126">Stock Periods:</span><span class="sxs-lookup"><span data-stu-id="b7468-126">Inventory Periods:</span></span>  

<span data-ttu-id="b7468-127">![Stock periods in the scenario](media/helene/TechArticleAdjustcost3.png "Stock periods in the scenario")</span><span class="sxs-lookup"><span data-stu-id="b7468-127">![Inventory periods in the scenario](media/helene/TechArticleAdjustcost3.png "Inventory periods in the scenario")</span></span>

 <span data-ttu-id="b7468-128">First allowed posting date is the first day in the first open period.</span><span class="sxs-lookup"><span data-stu-id="b7468-128">First allowed posting date is the first day in the first open period.</span></span> <span data-ttu-id="b7468-129">September 1, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-129">September 1, 2013.</span></span>  

 <span data-ttu-id="b7468-130">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-130">General Ledger Setup:</span></span>  

<span data-ttu-id="b7468-131">![G/L Setup in the scenario](media/helene/TechArticleAdjustcost4.png "G/L Setup in the scenario")</span><span class="sxs-lookup"><span data-stu-id="b7468-131">![G/L Setup in the scenario](media/helene/TechArticleAdjustcost4.png "G/L Setup in the scenario")</span></span>

 <span data-ttu-id="b7468-132">First allowed posting date is the date stated in field Allow Posting From: September 10, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-132">First allowed posting date is the date stated in field Allow Posting From: September 10, 2013.</span></span>  

 <span data-ttu-id="b7468-133">If both Stock Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will define the allowed posting date range.</span><span class="sxs-lookup"><span data-stu-id="b7468-133">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will define the allowed posting date range.</span></span>  

 <span data-ttu-id="b7468-134">Step 3: Assignment of an allowed posting date;</span><span class="sxs-lookup"><span data-stu-id="b7468-134">Step 3: Assignment of an allowed posting date;</span></span>  

 <span data-ttu-id="b7468-135">The initial assigned Posting Date was September 6 as illustrated in step 1.</span><span class="sxs-lookup"><span data-stu-id="b7468-135">The initial assigned Posting Date was September 6 as illustrated in step 1.</span></span> <span data-ttu-id="b7468-136">However, in the second step the Adjust Cost – Item entries batch job identifies that earliest allowed Posting Date is September 10 and thereby assigns September 10 to the Adjustment Value Entry, below.</span><span class="sxs-lookup"><span data-stu-id="b7468-136">However, in the second step the Adjust Cost – Item entries batch job identifies that earliest allowed Posting Date is September 10 and thereby assigns September 10 to the Adjustment Value Entry, below.</span></span>  

 <span data-ttu-id="b7468-137">![State of value entries in the scenario 2](media/helene/TechArticleAdjustcost5.png "State of value entries in the scenario 2")</span><span class="sxs-lookup"><span data-stu-id="b7468-137">![State of value entries in the scenario 2](media/helene/TechArticleAdjustcost5.png "State of value entries in the scenario 2")</span></span>

 <span data-ttu-id="b7468-138">We have now reviewed the concept for assigning Posting Dates to Value Entries created by the Adjust Cost - Item entries batch job.</span><span class="sxs-lookup"><span data-stu-id="b7468-138">We have now reviewed the concept for assigning Posting Dates to Value Entries created by the Adjust Cost - Item entries batch job.</span></span>  

 <span data-ttu-id="b7468-139">Let’s continue to review some scenarios that we in the support team comes across from time to time in relation to assigned Posting Dates in the Adjust Cost – Item entries batch job and related setups.</span><span class="sxs-lookup"><span data-stu-id="b7468-139">Let’s continue to review some scenarios that we in the support team comes across from time to time in relation to assigned Posting Dates in the Adjust Cost – Item entries batch job and related setups.</span></span>  

## <a name="scenarios"></a><span data-ttu-id="b7468-140">Scenarios</span><span class="sxs-lookup"><span data-stu-id="b7468-140">Scenarios</span></span>  

### <a name="scenario-i-posting-date-is-not-within-your-range-of-allowed-posting-dates"></a><span data-ttu-id="b7468-141">Scenario I: “Posting Date is not within your range of allowed posting dates…”</span><span class="sxs-lookup"><span data-stu-id="b7468-141">Scenario I: “Posting Date is not within your range of allowed posting dates…”</span></span>  
 <span data-ttu-id="b7468-142">This is a scenario where a user is experiencing mentioned error message when the Adjust Cost – Item entries batch job is run.</span><span class="sxs-lookup"><span data-stu-id="b7468-142">This is a scenario where a user is experiencing mentioned error message when the Adjust Cost – Item entries batch job is run.</span></span>  

 <span data-ttu-id="b7468-143">In the previous section, describing the concept of assigning posting dates, the intention of the Adjust Cost – Item entries batch job is to create a Value Entry with Posting Date September 10th.</span><span class="sxs-lookup"><span data-stu-id="b7468-143">In the previous section, describing the concept of assigning posting dates, the intention of the Adjust Cost – Item entries batch job is to create a Value Entry with Posting Date September 10th.</span></span>  

<span data-ttu-id="b7468-144">![Error message about posting date](media/helene/TechArticleAdjustcost6.png "Error message about posting date")</span><span class="sxs-lookup"><span data-stu-id="b7468-144">![Error message about posting date](media/helene/TechArticleAdjustcost6.png "Error message about posting date")</span></span>

 <span data-ttu-id="b7468-145">We follow up on the User Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-145">We follow up on the User Setup:</span></span>  

<span data-ttu-id="b7468-146">![User's allowed posting dates setup](media/helene/TechArticleAdjustcost7.png "User's allowed posting dates setup")</span><span class="sxs-lookup"><span data-stu-id="b7468-146">![User's allowed posting dates setup](media/helene/TechArticleAdjustcost7.png "User's allowed posting dates setup")</span></span>

 <span data-ttu-id="b7468-147">The user in this case has an allowed posting date range from September 11 to September 30 and is thereby not allowed to post the Adjustment Value Entry with Posting Date September 10th.</span><span class="sxs-lookup"><span data-stu-id="b7468-147">The user in this case has an allowed posting date range from September 11 to September 30 and is thereby not allowed to post the Adjustment Value Entry with Posting Date September 10th.</span></span>  

<span data-ttu-id="b7468-148">![Overview of involved posting date setup](media/helene/TechArticleAdjustcost8.png "Overview of involved posting date setup")</span><span class="sxs-lookup"><span data-stu-id="b7468-148">![Overview of involved posting date setup](media/helene/TechArticleAdjustcost8.png "Overview of involved posting date setup")</span></span>

 <span data-ttu-id="b7468-149">Knowledge Base article [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) discusses more scenarios related to mentioned error message.</span><span class="sxs-lookup"><span data-stu-id="b7468-149">Knowledge Base article [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) discusses more scenarios related to mentioned error message.</span></span>  

### <a name="scenario-ii-posting-date-on-adjustment-value-entry-versus-posting-date-on-entry-causing-the-adjustment-such-as-revaluation-or-item-charge"></a><span data-ttu-id="b7468-150">Scenario II: Posting Date on Adjustment Value Entry versus Posting Date on entry causing the adjustment such as Revaluation or Item charge.</span><span class="sxs-lookup"><span data-stu-id="b7468-150">Scenario II: Posting Date on Adjustment Value Entry versus Posting Date on entry causing the adjustment such as Revaluation or Item charge.</span></span>  

### <a name="revaluation-scenario"></a><span data-ttu-id="b7468-151">Revaluation scenario:</span><span class="sxs-lookup"><span data-stu-id="b7468-151">Revaluation scenario:</span></span>  
 <span data-ttu-id="b7468-152">Prerequisites:</span><span class="sxs-lookup"><span data-stu-id="b7468-152">Prerequisites:</span></span>  

 <span data-ttu-id="b7468-153">Stock setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-153">Inventory setup:</span></span>  

-   <span data-ttu-id="b7468-154">Automatic Cost Posting = Yes</span><span class="sxs-lookup"><span data-stu-id="b7468-154">Automatic Cost Posting = Yes</span></span>  

-   <span data-ttu-id="b7468-155">Automatic Cost Adjustment=Always</span><span class="sxs-lookup"><span data-stu-id="b7468-155">Automatic Cost Adjustment=Always</span></span>  

-   <span data-ttu-id="b7468-156">Average Cost Calc. Type=item</span><span class="sxs-lookup"><span data-stu-id="b7468-156">Average Cost Calc. Type=item</span></span>  

-   <span data-ttu-id="b7468-157">Average Cost Period=Day</span><span class="sxs-lookup"><span data-stu-id="b7468-157">Average Cost Period=Day</span></span>  

 <span data-ttu-id="b7468-158">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-158">General Ledger Setup:</span></span>  

-   <span data-ttu-id="b7468-159">Allow Posting From = January 1, 2014</span><span class="sxs-lookup"><span data-stu-id="b7468-159">Allow Posting From = January 1, 2014</span></span>  

-   <span data-ttu-id="b7468-160">Allow Posting To = empty</span><span class="sxs-lookup"><span data-stu-id="b7468-160">Allow Posting To = empty</span></span>  

 <span data-ttu-id="b7468-161">User Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-161">User Setup:</span></span>  

-   <span data-ttu-id="b7468-162">Allow Posting From = December 1, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-162">Allow Posting From = December 1, 2013.</span></span>  

-   <span data-ttu-id="b7468-163">Allow Posting to = empty</span><span class="sxs-lookup"><span data-stu-id="b7468-163">Allow Posting to = empty</span></span>  

##### <a name="to-test-the-scenario"></a><span data-ttu-id="b7468-164">To test the scenario</span><span class="sxs-lookup"><span data-stu-id="b7468-164">To test the scenario</span></span>  

1.  <span data-ttu-id="b7468-165">Create item TEST:</span><span class="sxs-lookup"><span data-stu-id="b7468-165">Create item TEST:</span></span>  

     <span data-ttu-id="b7468-166">Base unit of measurement = PCS</span><span class="sxs-lookup"><span data-stu-id="b7468-166">Base unit of measure = PCS</span></span>  

     <span data-ttu-id="b7468-167">Costing Method = Average</span><span class="sxs-lookup"><span data-stu-id="b7468-167">Costing Method = Average</span></span>  

     <span data-ttu-id="b7468-168">Select optional posting groups.</span><span class="sxs-lookup"><span data-stu-id="b7468-168">Select optional posting groups.</span></span>  

2.  <span data-ttu-id="b7468-169">Open Item Journal, create, and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="b7468-169">Open Item Journal, create, and post a line as follows:</span></span>  

     <span data-ttu-id="b7468-170">Posting Date = December 15, 2013</span><span class="sxs-lookup"><span data-stu-id="b7468-170">Posting Date = December 15, 2013</span></span>  

     <span data-ttu-id="b7468-171">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="b7468-171">Item = TEST</span></span>  

     <span data-ttu-id="b7468-172">Entry Type = Purchase</span><span class="sxs-lookup"><span data-stu-id="b7468-172">Entry Type = Purchase</span></span>  

     <span data-ttu-id="b7468-173">Quantity = 100</span><span class="sxs-lookup"><span data-stu-id="b7468-173">Quantity = 100</span></span>  

     <span data-ttu-id="b7468-174">Unit Amount = 10</span><span class="sxs-lookup"><span data-stu-id="b7468-174">Unit Amount = 10</span></span>  

3.  <span data-ttu-id="b7468-175">Open Item Journal, create, and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="b7468-175">Open Item Journal, create, and post a line as follows:</span></span>  

     <span data-ttu-id="b7468-176">Date = December 20, 2013</span><span class="sxs-lookup"><span data-stu-id="b7468-176">Date = December 20, 2013</span></span>  

     <span data-ttu-id="b7468-177">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="b7468-177">Item = TEST</span></span>  

     <span data-ttu-id="b7468-178">Entry Type = Negative Adjustment</span><span class="sxs-lookup"><span data-stu-id="b7468-178">Entry Type = Negative Adjustment</span></span>  

     <span data-ttu-id="b7468-179">Quantity = 2</span><span class="sxs-lookup"><span data-stu-id="b7468-179">Quantity = 2</span></span>  

4.  <span data-ttu-id="b7468-180">Open Item Journal, create, and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="b7468-180">Open Item Journal, create, and post a line as follows:</span></span>  

     <span data-ttu-id="b7468-181">Date = January 15, 2014</span><span class="sxs-lookup"><span data-stu-id="b7468-181">Date = January 15, 2014</span></span>  

     <span data-ttu-id="b7468-182">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="b7468-182">Item = TEST</span></span>  

     <span data-ttu-id="b7468-183">Entry Type = Negative Adjustment</span><span class="sxs-lookup"><span data-stu-id="b7468-183">Entry Type = Negative Adjustment</span></span>  

     <span data-ttu-id="b7468-184">Quantity = 3</span><span class="sxs-lookup"><span data-stu-id="b7468-184">Quantity = 3</span></span>  

5.  <span data-ttu-id="b7468-185">Open Revaluation Journal, create, and post a line as follows:</span><span class="sxs-lookup"><span data-stu-id="b7468-185">Open Revaluation Journal, create, and post a line as follows:</span></span>  

     <span data-ttu-id="b7468-186">Item = TEST</span><span class="sxs-lookup"><span data-stu-id="b7468-186">Item = TEST</span></span>  

     <span data-ttu-id="b7468-187">Applies-to Entry = select Purchase entry posted at step 2.</span><span class="sxs-lookup"><span data-stu-id="b7468-187">Applies-to Entry = select Purchase entry posted at step 2.</span></span> <span data-ttu-id="b7468-188">The Posting Date of the revaluation will be the same as the entry it adjusts.</span><span class="sxs-lookup"><span data-stu-id="b7468-188">The Posting Date of the revaluation will be the same as the entry it adjusts.</span></span>  

     <span data-ttu-id="b7468-189">Unit Cost Revalued = 40</span><span class="sxs-lookup"><span data-stu-id="b7468-189">Unit Cost Revalued = 40</span></span>  

 <span data-ttu-id="b7468-190">The following Item Ledger and Value Entries have been posted:</span><span class="sxs-lookup"><span data-stu-id="b7468-190">The following Item Ledger and Value Entries have been posted:</span></span>  

<span data-ttu-id="b7468-191">![Overview of resulting item ledger and value entries 1](media/helene/TechArticleAdjustcost9.png "Overview of resulting item ledger and value entries 1")</span><span class="sxs-lookup"><span data-stu-id="b7468-191">![Overview of resulting item ledger and value entries 1](media/helene/TechArticleAdjustcost9.png "Overview of resulting item ledger and value entries 1")</span></span>

 <span data-ttu-id="b7468-192">![Overview of resulting item ledger and value entries 2](media/helene/TechArticleAdjustcost10.png "Overview of resulting item ledger and value entries 2")</span><span class="sxs-lookup"><span data-stu-id="b7468-192">![Overview of resulting item ledger and value entries 2](media/helene/TechArticleAdjustcost10.png "Overview of resulting item ledger and value entries 2")</span></span>

 <span data-ttu-id="b7468-193">The Adjust Cost – Item entries batch job has recognised a change in cost and adjusted the Negative Adjustments.</span><span class="sxs-lookup"><span data-stu-id="b7468-193">The Adjust Cost – Item entries batch job has recognized a change in cost and adjusted the Negative Adjustments.</span></span>  

 <span data-ttu-id="b7468-194">**Review of Posting Dates on created Adjustment Value Entries:** The earliest allowed Posting Date the Adjust Cost - Item Entries batch job has to relate to is January 1, 2014 as stated in the General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-194">**Review of Posting Dates on created Adjustment Value Entries:** The earliest allowed Posting Date the Adjust Cost - Item Entries batch job has to relate to is January 1, 2014 as stated in the General Ledger Setup.</span></span>  

 <span data-ttu-id="b7468-195">**Negative Adjustment in step 3:** assigned Posting Date is January 1, provided by General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-195">**Negative Adjustment in step 3:** assigned Posting Date is January 1, provided by General Ledger Setup.</span></span> <span data-ttu-id="b7468-196">The Posting Date of the Value Entry in scope for adjustment is December 20, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-196">The Posting Date of the Value Entry in scope for adjustment is December 20, 2013.</span></span> <span data-ttu-id="b7468-197">According to General Ledger Setup, the date is not within allowed posting date range.</span><span class="sxs-lookup"><span data-stu-id="b7468-197">According to General Ledger Setup, the date is not within allowed posting date range.</span></span> <span data-ttu-id="b7468-198">Therefore the Posting Date stated in the Allow Posting From field in the General Ledger Setup is assigned to the Adjustment Value Entry.</span><span class="sxs-lookup"><span data-stu-id="b7468-198">Therefore the Posting Date stated in the Allow Posting From field in the General Ledger Setup is assigned to the Adjustment Value Entry.</span></span>  

 <span data-ttu-id="b7468-199">**Negative Adjustment in step 4:** assigned Posting Date is January 15.</span><span class="sxs-lookup"><span data-stu-id="b7468-199">**Negative Adjustment in step 4:** assigned Posting Date is January 15.</span></span> <span data-ttu-id="b7468-200">The Value Entry in scope of adjustment has Posting Date January 15, which is within the allowed posting date range according to General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-200">The Value Entry in scope of adjustment has Posting Date January 15, which is within the allowed posting date range according to General Ledger Setup.</span></span>  

 <span data-ttu-id="b7468-201">The adjustment made for the Negative Adjustment in step 3 causes discussion.</span><span class="sxs-lookup"><span data-stu-id="b7468-201">The adjustment made for the Negative Adjustment in step 3 causes discussion.</span></span> <span data-ttu-id="b7468-202">The favorable Posting Date for the Adjustment Value Entry would have been December 20 or at least within December as the revaluation causing the change in COGS was posted in December.</span><span class="sxs-lookup"><span data-stu-id="b7468-202">The favorable Posting Date for the Adjustment Value Entry would have been December 20 or at least within December as the revaluation causing the change in COGS was posted in December.</span></span>  

 <span data-ttu-id="b7468-203">To achieve adjustment in December of the Negative Adjustment in step 3, the General Ledger Setup, Allow Posting From field, need to state a date in December.</span><span class="sxs-lookup"><span data-stu-id="b7468-203">To achieve adjustment in December of the Negative Adjustment in step 3, the General Ledger Setup, Allow Posting From field, need to state a date in December.</span></span>  

 <span data-ttu-id="b7468-204">**Conclusion:**</span><span class="sxs-lookup"><span data-stu-id="b7468-204">**Conclusion:**</span></span>  

 <span data-ttu-id="b7468-205">With the experiences from this scenario, considering most suitable setup of allowed posting date range for a company, you might want to consider the following information: As long as you allow changes in stock value to be posted in a period, December in this case, the setup that the company uses for allowed posting date ranges should be aligned with this decision.</span><span class="sxs-lookup"><span data-stu-id="b7468-205">With the experiences from this scenario, considering most suitable setup of allowed posting date range for a company, you might want to consider the following information: As long as you allow changes in inventory value to be posted in a period, December in this case, the setup that the company uses for allowed posting date ranges should be aligned with this decision.</span></span> <span data-ttu-id="b7468-206">The Allow Posting From in the General Ledger Setup, stating December 1, would allow the revaluation made in December to be forwarded to affected outbound entries in the same period.</span><span class="sxs-lookup"><span data-stu-id="b7468-206">The Allow Posting From in the General Ledger Setup, stating December 1, would allow the revaluation made in December to be forwarded to affected outbound entries in the same period.</span></span>  

 <span data-ttu-id="b7468-207">User groups not allowed to post in December but in January, which was probably intended to be limited by the General Ledger Setup in this scenario, should instead be addressed via the User setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-207">User groups not allowed to post in December but in January, which was probably intended to be limited by the General Ledger Setup in this scenario, should instead be addressed via the User setup.</span></span>  

### <a name="item-charge-scenario"></a><span data-ttu-id="b7468-208">Item charge scenario:</span><span class="sxs-lookup"><span data-stu-id="b7468-208">Item charge scenario:</span></span>  
 <span data-ttu-id="b7468-209">Prerequisites:</span><span class="sxs-lookup"><span data-stu-id="b7468-209">Prerequisites:</span></span>  

 <span data-ttu-id="b7468-210">Stock setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-210">Inventory setup:</span></span>  

-   <span data-ttu-id="b7468-211">Automatic Cost Posting = Yes</span><span class="sxs-lookup"><span data-stu-id="b7468-211">Automatic Cost Posting = Yes</span></span>  

-   <span data-ttu-id="b7468-212">Automatic Cost Adjustment=Always</span><span class="sxs-lookup"><span data-stu-id="b7468-212">Automatic Cost Adjustment=Always</span></span>  

-   <span data-ttu-id="b7468-213">Average Cost Calc. Type=item</span><span class="sxs-lookup"><span data-stu-id="b7468-213">Average Cost Calc. Type=item</span></span>  

-   <span data-ttu-id="b7468-214">Average Cost Period=Day</span><span class="sxs-lookup"><span data-stu-id="b7468-214">Average Cost Period=Day</span></span>  

 <span data-ttu-id="b7468-215">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-215">General Ledger Setup:</span></span>  

-   <span data-ttu-id="b7468-216">Allow Posting From = December 1, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-216">Allow Posting From = December 1, 2013.</span></span>  

-   <span data-ttu-id="b7468-217">Allow Posting To = empty</span><span class="sxs-lookup"><span data-stu-id="b7468-217">Allow Posting To = empty</span></span>  

 <span data-ttu-id="b7468-218">User Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-218">User Setup:</span></span>  

-   <span data-ttu-id="b7468-219">Allow Posting From = December 1, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-219">Allow Posting From = December 1, 2013.</span></span>  

-   <span data-ttu-id="b7468-220">Allow Posting to = empty</span><span class="sxs-lookup"><span data-stu-id="b7468-220">Allow Posting to = empty</span></span>  

##### <a name="to-test-the-scenario"></a><span data-ttu-id="b7468-221">To test the scenario</span><span class="sxs-lookup"><span data-stu-id="b7468-221">To test the scenario</span></span>  

1.  <span data-ttu-id="b7468-222">Create item charge:</span><span class="sxs-lookup"><span data-stu-id="b7468-222">Create item charge:</span></span>  

     <span data-ttu-id="b7468-223">Base unit of measurement = PCS</span><span class="sxs-lookup"><span data-stu-id="b7468-223">Base unit of measure = PCS</span></span>  

     <span data-ttu-id="b7468-224">Costing Method = Average</span><span class="sxs-lookup"><span data-stu-id="b7468-224">Costing Method = Average</span></span>  

     <span data-ttu-id="b7468-225">Select optional posting groups.</span><span class="sxs-lookup"><span data-stu-id="b7468-225">Select optional posting groups.</span></span>  

2.  <span data-ttu-id="b7468-226">Create new purchase order</span><span class="sxs-lookup"><span data-stu-id="b7468-226">Create new purchase order</span></span>  

     <span data-ttu-id="b7468-227">Buy-from Supplier No.: 10000</span><span class="sxs-lookup"><span data-stu-id="b7468-227">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="b7468-228">Posting Date = December 15, 2013</span><span class="sxs-lookup"><span data-stu-id="b7468-228">Posting Date = December 15, 2013</span></span>  

     <span data-ttu-id="b7468-229">Supplier Invoice No.: 1234</span><span class="sxs-lookup"><span data-stu-id="b7468-229">Vendor Invoice No.: 1234</span></span>  

     <span data-ttu-id="b7468-230">On the purchase order line:</span><span class="sxs-lookup"><span data-stu-id="b7468-230">On the purchase order line:</span></span>  

     <span data-ttu-id="b7468-231">Item = CHARGE</span><span class="sxs-lookup"><span data-stu-id="b7468-231">Item = CHARGE</span></span>  

     <span data-ttu-id="b7468-232">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="b7468-232">Quantity = 1</span></span>  

     <span data-ttu-id="b7468-233">Direct Unit Cost = 100</span><span class="sxs-lookup"><span data-stu-id="b7468-233">Direct Unit Cost = 100</span></span>  

     <span data-ttu-id="b7468-234">Post Receive and Invoice.</span><span class="sxs-lookup"><span data-stu-id="b7468-234">Post Receive and Invoice.</span></span>  

3.  <span data-ttu-id="b7468-235">Create new sales order:</span><span class="sxs-lookup"><span data-stu-id="b7468-235">Create new sales order:</span></span>  

     <span data-ttu-id="b7468-236">Sell-to Customer No.: 10000</span><span class="sxs-lookup"><span data-stu-id="b7468-236">Sell-to Customer No.: 10000</span></span>  

     <span data-ttu-id="b7468-237">Posting Date = December 16, 2013</span><span class="sxs-lookup"><span data-stu-id="b7468-237">Posting Date = December 16, 2013</span></span>  

     <span data-ttu-id="b7468-238">On the sales order line:</span><span class="sxs-lookup"><span data-stu-id="b7468-238">On the sales order line:</span></span>  

     <span data-ttu-id="b7468-239">Item = CHARGE</span><span class="sxs-lookup"><span data-stu-id="b7468-239">Item = CHARGE</span></span>  

     <span data-ttu-id="b7468-240">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="b7468-240">Quantity = 1</span></span>  

     <span data-ttu-id="b7468-241">Unit Price = 135</span><span class="sxs-lookup"><span data-stu-id="b7468-241">Unit Price = 135</span></span>  

     <span data-ttu-id="b7468-242">Post Ship and Invoice.</span><span class="sxs-lookup"><span data-stu-id="b7468-242">Post Ship and Invoice.</span></span>  

4.  <span data-ttu-id="b7468-243">General Ledger Setup:</span><span class="sxs-lookup"><span data-stu-id="b7468-243">General Ledger Setup:</span></span>  

     <span data-ttu-id="b7468-244">Allow Posting From = January 1, 2014</span><span class="sxs-lookup"><span data-stu-id="b7468-244">Allow Posting From = January 1, 2014</span></span>  

     <span data-ttu-id="b7468-245">Allow Posting To = blank</span><span class="sxs-lookup"><span data-stu-id="b7468-245">Allow Posting To = blank</span></span>  

5.  <span data-ttu-id="b7468-246">Create new purchase order:</span><span class="sxs-lookup"><span data-stu-id="b7468-246">Create new purchase order:</span></span>  

     <span data-ttu-id="b7468-247">Buy-from Supplier No.: 10000</span><span class="sxs-lookup"><span data-stu-id="b7468-247">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="b7468-248">Posting Date = January 2, 2014</span><span class="sxs-lookup"><span data-stu-id="b7468-248">Posting Date = January 2, 2014</span></span>  

     <span data-ttu-id="b7468-249">Supplier Invoice No.: 2345</span><span class="sxs-lookup"><span data-stu-id="b7468-249">Vendor Invoice No.: 2345</span></span>  

     <span data-ttu-id="b7468-250">On the purchase order line:</span><span class="sxs-lookup"><span data-stu-id="b7468-250">On the purchase order line:</span></span>  

     <span data-ttu-id="b7468-251">Item Charge = JB-FREIGHT</span><span class="sxs-lookup"><span data-stu-id="b7468-251">Item Charge = JB-FREIGHT</span></span>  

     <span data-ttu-id="b7468-252">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="b7468-252">Quantity = 1</span></span>  

     <span data-ttu-id="b7468-253">Direct Unit Cost = 3</span><span class="sxs-lookup"><span data-stu-id="b7468-253">Direct Unit Cost = 3</span></span>  

     <span data-ttu-id="b7468-254">Assign Item Charge to Purchase Receipt from step 2.</span><span class="sxs-lookup"><span data-stu-id="b7468-254">Assign Item Charge to Purchase Receipt from step 2.</span></span>  

     <span data-ttu-id="b7468-255">Post Receipt and Invoice.</span><span class="sxs-lookup"><span data-stu-id="b7468-255">Post Receipt and Invoice.</span></span>  

     <span data-ttu-id="b7468-256">![Overview of resulting item ledger and value entries 3](media/helene/TechArticleAdjustcost11.png "Overview of resulting item ledger and value entries 3")</span><span class="sxs-lookup"><span data-stu-id="b7468-256">![Overview of resulting item ledger and value entries 3](media/helene/TechArticleAdjustcost11.png "Overview of resulting item ledger and value entries 3")</span></span>

6.  <span data-ttu-id="b7468-257">On work date January 3, a purchase invoice arrives, containing an additional item charge to the purchase made in step 2.</span><span class="sxs-lookup"><span data-stu-id="b7468-257">On work date January 3, a purchase invoice arrives, containing an additional item charge to the purchase made in step 2.</span></span> <span data-ttu-id="b7468-258">This invoice has document date December 30 and is therefore posted with Posting Date December 30, 2013.</span><span class="sxs-lookup"><span data-stu-id="b7468-258">This invoice has document date December 30 and is therefore posted with Posting Date December 30, 2013.</span></span>  

     <span data-ttu-id="b7468-259">Create new purchase order:</span><span class="sxs-lookup"><span data-stu-id="b7468-259">Create new purchase order:</span></span>  

     <span data-ttu-id="b7468-260">Buy-from Supplier No.: 10000</span><span class="sxs-lookup"><span data-stu-id="b7468-260">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="b7468-261">Posting Date = December 30, 2013</span><span class="sxs-lookup"><span data-stu-id="b7468-261">Posting Date = December 30, 2013</span></span>  

     <span data-ttu-id="b7468-262">Supplier Invoice No.: 3456</span><span class="sxs-lookup"><span data-stu-id="b7468-262">Vendor Invoice No.: 3456</span></span>  

     <span data-ttu-id="b7468-263">On the purchase order line:</span><span class="sxs-lookup"><span data-stu-id="b7468-263">On the purchase order line:</span></span>  

     <span data-ttu-id="b7468-264">Item Charge = JB-FREIGHT</span><span class="sxs-lookup"><span data-stu-id="b7468-264">Item Charge = JB-FREIGHT</span></span>  

     <span data-ttu-id="b7468-265">Quantity = 1</span><span class="sxs-lookup"><span data-stu-id="b7468-265">Quantity = 1</span></span>  

     <span data-ttu-id="b7468-266">Direct Unit Cost = 2</span><span class="sxs-lookup"><span data-stu-id="b7468-266">Direct Unit Cost = 2</span></span>  

     <span data-ttu-id="b7468-267">Assign Item Charge to Purchase Receipt from step 2</span><span class="sxs-lookup"><span data-stu-id="b7468-267">Assign Item Charge to Purchase Receipt from step 2</span></span>  

     <span data-ttu-id="b7468-268">Post Receipt and Invoice.</span><span class="sxs-lookup"><span data-stu-id="b7468-268">Post Receipt and Invoice.</span></span>  

   <span data-ttu-id="b7468-269">![Overview of resulting item ledger and value entries 4](media/helene/TechArticleAdjustcost12.png "Overview of resulting item ledger and value entries 4")</span><span class="sxs-lookup"><span data-stu-id="b7468-269">![Overview of resulting item ledger and value entries 4](media/helene/TechArticleAdjustcost12.png "Overview of resulting item ledger and value entries 4")</span></span>

 <span data-ttu-id="b7468-270">Stock Valuation report is printed as at Date December 31, 2013</span><span class="sxs-lookup"><span data-stu-id="b7468-270">Inventory Valuation report is printed as of Date December 31 , 2013</span></span>  

<span data-ttu-id="b7468-271">![Content of the Stock Valuation report](media/helene/TechArticleAdjustcost13.png "Content of the Stock Valuation report")</span><span class="sxs-lookup"><span data-stu-id="b7468-271">![Content of the Inventory Valuation report](media/helene/TechArticleAdjustcost13.png "Content of the Inventory Valuation report")</span></span>

 <span data-ttu-id="b7468-272">**Summary of scenario:**</span><span class="sxs-lookup"><span data-stu-id="b7468-272">**Summary of scenario:**</span></span>  

 <span data-ttu-id="b7468-273">The described scenario ends up with an Stock Valuation report demonstrating Quantity = 0 while the Value = 2.</span><span class="sxs-lookup"><span data-stu-id="b7468-273">The described scenario ends up with an Inventory Valuation report demonstrating Quantity = 0 while the Value = 2.</span></span> <span data-ttu-id="b7468-274">The Item charge posted in step 11 is part of the Stock Increase value of December while the Stock Decrease of the same period is not affected.</span><span class="sxs-lookup"><span data-stu-id="b7468-274">The Item charge posted in step 11 is part of the Inventory Increase value of December while the Inventory Decrease of the same period is not affected.</span></span>  

 <span data-ttu-id="b7468-275">Having the General Ledger Setup stating Allow Posting From January 1 was a good thing for the first Item charge.</span><span class="sxs-lookup"><span data-stu-id="b7468-275">Having the General Ledger Setup stating Allow Posting From January 1 was a good thing for the first Item charge.</span></span> <span data-ttu-id="b7468-276">The costs of the Stock Increase and Decrease was recorded in the same period.</span><span class="sxs-lookup"><span data-stu-id="b7468-276">The costs of the Inventory Increase and Decrease was recorded in the same period.</span></span> <span data-ttu-id="b7468-277">For the second Item charge however, the General Ledger Setup causes the change in COGS to be recognised in the period after.</span><span class="sxs-lookup"><span data-stu-id="b7468-277">For the second Item charge however, the General Ledger Setup causes the change in COGS to be recognized in the period after.</span></span>  

 <span data-ttu-id="b7468-278">**Conclusion:**</span><span class="sxs-lookup"><span data-stu-id="b7468-278">**Conclusion:**</span></span>  

 <span data-ttu-id="b7468-279">It’s a challenge to have the Stock Valuation report to demonstrate Quantity = 0 while the Value <> 0.</span><span class="sxs-lookup"><span data-stu-id="b7468-279">It’s a challenge to have the Inventory Valuation report to demonstrate Quantity = 0 while the Value <> 0.</span></span> <span data-ttu-id="b7468-280">In this case it’s also more difficult to express the optimal settings, having purchase invoices arriving the same day but addressing different periods or even financial years.</span><span class="sxs-lookup"><span data-stu-id="b7468-280">In this case it’s also more difficult to express the optimal settings, having purchase invoices arriving the same day but addressing different periods or even fiscal years.</span></span> <span data-ttu-id="b7468-281">Crossing to a new financial year usually requires some planning and as part of that the insight of Adjust Cost – Item entries process, recognising COGS, is to be considered.</span><span class="sxs-lookup"><span data-stu-id="b7468-281">Crossing to a new fiscal year usually requires some planning and as part of that the insight of Adjust Cost – Item entries process, recognizing COGS, is to be considered.</span></span>  

 <span data-ttu-id="b7468-282">In this scenario one option could have been to have the General Ledger Setup, field Allow Posting From, stating a date in December for a couple of more days and the posting of the first item charge postponed to allow all costs for the previous period/financial year to be recognised for the period they belong to first, having the Adjust Cost – Item entries batch job run and thereafter move the allowed posting date to the new period\/financial year.</span><span class="sxs-lookup"><span data-stu-id="b7468-282">In this scenario one option could have been to have the General Ledger Setup, field Allow Posting From, stating a date in December for a couple of more days and the posting of the first item charge postponed to allow all costs for the previous period/fiscal year to be recognized for the period they belong to first, having the Adjust Cost – Item entries batch job run and thereafter move the allowed posting date to the new period\/fiscal year.</span></span> <span data-ttu-id="b7468-283">The first item charge with posting date January 2 could then be posted.</span><span class="sxs-lookup"><span data-stu-id="b7468-283">The first item charge with posting date January 2 could then be posted.</span></span>  

## <a name="history-of-adjust-cost--item-entries-batch-job"></a><span data-ttu-id="b7468-284">History of Adjust Cost – Item entries batch job</span><span class="sxs-lookup"><span data-stu-id="b7468-284">History of Adjust Cost – Item entries batch job</span></span>  
 <span data-ttu-id="b7468-285">Below is a summary of the concept assigning Posting Dates to Adjustment Value Entries by the Adjust Cost – Item entries batch job.</span><span class="sxs-lookup"><span data-stu-id="b7468-285">Below is a summary of the concept assigning Posting Dates to Adjustment Value Entries by the Adjust Cost – Item entries batch job.</span></span>  

### <a name="about-the-request-form-posting-date"></a><span data-ttu-id="b7468-286">About the request form posting date:</span><span class="sxs-lookup"><span data-stu-id="b7468-286">About the request form posting date:</span></span>  
 <span data-ttu-id="b7468-287">There is no longer a posting date to be stated in the request form of the Adjust Cost - Item entries batch job.</span><span class="sxs-lookup"><span data-stu-id="b7468-287">There is no longer a posting date to be stated in the request form of the Adjust Cost - Item entries batch job.</span></span> <span data-ttu-id="b7468-288">The batch job runs through all necessary changes and creates value entries with the posting date of the value entry it adjusts.</span><span class="sxs-lookup"><span data-stu-id="b7468-288">The batch job runs through all necessary changes and creates value entries with the posting date of the value entry it adjusts.</span></span> <span data-ttu-id="b7468-289">If the posting date is not within allowed posting date range the posting date in the Allow Posting From field in the General Ledger Setup, OR if the Stock periods are used, the later date of the two will be used.</span><span class="sxs-lookup"><span data-stu-id="b7468-289">If the posting date is not within allowed posting date range the posting date in the Allow Posting From field in the General Ledger Setup, OR if the Inventory periods are used, the later date of the two will be used.</span></span> <span data-ttu-id="b7468-290">See described concept above.</span><span class="sxs-lookup"><span data-stu-id="b7468-290">See described concept above.</span></span>  

## <a name="history-of-post-inventory-cost-to-gl-batch-job"></a><span data-ttu-id="b7468-291">History of Post Stock cost to G/L batch job</span><span class="sxs-lookup"><span data-stu-id="b7468-291">History of Post Inventory cost to G/L batch job</span></span>  
 <span data-ttu-id="b7468-292">The Post Stock Cost to G/L batch job is closely related to the Adjust Cost – Item entries batch job why the history of this batch job is summarised and shared here as well.</span><span class="sxs-lookup"><span data-stu-id="b7468-292">The Post Inventory Cost to G/L batch job is closely related to the Adjust Cost – Item entries batch job why the history of this batch job is summarized and shared here as well.</span></span>  
 
<span data-ttu-id="b7468-293">![Actual cost versus expected cost](media/helene/TechArticleAdjustcost14.png "Actual cost versus expected cost")</span><span class="sxs-lookup"><span data-stu-id="b7468-293">![Actual cost versus expected cost](media/helene/TechArticleAdjustcost14.png "Actual cost versus expected cost")</span></span>

### <a name="about-the-posting-date"></a><span data-ttu-id="b7468-294">About the posting date</span><span class="sxs-lookup"><span data-stu-id="b7468-294">About the posting date</span></span>
 <span data-ttu-id="b7468-295">There is no longer a posting date to be stated in the request form of the Post Stock Cost to G/L batch job.</span><span class="sxs-lookup"><span data-stu-id="b7468-295">There is no longer a posting date to be stated in the request form of the Post Inventory Cost to G/L batch job.</span></span> <span data-ttu-id="b7468-296">The G/L entry is created with the same Posting Date as the related value entry.</span><span class="sxs-lookup"><span data-stu-id="b7468-296">The G/L entry is created with the same Posting Date as the related value entry.</span></span> <span data-ttu-id="b7468-297">In order to complete the batch job, the allowed posting date range must allow the Posting Date of the created G/L entry.</span><span class="sxs-lookup"><span data-stu-id="b7468-297">In order to complete the batch job, the allowed posting date range must allow the Posting Date of the created G/L entry.</span></span> <span data-ttu-id="b7468-298">If not, the allowed posting date range must be temporarily reopened by changing or removing the dates in the Allow Posting From and To fields in the General Ledger Setup.</span><span class="sxs-lookup"><span data-stu-id="b7468-298">If not, the allowed posting date range must be temporarily reopened by changing or removing the dates in the Allow Posting From and To fields in the General Ledger Setup.</span></span> <span data-ttu-id="b7468-299">To avoid reconciliation issues, it is required that Posting Date of the G/L Entry corresponds to the Posting Date of the Value Entry.</span><span class="sxs-lookup"><span data-stu-id="b7468-299">To avoid reconciliation issues, it is required that Posting Date of the G/L Entry corresponds to the Posting Date of the Value Entry.</span></span>  

 <span data-ttu-id="b7468-300">The batch job scans Table 5811 - Post Value Entry to G/L, to identify the Value Entries in scope for posting to General Ledger.</span><span class="sxs-lookup"><span data-stu-id="b7468-300">The batch job scans Table 5811 - Post Value Entry to G/L, to identify the Value Entries in scope for posting to General Ledger.</span></span> <span data-ttu-id="b7468-301">After a successful run, the table is emptied.</span><span class="sxs-lookup"><span data-stu-id="b7468-301">After a successful run, the table is emptied.</span></span>

## <a name="see-also"></a><span data-ttu-id="b7468-302">See Also</span><span class="sxs-lookup"><span data-stu-id="b7468-302">See Also</span></span>  
[<span data-ttu-id="b7468-303">Design Details: Stock Costing</span><span class="sxs-lookup"><span data-stu-id="b7468-303">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)  
[<span data-ttu-id="b7468-304">Design Details: Item Application</span><span class="sxs-lookup"><span data-stu-id="b7468-304">Design Details: Item Application</span></span>](design-details-item-application.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
