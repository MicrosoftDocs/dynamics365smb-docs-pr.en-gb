---
title: How to Connect Power BI to Business Central | Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with Power BI and the Business Central content packs.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2018
ms.author: solsen
redirect_url: admin-powerbi
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 48c57e03f4679ea05792304fe13bdf896be2f1e3
ms.contentlocale: en-gb
ms.lasthandoff: 11/22/2018

---
# <a name="connecting-power-bi-to-dynamics-365-business-central-content-packs"></a><span data-ttu-id="a47c0-103">Connecting Power BI to Dynamics 365 Business Central Content Packs</span><span class="sxs-lookup"><span data-stu-id="a47c0-103">Connecting Power BI to Dynamics 365 Business Central Content Packs</span></span>
<span data-ttu-id="a47c0-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span><span class="sxs-lookup"><span data-stu-id="a47c0-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="a47c0-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span><span class="sxs-lookup"><span data-stu-id="a47c0-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

<span data-ttu-id="a47c0-106">You must have a valid account with Dynamics 365 and with Power BI.</span><span class="sxs-lookup"><span data-stu-id="a47c0-106">You must have a valid account with Dynamics 365 and with Power BI.</span></span> <span data-ttu-id="a47c0-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) if you wish to create your own Power BI reports.</span><span class="sxs-lookup"><span data-stu-id="a47c0-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) if you wish to create your own Power BI reports.</span></span> <span data-ttu-id="a47c0-108">Power BI content packs require permissions to the tables where data is retrieved from.</span><span class="sxs-lookup"><span data-stu-id="a47c0-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="a47c0-109">More details on the requirements are described below.</span><span class="sxs-lookup"><span data-stu-id="a47c0-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="a47c0-110">How to Connect</span><span class="sxs-lookup"><span data-stu-id="a47c0-110">How to Connect</span></span>
1. <span data-ttu-id="a47c0-111">Select **Get Data** at the bottom of the left navigation pane.</span><span class="sxs-lookup"><span data-stu-id="a47c0-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="a47c0-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="a47c0-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>

<span data-ttu-id="a47c0-113">You may also get starting from within Dynamics 365 Business Edition.</span><span class="sxs-lookup"><span data-stu-id="a47c0-113">You may also get starting from within Dynamics 365 Business Edition.</span></span> <span data-ttu-id="a47c0-114">From the role centre, navigate to **Report Selection** in the Power BI Role Centre part.</span><span class="sxs-lookup"><span data-stu-id="a47c0-114">From the role center, navigate to **Report Selection** in the Power BI Role Center part.</span></span> <span data-ttu-id="a47c0-115">Select either **Service** or **My Organisation** from the ribbon.</span><span class="sxs-lookup"><span data-stu-id="a47c0-115">Select either **Service** or **My Organization** from the ribbon.</span></span> <span data-ttu-id="a47c0-116">When either of these actions are selected, you will be taken to either the Organisation gallery in Power BI or to the services library in Power BI, which will also be filtered to only display content packs related to [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a47c0-116">When either of these actions are selected, you will be taken to either the Organization gallery in Power BI or to the services library in Power BI, which will also be filtered to only display content packs related to [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span>

2. <span data-ttu-id="a47c0-117">In the **Services** box, select **Get**.</span><span class="sxs-lookup"><span data-stu-id="a47c0-117">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="a47c0-118">This will open a page with the **AppSource** and **Apps for Power BI apps**.</span><span class="sxs-lookup"><span data-stu-id="a47c0-118">This will open a page with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="a47c0-119">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="a47c0-119">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="a47c0-120">Select **Apps** from the **Apps for Power BI apps** tab, choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span><span class="sxs-lookup"><span data-stu-id="a47c0-120">Select **Apps** from the **Apps for Power BI apps** tab, choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="a47c0-121">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="a47c0-121">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="a47c0-122">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a47c0-122">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="a47c0-123">This is not the display name.</span><span class="sxs-lookup"><span data-stu-id="a47c0-123">This is not the display name.</span></span> <span data-ttu-id="a47c0-124">The company name can be found on the 'Companies' page within your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] instance.</span><span class="sxs-lookup"><span data-stu-id="a47c0-124">The company name can be found on the 'Companies' page within your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] instance.</span></span> 
<span data-ttu-id="a47c0-125">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="a47c0-125">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="a47c0-126">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span><span class="sxs-lookup"><span data-stu-id="a47c0-126">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="a47c0-127">When completed, the tiles will update with data from your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="a47c0-127">When completed, the tiles will update with data from your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] company.</span></span>
<span data-ttu-id="a47c0-128">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="a47c0-128">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="a47c0-129">What Now?</span><span class="sxs-lookup"><span data-stu-id="a47c0-129">What Now?</span></span>

