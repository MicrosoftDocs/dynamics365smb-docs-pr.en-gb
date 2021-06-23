---
title: Create a sandbox environment
description: Create an environment for exploring, learning, demoing, developing, and testing from inside Business Central.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sandbox, demo, develop
ms.date: 06/08/2021
ms.author: solsen
ms.openlocfilehash: a76ae33815b8e9368f45b72fd8703bfc47cbd079
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215635"
---
# <a name="creating-a-sandbox-environment-in-prod_short"></a><span data-ttu-id="c3b83-103">Creating a Sandbox Environment in [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="c3b83-103">Creating a Sandbox Environment in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

<span data-ttu-id="c3b83-104">With [!INCLUDE[prod_short](includes/prod_short.md)], you can easily create a safe environment where you can test, train, or troubleshoot without disturbing your company's work processes or business data.</span><span class="sxs-lookup"><span data-stu-id="c3b83-104">With [!INCLUDE[prod_short](includes/prod_short.md)], you can easily create a safe environment where you can test, train, or troubleshoot without disturbing your company's work processes or business data.</span></span> <span data-ttu-id="c3b83-105">Such a non-production environment is called a *sandbox*.</span><span class="sxs-lookup"><span data-stu-id="c3b83-105">Such a non-production environment is called a *sandbox*.</span></span> <span data-ttu-id="c3b83-106">Isolated from production, a sandbox environment is the place to safely explore, learn, demo, develop, and test the service without the risk of affecting the data and settings of your production environment.</span><span class="sxs-lookup"><span data-stu-id="c3b83-106">Isolated from production, a sandbox environment is the place to safely explore, learn, demo, develop, and test the service without the risk of affecting the data and settings of your production environment.</span></span>  

