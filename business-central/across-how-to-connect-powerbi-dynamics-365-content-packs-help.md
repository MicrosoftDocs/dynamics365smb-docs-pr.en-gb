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
ms.date: 04/03/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 9cad9c7e2b54506e60af7d38d42f413599a44d01
ms.openlocfilehash: 7b9140611a47b8b823274763731cf000258c681e
ms.contentlocale: en-gb
ms.lasthandoff: 04/03/2018

---
# <a name="connecting-power-bi-to-dynamics-365-business-central-content-packs"></a><span data-ttu-id="07f0b-103">Connecting Power BI to Dynamics 365 Business Central Content Packs</span><span class="sxs-lookup"><span data-stu-id="07f0b-103">Connecting Power BI to Dynamics 365 Business Central Content Packs</span></span>
<span data-ttu-id="07f0b-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span><span class="sxs-lookup"><span data-stu-id="07f0b-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="07f0b-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span><span class="sxs-lookup"><span data-stu-id="07f0b-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

<span data-ttu-id="07f0b-106">You must have a valid account with Dynamics 365 and with Power BI.</span><span class="sxs-lookup"><span data-stu-id="07f0b-106">You must have a valid account with Dynamics 365 and with Power BI.</span></span> <span data-ttu-id="07f0b-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) if you wish to create your own Power BI reports.</span><span class="sxs-lookup"><span data-stu-id="07f0b-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) if you wish to create your own Power BI reports.</span></span> <span data-ttu-id="07f0b-108">Power BI content packs require permissions to the tables where data is retrieved from.</span><span class="sxs-lookup"><span data-stu-id="07f0b-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="07f0b-109">More details on the requirements are described below.</span><span class="sxs-lookup"><span data-stu-id="07f0b-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="07f0b-110">How to Connect</span><span class="sxs-lookup"><span data-stu-id="07f0b-110">How to Connect</span></span>
1. <span data-ttu-id="07f0b-111">Select **Get Data** at the bottom of the left navigation pane.</span><span class="sxs-lookup"><span data-stu-id="07f0b-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="07f0b-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="07f0b-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>

<span data-ttu-id="07f0b-113">You may also get starting from within Dynamics 365 Business Edition.</span><span class="sxs-lookup"><span data-stu-id="07f0b-113">You may also get starting from within Dynamics 365 Business Edition.</span></span> <span data-ttu-id="07f0b-114">From the role centre, navigate to **Report Selection** in the Power BI Role Centre part.</span><span class="sxs-lookup"><span data-stu-id="07f0b-114">From the role center, navigate to **Report Selection** in the Power BI Role Center part.</span></span> <span data-ttu-id="07f0b-115">Select either **Service** or **My Organisation** from the ribbon.</span><span class="sxs-lookup"><span data-stu-id="07f0b-115">Select either **Service** or **My Organization** from the ribbon.</span></span> <span data-ttu-id="07f0b-116">When either of these actions are selected, you will be taken to either the Organisation gallery in Power BI or to the services library in Power BI, which will also be filtered to only display content packs related to [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07f0b-116">When either of these actions are selected, you will be taken to either the Organization gallery in Power BI or to the services library in Power BI, which will also be filtered to only display content packs related to [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span>

2. <span data-ttu-id="07f0b-117">In the **Services** box, select **Get**.</span><span class="sxs-lookup"><span data-stu-id="07f0b-117">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="07f0b-118">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span><span class="sxs-lookup"><span data-stu-id="07f0b-118">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="07f0b-119">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="07f0b-119">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="07f0b-120">Select **Apps** from the **Apps for Power BI apps** tab, choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span><span class="sxs-lookup"><span data-stu-id="07f0b-120">Select **Apps** from the **Apps for Power BI apps** tab, choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="07f0b-121">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="07f0b-121">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="07f0b-122">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07f0b-122">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="07f0b-123">This is not the display name.</span><span class="sxs-lookup"><span data-stu-id="07f0b-123">This is not the display name.</span></span> <span data-ttu-id="07f0b-124">The company name can be found on the 'Companies' page within your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] instance.</span><span class="sxs-lookup"><span data-stu-id="07f0b-124">The company name can be found on the 'Companies' page within your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] instance.</span></span> 
<span data-ttu-id="07f0b-125">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="07f0b-125">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="07f0b-126">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span><span class="sxs-lookup"><span data-stu-id="07f0b-126">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="07f0b-127">When completed, the tiles will update with data from your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] company.</span><span class="sxs-lookup"><span data-stu-id="07f0b-127">When completed, the tiles will update with data from your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] company.</span></span>
<span data-ttu-id="07f0b-128">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="07f0b-128">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="07f0b-129">What Now?</span><span class="sxs-lookup"><span data-stu-id="07f0b-129">What Now?</span></span>

