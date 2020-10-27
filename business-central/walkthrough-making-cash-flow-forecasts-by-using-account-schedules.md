---
title: Walkthrough - Making Cash Flow Forecasts by Using Account Schedules | Microsoft Docs
description: This walkthrough describes how you can use account schedules to make cash flow forecasts. Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts. In the account schedules, you can set up subtotals for cash flow receipts and disbursements. These subtotals can be included in new totals that can then be used in making cash flow forecasts.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 67a6e963800bf5f0ce8e1a293463d53b51470ee5
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3914792"
---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a><span data-ttu-id="127a3-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span><span class="sxs-lookup"><span data-stu-id="127a3-106">Walkthrough: Making Cash Flow Forecasts by Using Account Schedules</span></span>
<span data-ttu-id="127a3-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="127a3-107">This walkthrough describes how you can use account schedules to make cash flow forecasts.</span></span> <span data-ttu-id="127a3-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span><span class="sxs-lookup"><span data-stu-id="127a3-108">Account schedules perform calculations that cannot be done directly in the chart of cash flow accounts.</span></span> <span data-ttu-id="127a3-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span><span class="sxs-lookup"><span data-stu-id="127a3-109">In the account schedules, you can set up subtotals for cash flow receipts and disbursements.</span></span> <span data-ttu-id="127a3-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="127a3-110">These subtotals can be included in new totals that can then be used in making cash flow forecasts.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="127a3-111">About This Walkthrough</span><span class="sxs-lookup"><span data-stu-id="127a3-111">About This Walkthrough</span></span>  
<span data-ttu-id="127a3-112">This walkthrough describes the following tasks:</span><span class="sxs-lookup"><span data-stu-id="127a3-112">This walkthrough describes the following tasks:</span></span>  

- <span data-ttu-id="127a3-113">Setting up a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="127a3-113">Setting up a new cash flow account schedule name.</span></span>  
- <span data-ttu-id="127a3-114">Setting up account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="127a3-114">Setting up account schedule lines.</span></span>  
- <span data-ttu-id="127a3-115">Setting up a new column layout.</span><span class="sxs-lookup"><span data-stu-id="127a3-115">Setting up a new column layout.</span></span>  
- <span data-ttu-id="127a3-116">Assigning a column layout to an account schedule.</span><span class="sxs-lookup"><span data-stu-id="127a3-116">Assigning a column layout to an account schedule.</span></span>  
- <span data-ttu-id="127a3-117">Viewing and printing the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="127a3-117">Viewing and printing the cash flow forecast.</span></span>  

### <a name="prerequisites"></a><span data-ttu-id="127a3-118">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="127a3-118">Prerequisites</span></span>  
<span data-ttu-id="127a3-119">To complete this walkthrough, you will need:</span><span class="sxs-lookup"><span data-stu-id="127a3-119">To complete this walkthrough, you will need:</span></span>  

