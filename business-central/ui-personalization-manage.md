---
title: Managing Personalisation as an Administrator in Business Central | Microsoft Docs
description: Learn how to customise the user interface to suit your way of working.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: 37cdf2d7dcc46b1286cbb7a5ad620547e364309e
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1250602"
---
# <a name="managing-personalization-as-an-administrator"></a><span data-ttu-id="0d00f-103">Managing Personalisation as an Administrator</span><span class="sxs-lookup"><span data-stu-id="0d00f-103">Managing Personalization as an Administrator</span></span>

<span data-ttu-id="0d00f-104">Users can personalise their workspace to suit their own preferences.</span><span class="sxs-lookup"><span data-stu-id="0d00f-104">Users can personalize their workspace to suit their own preferences.</span></span> <span data-ttu-id="0d00f-105">As an administrator, you control and manage personalisation by:</span><span class="sxs-lookup"><span data-stu-id="0d00f-105">As an administrator, you control and manage personalization by:</span></span>

-   <span data-ttu-id="0d00f-106">Enabling or disabling the personalisation feature for the entire the application (on-premises installation only).</span><span class="sxs-lookup"><span data-stu-id="0d00f-106">Enabling or disabling the personalization feature for the entire the application (on-premises installation only).</span></span>
-   <span data-ttu-id="0d00f-107">Enabling or disabling the personalisation feature for users of a specific profile.</span><span class="sxs-lookup"><span data-stu-id="0d00f-107">Enabling or disabling the personalization feature for users of a specific profile.</span></span>
-   <span data-ttu-id="0d00f-108">Clearing any page personalisations that users have made.</span><span class="sxs-lookup"><span data-stu-id="0d00f-108">Clearing any page personalizations that users have made.</span></span>

## <a name="EnablePersonalization"></a><span data-ttu-id="0d00f-109">To enable or disable personalisation (On-Premises Only)</span><span class="sxs-lookup"><span data-stu-id="0d00f-109">To enable or disable personalization (On-Premises Only)</span></span>

<span data-ttu-id="0d00f-110">By default, personalisation is not enabled in the client.</span><span class="sxs-lookup"><span data-stu-id="0d00f-110">By default, personalization is not enabled in the client.</span></span> <span data-ttu-id="0d00f-111">You enable or disable personalisation by modifying the configuration file (navsettings.json) of the Business Central Web Server instance that serves the clients.</span><span class="sxs-lookup"><span data-stu-id="0d00f-111">You enable or disable personalization by modifying the configuration file (navsettings.json) of the Business Central Web Server instance that serves the clients.</span></span>