- <span data-ttu-id="07f0b-130">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span><span class="sxs-lookup"><span data-stu-id="07f0b-130">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span></span>
- <span data-ttu-id="07f0b-131">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span><span class="sxs-lookup"><span data-stu-id="07f0b-131">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="07f0b-132">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span><span class="sxs-lookup"><span data-stu-id="07f0b-132">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="07f0b-133">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span><span class="sxs-lookup"><span data-stu-id="07f0b-133">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="07f0b-134">System Requirements</span><span class="sxs-lookup"><span data-stu-id="07f0b-134">System Requirements</span></span>
<span data-ttu-id="07f0b-135">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span><span class="sxs-lookup"><span data-stu-id="07f0b-135">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="07f0b-136">The web services required for each content pack include:</span><span class="sxs-lookup"><span data-stu-id="07f0b-136">The web services required for each content pack include:</span></span>

## <a name="role-center-reports"></a><span data-ttu-id="07f0b-137">Role Centre Reports</span><span class="sxs-lookup"><span data-stu-id="07f0b-137">Role Center Reports</span></span>

<span data-ttu-id="07f0b-138">**Microsoft Dynamics 365 Business Central – CRM**</span><span class="sxs-lookup"><span data-stu-id="07f0b-138">**Microsoft Dynamics 365 Business Central – CRM**</span></span>
- <span data-ttu-id="07f0b-139">Sales Opportunities</span><span class="sxs-lookup"><span data-stu-id="07f0b-139">Sales Opportunities</span></span>
- <span data-ttu-id="07f0b-140">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="07f0b-140">Excel Template View Company</span></span>
- <span data-ttu-id="07f0b-141">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-141">Power BI Report Labels</span></span>

<span data-ttu-id="07f0b-142">**Microsoft Dynamics 365 Business Central – Finance**</span><span class="sxs-lookup"><span data-stu-id="07f0b-142">**Microsoft Dynamics 365 Business Central – Finance**</span></span>
- <span data-ttu-id="07f0b-143">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="07f0b-143">PowerBIFinance</span></span>
- <span data-ttu-id="07f0b-144">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="07f0b-144">Excel Template View Company</span></span>
- <span data-ttu-id="07f0b-145">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-145">Power BI Report Labels</span></span>

<span data-ttu-id="07f0b-146">**Microsoft Dynamics 365 Business Central – Jobs**</span><span class="sxs-lookup"><span data-stu-id="07f0b-146">**Microsoft Dynamics 365 Business Central – Jobs**</span></span>
- <span data-ttu-id="07f0b-147">Job List</span><span class="sxs-lookup"><span data-stu-id="07f0b-147">Job List</span></span>
- <span data-ttu-id="07f0b-148">Job Planning Lines</span><span class="sxs-lookup"><span data-stu-id="07f0b-148">Job Planning Lines</span></span>
- <span data-ttu-id="07f0b-149">Job Task Lines</span><span class="sxs-lookup"><span data-stu-id="07f0b-149">Job Task Lines</span></span>
- <span data-ttu-id="07f0b-150">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-150">Power BI Report Labels</span></span>
- <span data-ttu-id="07f0b-151">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="07f0b-151">Excel Template View Company</span></span>

<span data-ttu-id="07f0b-152">**Microsoft Dynamics 365 Business Central - Sales**</span><span class="sxs-lookup"><span data-stu-id="07f0b-152">**Microsoft Dynamics 365 Business Central - Sales**</span></span>
- <span data-ttu-id="07f0b-153">Sales Dashboard</span><span class="sxs-lookup"><span data-stu-id="07f0b-153">Sales Dashboard</span></span>
- <span data-ttu-id="07f0b-154">Excel Template View Company</span><span class="sxs-lookup"><span data-stu-id="07f0b-154">Excel Template View Company</span></span>
- <span data-ttu-id="07f0b-155">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-155">Power BI Report Labels</span></span>

