---
title: Installing Extensions to Customise Business Central  | Microsoft Docs
description: Learn about adding functionality and customising Business Central  by installing extensions.
documentationcenter: ''
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 08/12/2020
ms.author: edupont
ms.openlocfilehash: 2011728e8e036442418c6a2d8b51477b45b02d1e
ms.sourcegitcommit: 43284728c34b72ad1984a516273dc80e4cdc99ab
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 09/04/2020
ms.locfileid: "3765928"
---
# <a name="customizing-business-central-using-extensions"></a><span data-ttu-id="9f613-103">Customising Business Central Using Extensions</span><span class="sxs-lookup"><span data-stu-id="9f613-103">Customizing Business Central Using Extensions</span></span>

<span data-ttu-id="9f613-104">You can change [!INCLUDE[d365fin](includes/d365fin_md.md)] by installing extensions that add functionality, changes behaviour, or gives you access to new online services, for example.</span><span class="sxs-lookup"><span data-stu-id="9f613-104">You can change [!INCLUDE[d365fin](includes/d365fin_md.md)] by installing extensions that add functionality, changes behavior, or gives you access to new online services, for example.</span></span>

> [!NOTE]
> <span data-ttu-id="9f613-105">To install extensions from AppSource or add per-tenant extensions, you must have the right permissions.</span><span class="sxs-lookup"><span data-stu-id="9f613-105">To install extensions from AppSource or add per-tenant extensions, you must have the right permissions.</span></span> <span data-ttu-id="9f613-106">You must either be a member of the D365 EXTENSION MGMT user group or you must have the D365 EXTENSION MGMT permission set.</span><span class="sxs-lookup"><span data-stu-id="9f613-106">You must either be a member of the D365 EXTENSION MGMT user group or you must have the D365 EXTENSION MGMT permission set.</span></span> <span data-ttu-id="9f613-107">If you are an administrator, you can assign user groups and permissions to other users in your company.</span><span class="sxs-lookup"><span data-stu-id="9f613-107">If you are an administrator, you can assign user groups and permissions to other users in your company.</span></span><br /><br />
<span data-ttu-id="9f613-108">To use the functionality that is provided by an extension, such as opening pages, running reports, selecting actions, and so on, you must be assigned the permission sets that are installed as part of the extension.</span><span class="sxs-lookup"><span data-stu-id="9f613-108">To use the functionality that is provided by an extension, such as opening pages, running reports, selecting actions, and so on, you must be assigned the permission sets that are installed as part of the extension.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="9f613-109">The upload of per-tenant extensions and the installation of AppSource extensions is not supported through the **Extension Management** page for on-premise installations.</span><span class="sxs-lookup"><span data-stu-id="9f613-109">The upload of per-tenant extensions and the installation of AppSource extensions is not supported through the **Extension Management** page for on-premise installations.</span></span>

<span data-ttu-id="9f613-110">When you first launch [!INCLUDE[d365fin](includes/d365fin_md.md)], some extensions are already installed for you.</span><span class="sxs-lookup"><span data-stu-id="9f613-110">When you first launch [!INCLUDE[d365fin](includes/d365fin_md.md)], some extensions are already installed for you.</span></span> <span data-ttu-id="9f613-111">Over time, more extensions will be made available to you, and you can then choose if you want to use the extension or not.</span><span class="sxs-lookup"><span data-stu-id="9f613-111">Over time, more extensions will be made available to you, and you can then choose if you want to use the extension or not.</span></span>

<span data-ttu-id="9f613-112">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="9f613-112">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span></span> <span data-ttu-id="9f613-113">This extension is installed by default.</span><span class="sxs-lookup"><span data-stu-id="9f613-113">This extension is installed by default.</span></span>
<span data-ttu-id="9f613-114">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span><span class="sxs-lookup"><span data-stu-id="9f613-114">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span></span>  

