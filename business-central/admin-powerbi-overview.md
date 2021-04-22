---
title: Power BI Integration Component and Architecture Overview for Business Central| Microsoft Docs
description: Getting insight, business intelligence, and KPIs from your Business Central data is easy with the Business Central apps for Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.reviewer: edupont
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: e1091496b7d4ec4bed4cc8c49fa1e2e00a336a3c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777423"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prod_short"></a><span data-ttu-id="c83d0-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="c83d0-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

<span data-ttu-id="c83d0-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prod_short](includes/prod_short.md)] to help you understand its implementation and use.</span><span class="sxs-lookup"><span data-stu-id="c83d0-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prod_short](includes/prod_short.md)] to help you understand its implementation and use.</span></span>

## <a name="components"></a><span data-ttu-id="c83d0-105">Components</span><span class="sxs-lookup"><span data-stu-id="c83d0-105">Components</span></span>

<span data-ttu-id="c83d0-106">The following table describes the major components involved with Power BI integration.</span><span class="sxs-lookup"><span data-stu-id="c83d0-106">The following table describes the major components involved with Power BI integration.</span></span>

|<span data-ttu-id="c83d0-107">Component</span><span class="sxs-lookup"><span data-stu-id="c83d0-107">Component</span></span>|<span data-ttu-id="c83d0-108">Description</span><span class="sxs-lookup"><span data-stu-id="c83d0-108">Description</span></span>|
|---------|-----------|
|<span data-ttu-id="c83d0-109">Power BI</span><span class="sxs-lookup"><span data-stu-id="c83d0-109">Power BI</span></span>|<span data-ttu-id="c83d0-110">A cloud-based report hosting and management service.</span><span class="sxs-lookup"><span data-stu-id="c83d0-110">A cloud-based report hosting and management service.</span></span>|
|<span data-ttu-id="c83d0-111">Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="c83d0-111">Power BI Desktop</span></span>|<span data-ttu-id="c83d0-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span><span class="sxs-lookup"><span data-stu-id="c83d0-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span></span> <span data-ttu-id="c83d0-113">It's available as a free download on Microsoft Store and is installed locally.</span><span class="sxs-lookup"><span data-stu-id="c83d0-113">It's available as a free download on Microsoft Store and is installed locally.</span></span>|
|[!INCLUDE[prod_short](includes/prod_short.md)]|<span data-ttu-id="c83d0-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span><span class="sxs-lookup"><span data-stu-id="c83d0-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span></span>|

## <a name="whats-available-from-the-start"></a><span data-ttu-id="c83d0-115">What's available from the start</span><span class="sxs-lookup"><span data-stu-id="c83d0-115">What's available from the start</span></span>

<span data-ttu-id="c83d0-116">The following table describes available features.</span><span class="sxs-lookup"><span data-stu-id="c83d0-116">The following table describes available features.</span></span>

