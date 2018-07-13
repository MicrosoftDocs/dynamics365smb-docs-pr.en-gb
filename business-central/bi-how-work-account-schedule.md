---
title: Build financial reports using account schedules
description: Describes how to use account schedules to create various views and report for analysing financial performance data.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 05/31/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: e73c2dd0533aade4aa6225c9d2f385baaea3cfd1
ms.openlocfilehash: 69034b0eb97b595d0fbf5795e1fac34ecd775afe
ms.contentlocale: en-gb
ms.lasthandoff: 06/11/2018

---
# <a name="prepare-financial-reporting-with-account-schedules-and-account-categories"></a><span data-ttu-id="a2c58-103">Prepare Financial Reporting with Account Schedules and Account Categories</span><span class="sxs-lookup"><span data-stu-id="a2c58-103">Prepare Financial Reporting with Account Schedules and Account Categories</span></span>
<span data-ttu-id="a2c58-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="a2c58-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span></span> <span data-ttu-id="a2c58-105">Account schedules analyse figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span><span class="sxs-lookup"><span data-stu-id="a2c58-105">Account schedules analyze figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="a2c58-106">The results display in charts on your Role Centre, such as the Cash Flow chart, and in reports, such as the Income Statement and the Balance Sheet reports.</span><span class="sxs-lookup"><span data-stu-id="a2c58-106">The results display in charts on your Role Center, such as the Cash Flow chart, and in reports, such as the Income Statement and the Balance Sheet reports.</span></span>

<span data-ttu-id="a2c58-107">You access these two reports, for example, with the **Financials Statements** action on the Business Manager and Accountant Role Centres.</span><span class="sxs-lookup"><span data-stu-id="a2c58-107">You access these two reports, for example, with the **Financials Statements** action on the Business Manager and Accountant Role Centers.</span></span>   

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="a2c58-108"> provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span><span class="sxs-lookup"><span data-stu-id="a2c58-108"> provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span></span> <span data-ttu-id="a2c58-109">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span><span class="sxs-lookup"><span data-stu-id="a2c58-109">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span></span> <span data-ttu-id="a2c58-110">You can create as many customised financial statements as you want.</span><span class="sxs-lookup"><span data-stu-id="a2c58-110">You can create as many customized financial statements as you want.</span></span>  

<span data-ttu-id="a2c58-111">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="a2c58-111">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span></span> <span data-ttu-id="a2c58-112">For example, you can view general ledger entries as percentages of budget entries.</span><span class="sxs-lookup"><span data-stu-id="a2c58-112">For example, you can view general ledger entries as percentages of budget entries.</span></span> <span data-ttu-id="a2c58-113">This requires that budgets are created.</span><span class="sxs-lookup"><span data-stu-id="a2c58-113">This requires that budgets are created.</span></span> <span data-ttu-id="a2c58-114">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="a2c58-114">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