- <span data-ttu-id="a47c0-130">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span><span class="sxs-lookup"><span data-stu-id="a47c0-130">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span></span>
- <span data-ttu-id="a47c0-131">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span><span class="sxs-lookup"><span data-stu-id="a47c0-131">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="a47c0-132">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span><span class="sxs-lookup"><span data-stu-id="a47c0-132">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="a47c0-133">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span><span class="sxs-lookup"><span data-stu-id="a47c0-133">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="a47c0-134">System Requirements</span><span class="sxs-lookup"><span data-stu-id="a47c0-134">System Requirements</span></span>
<span data-ttu-id="a47c0-135">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span><span class="sxs-lookup"><span data-stu-id="a47c0-135">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="a47c0-136">The web services required for each content pack include:</span><span class="sxs-lookup"><span data-stu-id="a47c0-136">The web services required for each content pack include:</span></span>

## <a name="role-center-reports"></a><span data-ttu-id="a47c0-137">Role Centre Reports</span><span class="sxs-lookup"><span data-stu-id="a47c0-137">Role Center Reports</span></span>

<span data-ttu-id="a47c0-138">**Microsoft Dynamics 365 Business Central – CRM**</span><span class="sxs-lookup"><span data-stu-id="a47c0-138">**Microsoft Dynamics 365 Business Central – CRM**</span></span>
- <span data-ttu-id="a47c0-139">Sales Opportunities</span><span class="sxs-lookup"><span data-stu-id="a47c0-139">Sales Opportunities</span></span>
- <span data-ttu-id="a47c0-140">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="a47c0-140">Excel Template View Company</span></span>
- <span data-ttu-id="a47c0-141">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-141">Power BI Report Labels</span></span>

<span data-ttu-id="a47c0-142">**Microsoft Dynamics 365 Business Central – Finance**</span><span class="sxs-lookup"><span data-stu-id="a47c0-142">**Microsoft Dynamics 365 Business Central – Finance**</span></span>
- <span data-ttu-id="a47c0-143">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="a47c0-143">PowerBIFinance</span></span>
- <span data-ttu-id="a47c0-144">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="a47c0-144">Excel Template View Company</span></span>
- <span data-ttu-id="a47c0-145">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-145">Power BI Report Labels</span></span>

<span data-ttu-id="a47c0-146">**Microsoft Dynamics 365 Business Central – Jobs**</span><span class="sxs-lookup"><span data-stu-id="a47c0-146">**Microsoft Dynamics 365 Business Central – Jobs**</span></span>
- <span data-ttu-id="a47c0-147">Job List</span><span class="sxs-lookup"><span data-stu-id="a47c0-147">Job List</span></span>
- <span data-ttu-id="a47c0-148">Job Planning Lines</span><span class="sxs-lookup"><span data-stu-id="a47c0-148">Job Planning Lines</span></span>
- <span data-ttu-id="a47c0-149">Job Task Lines</span><span class="sxs-lookup"><span data-stu-id="a47c0-149">Job Task Lines</span></span>
- <span data-ttu-id="a47c0-150">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-150">Power BI Report Labels</span></span>
- <span data-ttu-id="a47c0-151">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="a47c0-151">Excel Template View Company</span></span>

<span data-ttu-id="a47c0-152">**Microsoft Dynamics 365 Business Central - Sales**</span><span class="sxs-lookup"><span data-stu-id="a47c0-152">**Microsoft Dynamics 365 Business Central - Sales**</span></span>
- <span data-ttu-id="a47c0-153">Sales Dashboard</span><span class="sxs-lookup"><span data-stu-id="a47c0-153">Sales Dashboard</span></span>
- <span data-ttu-id="a47c0-154">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="a47c0-154">Excel Template View Company</span></span>
- <span data-ttu-id="a47c0-155">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-155">Power BI Report Labels</span></span>