- [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="127a3-120">installed.</span><span class="sxs-lookup"><span data-stu-id="127a3-120">installed.</span></span>  
- <span data-ttu-id="127a3-121">The cash flow worksheet lines are registered.</span><span class="sxs-lookup"><span data-stu-id="127a3-121">The cash flow worksheet lines are registered.</span></span>  

## <a name="roles"></a><span data-ttu-id="127a3-122">Roles</span><span class="sxs-lookup"><span data-stu-id="127a3-122">Roles</span></span>  
<span data-ttu-id="127a3-123">This walkthrough demonstrates tasks that are performed by the following user role:</span><span class="sxs-lookup"><span data-stu-id="127a3-123">This walkthrough demonstrates tasks that are performed by the following user role:</span></span>  

- <span data-ttu-id="127a3-124">Controller</span><span class="sxs-lookup"><span data-stu-id="127a3-124">Controller</span></span>  

## <a name="story"></a><span data-ttu-id="127a3-125">Story</span><span class="sxs-lookup"><span data-stu-id="127a3-125">Story</span></span>  
<span data-ttu-id="127a3-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span><span class="sxs-lookup"><span data-stu-id="127a3-126">Ken is a controller at CRONUS who makes monthly cash flow forecasts.</span></span> <span data-ttu-id="127a3-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span><span class="sxs-lookup"><span data-stu-id="127a3-127">He includes finance, sales, purchase, and fixed assets in the forecast, and then he presents it to CFO Sara for business insight.</span></span>  

## <a name="setting-up-a-new-account-schedule-name"></a><span data-ttu-id="127a3-128">Setting Up a New Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="127a3-128">Setting Up a New Account Schedule Name</span></span>  
<span data-ttu-id="127a3-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span><span class="sxs-lookup"><span data-stu-id="127a3-129">An account schedule consists of a cash flow account schedule name with a series of lines and a column layout.</span></span>  

### <a name="to-set-up-a-new-account-schedule-name"></a><span data-ttu-id="127a3-130">To set up a new account schedule name</span><span class="sxs-lookup"><span data-stu-id="127a3-130">To set up a new account schedule name</span></span>  

1.  <span data-ttu-id="127a3-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules** , and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="127a3-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules** , and then choose the related link.</span></span>  
2.  <span data-ttu-id="127a3-132">On the **Account Schedule Names** page, choose the **New** to create a new cash flow account schedule name.</span><span class="sxs-lookup"><span data-stu-id="127a3-132">On the **Account Schedule Names** page, choose the **New** to create a new cash flow account schedule name.</span></span>  
3.  <span data-ttu-id="127a3-133">In the **Name** field, enter **Forecast** .</span><span class="sxs-lookup"><span data-stu-id="127a3-133">In the **Name** field, enter **Forecast** .</span></span>  
4.  <span data-ttu-id="127a3-134">In the **Description** field, enter **Cash Flow Forecast** .</span><span class="sxs-lookup"><span data-stu-id="127a3-134">In the **Description** field, enter **Cash Flow Forecast** .</span></span>  
5.  <span data-ttu-id="127a3-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span><span class="sxs-lookup"><span data-stu-id="127a3-135">Leave the **Default Column Layout** and **Analysis View Name** fields blank.</span></span>  

## <a name="setting-up-account-schedule-lines"></a><span data-ttu-id="127a3-136">Setting Up Account Schedule Lines</span><span class="sxs-lookup"><span data-stu-id="127a3-136">Setting Up Account Schedule Lines</span></span>  
<span data-ttu-id="127a3-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span><span class="sxs-lookup"><span data-stu-id="127a3-137">After an account schedule name is set up, Ken defines each line that appears in the cash flow account schedule.</span></span> <span data-ttu-id="127a3-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span><span class="sxs-lookup"><span data-stu-id="127a3-138">Ken defines lines that can be shown in reports in addition to lines that are only for calculation purposes.</span></span>  

### <a name="to-set-up-account-schedule-lines"></a><span data-ttu-id="127a3-139">To set up account schedule lines</span><span class="sxs-lookup"><span data-stu-id="127a3-139">To set up account schedule lines</span></span>  

1.  <span data-ttu-id="127a3-140">On the **Account Schedule Names** page, select the new **Forecast** account schedule name that you have created, and then choose the **Edit Account Schedule** action.</span><span class="sxs-lookup"><span data-stu-id="127a3-140">On the **Account Schedule Names** page, select the new **Forecast** account schedule name that you have created, and then choose the **Edit Account Schedule** action.</span></span>  
2.  <span data-ttu-id="127a3-141">On the **Account Schedule** page, enter each line exactly as shown in the following table.</span><span class="sxs-lookup"><span data-stu-id="127a3-141">On the **Account Schedule** page, enter each line exactly as shown in the following table.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="127a3-142">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span><span class="sxs-lookup"><span data-stu-id="127a3-142">Using the **Insert CF Accounts** function, you can quickly mark the cash flow accounts from the chart of cash flow accounts and copy them to account schedule lines.</span></span>  

    |<span data-ttu-id="127a3-143">Row No.</span><span class="sxs-lookup"><span data-stu-id="127a3-143">Row No.</span></span>|<span data-ttu-id="127a3-144">Description</span><span class="sxs-lookup"><span data-stu-id="127a3-144">Description</span></span>|<span data-ttu-id="127a3-145">Totalling Type</span><span class="sxs-lookup"><span data-stu-id="127a3-145">Totaling Type</span></span>|<span data-ttu-id="127a3-146">Totalling</span><span class="sxs-lookup"><span data-stu-id="127a3-146">Totaling</span></span>|<span data-ttu-id="127a3-147">Row Type</span><span class="sxs-lookup"><span data-stu-id="127a3-147">Row Type</span></span>|<span data-ttu-id="127a3-148">Amount Type</span><span class="sxs-lookup"><span data-stu-id="127a3-148">Amount Type</span></span>|<span data-ttu-id="127a3-149">Show</span><span class="sxs-lookup"><span data-stu-id="127a3-149">Show</span></span>|  
    |-------|-----------|-------------|--------|--------|-----------|----|
    |<span data-ttu-id="127a3-150">C10</span><span class="sxs-lookup"><span data-stu-id="127a3-150">C10</span></span>|<span data-ttu-id="127a3-151">Amount</span><span class="sxs-lookup"><span data-stu-id="127a3-151">Amount</span></span>|<span data-ttu-id="127a3-152">Net Change</span><span class="sxs-lookup"><span data-stu-id="127a3-152">Net Change</span></span>|<span data-ttu-id="127a3-153">Entries</span><span class="sxs-lookup"><span data-stu-id="127a3-153">Entries</span></span>|<span data-ttu-id="127a3-154">Net Amount</span><span class="sxs-lookup"><span data-stu-id="127a3-154">Net Amount</span></span>|<span data-ttu-id="127a3-155">Always</span><span class="sxs-lookup"><span data-stu-id="127a3-155">Always</span></span>|  
    |<span data-ttu-id="127a3-156">C20</span><span class="sxs-lookup"><span data-stu-id="127a3-156">C20</span></span>|<span data-ttu-id="127a3-157">Amount until Date</span><span class="sxs-lookup"><span data-stu-id="127a3-157">Amount until Date</span></span>|<span data-ttu-id="127a3-158">Balance at Date</span><span class="sxs-lookup"><span data-stu-id="127a3-158">Balance at Date</span></span>|<span data-ttu-id="127a3-159">Entries</span><span class="sxs-lookup"><span data-stu-id="127a3-159">Entries</span></span>|<span data-ttu-id="127a3-160">Net Amount</span><span class="sxs-lookup"><span data-stu-id="127a3-160">Net Amount</span></span>|<span data-ttu-id="127a3-161">Always</span><span class="sxs-lookup"><span data-stu-id="127a3-161">Always</span></span>|  
    |<span data-ttu-id="127a3-162">C30</span><span class="sxs-lookup"><span data-stu-id="127a3-162">C30</span></span>|<span data-ttu-id="127a3-163">Entire Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="127a3-163">Entire Fiscal Year</span></span>|<span data-ttu-id="127a3-164">Entire Fiscal Year</span><span class="sxs-lookup"><span data-stu-id="127a3-164">Entire Fiscal Year</span></span>|<span data-ttu-id="127a3-165">Entries</span><span class="sxs-lookup"><span data-stu-id="127a3-165">Entries</span></span>|<span data-ttu-id="127a3-166">Net Amount</span><span class="sxs-lookup"><span data-stu-id="127a3-166">Net Amount</span></span>|<span data-ttu-id="127a3-167">Always</span><span class="sxs-lookup"><span data-stu-id="127a3-167">Always</span></span>|  

4.  <span data-ttu-id="127a3-168">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="127a3-168">Choose the **OK** button.</span></span>  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="127a3-169">Assigning the Column Layout to the Account Schedule Name</span><span class="sxs-lookup"><span data-stu-id="127a3-169">Assigning the Column Layout to the Account Schedule Name</span></span>  
<span data-ttu-id="127a3-170">Ken is now ready to assign the column layout to the account schedule name.</span><span class="sxs-lookup"><span data-stu-id="127a3-170">Ken is now ready to assign the column layout to the account schedule name.</span></span>  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a><span data-ttu-id="127a3-171">To assign the column layout to the account schedule name</span><span class="sxs-lookup"><span data-stu-id="127a3-171">To assign the column layout to the account schedule name</span></span>  

1.  <span data-ttu-id="127a3-172">On the **Account Schedule Names** page, select **Forecast** in the **Name** field.</span><span class="sxs-lookup"><span data-stu-id="127a3-172">On the **Account Schedule Names** page, select **Forecast** in the **Name** field.</span></span>  
2.  <span data-ttu-id="127a3-173">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span><span class="sxs-lookup"><span data-stu-id="127a3-173">In the **Default Column Layout** field, choose the column layout **Cash Flow** to assign as the default column layout.</span></span>  

### <a name="to-view-and-print-the-cash-flow-forecast"></a><span data-ttu-id="127a3-174">To view and print the cash flow forecast</span><span class="sxs-lookup"><span data-stu-id="127a3-174">To view and print the cash flow forecast</span></span>  
1.  <span data-ttu-id="127a3-175">On the **Account Schedule Names** page, choose the **Overview** action to view the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="127a3-175">On the **Account Schedule Names** page, choose the **Overview** action to view the cash flow forecast.</span></span>  
2.  <span data-ttu-id="127a3-176">On the **Acc. Schedule Overview** page, you can select an amount and then view the cash flow forecast entries that make up the amount.</span><span class="sxs-lookup"><span data-stu-id="127a3-176">On the **Acc. Schedule Overview** page, you can select an amount and then view the cash flow forecast entries that make up the amount.</span></span> <span data-ttu-id="127a3-177">In addition, you can view the formula that is used to calculate the amount.</span><span class="sxs-lookup"><span data-stu-id="127a3-177">In addition, you can view the formula that is used to calculate the amount.</span></span> <span data-ttu-id="127a3-178">You can also filter the amounts by date and dimension.</span><span class="sxs-lookup"><span data-stu-id="127a3-178">You can also filter the amounts by date and dimension.</span></span>  
3.  <span data-ttu-id="127a3-179">Choose the **Print** action to print the cash flow forecast.</span><span class="sxs-lookup"><span data-stu-id="127a3-179">Choose the **Print** action to print the cash flow forecast.</span></span>  

## <a name="see-also"></a><span data-ttu-id="127a3-180">See Also</span><span class="sxs-lookup"><span data-stu-id="127a3-180">See Also</span></span>  
 <span data-ttu-id="127a3-181">[Work with Account Schedules](bi-how-work-account-schedule.md) </span><span class="sxs-lookup"><span data-stu-id="127a3-181">[Work with Account Schedules](bi-how-work-account-schedule.md) </span></span>  
 [<span data-ttu-id="127a3-182">Business Process Walkthroughs</span><span class="sxs-lookup"><span data-stu-id="127a3-182">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="127a3-183">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="127a3-183">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