## <a name="account-categories-and-account-schedules"></a><span data-ttu-id="a2c58-115">Account Categories and Account Schedules</span><span class="sxs-lookup"><span data-stu-id="a2c58-115">Account Categories and Account Schedules</span></span>
<span data-ttu-id="a2c58-116">You can use account categories to change the layout of your financial statements.</span><span class="sxs-lookup"><span data-stu-id="a2c58-116">You can use account categories to change the layout of your financial statements.</span></span> <span data-ttu-id="a2c58-117">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span><span class="sxs-lookup"><span data-stu-id="a2c58-117">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span></span> <span data-ttu-id="a2c58-118">The next time you run one of these reports, such as the Balance Statement report, new totals and subentries are added, based on your changes.</span><span class="sxs-lookup"><span data-stu-id="a2c58-118">The next time you run one of these reports, such as the Balance Statement report, new totals and subentries are added, based on your changes.</span></span> <span data-ttu-id="a2c58-119">For more information, see The "Account Categories" section in [Understanding the General Ledger and the COA](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="a2c58-119">For more information, see The "Account Categories" section in [Understanding the General Ledger and the COA](finance-general-ledger.md).</span></span>  

## <a name="to-create-new-account-schedules"></a><span data-ttu-id="a2c58-120">To create new account schedules</span><span class="sxs-lookup"><span data-stu-id="a2c58-120">To create new account schedules</span></span>  
 <span data-ttu-id="a2c58-121">You use account schedules to analyse figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span><span class="sxs-lookup"><span data-stu-id="a2c58-121">You use account schedules to analyze figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="a2c58-122">For example, you can view the general ledger entries as percentages of the budget entries.</span><span class="sxs-lookup"><span data-stu-id="a2c58-122">For example, you can view the general ledger entries as percentages of the budget entries.</span></span>

1. <span data-ttu-id="a2c58-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a2c58-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a2c58-124">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span><span class="sxs-lookup"><span data-stu-id="a2c58-124">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span></span>
3. <span data-ttu-id="a2c58-125">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a2c58-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="a2c58-126">Choose the **Edit Account Schedule** action.</span><span class="sxs-lookup"><span data-stu-id="a2c58-126">Choose the **Edit Account Schedule** action.</span></span>
5. <span data-ttu-id="a2c58-127">In the **Account Schedule** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a2c58-127">In the **Account Schedule** window, fill in the fields as necessary.</span></span>  

    <span data-ttu-id="a2c58-128">When you have created a new account schedule and set up the rows, you must set up columns.</span><span class="sxs-lookup"><span data-stu-id="a2c58-128">When you have created a new account schedule and set up the rows, you must set up columns.</span></span> <span data-ttu-id="a2c58-129">You can either set them up manually or assign a predefined column layout to your account schedule.</span><span class="sxs-lookup"><span data-stu-id="a2c58-129">You can either set them up manually or assign a predefined column layout to your account schedule.</span></span>
6. <span data-ttu-id="a2c58-130">Choose the **Edit Column Layout Setup** action.</span><span class="sxs-lookup"><span data-stu-id="a2c58-130">Choose the **Edit Column Layout Setup** action.</span></span>
7. <span data-ttu-id="a2c58-131">In the **Column Layout** window, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="a2c58-131">In the **Column Layout** window, fill in the fields as necessary.</span></span>

> [!NOTE]  
> <span data-ttu-id="a2c58-132">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span><span class="sxs-lookup"><span data-stu-id="a2c58-132">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span></span>

### <a name="to-copy-an-existing-account-schedule"></a><span data-ttu-id="a2c58-133">To copy an existing account schedule</span><span class="sxs-lookup"><span data-stu-id="a2c58-133">To copy an existing account schedule</span></span>
<span data-ttu-id="a2c58-134">The account schedules in the standard version of [!INCLUDE[d365fin](includes/d365fin_md.md)] are the basis of the standard financial reports, which may not suit the needs of your business.</span><span class="sxs-lookup"><span data-stu-id="a2c58-134">The account schedules in the standard version of [!INCLUDE[d365fin](includes/d365fin_md.md)] are the basis of the standard financial reports, which may not suit the needs of your business.</span></span> <span data-ttu-id="a2c58-135">To quickly create your own financial reports, you can start by copying an existing account schedule.</span><span class="sxs-lookup"><span data-stu-id="a2c58-135">To quickly create your own financial reports, you can start by copying an existing account schedule.</span></span>
1. <span data-ttu-id="a2c58-136">In the **Account Schedules** window, select an account schedule, and then choose the **Copy Account Schedule** action.</span><span class="sxs-lookup"><span data-stu-id="a2c58-136">In the **Account Schedules** window, select an account schedule, and then choose the **Copy Account Schedule** action.</span></span>
2. <span data-ttu-id="a2c58-137">In the **Copy Account Schedule** window, fill in the fields as necessary, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a2c58-137">In the **Copy Account Schedule** window, fill in the fields as necessary, and then choose the **OK** button.</span></span>

### <a name="to-create-a-column-that-calculates-percentages"></a><span data-ttu-id="a2c58-138">To create a column that calculates percentages</span><span class="sxs-lookup"><span data-stu-id="a2c58-138">To create a column that calculates percentages</span></span>  
<span data-ttu-id="a2c58-139">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span><span class="sxs-lookup"><span data-stu-id="a2c58-139">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span></span> <span data-ttu-id="a2c58-140">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span><span class="sxs-lookup"><span data-stu-id="a2c58-140">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span></span>

1. <span data-ttu-id="a2c58-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a2c58-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="a2c58-142">In the **Account Schedule Names** window, select an account schedule.</span><span class="sxs-lookup"><span data-stu-id="a2c58-142">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="a2c58-143">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span><span class="sxs-lookup"><span data-stu-id="a2c58-143">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span></span>  
4. <span data-ttu-id="a2c58-144">Insert a line immediately above the first row for which you want to display a percentage.</span><span class="sxs-lookup"><span data-stu-id="a2c58-144">Insert a line immediately above the first row for which you want to display a percentage.</span></span>  
5. <span data-ttu-id="a2c58-145">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span><span class="sxs-lookup"><span data-stu-id="a2c58-145">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span></span> <span data-ttu-id="a2c58-146">In the **Totalling** field, enter a formula for the total that the percentage will be based on.</span><span class="sxs-lookup"><span data-stu-id="a2c58-146">In the **Totaling** field, enter a formula for the total that the percentage will be based on.</span></span> <span data-ttu-id="a2c58-147">For example, if row 11 contains the total sales, enter **11**.</span><span class="sxs-lookup"><span data-stu-id="a2c58-147">For example, if row 11 contains the total sales, enter **11**.</span></span>  
6. <span data-ttu-id="a2c58-148">Choose the **Edit Column Layout Setup** action to set up a column.</span><span class="sxs-lookup"><span data-stu-id="a2c58-148">Choose the **Edit Column Layout Setup** action to set up a column.</span></span>  
7. <span data-ttu-id="a2c58-149">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span><span class="sxs-lookup"><span data-stu-id="a2c58-149">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span></span> <span data-ttu-id="a2c58-150">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span><span class="sxs-lookup"><span data-stu-id="a2c58-150">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span></span> <span data-ttu-id="a2c58-151">For example, if column number N contains the net change, enter **N%**.</span><span class="sxs-lookup"><span data-stu-id="a2c58-151">For example, if column number N contains the net change, enter **N%**.</span></span>  
8. <span data-ttu-id="a2c58-152">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span><span class="sxs-lookup"><span data-stu-id="a2c58-152">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span></span>

## <a name="to-set-up-account-schedules-with-overviews"></a><span data-ttu-id="a2c58-153">To set up account schedules with overviews</span><span class="sxs-lookup"><span data-stu-id="a2c58-153">To set up account schedules with overviews</span></span>  
<span data-ttu-id="a2c58-154">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span><span class="sxs-lookup"><span data-stu-id="a2c58-154">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span></span>

1. <span data-ttu-id="a2c58-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a2c58-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="a2c58-156">In the **Account Schedule Names** window, select an account schedule.</span><span class="sxs-lookup"><span data-stu-id="a2c58-156">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="a2c58-157">Choose the **Edit Account Schedule** action</span><span class="sxs-lookup"><span data-stu-id="a2c58-157">Choose the **Edit Account Schedule** action</span></span>  
4. <span data-ttu-id="a2c58-158">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span><span class="sxs-lookup"><span data-stu-id="a2c58-158">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span></span>
5. <span data-ttu-id="a2c58-159">Choose the **Insert Accounts** action.</span><span class="sxs-lookup"><span data-stu-id="a2c58-159">Choose the **Insert Accounts** action.</span></span>  
6. <span data-ttu-id="a2c58-160">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a2c58-160">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span></span>

    <span data-ttu-id="a2c58-161">The accounts are now inserted into your account schedule.</span><span class="sxs-lookup"><span data-stu-id="a2c58-161">The accounts are now inserted into your account schedule.</span></span> <span data-ttu-id="a2c58-162">If you want you can also change the column layout.</span><span class="sxs-lookup"><span data-stu-id="a2c58-162">If you want you can also change the column layout.</span></span>  
7. <span data-ttu-id="a2c58-163">Choose the **Overview** action.</span><span class="sxs-lookup"><span data-stu-id="a2c58-163">Choose the **Overview** action.</span></span>  
8. <span data-ttu-id="a2c58-164">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span><span class="sxs-lookup"><span data-stu-id="a2c58-164">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span></span>  
9. <span data-ttu-id="a2c58-165">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="a2c58-165">Choose the **OK** button.</span></span>  

<span data-ttu-id="a2c58-166">Now you can copy and paste your budget statement into a spreadsheet.</span><span class="sxs-lookup"><span data-stu-id="a2c58-166">Now you can copy and paste your budget statement into a spreadsheet.</span></span>  

## <a name="comparing-accounting-periods-using-period-formulas"></a><span data-ttu-id="a2c58-167">Comparing Accounting Periods using Period Formulas</span><span class="sxs-lookup"><span data-stu-id="a2c58-167">Comparing Accounting Periods using Period Formulas</span></span>
<span data-ttu-id="a2c58-168">Your account schedule can compare the results of different accounting periods, such as this month versus same month last year.</span><span class="sxs-lookup"><span data-stu-id="a2c58-168">Your account schedule can compare the results of different accounting periods, such as this month versus same month last year.</span></span> <span data-ttu-id="a2c58-169">To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.</span><span class="sxs-lookup"><span data-stu-id="a2c58-169">To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.</span></span>  

<span data-ttu-id="a2c58-170">An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.</span><span class="sxs-lookup"><span data-stu-id="a2c58-170">An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.</span></span>   

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="a2c58-171"> uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request.</span><span class="sxs-lookup"><span data-stu-id="a2c58-171"> uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request.</span></span> <span data-ttu-id="a2c58-172">The comparison period is based on the period of the start date of the date filter.</span><span class="sxs-lookup"><span data-stu-id="a2c58-172">The comparison period is based on the period of the start date of the date filter.</span></span> <span data-ttu-id="a2c58-173">The abbreviations for period specifications are:</span><span class="sxs-lookup"><span data-stu-id="a2c58-173">The abbreviations for period specifications are:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a2c58-174">Abbreviation</span><span class="sxs-lookup"><span data-stu-id="a2c58-174">Abbreviation</span></span></th>
<th><span data-ttu-id="a2c58-175">Description</span><span class="sxs-lookup"><span data-stu-id="a2c58-175">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="a2c58-176">P</span><span class="sxs-lookup"><span data-stu-id="a2c58-176">P</span></span></p></td>
<td><p><span data-ttu-id="a2c58-177">Period</span><span class="sxs-lookup"><span data-stu-id="a2c58-177">Period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a2c58-178">LP</span><span class="sxs-lookup"><span data-stu-id="a2c58-178">LP</span></span></p></td>
<td><p><span data-ttu-id="a2c58-179">Last period of a fiscal year, half-year or quarter.</span><span class="sxs-lookup"><span data-stu-id="a2c58-179">Last period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a2c58-180">CP</span><span class="sxs-lookup"><span data-stu-id="a2c58-180">CP</span></span></p></td>
<td><p><span data-ttu-id="a2c58-181">Current period of a fiscal year, half-year or quarter.</span><span class="sxs-lookup"><span data-stu-id="a2c58-181">Current period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a2c58-182">FY</span><span class="sxs-lookup"><span data-stu-id="a2c58-182">FY</span></span></p></td>
<td><p><span data-ttu-id="a2c58-183">Fiscal year.</span><span class="sxs-lookup"><span data-stu-id="a2c58-183">Fiscal year.</span></span> <span data-ttu-id="a2c58-184">For example, FY[1..3] denotes first quarter of the current fiscal year</span><span class="sxs-lookup"><span data-stu-id="a2c58-184">For example, FY[1..3] denotes first quarter of the current fiscal year</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="a2c58-185">Examples of formulas:</span><span class="sxs-lookup"><span data-stu-id="a2c58-185">Examples of formulas:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a2c58-186">Formula</span><span class="sxs-lookup"><span data-stu-id="a2c58-186">Formula</span></span></th>
<th><span data-ttu-id="a2c58-187">Description</span><span class="sxs-lookup"><span data-stu-id="a2c58-187">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="a2c58-188">&lt;Blank&gt;</span><span class="sxs-lookup"><span data-stu-id="a2c58-188">&lt;Blank&gt;</span></span></p></td>
<td><p><span data-ttu-id="a2c58-189">Current period</span><span class="sxs-lookup"><span data-stu-id="a2c58-189">Current period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a2c58-190">-1P</span><span class="sxs-lookup"><span data-stu-id="a2c58-190">-1P</span></span></p></td>
<td><p><span data-ttu-id="a2c58-191">Previous period</span><span class="sxs-lookup"><span data-stu-id="a2c58-191">Previous period</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a2c58-192">-1FY[1..LP]</span><span class="sxs-lookup"><span data-stu-id="a2c58-192">-1FY[1..LP]</span></span></p></td>
<td><p><span data-ttu-id="a2c58-193">Entire previous fiscal year</span><span class="sxs-lookup"><span data-stu-id="a2c58-193">Entire previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a2c58-194">-1FY</span><span class="sxs-lookup"><span data-stu-id="a2c58-194">-1FY</span></span></p></td>
<td><p><span data-ttu-id="a2c58-195">Current period in previous fiscal year</span><span class="sxs-lookup"><span data-stu-id="a2c58-195">Current period in previous fiscal year</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a2c58-196">-1FY[1..3]</span><span class="sxs-lookup"><span data-stu-id="a2c58-196">-1FY[1..3]</span></span></p></td>
<td><p><span data-ttu-id="a2c58-197">First quarter of previous fiscal year</span><span class="sxs-lookup"><span data-stu-id="a2c58-197">First quarter of previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a2c58-198">-1FY[1..CP]</span><span class="sxs-lookup"><span data-stu-id="a2c58-198">-1FY[1..CP]</span></span></p></td>
<td><p><span data-ttu-id="a2c58-199">From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</span><span class="sxs-lookup"><span data-stu-id="a2c58-199">From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a2c58-200">-1FY[CP..LP]</span><span class="sxs-lookup"><span data-stu-id="a2c58-200">-1FY[CP..LP]</span></span></p></td>
<td><p><span data-ttu-id="a2c58-201">From current period in previous fiscal year to last period of previous fiscal year, inclusive</span><span class="sxs-lookup"><span data-stu-id="a2c58-201">From current period in previous fiscal year to last period of previous fiscal year, inclusive</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="a2c58-202">If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.</span><span class="sxs-lookup"><span data-stu-id="a2c58-202">If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.</span></span>

> [!NOTE]
> <span data-ttu-id="a2c58-203">It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts.</span><span class="sxs-lookup"><span data-stu-id="a2c58-203">It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts.</span></span> <span data-ttu-id="a2c58-204">For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*.</span><span class="sxs-lookup"><span data-stu-id="a2c58-204">For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*.</span></span> <span data-ttu-id="a2c58-205">Then, you run the report on February 28th and set the date filter to January and February.</span><span class="sxs-lookup"><span data-stu-id="a2c58-205">Then, you run the report on February 28th and set the date filter to January and February.</span></span> <span data-ttu-id="a2c58-206">As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.</span><span class="sxs-lookup"><span data-stu-id="a2c58-206">As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.</span></span>  


## <a name="see-also"></a><span data-ttu-id="a2c58-207">See Also</span><span class="sxs-lookup"><span data-stu-id="a2c58-207">See Also</span></span>
[<span data-ttu-id="a2c58-208">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="a2c58-208">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="a2c58-209">Finance</span><span class="sxs-lookup"><span data-stu-id="a2c58-209">Finance</span></span>](finance.md)  
[<span data-ttu-id="a2c58-210">Setting Up Finance</span><span class="sxs-lookup"><span data-stu-id="a2c58-210">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="a2c58-211">The General Ledger and the Chart of Accounts</span><span class="sxs-lookup"><span data-stu-id="a2c58-211">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="a2c58-212">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a2c58-212">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