## <a name="list-page-reports"></a><span data-ttu-id="a47c0-156">List Page Reports</span><span class="sxs-lookup"><span data-stu-id="a47c0-156">List Page Reports</span></span> 

<span data-ttu-id="a47c0-157">**Microsoft Dynamics 365 Business Central – Customers List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-157">**Microsoft Dynamics 365 Business Central – Customers List**</span></span>
- <span data-ttu-id="a47c0-158">Item Sales by Customer</span><span class="sxs-lookup"><span data-stu-id="a47c0-158">Item Sales by Customer</span></span>
- <span data-ttu-id="a47c0-159">Power BI Item Purchase List</span><span class="sxs-lookup"><span data-stu-id="a47c0-159">Power BI Item Purchase List</span></span>
- <span data-ttu-id="a47c0-160">Power BI Item Sales List</span><span class="sxs-lookup"><span data-stu-id="a47c0-160">Power BI Item Sales List</span></span>
- <span data-ttu-id="a47c0-161">Sales Dashboard</span><span class="sxs-lookup"><span data-stu-id="a47c0-161">Sales Dashboard</span></span>
- <span data-ttu-id="a47c0-162">Power BI Customer List</span><span class="sxs-lookup"><span data-stu-id="a47c0-162">Power BI Customer List</span></span>
- <span data-ttu-id="a47c0-163">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-163">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-164">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-164">Power BI Report Labels</span></span> 

<span data-ttu-id="a47c0-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span></span>
- <span data-ttu-id="a47c0-166">Power BI GL Amount List</span><span class="sxs-lookup"><span data-stu-id="a47c0-166">Power BI GL Amount List</span></span>
- <span data-ttu-id="a47c0-167">Power BI GL Budgeted Amount</span><span class="sxs-lookup"><span data-stu-id="a47c0-167">Power BI GL Budgeted Amount</span></span>
- <span data-ttu-id="a47c0-168">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-168">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-169">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-169">Power BI Report Labels</span></span>

<span data-ttu-id="a47c0-170">**Microsoft Dynamics 365 Business Central – Items List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-170">**Microsoft Dynamics 365 Business Central – Items List**</span></span>
- <span data-ttu-id="a47c0-171">Item Sales by Customer</span><span class="sxs-lookup"><span data-stu-id="a47c0-171">Item Sales by Customer</span></span>
- <span data-ttu-id="a47c0-172">Power BI Item Purchase List</span><span class="sxs-lookup"><span data-stu-id="a47c0-172">Power BI Item Purchase List</span></span>
- <span data-ttu-id="a47c0-173">Power BI Item Sales List</span><span class="sxs-lookup"><span data-stu-id="a47c0-173">Power BI Item Sales List</span></span>
- <span data-ttu-id="a47c0-174">Sales Dashboard</span><span class="sxs-lookup"><span data-stu-id="a47c0-174">Sales Dashboard</span></span>
- <span data-ttu-id="a47c0-175">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-175">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-176">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-176">Power BI Report Labels</span></span>

<span data-ttu-id="a47c0-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span></span>
- <span data-ttu-id="a47c0-178">Power BI Jobs List</span><span class="sxs-lookup"><span data-stu-id="a47c0-178">Power BI Jobs List</span></span>
- <span data-ttu-id="a47c0-179">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-179">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-180">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-180">Power BI Report Labels</span></span>

<span data-ttu-id="a47c0-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span></span>
- <span data-ttu-id="a47c0-182">Power BI Purchase List</span><span class="sxs-lookup"><span data-stu-id="a47c0-182">Power BI Purchase List</span></span>
- <span data-ttu-id="a47c0-183">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-183">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-184">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-184">Power BI Report Labels</span></span>

<span data-ttu-id="a47c0-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span></span>
- <span data-ttu-id="a47c0-186">Power BI Sales List</span><span class="sxs-lookup"><span data-stu-id="a47c0-186">Power BI Sales List</span></span>
- <span data-ttu-id="a47c0-187">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-187">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-188">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-188">Power BI Report Labels</span></span>


