---
title: Administrative tasks in Dynamics 365 | Microsoft Docs
description: Some tasks in [!INCLUDE[d365fin](includes/d365fin_md.md)] requires central administration and setup. See what they are and learn what to do.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 09c3460a50088098bfe5c2fb633e76dccbac0794
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="setup-and-administration-in-dynamics-365-for-financials"></a><span data-ttu-id="48545-104">Setup and Administration in Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="48545-104">Setup and Administration in Dynamics 365 for Financials</span></span>
<span data-ttu-id="48545-105">Central administration tasks are usually performed by one role in the company.</span><span class="sxs-lookup"><span data-stu-id="48545-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="48545-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span><span class="sxs-lookup"><span data-stu-id="48545-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="48545-107">These tasks can include managing database synchronisation of job and email queues, setting up users, customising the user interface, and managing encryption keys.</span><span class="sxs-lookup"><span data-stu-id="48545-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="48545-108">Entering the correct setup values from the start is important to the success of any new business software.</span><span class="sxs-lookup"><span data-stu-id="48545-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="48545-109"> includes a number of setup guides that help you set up core data.</span><span class="sxs-lookup"><span data-stu-id="48545-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="48545-110">For more information, see [Setting Up Dynamics 365 for Financials](setup.md).</span><span class="sxs-lookup"><span data-stu-id="48545-110">For more information, see [Setting Up Dynamics 365 for Financials](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="48545-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span><span class="sxs-lookup"><span data-stu-id="48545-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="48545-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span><span class="sxs-lookup"><span data-stu-id="48545-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="48545-113">**To**</span><span class="sxs-lookup"><span data-stu-id="48545-113">**To**</span></span>|<span data-ttu-id="48545-114">**See**</span><span class="sxs-lookup"><span data-stu-id="48545-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="48545-115">Add users, manage permissions and access to data, assign roles.</span><span class="sxs-lookup"><span data-stu-id="48545-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="48545-116">Users, Profiles, and Role Centres in Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="48545-116">Users, Profiles, and Role Centers in Dynamics 365 for Financials</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="48545-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span><span class="sxs-lookup"><span data-stu-id="48545-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="48545-118">Logging Changes in Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="48545-118">Logging Changes in Dynamics 365 for Financials</span></span>](across-log-changes.md)|  
|<span data-ttu-id="48545-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span><span class="sxs-lookup"><span data-stu-id="48545-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="48545-120">Set Up Complex Application Areas Using Best Practices</span><span class="sxs-lookup"><span data-stu-id="48545-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="48545-121">Expose pages, codeunits, and queries as web services.</span><span class="sxs-lookup"><span data-stu-id="48545-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="48545-122">How to: Publish a Web Service</span><span class="sxs-lookup"><span data-stu-id="48545-122">How to: Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="48545-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="48545-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics 365 for Financials</span></span>| [<span data-ttu-id="48545-124">How to: Set Up Email Manually or Using the Assisted Setup</span><span class="sxs-lookup"><span data-stu-id="48545-124">How to: Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="48545-125">Enter single or recurring requests to run reports or codeunits.</span><span class="sxs-lookup"><span data-stu-id="48545-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="48545-126">Use Job Queues to Schedule Tasks</span><span class="sxs-lookup"><span data-stu-id="48545-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="48545-127">Manage, delete, or compress documents</span><span class="sxs-lookup"><span data-stu-id="48545-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="48545-128">Manage Documents</span><span class="sxs-lookup"><span data-stu-id="48545-128">Manage Documents</span></span>](admin-manage-documents.md)|  
|<span data-ttu-id="48545-129">Set up a new business unit using templates</span><span class="sxs-lookup"><span data-stu-id="48545-129">Set up a new business unit using templates</span></span>|<span data-ttu-id="48545-130">[Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md)</span><span class="sxs-lookup"><span data-stu-id="48545-130">[Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md)</span></span>|  

## <a name="see-also"></a><span data-ttu-id="48545-131">See Also</span><span class="sxs-lookup"><span data-stu-id="48545-131">See Also</span></span>
[<span data-ttu-id="48545-132">Overview of Business Functionality</span><span class="sxs-lookup"><span data-stu-id="48545-132">Overview of Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="48545-133">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="48545-133">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="48545-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="48545-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="48545-135">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="48545-135">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

