---
title: Manage users and roles | Microsoft Docs
description: Learn how to manage users and Role Centres in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: profiles, users
ms.date: 08/02/2019
ms.author: edupont
ms.openlocfilehash: 27a57490101195f8dc05cc39538260e7db5e46af
ms.sourcegitcommit: 5bcc5f95e450ee9a3d9f7a380e592a5e75c4185b
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 08/05/2019
ms.locfileid: "1858227"
---
# <a name="understanding-users-roles-and-profiles"></a><span data-ttu-id="93aa0-103">Understanding Users, Roles, and Profiles</span><span class="sxs-lookup"><span data-stu-id="93aa0-103">Understanding Users, Roles, and Profiles</span></span>

<span data-ttu-id="93aa0-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span><span class="sxs-lookup"><span data-stu-id="93aa0-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span></span>  

<span data-ttu-id="93aa0-105">Access to functionality is managed through *user groups* and *profiles (roles)*.</span><span class="sxs-lookup"><span data-stu-id="93aa0-105">Access to functionality is managed through *user groups* and *profiles (roles)*.</span></span> <span data-ttu-id="93aa0-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span><span class="sxs-lookup"><span data-stu-id="93aa0-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span></span>  

## <a name="adding-users"></a><span data-ttu-id="93aa0-107">Adding Users</span><span class="sxs-lookup"><span data-stu-id="93aa0-107">Adding Users</span></span>

<span data-ttu-id="93aa0-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Centre.</span><span class="sxs-lookup"><span data-stu-id="93aa0-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="93aa0-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span><span class="sxs-lookup"><span data-stu-id="93aa0-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span></span>

<span data-ttu-id="93aa0-110">Then, the administrator can assign permissions to each user and groups of users.</span><span class="sxs-lookup"><span data-stu-id="93aa0-110">Then, the administrator can assign permissions to each user and groups of users.</span></span> <span data-ttu-id="93aa0-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="93aa0-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>  

<span data-ttu-id="93aa0-112">The most powerful permissions that a user can have is the SUPER permission set.</span><span class="sxs-lookup"><span data-stu-id="93aa0-112">The most powerful permissions that a user can have is the SUPER permission set.</span></span> <span data-ttu-id="93aa0-113">Each company must have at least one user with this permission set, but it is a best practice to give each user permissions that match their work needs in [!INCLUDE[prodshort](includes/prodshort.md)] and not more than that.</span><span class="sxs-lookup"><span data-stu-id="93aa0-113">Each company must have at least one user with this permission set, but it is a best practice to give each user permissions that match their work needs in [!INCLUDE[prodshort](includes/prodshort.md)] and not more than that.</span></span> <span data-ttu-id="93aa0-114">This helps ensure that users only have access to data that is relevant to their work, for example.</span><span class="sxs-lookup"><span data-stu-id="93aa0-114">This helps ensure that users only have access to data that is relevant to their work, for example.</span></span>  

> [!TIP]
> <span data-ttu-id="93aa0-115">It's a best practice to make sure that the Office 365 administrator also has the SUPER permission set in [!INCLUDE[prodshort](includes/prodshort.md)] because that makes many administrative tasks easier, including setting up integration with other apps.</span><span class="sxs-lookup"><span data-stu-id="93aa0-115">It's a best practice to make sure that the Office 365 administrator also has the SUPER permission set in [!INCLUDE[prodshort](includes/prodshort.md)] because that makes many administrative tasks easier, including setting up integration with other apps.</span></span>

### <a name="users-of-on-premises-deployments"></a><span data-ttu-id="93aa0-116">Users of on-premises deployments</span><span class="sxs-lookup"><span data-stu-id="93aa0-116">Users of on-premises deployments</span></span>

<span data-ttu-id="93aa0-117">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorisation mechanisms for users.</span><span class="sxs-lookup"><span data-stu-id="93aa0-117">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorization mechanisms for users.</span></span> <span data-ttu-id="93aa0-118">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span><span class="sxs-lookup"><span data-stu-id="93aa0-118">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span></span> <span data-ttu-id="93aa0-119">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="93aa0-119">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="profiles-roles"></a><span data-ttu-id="93aa0-120">Profiles (Roles)</span><span class="sxs-lookup"><span data-stu-id="93aa0-120">Profiles (Roles)</span></span>

<span data-ttu-id="93aa0-121">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a role that gives them access to a *Role Centre*.</span><span class="sxs-lookup"><span data-stu-id="93aa0-121">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a role that gives them access to a *Role Center*.</span></span>

<span data-ttu-id="93aa0-122">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same role.</span><span class="sxs-lookup"><span data-stu-id="93aa0-122">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same role.</span></span> <span data-ttu-id="93aa0-123">A Role Centre is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span><span class="sxs-lookup"><span data-stu-id="93aa0-123">A Role Center is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="93aa0-124">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span><span class="sxs-lookup"><span data-stu-id="93aa0-124">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span></span>  

### <a name="CreateProfile"></a><span data-ttu-id="93aa0-125">To create a profile</span><span class="sxs-lookup"><span data-stu-id="93aa0-125">To create a profile</span></span>

1.  <span data-ttu-id="93aa0-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="93aa0-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="93aa0-127">On the **Profiles** page, choose the **New** action to open the **New Profile Card** page.</span><span class="sxs-lookup"><span data-stu-id="93aa0-127">On the **Profiles** page, choose the **New** action to open the **New Profile Card** page.</span></span>  

3.  <span data-ttu-id="93aa0-128">In the **Profile ID** field, enter a name that describes the intended role of the users.</span><span class="sxs-lookup"><span data-stu-id="93aa0-128">In the **Profile ID** field, enter a name that describes the intended role of the users.</span></span>  

