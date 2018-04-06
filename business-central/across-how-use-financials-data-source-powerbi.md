---
title: Setup Reporting for Business Central in Power BI | Microsoft Docs
description: You can make your Financials data available as a data source in Power BI and build powerful reports of the state of your business.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 12/21/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 42939e97d121bd3a2abff91671d9f9571faffbfd
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="using-included365finincludesd365finmdmd-as-power-bi-data-source-for-building-reports"></a><span data-ttu-id="13d98-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as Power BI Data Source for Building Reports</span><span class="sxs-lookup"><span data-stu-id="13d98-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as Power BI Data Source for Building Reports</span></span>
<span data-ttu-id="13d98-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span><span class="sxs-lookup"><span data-stu-id="13d98-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

> [!NOTE]  
> <span data-ttu-id="13d98-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span><span class="sxs-lookup"><span data-stu-id="13d98-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="13d98-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="13d98-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="13d98-107">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="13d98-107">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop</span></span>
1. <span data-ttu-id="13d98-108">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span><span class="sxs-lookup"><span data-stu-id="13d98-108">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="13d98-109">In the **Get Data** window, choose **Online Services**, choose **Dynamics 365 Business Central**, and then choose the **Connect** button.</span><span class="sxs-lookup"><span data-stu-id="13d98-109">In the **Get Data** window, choose **Online Services**, choose **Dynamics 365 Business Central**, and then choose the **Connect** button.</span></span>
3. <span data-ttu-id="13d98-110">Power BI displays a wizard that will guide you through the [connection process](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md).</span><span class="sxs-lookup"><span data-stu-id="13d98-110">Power BI displays a wizard that will guide you through the [connection process](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md).</span></span> <span data-ttu-id="13d98-111">The first step will be to sign into the service.</span><span class="sxs-lookup"><span data-stu-id="13d98-111">The first step will be to sign into the service.</span></span> <span data-ttu-id="13d98-112">Select **Sign in** and choose the account you would like to sign in as.</span><span class="sxs-lookup"><span data-stu-id="13d98-112">Select **Sign in** and choose the account you would like to sign in as.</span></span> <span data-ttu-id="13d98-113">This should be the same account you sign into [!INCLUDE[d365fin](includes/d365fin_md.md)] with.</span><span class="sxs-lookup"><span data-stu-id="13d98-113">This should be the same account you sign into [!INCLUDE[d365fin](includes/d365fin_md.md)] with.</span></span>
4. <span data-ttu-id="13d98-114">Choose the **Connect** button to continue.</span><span class="sxs-lookup"><span data-stu-id="13d98-114">Choose the **Connect** button to continue.</span></span> <span data-ttu-id="13d98-115">The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] companies and data sources.</span><span class="sxs-lookup"><span data-stu-id="13d98-115">The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] companies and data sources.</span></span> <span data-ttu-id="13d98-116">These data source represent all the web services that you have published from each company in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="13d98-116">These data source represent all the web services that you have published from each company in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
5. <span data-ttu-id="13d98-117">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span><span class="sxs-lookup"><span data-stu-id="13d98-117">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>
6. <span data-ttu-id="13d98-118">Specify the data you want to add to your data model, and then choose the **Load** button.</span><span class="sxs-lookup"><span data-stu-id="13d98-118">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
7. <span data-ttu-id="13d98-119">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span><span class="sxs-lookup"><span data-stu-id="13d98-119">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

> [!NOTE]  
> <span data-ttu-id="13d98-120">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again to sign in.</span><span class="sxs-lookup"><span data-stu-id="13d98-120">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again to sign in.</span></span>

<span data-ttu-id="13d98-121">Once the data is loaded it will appear in the right navigation on the page.</span><span class="sxs-lookup"><span data-stu-id="13d98-121">Once the data is loaded it will appear in the right navigation on the page.</span></span> <span data-ttu-id="13d98-122">At this point, you have successfully connected to your Business Central data and are ready to begin building your Power BI report.</span><span class="sxs-lookup"><span data-stu-id="13d98-122">At this point, you have successfully connected to your Business Central data and are ready to begin building your Power BI report.</span></span> <span data-ttu-id="13d98-123">For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span><span class="sxs-lookup"><span data-stu-id="13d98-123">For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span></span>

## <a name="see-also"></a><span data-ttu-id="13d98-124">See Also</span><span class="sxs-lookup"><span data-stu-id="13d98-124">See Also</span></span>
[<span data-ttu-id="13d98-125">Business Intelligence</span><span class="sxs-lookup"><span data-stu-id="13d98-125">Business Intelligence</span></span>](bi.md)  
<span data-ttu-id="13d98-126">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="13d98-126">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="13d98-127">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="13d98-127">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="13d98-128">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md) </span><span class="sxs-lookup"><span data-stu-id="13d98-128">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md) </span></span>  
[<span data-ttu-id="13d98-129">Finance</span><span class="sxs-lookup"><span data-stu-id="13d98-129">Finance</span></span>](finance.md)  
<span data-ttu-id="13d98-130">[Connecting Power BI to [!INCLUDE[d365fin](includes/d365fin_md.md)]](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md)</span><span class="sxs-lookup"><span data-stu-id="13d98-130">[Connecting Power BI to [!INCLUDE[d365fin](includes/d365fin_md.md)]](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md)</span></span>  