## <a name="list-page-reports"></a><span data-ttu-id="07f0b-156">List Page Reports</span><span class="sxs-lookup"><span data-stu-id="07f0b-156">List Page Reports</span></span> 

<span data-ttu-id="07f0b-157">**Microsoft Dynamics 365 Business Central – Customers List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-157">**Microsoft Dynamics 365 Business Central – Customers List**</span></span>
- <span data-ttu-id="07f0b-158">Item Sales by Customer</span><span class="sxs-lookup"><span data-stu-id="07f0b-158">Item Sales by Customer</span></span>
- <span data-ttu-id="07f0b-159">Power BI Item Purchase List</span><span class="sxs-lookup"><span data-stu-id="07f0b-159">Power BI Item Purchase List</span></span>
- <span data-ttu-id="07f0b-160">Power BI Item Sales List</span><span class="sxs-lookup"><span data-stu-id="07f0b-160">Power BI Item Sales List</span></span>
- <span data-ttu-id="07f0b-161">Sales Dashboard</span><span class="sxs-lookup"><span data-stu-id="07f0b-161">Sales Dashboard</span></span>
- <span data-ttu-id="07f0b-162">Power BI Customer List</span><span class="sxs-lookup"><span data-stu-id="07f0b-162">Power BI Customer List</span></span>
- <span data-ttu-id="07f0b-163">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-163">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-164">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-164">Power BI Report Labels</span></span> 

<span data-ttu-id="07f0b-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span></span>
- <span data-ttu-id="07f0b-166">Power BI GL Amount List</span><span class="sxs-lookup"><span data-stu-id="07f0b-166">Power BI GL Amount List</span></span>
- <span data-ttu-id="07f0b-167">Power BI GL Budgeted Amount</span><span class="sxs-lookup"><span data-stu-id="07f0b-167">Power BI GL Budgeted Amount</span></span>
- <span data-ttu-id="07f0b-168">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-168">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-169">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-169">Power BI Report Labels</span></span>

<span data-ttu-id="07f0b-170">**Microsoft Dynamics 365 Business Central – Items List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-170">**Microsoft Dynamics 365 Business Central – Items List**</span></span>
- <span data-ttu-id="07f0b-171">Item Sales by Customer</span><span class="sxs-lookup"><span data-stu-id="07f0b-171">Item Sales by Customer</span></span>
- <span data-ttu-id="07f0b-172">Power BI Item Purchase List</span><span class="sxs-lookup"><span data-stu-id="07f0b-172">Power BI Item Purchase List</span></span>
- <span data-ttu-id="07f0b-173">Power BI Item Sales List</span><span class="sxs-lookup"><span data-stu-id="07f0b-173">Power BI Item Sales List</span></span>
- <span data-ttu-id="07f0b-174">Sales Dashboard</span><span class="sxs-lookup"><span data-stu-id="07f0b-174">Sales Dashboard</span></span>
- <span data-ttu-id="07f0b-175">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-175">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-176">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-176">Power BI Report Labels</span></span>

<span data-ttu-id="07f0b-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span></span>
- <span data-ttu-id="07f0b-178">Power BI Jobs List</span><span class="sxs-lookup"><span data-stu-id="07f0b-178">Power BI Jobs List</span></span>
- <span data-ttu-id="07f0b-179">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-179">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-180">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-180">Power BI Report Labels</span></span>

<span data-ttu-id="07f0b-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span></span>
- <span data-ttu-id="07f0b-182">Power BI Purchase List</span><span class="sxs-lookup"><span data-stu-id="07f0b-182">Power BI Purchase List</span></span>
- <span data-ttu-id="07f0b-183">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-183">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-184">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-184">Power BI Report Labels</span></span>

<span data-ttu-id="07f0b-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span></span>
- <span data-ttu-id="07f0b-186">Power BI Sales List</span><span class="sxs-lookup"><span data-stu-id="07f0b-186">Power BI Sales List</span></span>
- <span data-ttu-id="07f0b-187">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-187">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-188">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-188">Power BI Report Labels</span></span>