4.  <span data-ttu-id="93aa0-129">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span><span class="sxs-lookup"><span data-stu-id="93aa0-129">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span></span>  

5.  <span data-ttu-id="93aa0-130">Set the **Role Centre ID** field to the Role Centre that you want to assign to the profile.</span><span class="sxs-lookup"><span data-stu-id="93aa0-130">Set the **Role Center ID** field to the Role Center that you want to assign to the profile.</span></span>  

<span data-ttu-id="93aa0-131">The procedure for modifying an existing profile is the same, except you select an existing profile on the **Profiles** page instead of choosing the **New** action.</span><span class="sxs-lookup"><span data-stu-id="93aa0-131">The procedure for modifying an existing profile is the same, except you select an existing profile on the **Profiles** page instead of choosing the **New** action.</span></span>  


### <a name="copy-a-profile"></a><span data-ttu-id="93aa0-132">Copy a profile</span><span class="sxs-lookup"><span data-stu-id="93aa0-132">Copy a profile</span></span>
<span data-ttu-id="93aa0-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span><span class="sxs-lookup"><span data-stu-id="93aa0-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span></span>

1.  <span data-ttu-id="93aa0-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span><span class="sxs-lookup"><span data-stu-id="93aa0-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span></span>

2.  <span data-ttu-id="93aa0-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span><span class="sxs-lookup"><span data-stu-id="93aa0-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span></span>

3.  <span data-ttu-id="93aa0-136">Set the **New Profile Scope** field to one of the following:</span><span class="sxs-lookup"><span data-stu-id="93aa0-136">Set the **New Profile Scope** field to one of the following:</span></span>

    - <span data-ttu-id="93aa0-137">**System** to make the new profile available to all tenant databases that use the application.</span><span class="sxs-lookup"><span data-stu-id="93aa0-137">**System** to make the new profile available to all tenant databases that use the application.</span></span>
    - <span data-ttu-id="93aa0-138">**Tenant** to make the new profile available to just the current tenant database.</span><span class="sxs-lookup"><span data-stu-id="93aa0-138">**Tenant** to make the new profile available to just the current tenant database.</span></span>
4. <span data-ttu-id="93aa0-139">Choose the **OK** button when done.</span><span class="sxs-lookup"><span data-stu-id="93aa0-139">Choose the **OK** button when done.</span></span>

### <a name="ExportImportProfile"></a><span data-ttu-id="93aa0-140">Export and import profiles</span><span class="sxs-lookup"><span data-stu-id="93aa0-140">Export and import profiles</span></span>

<span data-ttu-id="93aa0-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span><span class="sxs-lookup"><span data-stu-id="93aa0-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span></span> <span data-ttu-id="93aa0-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span><span class="sxs-lookup"><span data-stu-id="93aa0-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span></span> <span data-ttu-id="93aa0-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span><span class="sxs-lookup"><span data-stu-id="93aa0-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span></span> <span data-ttu-id="93aa0-144">Then, you can import the profile XML file into the other database.</span><span class="sxs-lookup"><span data-stu-id="93aa0-144">Then, you can import the profile XML file into the other database.</span></span>

-   <span data-ttu-id="93aa0-145">To export a profile, you can either choose the **Export Profiles** action from the **Profile List** or **Profile Card** page or you can search for and open the **Export Profiles** page.</span><span class="sxs-lookup"><span data-stu-id="93aa0-145">To export a profile, you can either choose the **Export Profiles** action from the **Profile List** or **Profile Card** page or you can search for and open the **Export Profiles** page.</span></span> <span data-ttu-id="93aa0-146">Save the XML file to a location on your computer or network.</span><span class="sxs-lookup"><span data-stu-id="93aa0-146">Save the XML file to a location on your computer or network.</span></span>

-   <span data-ttu-id="93aa0-147">To import a profile, you can either choose the **Import Profile** action from the **Profile List** page, or you can search for and open the **Import Profiles** page.</span><span class="sxs-lookup"><span data-stu-id="93aa0-147">To import a profile, you can either choose the **Import Profile** action from the **Profile List** page, or you can search for and open the **Import Profiles** page.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="93aa0-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span><span class="sxs-lookup"><span data-stu-id="93aa0-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span></span> <span data-ttu-id="93aa0-149">You must delete the existing profile before you can import the new profile.</span><span class="sxs-lookup"><span data-stu-id="93aa0-149">You must delete the existing profile before you can import the new profile.</span></span>


## <a name="configuration-and-personalization"></a><span data-ttu-id="93aa0-150">Configuration and Personalisation</span><span class="sxs-lookup"><span data-stu-id="93aa0-150">Configuration and Personalization</span></span>
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->

<span data-ttu-id="93aa0-151">Users personalise the user interface of their personal version by customising the user interface under their own user logon.</span><span class="sxs-lookup"><span data-stu-id="93aa0-151">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span></span> <span data-ttu-id="93aa0-152">This personalisation can be deleted by the administrator.</span><span class="sxs-lookup"><span data-stu-id="93aa0-152">This personalization can be deleted by the administrator.</span></span> <span data-ttu-id="93aa0-153">For more information, see [Personalising Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="93aa0-153">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="93aa0-154">See Also</span><span class="sxs-lookup"><span data-stu-id="93aa0-154">See Also</span></span>  
[<span data-ttu-id="93aa0-155">Managing Users and Permissions</span><span class="sxs-lookup"><span data-stu-id="93aa0-155">Managing Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="93aa0-156">Managing Personalisation as an Administrator</span><span class="sxs-lookup"><span data-stu-id="93aa0-156">Managing Personalization as an Administrator</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="93aa0-157">Personalising Your Workspace</span><span class="sxs-lookup"><span data-stu-id="93aa0-157">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  