|<span data-ttu-id="c83d0-117">Feature</span><span class="sxs-lookup"><span data-stu-id="c83d0-117">Feature</span></span>|[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="c83d0-118">online or on-premises support</span><span class="sxs-lookup"><span data-stu-id="c83d0-118">online or on-premises support</span></span>|
|-------|---------------------|
|<span data-ttu-id="c83d0-119">Power BI connectors</span><span class="sxs-lookup"><span data-stu-id="c83d0-119">Power BI connectors</span></span>|<span data-ttu-id="c83d0-120">Both.</span><span class="sxs-lookup"><span data-stu-id="c83d0-120">Both.</span></span> <span data-ttu-id="c83d0-121">Different connectors for online and on-premises.</span><span class="sxs-lookup"><span data-stu-id="c83d0-121">Different connectors for online and on-premises.</span></span> <span data-ttu-id="c83d0-122">Same connector used for Power BI Desktop and Power BI Service</span><span class="sxs-lookup"><span data-stu-id="c83d0-122">Same connector used for Power BI Desktop and Power BI Service</span></span> |
|<span data-ttu-id="c83d0-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="c83d0-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>|<span data-ttu-id="c83d0-124">Both.</span><span class="sxs-lookup"><span data-stu-id="c83d0-124">Both.</span></span> <span data-ttu-id="c83d0-125">Requires configuration to display reports for on-premises.</span><span class="sxs-lookup"><span data-stu-id="c83d0-125">Requires configuration to display reports for on-premises.</span></span>|
|<span data-ttu-id="c83d0-126">Power BI report management from [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="c83d0-126">Power BI report management from [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>|<span data-ttu-id="c83d0-127">Online</span><span class="sxs-lookup"><span data-stu-id="c83d0-127">Online</span></span>|
|<span data-ttu-id="c83d0-128">Default Power BI reports on role centres deployed to Power BI</span><span class="sxs-lookup"><span data-stu-id="c83d0-128">Default Power BI reports on role centers deployed to Power BI</span></span>|<span data-ttu-id="c83d0-129">Online</span><span class="sxs-lookup"><span data-stu-id="c83d0-129">Online</span></span>|
|<span data-ttu-id="c83d0-130">Power BI Apps on Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="c83d0-130">Power BI Apps on Microsoft AppSource</span></span>|<span data-ttu-id="c83d0-131">Online.</span><span class="sxs-lookup"><span data-stu-id="c83d0-131">Online.</span></span>|

## <a name="architecture"></a><span data-ttu-id="c83d0-132">Architecture</span><span class="sxs-lookup"><span data-stu-id="c83d0-132">Architecture</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="c83d0-133">integrates with Power BI through a connector using OData.</span><span class="sxs-lookup"><span data-stu-id="c83d0-133">integrates with Power BI through a connector using OData.</span></span> <span data-ttu-id="c83d0-134">The data source for Power BI reports is exposed as OData web services.</span><span class="sxs-lookup"><span data-stu-id="c83d0-134">The data source for Power BI reports is exposed as OData web services.</span></span>

![Power BI architecture for integration with Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a><span data-ttu-id="c83d0-136">General Flow</span><span class="sxs-lookup"><span data-stu-id="c83d0-136">General Flow</span></span>

<span data-ttu-id="c83d0-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prod_short](includes/prod_short.md)] to Power BI.</span><span class="sxs-lookup"><span data-stu-id="c83d0-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prod_short](includes/prod_short.md)] to Power BI.</span></span>

![Power BI workflow  for integration with Business Central](./media/power-bi-flow.png)

1. <span data-ttu-id="c83d0-139">User signs up for a Power BI account.</span><span class="sxs-lookup"><span data-stu-id="c83d0-139">User signs up for a Power BI account.</span></span>
2. <span data-ttu-id="c83d0-140">User connects to Power BI from [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="c83d0-140">User connects to Power BI from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
3. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="c83d0-141">verifies the licence.</span><span class="sxs-lookup"><span data-stu-id="c83d0-141">verifies the license.</span></span>
4. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="c83d0-142">deploys default reports to the Power BI service.</span><span class="sxs-lookup"><span data-stu-id="c83d0-142">deploys default reports to the Power BI service.</span></span> <span data-ttu-id="c83d0-143">This step only happens for [!INCLUDE[prod_short](includes/prod_short.md)] online.</span><span class="sxs-lookup"><span data-stu-id="c83d0-143">This step only happens for [!INCLUDE[prod_short](includes/prod_short.md)] online.</span></span>
5. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="c83d0-144">makes reports in Power BI available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="c83d0-144">makes reports in Power BI available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="c83d0-145">Default reports are automatically displayed in Power BI parts.</span><span class="sxs-lookup"><span data-stu-id="c83d0-145">Default reports are automatically displayed in Power BI parts.</span></span>
6. <span data-ttu-id="c83d0-146">User creates a report in Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="c83d0-146">User creates a report in Power BI Desktop.</span></span>
7. <span data-ttu-id="c83d0-147">User publishes the report to the Power BI service.</span><span class="sxs-lookup"><span data-stu-id="c83d0-147">User publishes the report to the Power BI service.</span></span> <span data-ttu-id="c83d0-148">The reports are then available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="c83d0-148">The reports are then available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="c83d0-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="c83d0-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="c83d0-150">See Also</span><span class="sxs-lookup"><span data-stu-id="c83d0-150">See Also</span></span>

[<span data-ttu-id="c83d0-151">Business Central and Power BI</span><span class="sxs-lookup"><span data-stu-id="c83d0-151">Business Central and Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="c83d0-152">Power BI for consumers</span><span class="sxs-lookup"><span data-stu-id="c83d0-152">Power BI for consumers</span></span>](/power-bi/consumer/end-user-consumer)  
[<span data-ttu-id="c83d0-153">The 'new look' of the Power BI service</span><span class="sxs-lookup"><span data-stu-id="c83d0-153">The 'new look' of the Power BI service</span></span>](/power-bi/service-new-look)  
[<span data-ttu-id="c83d0-154">Quickstart: Connect to data in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="c83d0-154">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
[<span data-ttu-id="c83d0-155">Power BI documentation</span><span class="sxs-lookup"><span data-stu-id="c83d0-155">Power BI documentation</span></span>](/power-bi/)  
[<span data-ttu-id="c83d0-156">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="c83d0-156">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="c83d0-157">Getting Ready for Doing Business</span><span class="sxs-lookup"><span data-stu-id="c83d0-157">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
[<span data-ttu-id="c83d0-158">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="c83d0-158">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="c83d0-159">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="c83d0-159">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
<span data-ttu-id="c83d0-160">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="c83d0-160">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="c83d0-161">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span><span class="sxs-lookup"><span data-stu-id="c83d0-161">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span></span>  
<span data-ttu-id="c83d0-162">[Using [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="c83d0-162">[Using [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span></span>  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]