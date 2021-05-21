---
title: Power BI Integration Component and Architecture Overview for Business Central| Microsoft Docs
description: Learn about the different aspects of Power BI integration with Business Central.
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
ms.openlocfilehash: a1d0d0403798f8cd2af6b29249f01f529fb789be
ms.sourcegitcommit: c11ad91a389ed72532f5513654fdc7909b20aed9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/22/2021
ms.locfileid: "5935243"
---
# <a name="power-bi-integration-component-and-architecture-overview-for-prod_short"></a><span data-ttu-id="e707b-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="e707b-103">Power BI Integration Component and Architecture Overview for [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

<span data-ttu-id="e707b-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prod_short](includes/prod_short.md)] to help you understand its implementation and use.</span><span class="sxs-lookup"><span data-stu-id="e707b-104">In this article, you'll learn about the different aspects of Power BI integration with [!INCLUDE[prod_short](includes/prod_short.md)] to help you understand its implementation and use.</span></span>

## <a name="components"></a><span data-ttu-id="e707b-105">Components</span><span class="sxs-lookup"><span data-stu-id="e707b-105">Components</span></span>

<span data-ttu-id="e707b-106">The following table describes the major components involved with Power BI integration.</span><span class="sxs-lookup"><span data-stu-id="e707b-106">The following table describes the major components involved with Power BI integration.</span></span>

|<span data-ttu-id="e707b-107">Component</span><span class="sxs-lookup"><span data-stu-id="e707b-107">Component</span></span>|<span data-ttu-id="e707b-108">Description</span><span class="sxs-lookup"><span data-stu-id="e707b-108">Description</span></span>|
|---------|-----------|
|<span data-ttu-id="e707b-109">Power BI</span><span class="sxs-lookup"><span data-stu-id="e707b-109">Power BI</span></span>|<span data-ttu-id="e707b-110">A cloud-based report hosting and management service.</span><span class="sxs-lookup"><span data-stu-id="e707b-110">A cloud-based report hosting and management service.</span></span>|
|<span data-ttu-id="e707b-111">Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="e707b-111">Power BI Desktop</span></span>|<span data-ttu-id="e707b-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span><span class="sxs-lookup"><span data-stu-id="e707b-112">An authoring tool for building reports and dashboards, and allows you to run reports.</span></span> <span data-ttu-id="e707b-113">It's available as a free download on Microsoft Store and is installed locally.</span><span class="sxs-lookup"><span data-stu-id="e707b-113">It's available as a free download on Microsoft Store and is installed locally.</span></span>|
|[!INCLUDE[prod_short](includes/prod_short.md)]|<span data-ttu-id="e707b-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span><span class="sxs-lookup"><span data-stu-id="e707b-114">Online or on-premises solution with connectors exposed to Power BI and the ability to embed a Power BI part.</span></span>|

## <a name="whats-available-from-the-start"></a><span data-ttu-id="e707b-115">What's available from the start</span><span class="sxs-lookup"><span data-stu-id="e707b-115">What's available from the start</span></span>

<span data-ttu-id="e707b-116">The following table describes available features.</span><span class="sxs-lookup"><span data-stu-id="e707b-116">The following table describes available features.</span></span>