<span data-ttu-id="9f613-115">You manage the extensions on the **Extension Management** page.</span><span class="sxs-lookup"><span data-stu-id="9f613-115">You manage the extensions on the **Extension Management** page.</span></span> <span data-ttu-id="9f613-116">You can access this page from Home.</span><span class="sxs-lookup"><span data-stu-id="9f613-116">You can access this page from Home.</span></span> <span data-ttu-id="9f613-117">Alternatively, choose the **Search for Page or Report** icon ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") in the top right corner, enter **Extension**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="9f613-117">Alternatively, choose the **Search for Page or Report** icon ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") in the top right corner, enter **Extension**, and then choose the related link.</span></span> <span data-ttu-id="9f613-118">For more information, see [Installing and Uninstalling Extensions](ui-extensions-install-uninstall.md).</span><span class="sxs-lookup"><span data-stu-id="9f613-118">For more information, see [Installing and Uninstalling Extensions](ui-extensions-install-uninstall.md).</span></span>

> [!NOTE]  
> <span data-ttu-id="9f613-119">If you think you should have access to an extension but you cannot find its functionality, check the **Extension Management** page - if the extension is not listed there, you can install it as described in the following section.</span><span class="sxs-lookup"><span data-stu-id="9f613-119">If you think you should have access to an extension but you cannot find its functionality, check the **Extension Management** page - if the extension is not listed there, you can install it as described in the following section.</span></span>  

> [!NOTE]  
> <span data-ttu-id="9f613-120">New extensions are not available in AppSource immediately after we announce an update.</span><span class="sxs-lookup"><span data-stu-id="9f613-120">New extensions are not available in AppSource immediately after we announce an update.</span></span> <span data-ttu-id="9f613-121">You can keep an eye out for the extensions at  [AppSource.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2081646).</span><span class="sxs-lookup"><span data-stu-id="9f613-121">You can keep an eye out for the extensions at  [AppSource.microsoft.com](https://go.microsoft.com/fwlink/?linkid=2081646).</span></span>

## <a name="see-also"></a><span data-ttu-id="9f613-122">See Also</span><span class="sxs-lookup"><span data-stu-id="9f613-122">See Also</span></span>

[<span data-ttu-id="9f613-123">Extending Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="9f613-123">Extending Dynamics 365 Business Central</span></span>](about-develop-extensions.md)  
[<span data-ttu-id="9f613-124">Business Central Extensions by Other Providers</span><span class="sxs-lookup"><span data-stu-id="9f613-124">Business Central Extensions by Other Providers</span></span>](ui-extensions-other.md)  
[<span data-ttu-id="9f613-125">Set Up the Envestnet Yodlee Bank Feeds Service</span><span class="sxs-lookup"><span data-stu-id="9f613-125">Set Up the Envestnet Yodlee Bank Feeds Service</span></span>](bank-how-setup-bank-statement-service.md)  
[<span data-ttu-id="9f613-126">Enable Customer Payment Through PayPal</span><span class="sxs-lookup"><span data-stu-id="9f613-126">Enable Customer Payment Through PayPal</span></span>](sales-how-enable-payment-service-extensions.md)  
[<span data-ttu-id="9f613-127">Migrating Business Data from Other Finance Systems</span><span class="sxs-lookup"><span data-stu-id="9f613-127">Migrating Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
[<span data-ttu-id="9f613-128">Setting Up the GetAddress.io UK Postcode extension</span><span class="sxs-lookup"><span data-stu-id="9f613-128">Setting Up the GetAddress.io UK Postal Code extension</span></span>](LocalFunctionality/UnitedKingdom/uk-setup-postal-code-service.md)  
<span data-ttu-id="9f613-129">[[!INCLUDE[d365fin](includes/d365fin_md.md)] Extensions by Other Providers](ui-extensions-other.md)</span><span class="sxs-lookup"><span data-stu-id="9f613-129">[[!INCLUDE[d365fin](includes/d365fin_md.md)] Extensions by Other Providers](ui-extensions-other.md)</span></span>  
[<span data-ttu-id="9f613-130">Getting Started</span><span class="sxs-lookup"><span data-stu-id="9f613-130">Getting Started</span></span>](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