<span data-ttu-id="c3b83-107">Your administrator manages sandbox environments in the [administration centre](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json), but if you want to quickly test something, you can create a sandbox environment from inside [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="c3b83-107">Your administrator manages sandbox environments in the [administration center](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json), but if you want to quickly test something, you can create a sandbox environment from inside [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="c3b83-108">Once you're done, you can remove the sandbox, using the administration centre.</span><span class="sxs-lookup"><span data-stu-id="c3b83-108">Once you're done, you can remove the sandbox, using the administration center.</span></span>  

> [!NOTE]
> <span data-ttu-id="c3b83-109">Technically, sandbox environments are very different from production environments, even if your administrator creates a sandbox that includes production data.</span><span class="sxs-lookup"><span data-stu-id="c3b83-109">Technically, sandbox environments are very different from production environments, even if your administrator creates a sandbox that includes production data.</span></span> <span data-ttu-id="c3b83-110">You cannot use a sandbox for benchmarking, and you cannot request a database export, for example.</span><span class="sxs-lookup"><span data-stu-id="c3b83-110">You cannot use a sandbox for benchmarking, and you cannot request a database export, for example.</span></span> <span data-ttu-id="c3b83-111">If you want to create a sandbox for benchmarking, your administrator can create a dedicated environment in the administration centre.</span><span class="sxs-lookup"><span data-stu-id="c3b83-111">If you want to create a sandbox for benchmarking, your administrator can create a dedicated environment in the administration center.</span></span> <span data-ttu-id="c3b83-112">For more information, see [Production and Sandbox Environments](/dynamics365/business-central/dev-itpro/administration/environment-types).</span><span class="sxs-lookup"><span data-stu-id="c3b83-112">For more information, see [Production and Sandbox Environments](/dynamics365/business-central/dev-itpro/administration/environment-types).</span></span>

## <a name="to-create-a-sandbox-environment-in-your-prod_short"></a><span data-ttu-id="c3b83-113">To create a sandbox environment in your [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="c3b83-113">To create a sandbox environment in your [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

1. <span data-ttu-id="c3b83-114">Sign in to your production instance of [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="c3b83-114">Sign in to your production instance of [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

2. <span data-ttu-id="c3b83-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sandbox Environment**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c3b83-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sandbox Environment**, and then choose the related link.</span></span>
    <!-- ![Sandbox Environment Setup](./media/across-sandbox/sandbox-environment-setup.png) -->
3. <span data-ttu-id="c3b83-116">Choose the **Create** button.</span><span class="sxs-lookup"><span data-stu-id="c3b83-116">Choose the **Create** button.</span></span>  

    <span data-ttu-id="c3b83-117">Another tab with [!INCLUDE[prod_short](includes/prod_short.md)] opens where you can finish the setup of your sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="c3b83-117">Another tab with [!INCLUDE[prod_short](includes/prod_short.md)] opens where you can finish the setup of your sandbox environment.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="c3b83-118">If you have pop-up blocker enabled in your browser, change it to allow URLs from the \*.businesscentral.dynamics.com address.</span><span class="sxs-lookup"><span data-stu-id="c3b83-118">If you have pop-up blocker enabled in your browser, change it to allow URLs from the \*.businesscentral.dynamics.com address.</span></span>

<span data-ttu-id="c3b83-119">When the sandbox environment is ready, you will be redirected to sandbox environment's Welcome wizard.</span><span class="sxs-lookup"><span data-stu-id="c3b83-119">When the sandbox environment is ready, you will be redirected to sandbox environment's Welcome wizard.</span></span>
<!-- ![Sandbox Welcome Wizard](./media/across-sandbox/sandbox-wizard.png) -->

<span data-ttu-id="c3b83-120">You can choose the **Learn more** button to read about developer scenarios that you can try in a sandbox environment or choose the **Close** button to continue to the Role Centre of your [!INCLUDE[prod_short](includes/prod_short.md)] sandbox instance.</span><span class="sxs-lookup"><span data-stu-id="c3b83-120">You can choose the **Learn more** button to read about developer scenarios that you can try in a sandbox environment or choose the **Close** button to continue to the Role Center of your [!INCLUDE[prod_short](includes/prod_short.md)] sandbox instance.</span></span>

<span data-ttu-id="c3b83-121">At the top of the Role Centre, a notification appears to inform you that this is a sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="c3b83-121">At the top of the Role Center, a notification appears to inform you that this is a sandbox environment.</span></span> <span data-ttu-id="c3b83-122">You can also see the type of the environment in the title bar of the client.</span><span class="sxs-lookup"><span data-stu-id="c3b83-122">You can also see the type of the environment in the title bar of the client.</span></span>
    <!-- ![Sandbox RoleCenter Notification](./media/across-sandbox/sandbox-rolecenter-notification.png) -->

> [!NOTE]
> <span data-ttu-id="c3b83-123">A sandbox environment created in this way only contains the default demonstration data for the CRONUS company.</span><span class="sxs-lookup"><span data-stu-id="c3b83-123">A sandbox environment created in this way only contains the default demonstration data for the CRONUS company.</span></span> <span data-ttu-id="c3b83-124">No data is copied or otherwise transferred from the production environment.</span><span class="sxs-lookup"><span data-stu-id="c3b83-124">No data is copied or otherwise transferred from the production environment.</span></span>
>
> <span data-ttu-id="c3b83-125">Alternatively, create a sandbox environment based on production data.</span><span class="sxs-lookup"><span data-stu-id="c3b83-125">Alternatively, create a sandbox environment based on production data.</span></span> <span data-ttu-id="c3b83-126">You must do this through the administration centre.</span><span class="sxs-lookup"><span data-stu-id="c3b83-126">You must do this through the administration center.</span></span> <span data-ttu-id="c3b83-127">For more information, see [Managing Environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) in the developer and administration content.</span><span class="sxs-lookup"><span data-stu-id="c3b83-127">For more information, see [Managing Environments](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments) in the developer and administration content.</span></span>  

<!--To switch between your production and sandbox environments, you can use the Business Central app launcher.
    ![Sandbox Dynamics365 Menu](./media/across-sandbox/sandbox-dynamics365-menu.png) -->

<span data-ttu-id="c3b83-128">An administrator can limit or even block access for some users to the sandbox environment.</span><span class="sxs-lookup"><span data-stu-id="c3b83-128">An administrator can limit or even block access for some users to the sandbox environment.</span></span> <span data-ttu-id="c3b83-129">This can be done by using the standard security features of the product, such as the User card, user groups, and permission sets.</span><span class="sxs-lookup"><span data-stu-id="c3b83-129">This can be done by using the standard security features of the product, such as the User card, user groups, and permission sets.</span></span> <span data-ttu-id="c3b83-130">For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="c3b83-130">For more information, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>  

<!-- ![Sandbox Permission Sets](./media/across-sandbox/sandbox-permission-sets.png) -->

## <a name="advanced-functionality-in-the-sandbox-environment"></a><span data-ttu-id="c3b83-131">Advanced Functionality in the Sandbox Environment</span><span class="sxs-lookup"><span data-stu-id="c3b83-131">Advanced Functionality in the Sandbox Environment</span></span>

<span data-ttu-id="c3b83-132">The sandbox environment is not least useful because it includes a couple of handy features:</span><span class="sxs-lookup"><span data-stu-id="c3b83-132">The sandbox environment is not least useful because it includes a couple of handy features:</span></span>

* [<span data-ttu-id="c3b83-133">Advanced user experience</span><span class="sxs-lookup"><span data-stu-id="c3b83-133">Advanced user experience</span></span>](#advanced-user-experience)  
* [<span data-ttu-id="c3b83-134">Complete sample data</span><span class="sxs-lookup"><span data-stu-id="c3b83-134">Complete sample data</span></span>](#complete-sample-data)  
* [<span data-ttu-id="c3b83-135">Designer</span><span class="sxs-lookup"><span data-stu-id="c3b83-135">Designer</span></span>](#designer)  

### <a name="advanced-user-experience"></a><span data-ttu-id="c3b83-136">Advanced user experience</span><span class="sxs-lookup"><span data-stu-id="c3b83-136">Advanced user experience</span></span>

<span data-ttu-id="c3b83-137">It is possible to enable and try the full functionality of the standard version of [!INCLUDE[prod_short](includes/prod_short.md)] in a sandbox tenant by setting the **Experience** field on the **Company Information** page to *Premium*.</span><span class="sxs-lookup"><span data-stu-id="c3b83-137">It is possible to enable and try the full functionality of the standard version of [!INCLUDE[prod_short](includes/prod_short.md)] in a sandbox tenant by setting the **Experience** field on the **Company Information** page to *Premium*.</span></span> Find the **Company Information** page in the :::image type="content" source="media/ui-experience/settings_icon_small.png" alt-text="Settings icon"::: menu.  

<span data-ttu-id="c3b83-139">After you have enabled the *Premium* user experience, you get access to all the standard profiles (roles) and Role Centres in the standard version.</span><span class="sxs-lookup"><span data-stu-id="c3b83-139">After you have enabled the *Premium* user experience, you get access to all the standard profiles (roles) and Role Centers in the standard version.</span></span> <span data-ttu-id="c3b83-140">You can also create an evaluation company that is fully set up, including demonstration data and access to the advanced areas of the product.</span><span class="sxs-lookup"><span data-stu-id="c3b83-140">You can also create an evaluation company that is fully set up, including demonstration data and access to the advanced areas of the product.</span></span> <span data-ttu-id="c3b83-141">Alternatively, contact a reselling partner for a demonstration of the capabilities.</span><span class="sxs-lookup"><span data-stu-id="c3b83-141">Alternatively, contact a reselling partner for a demonstration of the capabilities.</span></span> <span data-ttu-id="c3b83-142">For more information, see [How do I find a reselling partner?](/dynamics365/business-central/across-faq.yml#findpartner).</span><span class="sxs-lookup"><span data-stu-id="c3b83-142">For more information, see [How do I find a reselling partner?](/dynamics365/business-central/across-faq.yml#findpartner).</span></span>  

### <a name="complete-sample-data"></a><span data-ttu-id="c3b83-143">Complete sample data</span><span class="sxs-lookup"><span data-stu-id="c3b83-143">Complete sample data</span></span>

<span data-ttu-id="c3b83-144">For situations where you need additional sample data, please talk to your reselling partner.</span><span class="sxs-lookup"><span data-stu-id="c3b83-144">For situations where you need additional sample data, please talk to your reselling partner.</span></span>
<!-- In the sandbox environment, you can also create a new company with the **Advanced Evaluation - Complete Sample Data** option so that you can take training or step through walkthroughs that require additional sample data, such as [Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations](walkthrough-receiving-and-putting-away-in-basic-warehousing.md).   -->

#### <a name="to-create-a-company-with-complete-sample-data-in-a-sandbox"></a><span data-ttu-id="c3b83-145">To create a company with complete sample data in a sandbox</span><span class="sxs-lookup"><span data-stu-id="c3b83-145">To create a company with complete sample data in a sandbox</span></span>

1. <span data-ttu-id="c3b83-146">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c3b83-146">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.</span></span>  
2. <span data-ttu-id="c3b83-147">Choose the **New** action, and then choose **Create New Company**.</span><span class="sxs-lookup"><span data-stu-id="c3b83-147">Choose the **New** action, and then choose **Create New Company**.</span></span>  
3. <span data-ttu-id="c3b83-148">In the **Assisted Setup for Creating a Company** page, choose **Next**.</span><span class="sxs-lookup"><span data-stu-id="c3b83-148">In the **Assisted Setup for Creating a Company** page, choose **Next**.</span></span>  
4. <span data-ttu-id="c3b83-149">Specify a name for the new company, and then, in the **Select the data and setup to get started** field, choose **Advanced Evaluation - Complete Sample Data**.</span><span class="sxs-lookup"><span data-stu-id="c3b83-149">Specify a name for the new company, and then, in the **Select the data and setup to get started** field, choose **Advanced Evaluation - Complete Sample Data**.</span></span>  
5. <span data-ttu-id="c3b83-150">Complete the rest of the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="c3b83-150">Complete the rest of the assisted setup guide.</span></span>  

<span data-ttu-id="c3b83-151">When the assisted setup guide completes, you can start exploring the new company with the complete sample data.</span><span class="sxs-lookup"><span data-stu-id="c3b83-151">When the assisted setup guide completes, you can start exploring the new company with the complete sample data.</span></span> <span data-ttu-id="c3b83-152">For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="c3b83-152">For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).</span></span>  

### <a name="designer"></a><span data-ttu-id="c3b83-153">Designer</span><span class="sxs-lookup"><span data-stu-id="c3b83-153">Designer</span></span>

<span data-ttu-id="c3b83-154">In a sandbox environment, you will find the **Designer** enabled.</span><span class="sxs-lookup"><span data-stu-id="c3b83-154">In a sandbox environment, you will find the **Designer** enabled.</span></span> <span data-ttu-id="c3b83-155">You can activate Designer by selecting the design icon ![Designer](./media/across-sandbox/sandbox-inclient-design-icon.png) on a page, or by choosing the **Design** menu item in the ![Settings](media/ui-experience/settings_icon_small.png) Settings menu.</span><span class="sxs-lookup"><span data-stu-id="c3b83-155">You can activate Designer by selecting the design icon ![Designer](./media/across-sandbox/sandbox-inclient-design-icon.png) on a page, or by choosing the **Design** menu item in the ![Settings](media/ui-experience/settings_icon_small.png) Settings menu.</span></span>  

<span data-ttu-id="c3b83-156">For more information, see [Using Designer](/dynamics365/business-central/dev-itpro/developer/devenv-inclient-designer) in the developer and admin content (in English only).</span><span class="sxs-lookup"><span data-stu-id="c3b83-156">For more information, see [Using Designer](/dynamics365/business-central/dev-itpro/developer/devenv-inclient-designer) in the developer and admin content (in English only).</span></span>  

<!-- ![In-client Designer](./media/across-sandbox/sandbox-inclient-designer.png) -->

## <a name="see-also"></a><span data-ttu-id="c3b83-157">See Also</span><span class="sxs-lookup"><span data-stu-id="c3b83-157">See Also</span></span>

<span data-ttu-id="c3b83-158">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c3b83-158">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="c3b83-159">[[!INCLUDE[prod_long](includes/prod_long.md)] Trials and Subscriptions](across-preview.md)</span><span class="sxs-lookup"><span data-stu-id="c3b83-159">[[!INCLUDE[prod_long](includes/prod_long.md)] Trials and Subscriptions](across-preview.md)</span></span>  
[<span data-ttu-id="c3b83-160">Managing Environments in the Business Central administration centre</span><span class="sxs-lookup"><span data-stu-id="c3b83-160">Managing Environments in the Business Central administration center</span></span>](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
