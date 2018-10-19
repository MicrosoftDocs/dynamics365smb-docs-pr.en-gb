---
title: Manage users and roles | Microsoft Docs
description: Learn how to manage users and Role Centres in Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, users
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 1a94d023424c6eceb93af6e9ca89a90a3a94e996
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="understanding-users-profiles-and-role-centers"></a><span data-ttu-id="de2be-103">Understanding Users, Profiles, and Role Centres</span><span class="sxs-lookup"><span data-stu-id="de2be-103">Understanding Users, Profiles, and Role Centers</span></span>

<span data-ttu-id="de2be-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span><span class="sxs-lookup"><span data-stu-id="de2be-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], users are added by an administrator who also gives users access to the areas of [!INCLUDE[d365fin](includes/d365fin_md.md)] that they need in their work.</span></span>  

<span data-ttu-id="de2be-105">Access to functionality is managed through *user groups* and *profiles*.</span><span class="sxs-lookup"><span data-stu-id="de2be-105">Access to functionality is managed through *user groups* and *profiles*.</span></span> <span data-ttu-id="de2be-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span><span class="sxs-lookup"><span data-stu-id="de2be-106">As an administrator, you can add and remove users as part of your [!INCLUDE[d365fin](includes/d365fin_md.md)] subscription, and you can assign users permissions through user groups.</span></span>  

## <a name="adding-users"></a><span data-ttu-id="de2be-107">Adding Users</span><span class="sxs-lookup"><span data-stu-id="de2be-107">Adding Users</span></span>

<span data-ttu-id="de2be-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Centre.</span><span class="sxs-lookup"><span data-stu-id="de2be-108">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)] online, your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="de2be-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span><span class="sxs-lookup"><span data-stu-id="de2be-109">For more information, see [Add Users to Office 365 for business](https://aka.ms/CreateOffice365Users).</span></span>

<span data-ttu-id="de2be-110">Then, the administrator can assign permissions to each user and groups of users.</span><span class="sxs-lookup"><span data-stu-id="de2be-110">Then, the administrator can assign permissions to each user and groups of users.</span></span> <span data-ttu-id="de2be-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="de2be-111">For more information, see [Managing Users and Permissions](ui-how-users-permissions.md).</span></span>  

### <a name="users-of-on-premises-deployments"></a><span data-ttu-id="de2be-112">Users of on-premises deployments</span><span class="sxs-lookup"><span data-stu-id="de2be-112">Users of on-premises deployments</span></span>

<span data-ttu-id="de2be-113">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorisation mechanisms for users.</span><span class="sxs-lookup"><span data-stu-id="de2be-113">For on-premises deployments of [!INCLUDE[d365fin](includes/d365fin_md.md)], the administrator can choose between different credential authorization mechanisms for users.</span></span> <span data-ttu-id="de2be-114">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span><span class="sxs-lookup"><span data-stu-id="de2be-114">Then, when you create a user, you provide different information depending on the credential type that you are using in the specific [!INCLUDE[server](includes/server.md)] instance.</span></span> <span data-ttu-id="de2be-115">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="de2be-115">For more information, see the [Authentication and Credential Types](/dynamics365/business-central/dev-itpro/administration/users-credential-types) in the Administration section of the developer and ITPro content for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="profiles"></a><span data-ttu-id="de2be-116">Profiles</span><span class="sxs-lookup"><span data-stu-id="de2be-116">Profiles</span></span>

<span data-ttu-id="de2be-117">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Centre*.</span><span class="sxs-lookup"><span data-stu-id="de2be-117">The people in your company who have access to [!INCLUDE[d365fin](includes/d365fin_md.md)] are all assigned a *profile* that gives them access to a *Role Center*.</span></span>

<span data-ttu-id="de2be-118">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center.</span><span class="sxs-lookup"><span data-stu-id="de2be-118">Profiles are collections of [!INCLUDE[d365fin](includes/d365fin_md.md)] users who share the same Role Center.</span></span> <span data-ttu-id="de2be-119">A Role Centre is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span><span class="sxs-lookup"><span data-stu-id="de2be-119">A Role Center is the entry point and home page for [!INCLUDE[d365fin](includes/d365fin_md.md)] that gives you quick access to your most important tasks and displays various insights and key performance indicators (KPIs) about your work.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="de2be-120">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span><span class="sxs-lookup"><span data-stu-id="de2be-120">In the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)] online, you cannot add, edit, or delete profiles.</span></span>  

## <a name="configuration-and-personalization"></a><span data-ttu-id="de2be-121">Configuration and Personalisation</span><span class="sxs-lookup"><span data-stu-id="de2be-121">Configuration and Personalization</span></span>
<!--The concept of UI customization in [!INCLUDE[d365fin](includes/d365fin_md.md)] is divided in two:  

-   Configuration, performed by the administrator  

-   Personalization, performed by users  

The administrator configures the user interface for multiple users by customizing the user interface for a profile that the users are assigned to.  -->
<span data-ttu-id="de2be-122">Users personalise the user interface of their personal version by customising the user interface under their own user logon.</span><span class="sxs-lookup"><span data-stu-id="de2be-122">Users personalize the user interface of their personal version by customizing the user interface under their own user logon.</span></span> <span data-ttu-id="de2be-123">This personalisation can be deleted by the administrator.</span><span class="sxs-lookup"><span data-stu-id="de2be-123">This personalization can be deleted by the administrator.</span></span> <span data-ttu-id="de2be-124">For more information, see [Personalising Your Workspace](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="de2be-124">For more information, see [Personalizing Your Workspace](ui-personalization-user.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="de2be-125">See Also</span><span class="sxs-lookup"><span data-stu-id="de2be-125">See Also</span></span>  
[<span data-ttu-id="de2be-126">Managing Users and Permissions</span><span class="sxs-lookup"><span data-stu-id="de2be-126">Managing Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="de2be-127">Managing Personalisation as an Administrator</span><span class="sxs-lookup"><span data-stu-id="de2be-127">Managing Personalization as an Administrator</span></span>](ui-personalization-manage.md)  
[<span data-ttu-id="de2be-128">Personalising Your Workspace</span><span class="sxs-lookup"><span data-stu-id="de2be-128">Personalizing Your Workspace</span></span>](ui-personalization-user.md)  

