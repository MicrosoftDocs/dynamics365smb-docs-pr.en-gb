---
title: Use Your Data to Create an App| Microsoft Docs
description: You can make your Business Central data available as a data source and specify an OData URL of your web services to build a business app using Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 06/22/2020
ms.author: edupont
ms.openlocfilehash: 8f0eb7a1562a8300bd7181ef6470c70f60934470
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528645"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a><span data-ttu-id="9bb53-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span><span class="sxs-lookup"><span data-stu-id="9bb53-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span></span>

<span data-ttu-id="9bb53-104">You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.</span><span class="sxs-lookup"><span data-stu-id="9bb53-104">You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.</span></span>  

> [!NOTE]  
> <span data-ttu-id="9bb53-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.</span><span class="sxs-lookup"><span data-stu-id="9bb53-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.</span></span>  

## <a name="to-add-prodshort-as-a-data-source-in-power-apps"></a><span data-ttu-id="9bb53-106">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps</span><span class="sxs-lookup"><span data-stu-id="9bb53-106">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps</span></span>

1. <span data-ttu-id="9bb53-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span><span class="sxs-lookup"><span data-stu-id="9bb53-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span></span>
2. <span data-ttu-id="9bb53-108">On the Home page, in the **Start from data** section, choose the **Other data sources** tile.</span><span class="sxs-lookup"><span data-stu-id="9bb53-108">On the Home page, in the **Start from data** section, choose the **Other data sources** tile.</span></span>  

    <span data-ttu-id="9bb53-109">This opens Power Apps Studio.</span><span class="sxs-lookup"><span data-stu-id="9bb53-109">This opens Power Apps Studio.</span></span> <span data-ttu-id="9bb53-110">On first login, you must specify the country/region.</span><span class="sxs-lookup"><span data-stu-id="9bb53-110">On first login, you must specify the country/region.</span></span>  
3. <span data-ttu-id="9bb53-111">In the list of available connections, choose **Business Central**, and then choose the **Create** button.</span><span class="sxs-lookup"><span data-stu-id="9bb53-111">In the list of available connections, choose **Business Central**, and then choose the **Create** button.</span></span>

    <span data-ttu-id="9bb53-112">Power Apps will connect to your [!INCLUDE[prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span><span class="sxs-lookup"><span data-stu-id="9bb53-112">Power Apps will connect to your [!INCLUDE[prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span></span> <span data-ttu-id="9bb53-113">If you are not an administrator of your [!INCLUDE[prodshort](includes/prodshort.md)], you may have to sign in with another account.</span><span class="sxs-lookup"><span data-stu-id="9bb53-113">If you are not an administrator of your [!INCLUDE[prodshort](includes/prodshort.md)], you may have to sign in with another account.</span></span>  

4. <span data-ttu-id="9bb53-114">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="9bb53-114">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="9bb53-115">Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company*.</span><span class="sxs-lookup"><span data-stu-id="9bb53-115">Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company*.</span></span>  

5. <span data-ttu-id="9bb53-116">Next, you will be presented with a list of tables that are exposed as part of the API for your environment.</span><span class="sxs-lookup"><span data-stu-id="9bb53-116">Next, you will be presented with a list of tables that are exposed as part of the API for your environment.</span></span> <span data-ttu-id="9bb53-117">Select the table that you want to connect to, and then choose **Connect**.</span><span class="sxs-lookup"><span data-stu-id="9bb53-117">Select the table that you want to connect to, and then choose **Connect**.</span></span>

<span data-ttu-id="9bb53-118">These so-called tables are exposed as endpoints by the [!INCLUDE[prodshort](includes/prodshort.md)] connector for Power Apps.</span><span class="sxs-lookup"><span data-stu-id="9bb53-118">These so-called tables are exposed as endpoints by the [!INCLUDE[prodshort](includes/prodshort.md)] connector for Power Apps.</span></span>  

> [!NOTE]
> <span data-ttu-id="9bb53-119">If you want to include data from other tables in [!INCLUDE[prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps.</span><span class="sxs-lookup"><span data-stu-id="9bb53-119">If you want to include data from other tables in [!INCLUDE[prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps.</span></span> <span data-ttu-id="9bb53-120">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span><span class="sxs-lookup"><span data-stu-id="9bb53-120">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span></span>  

<span data-ttu-id="9bb53-121">At this point, you have successfully connected to your [!INCLUDE[prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span><span class="sxs-lookup"><span data-stu-id="9bb53-121">At this point, you have successfully connected to your [!INCLUDE[prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="9bb53-122">You can add additional screens and connect to additional data from your [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="9bb53-122">You can add additional screens and connect to additional data from your [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="9bb53-123">For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).</span><span class="sxs-lookup"><span data-stu-id="9bb53-123">For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).</span></span>  

<span data-ttu-id="9bb53-124">When you have designed and built your app, you can share it with your colleagues.</span><span class="sxs-lookup"><span data-stu-id="9bb53-124">When you have designed and built your app, you can share it with your colleagues.</span></span> <span data-ttu-id="9bb53-125">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span><span class="sxs-lookup"><span data-stu-id="9bb53-125">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span></span>  

> [!NOTE]
> <span data-ttu-id="9bb53-126">If you want to connect to [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span><span class="sxs-lookup"><span data-stu-id="9bb53-126">If you want to connect to [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9bb53-127">See Also</span><span class="sxs-lookup"><span data-stu-id="9bb53-127">See Also</span></span>

[<span data-ttu-id="9bb53-128">Create a canvas app from a template in Power Apps</span><span class="sxs-lookup"><span data-stu-id="9bb53-128">Create a canvas app from a template in Power Apps</span></span>](/powerapps/maker/canvas-apps/get-started-test-drive)  
[<span data-ttu-id="9bb53-129">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="9bb53-129">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="9bb53-130">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="9bb53-130">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="9bb53-131">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="9bb53-131">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