<span data-ttu-id="a47c0-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span><span class="sxs-lookup"><span data-stu-id="a47c0-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span></span>
- <span data-ttu-id="a47c0-190">Power BI Item Purchase List</span><span class="sxs-lookup"><span data-stu-id="a47c0-190">Power BI Item Purchase List</span></span>
- <span data-ttu-id="a47c0-191">Power BI Item Sales List</span><span class="sxs-lookup"><span data-stu-id="a47c0-191">Power BI Item Sales List</span></span>
- <span data-ttu-id="a47c0-192">Power BI Vendor List</span><span class="sxs-lookup"><span data-stu-id="a47c0-192">Power BI Vendor List</span></span>
- <span data-ttu-id="a47c0-193">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="a47c0-193">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="a47c0-194">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="a47c0-194">Power BI Report Labels</span></span>

## <a name="web-services"></a><span data-ttu-id="a47c0-195">Web Services</span><span class="sxs-lookup"><span data-stu-id="a47c0-195">Web Services</span></span>
<span data-ttu-id="a47c0-196">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a47c0-196">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="a47c0-197">In the list make sure the Publish box is marked for the web services listed above.</span><span class="sxs-lookup"><span data-stu-id="a47c0-197">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a47c0-198">Troubleshooting</span><span class="sxs-lookup"><span data-stu-id="a47c0-198">Troubleshooting</span></span>
<span data-ttu-id="a47c0-199">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span><span class="sxs-lookup"><span data-stu-id="a47c0-199">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="a47c0-200">However, if something goes wrong, this section provides a workaround for the most typical issues.</span><span class="sxs-lookup"><span data-stu-id="a47c0-200">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="a47c0-201">Incorrect Company Name</span><span class="sxs-lookup"><span data-stu-id="a47c0-201">Incorrect Company Name</span></span>  
<span data-ttu-id="a47c0-202">A common mistake is to enter the company display name instead of the company name.</span><span class="sxs-lookup"><span data-stu-id="a47c0-202">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="a47c0-203">To find the company name search for **Companies**.</span><span class="sxs-lookup"><span data-stu-id="a47c0-203">To find the company name search for **Companies**.</span></span> <span data-ttu-id="a47c0-204">Then use the **Name** field when entering your company name.</span><span class="sxs-lookup"><span data-stu-id="a47c0-204">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="a47c0-205">Incorrect User Name and Password</span><span class="sxs-lookup"><span data-stu-id="a47c0-205">Incorrect User Name and Password</span></span>  
<span data-ttu-id="a47c0-206">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span><span class="sxs-lookup"><span data-stu-id="a47c0-206">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="a47c0-207">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span><span class="sxs-lookup"><span data-stu-id="a47c0-207">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="a47c0-208">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span><span class="sxs-lookup"><span data-stu-id="a47c0-208">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="a47c0-209">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span><span class="sxs-lookup"><span data-stu-id="a47c0-209">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="a47c0-210">The Key Didn't Match Any Rows in the Table</span><span class="sxs-lookup"><span data-stu-id="a47c0-210">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="a47c0-211">If you enter a non-valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span><span class="sxs-lookup"><span data-stu-id="a47c0-211">If you enter a non-valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="a47c0-212">Provide the correct company name and try connecting again.</span><span class="sxs-lookup"><span data-stu-id="a47c0-212">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="a47c0-213">See Also</span><span class="sxs-lookup"><span data-stu-id="a47c0-213">See Also</span></span>
[<span data-ttu-id="a47c0-214">Get started with Power BI</span><span class="sxs-lookup"><span data-stu-id="a47c0-214">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
[<span data-ttu-id="a47c0-215">Power BI - Basic Concepts</span><span class="sxs-lookup"><span data-stu-id="a47c0-215">Power BI - Basic Concepts</span></span>](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)  
[<span data-ttu-id="a47c0-216">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="a47c0-216">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="a47c0-217">Getting Started</span><span class="sxs-lookup"><span data-stu-id="a47c0-217">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="a47c0-218">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="a47c0-218">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="a47c0-219">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="a47c0-219">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="a47c0-220">Finance</span><span class="sxs-lookup"><span data-stu-id="a47c0-220">Finance</span></span>](finance.md)  
<span data-ttu-id="a47c0-221">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="a47c0-221">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  

