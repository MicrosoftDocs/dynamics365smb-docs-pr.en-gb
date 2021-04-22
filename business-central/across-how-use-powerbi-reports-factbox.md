---
title: Display Custom Power BI Reports for Business Central data| Microsoft Docs
description: You can use Power BI reports to gain extra insight into data in lists.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a600b24e16172134d4f8e78cf47efa4e262cac09
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777523"
---
# <a name="creating-power-bi-reports-for-displaying-list-data-in-prod_short"></a><span data-ttu-id="27380-103">Creating Power BI Reports for Displaying List Data in [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="27380-103">Creating Power BI Reports for Displaying List Data in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

[!INCLUDE[prod_long](includes/prod_long.md)] <span data-ttu-id="27380-104">includes a Power BI FactBox control element on many key list pages.</span><span class="sxs-lookup"><span data-stu-id="27380-104">includes a Power BI FactBox control element on many key list pages.</span></span> <span data-ttu-id="27380-105">The purpose of this FactBox is to display Power BI reports that are related to records in the lists, providing extra insight into the data.</span><span class="sxs-lookup"><span data-stu-id="27380-105">The purpose of this FactBox is to display Power BI reports that are related to records in the lists, providing extra insight into the data.</span></span> <span data-ttu-id="27380-106">The idea is that as you move between rows in the list, the report is updated and filtered for the selected entry.</span><span class="sxs-lookup"><span data-stu-id="27380-106">The idea is that as you move between rows in the list, the report is updated and filtered for the selected entry.</span></span>

[!INCLUDE[prod_long](includes/prod_long.md)] <span data-ttu-id="27380-107">comes ready with some of these reports.</span><span class="sxs-lookup"><span data-stu-id="27380-107">comes ready with some of these reports.</span></span> <span data-ttu-id="27380-108">You can also create your own custom reports that display in this FactBox.</span><span class="sxs-lookup"><span data-stu-id="27380-108">You can also create your own custom reports that display in this FactBox.</span></span> <span data-ttu-id="27380-109">Creating these reports is similar to other reports.</span><span class="sxs-lookup"><span data-stu-id="27380-109">Creating these reports is similar to other reports.</span></span> <span data-ttu-id="27380-110">But there are a few design rules you'll have to follow to make sure the reports display as expected.</span><span class="sxs-lookup"><span data-stu-id="27380-110">But there are a few design rules you'll have to follow to make sure the reports display as expected.</span></span> <span data-ttu-id="27380-111">These rules are explained in this article.</span><span class="sxs-lookup"><span data-stu-id="27380-111">These rules are explained in this article.</span></span>

> [!NOTE]
> <span data-ttu-id="27380-112">For general information about creating and publishing Power BI reports for Business Central, see [Building Power BI Reports to Display [!INCLUDE [prod_long](includes/prod_long.md)] Data](across-how-use-financials-data-source-powerbi.md).</span><span class="sxs-lookup"><span data-stu-id="27380-112">For general information about creating and publishing Power BI reports for Business Central, see [Building Power BI Reports to Display [!INCLUDE [prod_long](includes/prod_long.md)] Data](across-how-use-financials-data-source-powerbi.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="27380-113">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="27380-113">Prerequisites</span></span>

- <span data-ttu-id="27380-114">A Power BI account.</span><span class="sxs-lookup"><span data-stu-id="27380-114">A Power BI account.</span></span>
- <span data-ttu-id="27380-115">Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="27380-115">Power BI Desktop.</span></span>

<!-- 
For more information about getting started, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md).-->

## <a name="create-a-report-for-a-list-page"></a><span data-ttu-id="27380-116">Create a report for a list page</span><span class="sxs-lookup"><span data-stu-id="27380-116">Create a report for a list page</span></span>

