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
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: f6b771b0107214702785d2b124983eb369741a84
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3187923"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a><span data-ttu-id="2cb59-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span><span class="sxs-lookup"><span data-stu-id="2cb59-103">Connecting to Your Business Central Data to Build a Business App Using Power Apps</span></span>

<span data-ttu-id="2cb59-104">You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.</span><span class="sxs-lookup"><span data-stu-id="2cb59-104">You can make your [!INCLUDE[prodshort](includes/prodshort.md)] data available as a data source in Power Apps.</span></span>  

> [!NOTE]  
> <span data-ttu-id="2cb59-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.</span><span class="sxs-lookup"><span data-stu-id="2cb59-105">You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power Apps.</span></span>  

## <a name="to-add-prodshort-as-a-data-source-in-power-apps"></a><span data-ttu-id="2cb59-106">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps</span><span class="sxs-lookup"><span data-stu-id="2cb59-106">To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power Apps</span></span>

1. <span data-ttu-id="2cb59-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span><span class="sxs-lookup"><span data-stu-id="2cb59-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.</span></span>
2. <span data-ttu-id="2cb59-108">On the Home page, choose the **Apps**, **Create an app** and **Canvas** to create a new canvas app.</span><span class="sxs-lookup"><span data-stu-id="2cb59-108">On the Home page, choose the **Apps**, **Create an app** and **Canvas** to create a new canvas app.</span></span> <span data-ttu-id="2cb59-109">This app will be designed for use on a mobile device, but you can also choose to use another template.</span><span class="sxs-lookup"><span data-stu-id="2cb59-109">This app will be designed for use on a mobile device, but you can also choose to use another template.</span></span>

    <span data-ttu-id="2cb59-110">The next step to create a Power App is to select your data.</span><span class="sxs-lookup"><span data-stu-id="2cb59-110">The next step to create a Power App is to select your data.</span></span> <span data-ttu-id="2cb59-111">Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.</span><span class="sxs-lookup"><span data-stu-id="2cb59-111">Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.</span></span>
3. <span data-ttu-id="2cb59-112">In the list of available connections, choose **Business Central**, and then choose the **Create** button.</span><span class="sxs-lookup"><span data-stu-id="2cb59-112">In the list of available connections, choose **Business Central**, and then choose the **Create** button.</span></span>

    <span data-ttu-id="2cb59-113">Power Apps will connect to your [!INCLUDE [prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span><span class="sxs-lookup"><span data-stu-id="2cb59-113">Power Apps will connect to your [!INCLUDE [prodshort](includes/prodshort.md)] using the credentials that you are signed in with.</span></span> <span data-ttu-id="2cb59-114">If you are not an administrator of your [!INCLUDE [prodshort](includes/prodshort.md)], you may have to sign in with another account.</span><span class="sxs-lookup"><span data-stu-id="2cb59-114">If you are not an administrator of your [!INCLUDE [prodshort](includes/prodshort.md)], you may have to sign in with another account.</span></span>  

4. <span data-ttu-id="2cb59-115">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="2cb59-115">Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="2cb59-116">Choose the environment and company that contains the data you want to connect to.</span><span class="sxs-lookup"><span data-stu-id="2cb59-116">Choose the environment and company that contains the data you want to connect to.</span></span> <span data-ttu-id="2cb59-117">Next, you will be presented with a list of APIs.</span><span class="sxs-lookup"><span data-stu-id="2cb59-117">Next, you will be presented with a list of APIs.</span></span> <span data-ttu-id="2cb59-118">Select the **API** you want to connect to.</span><span class="sxs-lookup"><span data-stu-id="2cb59-118">Select the **API** you want to connect to.</span></span>

<span data-ttu-id="2cb59-119">These so-called tables are part of the [!INCLUDE [prodshort](includes/prodshort.md)] API.</span><span class="sxs-lookup"><span data-stu-id="2cb59-119">These so-called tables are part of the [!INCLUDE [prodshort](includes/prodshort.md)] API.</span></span> <span data-ttu-id="2cb59-120">You do not have to configure the end points yourself - the [!INCLUDE [prodshort](includes/prodshort.md)] connector for Power Apps does it for you.</span><span class="sxs-lookup"><span data-stu-id="2cb59-120">You do not have to configure the end points yourself - the [!INCLUDE [prodshort](includes/prodshort.md)] connector for Power Apps does it for you.</span></span>  

> [!NOTE]
> <span data-ttu-id="2cb59-121">If you want to include data from other tables in [!INCLUDE [prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE [prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps.</span><span class="sxs-lookup"><span data-stu-id="2cb59-121">If you want to include data from other tables in [!INCLUDE [prodshort](includes/prodshort.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE [prodshort](includes/prodshort.md)] and then consume that custom API through a custom connector in Power Apps.</span></span> <span data-ttu-id="2cb59-122">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span><span class="sxs-lookup"><span data-stu-id="2cb59-122">For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).</span></span>  

<span data-ttu-id="2cb59-123">At this point, you have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span><span class="sxs-lookup"><span data-stu-id="2cb59-123">At this point, you have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="2cb59-124">You can add additional screens and connect to additional data from your [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="2cb59-124">You can add additional screens and connect to additional data from your [!INCLUDE [prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="2cb59-125">For more information, see [Create a canvas app from a template in Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive).</span><span class="sxs-lookup"><span data-stu-id="2cb59-125">For more information, see [Create a canvas app from a template in Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive).</span></span>  

<span data-ttu-id="2cb59-126">When you have designed and built your app, you can share it with your colleagues.</span><span class="sxs-lookup"><span data-stu-id="2cb59-126">When you have designed and built your app, you can share it with your colleagues.</span></span> <span data-ttu-id="2cb59-127">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span><span class="sxs-lookup"><span data-stu-id="2cb59-127">For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).</span></span>  

> [!NOTE]
> <span data-ttu-id="2cb59-128">If you want to connect to [!INCLUDE [prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span><span class="sxs-lookup"><span data-stu-id="2cb59-128">If you want to connect to [!INCLUDE [prodshort](includes/prodshort.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2cb59-129">See Also</span><span class="sxs-lookup"><span data-stu-id="2cb59-129">See Also</span></span>

[<span data-ttu-id="2cb59-130">Create a canvas app from a template in Power Apps</span><span class="sxs-lookup"><span data-stu-id="2cb59-130">Create a canvas app from a template in Power Apps</span></span>](/powerapps/maker/canvas-apps/get-started-test-drive)  
[<span data-ttu-id="2cb59-131">Getting Started</span><span class="sxs-lookup"><span data-stu-id="2cb59-131">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="2cb59-132">Importing Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="2cb59-132">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="2cb59-133">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="2cb59-133">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="2cb59-134">Finance</span><span class="sxs-lookup"><span data-stu-id="2cb59-134">Finance</span></span>](finance.md)  
[<span data-ttu-id="2cb59-135">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="2cb59-135">Getting Started Developing Connect Apps for Dynamics 365 Business Central</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  