|<span data-ttu-id="e707b-117">Feature</span><span class="sxs-lookup"><span data-stu-id="e707b-117">Feature</span></span>|[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e707b-118">online or on-premises support</span><span class="sxs-lookup"><span data-stu-id="e707b-118">online or on-premises support</span></span>|
|-------|---------------------|
|<span data-ttu-id="e707b-119">Power BI connectors</span><span class="sxs-lookup"><span data-stu-id="e707b-119">Power BI connectors</span></span>|<span data-ttu-id="e707b-120">Both.</span><span class="sxs-lookup"><span data-stu-id="e707b-120">Both.</span></span> <span data-ttu-id="e707b-121">Different connectors for online and on-premises.</span><span class="sxs-lookup"><span data-stu-id="e707b-121">Different connectors for online and on-premises.</span></span> <span data-ttu-id="e707b-122">Same connector used for Power BI Desktop and Power BI Service</span><span class="sxs-lookup"><span data-stu-id="e707b-122">Same connector used for Power BI Desktop and Power BI Service</span></span> |
|<span data-ttu-id="e707b-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="e707b-123">Embedded experience for viewing a given report inside a FactBox in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>|<span data-ttu-id="e707b-124">Both.</span><span class="sxs-lookup"><span data-stu-id="e707b-124">Both.</span></span> <span data-ttu-id="e707b-125">Requires configuration to display reports for on-premises.</span><span class="sxs-lookup"><span data-stu-id="e707b-125">Requires configuration to display reports for on-premises.</span></span>|
|<span data-ttu-id="e707b-126">Power BI report management from [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="e707b-126">Power BI report management from [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>|<span data-ttu-id="e707b-127">Online</span><span class="sxs-lookup"><span data-stu-id="e707b-127">Online</span></span>|
|<span data-ttu-id="e707b-128">Default Power BI reports on role centres deployed to Power BI</span><span class="sxs-lookup"><span data-stu-id="e707b-128">Default Power BI reports on role centers deployed to Power BI</span></span>|<span data-ttu-id="e707b-129">Online</span><span class="sxs-lookup"><span data-stu-id="e707b-129">Online</span></span>|
|<span data-ttu-id="e707b-130">Power BI Apps on Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="e707b-130">Power BI Apps on Microsoft AppSource</span></span>|<span data-ttu-id="e707b-131">Online.</span><span class="sxs-lookup"><span data-stu-id="e707b-131">Online.</span></span>|

## <a name="architecture"></a><span data-ttu-id="e707b-132">Architecture</span><span class="sxs-lookup"><span data-stu-id="e707b-132">Architecture</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e707b-133">integrates with Power BI through a connector using OData.</span><span class="sxs-lookup"><span data-stu-id="e707b-133">integrates with Power BI through a connector using OData.</span></span> <span data-ttu-id="e707b-134">The data source for Power BI reports is exposed as OData web services.</span><span class="sxs-lookup"><span data-stu-id="e707b-134">The data source for Power BI reports is exposed as OData web services.</span></span>

![Power BI architecture for integration with Business Central](./media/power-bi-architecture.png)

## <a name="general-flow"></a><span data-ttu-id="e707b-136">General Flow</span><span class="sxs-lookup"><span data-stu-id="e707b-136">General Flow</span></span>

<span data-ttu-id="e707b-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prod_short](includes/prod_short.md)] to Power BI.</span><span class="sxs-lookup"><span data-stu-id="e707b-137">The following diagram illustrates the basic workflow for users when connecting [!INCLUDE[prod_short](includes/prod_short.md)] to Power BI.</span></span>

![Power BI workflow  for integration with Business Central](./media/power-bi-flow.png)

1. <span data-ttu-id="e707b-139">User signs up for a Power BI account.</span><span class="sxs-lookup"><span data-stu-id="e707b-139">User signs up for a Power BI account.</span></span>
2. <span data-ttu-id="e707b-140">User connects to Power BI from [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="e707b-140">User connects to Power BI from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
3. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e707b-141">verifies the licence.</span><span class="sxs-lookup"><span data-stu-id="e707b-141">verifies the license.</span></span>
4. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e707b-142">deploys default reports to the Power BI service.</span><span class="sxs-lookup"><span data-stu-id="e707b-142">deploys default reports to the Power BI service.</span></span> <span data-ttu-id="e707b-143">This step only happens for [!INCLUDE[prod_short](includes/prod_short.md)] online.</span><span class="sxs-lookup"><span data-stu-id="e707b-143">This step only happens for [!INCLUDE[prod_short](includes/prod_short.md)] online.</span></span>
5. [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="e707b-144">makes reports in Power BI available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="e707b-144">makes reports in Power BI available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="e707b-145">Default reports are automatically displayed in Power BI parts.</span><span class="sxs-lookup"><span data-stu-id="e707b-145">Default reports are automatically displayed in Power BI parts.</span></span>
6. <span data-ttu-id="e707b-146">User creates a report in Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="e707b-146">User creates a report in Power BI Desktop.</span></span>
7. <span data-ttu-id="e707b-147">User publishes the report to the Power BI service.</span><span class="sxs-lookup"><span data-stu-id="e707b-147">User publishes the report to the Power BI service.</span></span> <span data-ttu-id="e707b-148">The reports are then available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="e707b-148">The reports are then available for selection in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="e707b-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="e707b-149">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="e707b-150">See Also</span><span class="sxs-lookup"><span data-stu-id="e707b-150">See Also</span></span>

[<span data-ttu-id="e707b-151">Business Central and Power BI</span><span class="sxs-lookup"><span data-stu-id="e707b-151">Business Central and Power BI</span></span>](admin-powerbi.md)  
[<span data-ttu-id="e707b-152">Power BI for consumers</span><span class="sxs-lookup"><span data-stu-id="e707b-152">Power BI for consumers</span></span>](/power-bi/consumer/end-user-consumer)  
[<span data-ttu-id="e707b-153">The 'new look' of the Power BI service</span><span class="sxs-lookup"><span data-stu-id="e707b-153">The 'new look' of the Power BI service</span></span>](/power-bi/service-new-look)  
[<span data-ttu-id="e707b-154">Quickstart: Connect to data in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="e707b-154">Quickstart: Connect to data in Power BI Desktop</span></span>](/power-bi/desktop-quickstart-connect-to-data)  
[<span data-ttu-id="e707b-155">Power BI documentation</span><span class="sxs-lookup"><span data-stu-id="e707b-155">Power BI documentation</span></span>](/power-bi/)  
[<span data-ttu-id="e707b-156">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="e707b-156">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="e707b-157">Getting Ready for Doing Business</span><span class="sxs-lookup"><span data-stu-id="e707b-157">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
[<span data-ttu-id="e707b-158">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="e707b-158">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="e707b-159">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="e707b-159">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
<span data-ttu-id="e707b-160">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="e707b-160">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
<span data-ttu-id="e707b-161">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span><span class="sxs-lookup"><span data-stu-id="e707b-161">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power Apps Data Source](across-how-use-financials-data-source-powerapps.md)</span></span>  
<span data-ttu-id="e707b-162">[Using [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="e707b-162">[Using [!INCLUDE[prod_short](includes/prod_short.md)] in Power Automate](across-how-use-financials-data-source-flow.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]