1. <span data-ttu-id="27380-117">Start Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="27380-117">Start Power BI Desktop.</span></span>
2. <span data-ttu-id="27380-118">Select **Get Data**, and start choosing the data source for the report.</span><span class="sxs-lookup"><span data-stu-id="27380-118">Select **Get Data**, and start choosing the data source for the report.</span></span>

    <span data-ttu-id="27380-119">In this step, you specify the Business Central list pages that contain the data that you want in the report.</span><span class="sxs-lookup"><span data-stu-id="27380-119">In this step, you specify the Business Central list pages that contain the data that you want in the report.</span></span> <span data-ttu-id="27380-120">For example, to create a report for the Sales List, ensure the data set contains information related to sales.</span><span class="sxs-lookup"><span data-stu-id="27380-120">For example, to create a report for the Sales List, ensure the data set contains information related to sales.</span></span>

    <span data-ttu-id="27380-121">For more information, follow the instructions [Add [!INCLUDE[prod_short](includes/prod_short.md)] as a data source in Power BI Desktop](across-how-use-financials-data-source-powerbi.md#getdata).</span><span class="sxs-lookup"><span data-stu-id="27380-121">For more information, follow the instructions [Add [!INCLUDE[prod_short](includes/prod_short.md)] as a data source in Power BI Desktop](across-how-use-financials-data-source-powerbi.md#getdata).</span></span>

3. <span data-ttu-id="27380-122">Set the report filter.</span><span class="sxs-lookup"><span data-stu-id="27380-122">Set the report filter.</span></span>

    <span data-ttu-id="27380-123">To make the data update to the selected record in the list, you add a filter to the report.</span><span class="sxs-lookup"><span data-stu-id="27380-123">To make the data update to the selected record in the list, you add a filter to the report.</span></span> <span data-ttu-id="27380-124">The filter must include a field of the data source that's used to uniquely identify each record in the list.</span><span class="sxs-lookup"><span data-stu-id="27380-124">The filter must include a field of the data source that's used to uniquely identify each record in the list.</span></span> <span data-ttu-id="27380-125">In developer terms, this field is the *primary key*.</span><span class="sxs-lookup"><span data-stu-id="27380-125">In developer terms, this field is the *primary key*.</span></span> <span data-ttu-id="27380-126">In most cases, the primary key for a list is the **No.**</span><span class="sxs-lookup"><span data-stu-id="27380-126">In most cases, the primary key for a list is the **No.**</span></span> <span data-ttu-id="27380-127">field.</span><span class="sxs-lookup"><span data-stu-id="27380-127">field.</span></span>

    <span data-ttu-id="27380-128">To set the filter, do the following steps:</span><span class="sxs-lookup"><span data-stu-id="27380-128">To set the filter, do the following steps:</span></span>

    1. <span data-ttu-id="27380-129">In the **Filters**, select the primary key field from the list of available fields.</span><span class="sxs-lookup"><span data-stu-id="27380-129">In the **Filters**, select the primary key field from the list of available fields.</span></span>
    2. <span data-ttu-id="27380-130">Drag the field to **Filters** pane and drop it in the **Filters on all pages** box.</span><span class="sxs-lookup"><span data-stu-id="27380-130">Drag the field to **Filters** pane and drop it in the **Filters on all pages** box.</span></span>
    3. <span data-ttu-id="27380-131">Set the **Filter type** to **Basic filtering**.</span><span class="sxs-lookup"><span data-stu-id="27380-131">Set the **Filter type** to **Basic filtering**.</span></span> <span data-ttu-id="27380-132">It can't be page, visual, or advanced filter.</span><span class="sxs-lookup"><span data-stu-id="27380-132">It can't be page, visual, or advanced filter.</span></span>

    ![Setting the report filter for the Sales Invoice Activity report](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-filter-v3.png)
4. <span data-ttu-id="27380-134">Design the report layout.</span><span class="sxs-lookup"><span data-stu-id="27380-134">Design the report layout.</span></span>

    <span data-ttu-id="27380-135">Create the layout by dragging fields and adding visualizations.</span><span class="sxs-lookup"><span data-stu-id="27380-135">Create the layout by dragging fields and adding visualizations.</span></span> <span data-ttu-id="27380-136">For more information, see, [Work with Report view in Power BI Desktop](/power-bi/create-reports/desktop-report-view) in the Power BI documentation.</span><span class="sxs-lookup"><span data-stu-id="27380-136">For more information, see, [Work with Report view in Power BI Desktop](/power-bi/create-reports/desktop-report-view) in the Power BI documentation.</span></span>

5. <span data-ttu-id="27380-137">See the next sections about sizing the report and using multiple pages.</span><span class="sxs-lookup"><span data-stu-id="27380-137">See the next sections about sizing the report and using multiple pages.</span></span>

6. <span data-ttu-id="27380-138">Save and name the report.</span><span class="sxs-lookup"><span data-stu-id="27380-138">Save and name the report.</span></span>

    <span data-ttu-id="27380-139">It's important to give the report a name that contains the name of the list page associated with the report.</span><span class="sxs-lookup"><span data-stu-id="27380-139">It's important to give the report a name that contains the name of the list page associated with the report.</span></span> <span data-ttu-id="27380-140">For example, if the report is for the **Items** list page, include the word *items* somewhere in the name.</span><span class="sxs-lookup"><span data-stu-id="27380-140">For example, if the report is for the **Items** list page, include the word *items* somewhere in the name.</span></span>  

    <span data-ttu-id="27380-141">This naming convention isn't a requirement.</span><span class="sxs-lookup"><span data-stu-id="27380-141">This naming convention isn't a requirement.</span></span> <span data-ttu-id="27380-142">However, it makes selecting reports in [!INCLUDE[prod_short](includes/prod_short.md)] quicker.</span><span class="sxs-lookup"><span data-stu-id="27380-142">However, it makes selecting reports in [!INCLUDE[prod_short](includes/prod_short.md)] quicker.</span></span> <span data-ttu-id="27380-143">When the report selection page opens from a list page, it's automatically filtered based on the page name.</span><span class="sxs-lookup"><span data-stu-id="27380-143">When the report selection page opens from a list page, it's automatically filtered based on the page name.</span></span> <span data-ttu-id="27380-144">This filtering is done to limit the reports that are displayed.</span><span class="sxs-lookup"><span data-stu-id="27380-144">This filtering is done to limit the reports that are displayed.</span></span> <span data-ttu-id="27380-145">Users can clear the filter to get a full list of reports available in Power BI.</span><span class="sxs-lookup"><span data-stu-id="27380-145">Users can clear the filter to get a full list of reports available in Power BI.</span></span>

7. <span data-ttu-id="27380-146">When you're done, publish the report as usual.</span><span class="sxs-lookup"><span data-stu-id="27380-146">When you're done, publish the report as usual.</span></span>

    <span data-ttu-id="27380-147">For more information, see [Publishing a Report](across-how-use-financials-data-source-powerbi.md#publish-reports).</span><span class="sxs-lookup"><span data-stu-id="27380-147">For more information, see [Publishing a Report](across-how-use-financials-data-source-powerbi.md#publish-reports).</span></span>

8. <span data-ttu-id="27380-148">Test the report.</span><span class="sxs-lookup"><span data-stu-id="27380-148">Test the report.</span></span>

    <span data-ttu-id="27380-149">Once the reports been published to your workspace, it should be available from the Power BI FactBox on the list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="27380-149">Once the reports been published to your workspace, it should be available from the Power BI FactBox on the list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

    <span data-ttu-id="27380-150">To test it, do the following steps.</span><span class="sxs-lookup"><span data-stu-id="27380-150">To test it, do the following steps.</span></span>

    1. <span data-ttu-id="27380-151">Open [!INCLUDE[prod_short](includes/prod_short.md)] and go to the list page.</span><span class="sxs-lookup"><span data-stu-id="27380-151">Open [!INCLUDE[prod_short](includes/prod_short.md)] and go to the list page.</span></span>
    2. <span data-ttu-id="27380-152">If you don't see the Power BI FactBox, go the action bar, then select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span><span class="sxs-lookup"><span data-stu-id="27380-152">If you don't see the Power BI FactBox, go the action bar, then select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span></span>
    3. <span data-ttu-id="27380-153">In the Power BI FactBox, select **Select Reports**, select the **Enable** box for the report, then select **OK**.</span><span class="sxs-lookup"><span data-stu-id="27380-153">In the Power BI FactBox, select **Select Reports**, select the **Enable** box for the report, then select **OK**.</span></span>

    <span data-ttu-id="27380-154">If designed correctly, the report displays.</span><span class="sxs-lookup"><span data-stu-id="27380-154">If designed correctly, the report displays.</span></span>  

## <a name="set-the-report-size-and-color"></a><span data-ttu-id="27380-155">Set the report size and colour</span><span class="sxs-lookup"><span data-stu-id="27380-155">Set the report size and color</span></span>

<span data-ttu-id="27380-156">The size of the report must be set to 325 pixels by 310 pixels.</span><span class="sxs-lookup"><span data-stu-id="27380-156">The size of the report must be set to 325 pixels by 310 pixels.</span></span> <span data-ttu-id="27380-157">This size provides the proper scaling of the report in the available space of the Power BI FactBox control in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="27380-157">This size provides the proper scaling of the report in the available space of the Power BI FactBox control in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="27380-158">To define the size of the report, place focus outside of the report layout area, and then choose the paint roller icon.</span><span class="sxs-lookup"><span data-stu-id="27380-158">To define the size of the report, place focus outside of the report layout area, and then choose the paint roller icon.</span></span>

![Setting the report width and height for the Sales Invoice Activity report](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-sizing-v3.png)

<span data-ttu-id="27380-160">You can change the width and height of the report by choosing **Custom** in the **Type** field.</span><span class="sxs-lookup"><span data-stu-id="27380-160">You can change the width and height of the report by choosing **Custom** in the **Type** field.</span></span>

<span data-ttu-id="27380-161">If you want the background of the report to blend with the background colour of the Power BI FactBox control, set report background colour to *#FFFFFF* (white).</span><span class="sxs-lookup"><span data-stu-id="27380-161">If you want the background of the report to blend with the background color of the Power BI FactBox control, set report background color to *#FFFFFF* (white).</span></span> 

> [!TIP]
> <span data-ttu-id="27380-162">Use the [!INCLUDE [prod_short](includes/prod_short.md)] theme file to build reports with the same colour styling as the [!INCLUDE [prod_short](includes/prod_short.md)] apps.</span><span class="sxs-lookup"><span data-stu-id="27380-162">Use the [!INCLUDE [prod_short](includes/prod_short.md)] theme file to build reports with the same color styling as the [!INCLUDE [prod_short](includes/prod_short.md)] apps.</span></span> <span data-ttu-id="27380-163">For more information, see [Using the [!INCLUDE [prod_short](includes/prod_short.md)] report theme](across-how-use-financials-data-source-powerbi.md#theme).</span><span class="sxs-lookup"><span data-stu-id="27380-163">For more information, see [Using the [!INCLUDE [prod_short](includes/prod_short.md)] report theme](across-how-use-financials-data-source-powerbi.md#theme).</span></span>

## <a name="reports-with-multiple-pages"></a><span data-ttu-id="27380-164">Reports with multiple pages</span><span class="sxs-lookup"><span data-stu-id="27380-164">Reports with multiple pages</span></span>

<span data-ttu-id="27380-165">With Power BI, you can create a single report with multiple pages.</span><span class="sxs-lookup"><span data-stu-id="27380-165">With Power BI, you can create a single report with multiple pages.</span></span> <span data-ttu-id="27380-166">However, for reports that will display with list pages, we don't recommend that they have more than one page.</span><span class="sxs-lookup"><span data-stu-id="27380-166">However, for reports that will display with list pages, we don't recommend that they have more than one page.</span></span> <span data-ttu-id="27380-167">The Power BI FactBox will only show the first page of your report.</span><span class="sxs-lookup"><span data-stu-id="27380-167">The Power BI FactBox will only show the first page of your report.</span></span>

## <a name="fixing-problems"></a><span data-ttu-id="27380-168">Fixing problems</span><span class="sxs-lookup"><span data-stu-id="27380-168">Fixing problems</span></span>

<span data-ttu-id="27380-169">This section provides instructions about how to fix problems that you might run into when trying to view a Power BI report for a list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="27380-169">This section provides instructions about how to fix problems that you might run into when trying to view a Power BI report for a list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

### <a name="you-cant-see-the-power-bi-factbox-on-a-list-page"></a><span data-ttu-id="27380-170">You can't see the Power BI FactBox on a list page</span><span class="sxs-lookup"><span data-stu-id="27380-170">You can't see the Power BI FactBox on a list page</span></span>

<span data-ttu-id="27380-171">By default, the Power BI FactBox is hidden from view.</span><span class="sxs-lookup"><span data-stu-id="27380-171">By default, the Power BI FactBox is hidden from view.</span></span> <span data-ttu-id="27380-172">To show the FactBox on a page, from the action bar, select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span><span class="sxs-lookup"><span data-stu-id="27380-172">To show the FactBox on a page, from the action bar, select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span></span>

### <a name="you-cant-see-the-report-in-the-select-report-pane"></a><span data-ttu-id="27380-173">You can't see the report in the Select Report pane</span><span class="sxs-lookup"><span data-stu-id="27380-173">You can't see the report in the Select Report pane</span></span>

<span data-ttu-id="27380-174">It's probably because the report's name doesn't contain the name of the list page that's being shown.</span><span class="sxs-lookup"><span data-stu-id="27380-174">It's probably because the report's name doesn't contain the name of the list page that's being shown.</span></span> <span data-ttu-id="27380-175">Clear the filter to get a full list of Power BI reports available.</span><span class="sxs-lookup"><span data-stu-id="27380-175">Clear the filter to get a full list of Power BI reports available.</span></span>  

### <a name="report-is-loaded-but-blank-not-filtered-or-filtered-incorrectly"></a><span data-ttu-id="27380-176">Report is loaded but blank, not filtered, or filtered incorrectly</span><span class="sxs-lookup"><span data-stu-id="27380-176">Report is loaded but blank, not filtered, or filtered incorrectly</span></span>

<span data-ttu-id="27380-177">Verify that the report filter contains the right primary key.</span><span class="sxs-lookup"><span data-stu-id="27380-177">Verify that the report filter contains the right primary key.</span></span> <span data-ttu-id="27380-178">In most cases, this field is the **No.**</span><span class="sxs-lookup"><span data-stu-id="27380-178">In most cases, this field is the **No.**</span></span> <span data-ttu-id="27380-179">field, but in the **G/L Entry** table, for example, you must use the **Entry No.** field.</span><span class="sxs-lookup"><span data-stu-id="27380-179">field, but in the **G/L Entry** table, for example, you must use the **Entry No.** field.</span></span>

### <a name="report-is-loaded-but-it-shows-a-page-you-didnt-expect"></a><span data-ttu-id="27380-180">Report is loaded, but it shows a page you didn't expect</span><span class="sxs-lookup"><span data-stu-id="27380-180">Report is loaded, but it shows a page you didn't expect</span></span>

<span data-ttu-id="27380-181">Verify that the page you want displayed is the first page in your report.</span><span class="sxs-lookup"><span data-stu-id="27380-181">Verify that the page you want displayed is the first page in your report.</span></span>  

### <a name="report-appears-with-an-unwanted-gray-boarder-or-its-too-small-or-too-large"></a><span data-ttu-id="27380-182">Report appears with an unwanted grey border, or it's too small or too large</span><span class="sxs-lookup"><span data-stu-id="27380-182">Report appears with an unwanted gray boarder, or it's too small or too large</span></span>

<span data-ttu-id="27380-183">Verify that the report size is set to 325 pixels x 310 pixels.</span><span class="sxs-lookup"><span data-stu-id="27380-183">Verify that the report size is set to 325 pixels x 310 pixels.</span></span> <span data-ttu-id="27380-184">Save the report, and then refresh the list page.</span><span class="sxs-lookup"><span data-stu-id="27380-184">Save the report, and then refresh the list page.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="27380-185">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="27380-185">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="27380-186">See Also</span><span class="sxs-lookup"><span data-stu-id="27380-186">See Also</span></span>

[<span data-ttu-id="27380-187">Enabling Your Business Data for Power BI</span><span class="sxs-lookup"><span data-stu-id="27380-187">Enabling Your Business Data for Power BI</span></span>](admin-powerbi.md)  
<span data-ttu-id="27380-188">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="27380-188">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
[<span data-ttu-id="27380-189">Getting Ready for Doing Business</span><span class="sxs-lookup"><span data-stu-id="27380-189">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
<span data-ttu-id="27380-190">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="27380-190">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
[<span data-ttu-id="27380-191">Finance</span><span class="sxs-lookup"><span data-stu-id="27380-191">Finance</span></span>](finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]