1. <span data-ttu-id="0d00f-112">To enable personalisation, add the following line in the navsettings.json file:</span><span class="sxs-lookup"><span data-stu-id="0d00f-112">To enable personalization, add the following line in the navsettings.json file:</span></span>

    ```
    "PersonalizationEnabled": "true"
    ```

    <span data-ttu-id="0d00f-113">To disable personalisation, remove this line or change it to:</span><span class="sxs-lookup"><span data-stu-id="0d00f-113">To disable personalization, remove this line or change it to:</span></span>

    ```
    "PersonalizationEnabled": "false"
    ```

    <span data-ttu-id="0d00f-114">For more information about how to modify the navsettings.json file, see [Modify the navsettings.json file directly](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-web-server?branch=master#Settings).</span><span class="sxs-lookup"><span data-stu-id="0d00f-114">For more information about how to modify the navsettings.json file, see [Modify the navsettings.json file directly](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-web-server?branch=master#Settings).</span></span>

2. <span data-ttu-id="0d00f-115">Generate and download the application symbols.</span><span class="sxs-lookup"><span data-stu-id="0d00f-115">Generate and download the application symbols.</span></span>

    <span data-ttu-id="0d00f-116">This step is optional, and not required to enable personalisation.</span><span class="sxs-lookup"><span data-stu-id="0d00f-116">This step is optional, and not required to enable personalization.</span></span> <span data-ttu-id="0d00f-117">However, it ensures that new pages that are created by developers can be personalised.</span><span class="sxs-lookup"><span data-stu-id="0d00f-117">However, it ensures that new pages that are created by developers can be personalized.</span></span>

    1. <span data-ttu-id="0d00f-118">First, you generate the symbols by running finsql.exe with `generatesymbolreference` command.</span><span class="sxs-lookup"><span data-stu-id="0d00f-118">First, you generate the symbols by running finsql.exe with `generatesymbolreference` command.</span></span> <span data-ttu-id="0d00f-119">The finsql.exe file is located in the installation folder for the [!INCLUDE[server](includes/server.md)] and Dynamics NAV Development Environment (CSIDE).</span><span class="sxs-lookup"><span data-stu-id="0d00f-119">The finsql.exe file is located in the installation folder for the [!INCLUDE[server](includes/server.md)] and Dynamics NAV Development Environment (CSIDE).</span></span> <span data-ttu-id="0d00f-120">To generate the symbols, open a command prompt, change to the directory where the file is store, and the run the following command:</span><span class="sxs-lookup"><span data-stu-id="0d00f-120">To generate the symbols, open a command prompt, change to the directory where the file is store, and the run the following command:</span></span>

        ```
        finsql.exe Command=generatesymbolreference, Database="<Database Name>", ServerName=<SQL Server Name\<Server Instance>
        ```
    <span data-ttu-id="0d00f-121">For example:</span><span class="sxs-lookup"><span data-stu-id="0d00f-121">For example:</span></span>

        ```
        finsql.exe Command=generatesymbolreference, Database="Demo Database BC", ServerName=MySQLServer\BCDEMO
        ```

    <span data-ttu-id="0d00f-122">For more information, see [Running C/SIDE and AL Side-by-Side](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-running-cside-and-al-side-by-side).</span><span class="sxs-lookup"><span data-stu-id="0d00f-122">For more information, see [Running C/SIDE and AL Side-by-Side](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-running-cside-and-al-side-by-side).</span></span>

    2. <span data-ttu-id="0d00f-123">Configure [!INCLUDE[nav_server_md](includes/nav_server_md.md)] instance to **Enable loading application symbol references at server startup** (EnableSymbolLoadingAtServerStartup).</span><span class="sxs-lookup"><span data-stu-id="0d00f-123">Configure [!INCLUDE[nav_server_md](includes/nav_server_md.md)] instance to **Enable loading application symbol references at server startup** (EnableSymbolLoadingAtServerStartup).</span></span> <span data-ttu-id="0d00f-124">For more information, see [Configuring Business Central Server](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-server-instance#development-settings).</span><span class="sxs-lookup"><span data-stu-id="0d00f-124">For more information, see [Configuring Business Central Server](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configure-server-instance#development-settings).</span></span>

## <a name="to-disable-personalization-for-a-profile"></a><span data-ttu-id="0d00f-125">To disable personalisation for a profile</span><span class="sxs-lookup"><span data-stu-id="0d00f-125">To disable personalization for a profile</span></span>

<span data-ttu-id="0d00f-126">You can prevent all users that belong to a specific profile from being able to personalise their pages.</span><span class="sxs-lookup"><span data-stu-id="0d00f-126">You can prevent all users that belong to a specific profile from being able to personalize their pages.</span></span>

1. <span data-ttu-id="0d00f-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d00f-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Profiles**, and then choose the related link.</span></span>
2. <span data-ttu-id="0d00f-128">Select the profile in the list that you want to modify.</span><span class="sxs-lookup"><span data-stu-id="0d00f-128">Select the profile in the list that you want to modify.</span></span>
3. <span data-ttu-id="0d00f-129">Select the **Disable personalisation** check box, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="0d00f-129">Select the **Disable personalization** check box, and then choose the **OK** button.</span></span>

## <a name="to-clear-user-personalizations"></a><span data-ttu-id="0d00f-130">To clear user personalisations</span><span class="sxs-lookup"><span data-stu-id="0d00f-130">To clear user personalizations</span></span>

<span data-ttu-id="0d00f-131">Clearing page personalisation changes the page back to its original layout before any personalisation was made.</span><span class="sxs-lookup"><span data-stu-id="0d00f-131">Clearing page personalization changes the page back to its original layout before any personalization was made.</span></span> <span data-ttu-id="0d00f-132">There are two ways to clear the personalisations that users have made to pages: using the **Delete User Personalisation** page and using the **User Personalisation Card** page.</span><span class="sxs-lookup"><span data-stu-id="0d00f-132">There are two ways to clear the personalizations that users have made to pages: using the **Delete User Personalization** page and using the **User Personalization Card** page.</span></span>

### <a name="to-clear-user-personalizations-by-using-the-delete-user-personalization-page"></a><span data-ttu-id="0d00f-133">To clear user personalisations by using the Delete User Personalisation page</span><span class="sxs-lookup"><span data-stu-id="0d00f-133">To clear user personalizations by using the Delete User Personalization page</span></span>

<span data-ttu-id="0d00f-134">The **Delete User Personalisation** page enables you to clear personalisations on a per-page basis for each user individually.</span><span class="sxs-lookup"><span data-stu-id="0d00f-134">The **Delete User Personalization** page enables you to clear personalizations on a per-page basis for each user individually.</span></span>

1. <span data-ttu-id="0d00f-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete User Personalisation**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d00f-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="0d00f-136">The page lists all the pages that have been personalised and the user it belongs to.</span><span class="sxs-lookup"><span data-stu-id="0d00f-136">The page lists all the pages that have been personalized and the user it belongs to.</span></span>

    >[!NOTE]
    > <span data-ttu-id="0d00f-137">A check mark in the **Legacy Personalisation** columns indicates that the personalisation was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalisation different than it does now.</span><span class="sxs-lookup"><span data-stu-id="0d00f-137">A check mark in the **Legacy Personalization** columns indicates that the personalization was done in an older version of [!INCLUDE[d365fin](includes/d365fin_md.md)], which handled personalization different than it does now.</span></span> <span data-ttu-id="0d00f-138">Users who try to personalise these pages are locked from doing so unless they choose to unlock the page.</span><span class="sxs-lookup"><span data-stu-id="0d00f-138">Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.</span></span> <span data-ttu-id="0d00f-139">For more information, see [Why a page is locked from personalising](ui-personalization-locked.md).</span><span class="sxs-lookup"><span data-stu-id="0d00f-139">For more information, see [Why a page is locked from personalizing](ui-personalization-locked.md).</span></span>

2. <span data-ttu-id="0d00f-140">Select the entry that you want to delete, and then choose the **Delete** action.</span><span class="sxs-lookup"><span data-stu-id="0d00f-140">Select the entry that you want to delete, and then choose the **Delete** action.</span></span>

    <span data-ttu-id="0d00f-141">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="0d00f-141">The user will see the changes the next time they sign-in.</span></span>

### <a name="to-clear-user-personalizations-by-using-the-user-personalization-card-page"></a><span data-ttu-id="0d00f-142">To clear user personalisations by using the User Personalisation Card page</span><span class="sxs-lookup"><span data-stu-id="0d00f-142">To clear user personalizations by using the User Personalization Card page</span></span>

<span data-ttu-id="0d00f-143">The **User Personalisation Card** page enables you to clear the personalisation on all pages for specific user.</span><span class="sxs-lookup"><span data-stu-id="0d00f-143">The **User Personalization Card** page enables you to clear the personalization on all pages for specific user.</span></span> <span data-ttu-id="0d00f-144">This requires write permission to Table 2000000072 **Profile**.</span><span class="sxs-lookup"><span data-stu-id="0d00f-144">This requires write permission to Table 2000000072 **Profile**.</span></span>

1. <span data-ttu-id="0d00f-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Personalisation**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="0d00f-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **User Personalization**, and then choose the related link.</span></span>

    <span data-ttu-id="0d00f-146">The **User Personalisation** page lists all users who potentially have personalised pages.</span><span class="sxs-lookup"><span data-stu-id="0d00f-146">The **User Personalization** page lists all users who potentially have personalized pages.</span></span> <span data-ttu-id="0d00f-147">If you cannot find a user in the list, this means that they do not have any personalised pages.</span><span class="sxs-lookup"><span data-stu-id="0d00f-147">If you cannot find a user in the list, this means that they do not have any personalized pages.</span></span>

2. <span data-ttu-id="0d00f-148">Select the user from the list, and then choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="0d00f-148">Select the user from the list, and then choose the **Edit** action.</span></span>

3. <span data-ttu-id="0d00f-149">On the **Actions** tab, choose **Clear Personalised Pages**.</span><span class="sxs-lookup"><span data-stu-id="0d00f-149">On the **Actions** tab, choose **Clear Personalized Pages**.</span></span>

    <span data-ttu-id="0d00f-150">The user will see the changes the next time they sign-in.</span><span class="sxs-lookup"><span data-stu-id="0d00f-150">The user will see the changes the next time they sign-in.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d00f-151">See Also</span><span class="sxs-lookup"><span data-stu-id="0d00f-151">See Also</span></span>
[<span data-ttu-id="0d00f-152">Personalising Your Workspace</span><span class="sxs-lookup"><span data-stu-id="0d00f-152">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
<span data-ttu-id="0d00f-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0d00f-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="0d00f-154">Changing Basic Settings</span><span class="sxs-lookup"><span data-stu-id="0d00f-154">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="0d00f-155">Changing Which Features are Displayed</span><span class="sxs-lookup"><span data-stu-id="0d00f-155">Changing Which Features are Displayed</span></span>](ui-experiences.md)  