<span data-ttu-id="07f0b-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span><span class="sxs-lookup"><span data-stu-id="07f0b-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span></span>
- <span data-ttu-id="07f0b-190">Power BI Item Purchase List</span><span class="sxs-lookup"><span data-stu-id="07f0b-190">Power BI Item Purchase List</span></span>
- <span data-ttu-id="07f0b-191">Power BI Item Sales List</span><span class="sxs-lookup"><span data-stu-id="07f0b-191">Power BI Item Sales List</span></span>
- <span data-ttu-id="07f0b-192">Power BI Vendor List</span><span class="sxs-lookup"><span data-stu-id="07f0b-192">Power BI Vendor List</span></span>
- <span data-ttu-id="07f0b-193">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="07f0b-193">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="07f0b-194">Power BI Report Labels</span><span class="sxs-lookup"><span data-stu-id="07f0b-194">Power BI Report Labels</span></span>

## <a name="web-services"></a><span data-ttu-id="07f0b-195">Web Services</span><span class="sxs-lookup"><span data-stu-id="07f0b-195">Web Services</span></span>
<span data-ttu-id="07f0b-196">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="07f0b-196">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="07f0b-197">In the list make sure the Publish box is marked for the web services listed above.</span><span class="sxs-lookup"><span data-stu-id="07f0b-197">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="07f0b-198">Troubleshooting</span><span class="sxs-lookup"><span data-stu-id="07f0b-198">Troubleshooting</span></span>
<span data-ttu-id="07f0b-199">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span><span class="sxs-lookup"><span data-stu-id="07f0b-199">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="07f0b-200">However, if something goes wrong, this section provides a workaround for the most typical issues.</span><span class="sxs-lookup"><span data-stu-id="07f0b-200">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="07f0b-201">Incorrect Company Name</span><span class="sxs-lookup"><span data-stu-id="07f0b-201">Incorrect Company Name</span></span>  
<span data-ttu-id="07f0b-202">A common mistake is to enter the company display name instead of the company name.</span><span class="sxs-lookup"><span data-stu-id="07f0b-202">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="07f0b-203">To find the company name search for **Companies**.</span><span class="sxs-lookup"><span data-stu-id="07f0b-203">To find the company name search for **Companies**.</span></span> <span data-ttu-id="07f0b-204">Then use the **Name** field when entering your company name.</span><span class="sxs-lookup"><span data-stu-id="07f0b-204">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="07f0b-205">Incorrect User Name and Password</span><span class="sxs-lookup"><span data-stu-id="07f0b-205">Incorrect User Name and Password</span></span>  
<span data-ttu-id="07f0b-206">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span><span class="sxs-lookup"><span data-stu-id="07f0b-206">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="07f0b-207">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span><span class="sxs-lookup"><span data-stu-id="07f0b-207">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="07f0b-208">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span><span class="sxs-lookup"><span data-stu-id="07f0b-208">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="07f0b-209">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span><span class="sxs-lookup"><span data-stu-id="07f0b-209">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="07f0b-210">The Key Didn't Match Any Rows in the Table</span><span class="sxs-lookup"><span data-stu-id="07f0b-210">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="07f0b-211">If you enter a non-valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span><span class="sxs-lookup"><span data-stu-id="07f0b-211">If you enter a non-valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="07f0b-212">Provide the correct company name and try connecting again.</span><span class="sxs-lookup"><span data-stu-id="07f0b-212">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="07f0b-213">See Also</span><span class="sxs-lookup"><span data-stu-id="07f0b-213">See Also</span></span>
[<span data-ttu-id="07f0b-214">Get started with Power BI</span><span class="sxs-lookup"><span data-stu-id="07f0b-214">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
[<span data-ttu-id="07f0b-215">Power BI - Basic Concepts</span><span class="sxs-lookup"><span data-stu-id="07f0b-215">Power BI - Basic Concepts</span></span>](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)  
[<span data-ttu-id="07f0b-216">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="07f0b-216">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="07f0b-217">Getting Started</span><span class="sxs-lookup"><span data-stu-id="07f0b-217">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="07f0b-218">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="07f0b-218">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="07f0b-219">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="07f0b-219">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="07f0b-220">Finance</span><span class="sxs-lookup"><span data-stu-id="07f0b-220">Finance</span></span>](finance.md)  
<span data-ttu-id="07f0b-221">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="07f0b-221">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  

