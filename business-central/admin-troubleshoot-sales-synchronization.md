---
title: Troubleshooting Synchronisation Errors | Microsoft Docs
description: Provides some guidance for identifying and resolving synchronisation errors.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2019
ms.author: bholtorf
ms.openlocfilehash: bb6d0837f91240eb31abc7c02895cf2da420bf7d
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/04/2019
ms.locfileid: "1726797"
---
# <a name="troubleshooting-synchronization-errors"></a><span data-ttu-id="34f7c-103">Troubleshooting Synchronisation Errors</span><span class="sxs-lookup"><span data-stu-id="34f7c-103">Troubleshooting Synchronization Errors</span></span>
<span data-ttu-id="34f7c-104">There are lots of moving parts involved in integrating [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[crm_md](includes/crm_md.md)], and sometimes things go wrong.</span><span class="sxs-lookup"><span data-stu-id="34f7c-104">There are lots of moving parts involved in integrating [!INCLUDE[d365fin](includes/d365fin_md.md)] with [!INCLUDE[crm_md](includes/crm_md.md)], and sometimes things go wrong.</span></span> <span data-ttu-id="34f7c-105">This topic points out some of the typical errors that occur and gives some pointers for how to fix them.</span><span class="sxs-lookup"><span data-stu-id="34f7c-105">This topic points out some of the typical errors that occur and gives some pointers for how to fix them.</span></span>

<span data-ttu-id="34f7c-106">Errors often occur either because of something that a user has done to coupled records or something is wrong with how the integration is set up.</span><span class="sxs-lookup"><span data-stu-id="34f7c-106">Errors often occur either because of something that a user has done to coupled records or something is wrong with how the integration is set up.</span></span> <span data-ttu-id="34f7c-107">For errors related to coupled records, users can resolve those themselves.</span><span class="sxs-lookup"><span data-stu-id="34f7c-107">For errors related to coupled records, users can resolve those themselves.</span></span> <span data-ttu-id="34f7c-108">These errors are caused by actions such as deleting a record in one, but not both, business apps and then synchronising.</span><span class="sxs-lookup"><span data-stu-id="34f7c-108">These errors are caused by actions such as deleting a record in one, but not both, business apps and then synchronizing.</span></span> <span data-ttu-id="34f7c-109">For more information, see [View the Status of a Synchronisation](admin-how-to-view-synchronization-status.md).</span><span class="sxs-lookup"><span data-stu-id="34f7c-109">For more information, see [View the Status of a Synchronization](admin-how-to-view-synchronization-status.md).</span></span>

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2097304]

<span data-ttu-id="34f7c-110">Errors that are related to how the integration is set up typically require an administrator's attention.</span><span class="sxs-lookup"><span data-stu-id="34f7c-110">Errors that are related to how the integration is set up typically require an administrator's attention.</span></span> <span data-ttu-id="34f7c-111">You can view these errors on the **Integration Synchronisation Errors** page.</span><span class="sxs-lookup"><span data-stu-id="34f7c-111">You can view these errors on the **Integration Synchronization Errors** page.</span></span> <span data-ttu-id="34f7c-112">Examples of some typical issues include:</span><span class="sxs-lookup"><span data-stu-id="34f7c-112">Examples of some typical issues include:</span></span>  
  
* <span data-ttu-id="34f7c-113">The permissions and roles assigned to users are not correct.</span><span class="sxs-lookup"><span data-stu-id="34f7c-113">The permissions and roles assigned to users are not correct.</span></span>  
* <span data-ttu-id="34f7c-114">The administrator account was specified as the integration user.</span><span class="sxs-lookup"><span data-stu-id="34f7c-114">The administrator account was specified as the integration user.</span></span>  
* <span data-ttu-id="34f7c-115">The integration user’s password is set to require a change when the user signs in.</span><span class="sxs-lookup"><span data-stu-id="34f7c-115">The integration user’s password is set to require a change when the user signs in.</span></span>  
* <span data-ttu-id="34f7c-116">The exchange rates for currencies are not specified in one or the other app.</span><span class="sxs-lookup"><span data-stu-id="34f7c-116">The exchange rates for currencies are not specified in one or the other app.</span></span>  
  
<span data-ttu-id="34f7c-117">You must manually resolve the errors, but there are a few ways in which the page helps you.</span><span class="sxs-lookup"><span data-stu-id="34f7c-117">You must manually resolve the errors, but there are a few ways in which the page helps you.</span></span> <span data-ttu-id="34f7c-118">For example:</span><span class="sxs-lookup"><span data-stu-id="34f7c-118">For example:</span></span>  

* <span data-ttu-id="34f7c-119">The **Source** and **Destination** fields may contain links to the record where the error was found.</span><span class="sxs-lookup"><span data-stu-id="34f7c-119">The **Source** and **Destination** fields may contain links to the record where the error was found.</span></span> <span data-ttu-id="34f7c-120">Click the link to open the record and investigate the error.</span><span class="sxs-lookup"><span data-stu-id="34f7c-120">Click the link to open the record and investigate the error.</span></span>  
* <span data-ttu-id="34f7c-121">The **Delete Entries Older than 7 Days** and the **Delete All Entries** actions will clean up the list.</span><span class="sxs-lookup"><span data-stu-id="34f7c-121">The **Delete Entries Older than 7 Days** and the **Delete All Entries** actions will clean up the list.</span></span> <span data-ttu-id="34f7c-122">Typically, you use these actions after you have resolved the cause of an error that affects many records.</span><span class="sxs-lookup"><span data-stu-id="34f7c-122">Typically, you use these actions after you have resolved the cause of an error that affects many records.</span></span> <span data-ttu-id="34f7c-123">Use caution, however.</span><span class="sxs-lookup"><span data-stu-id="34f7c-123">Use caution, however.</span></span> <span data-ttu-id="34f7c-124">These actions might delete errors that are still relevant.</span><span class="sxs-lookup"><span data-stu-id="34f7c-124">These actions might delete errors that are still relevant.</span></span>

## <a name="see-also"></a><span data-ttu-id="34f7c-125">See Also</span><span class="sxs-lookup"><span data-stu-id="34f7c-125">See Also</span></span>
<span data-ttu-id="34f7c-126">[Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)</span><span class="sxs-lookup"><span data-stu-id="34f7c-126">[Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)</span></span>  
<span data-ttu-id="34f7c-127">[Setting Up User Accounts for Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)</span><span class="sxs-lookup"><span data-stu-id="34f7c-127">[Setting Up User Accounts for Integrating with [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)</span></span>  
<span data-ttu-id="34f7c-128">[Set Up a Connection to [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)</span><span class="sxs-lookup"><span data-stu-id="34f7c-128">[Set Up a Connection to [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)</span></span>  
[<span data-ttu-id="34f7c-129">Couple and Synchronise Records Manually</span><span class="sxs-lookup"><span data-stu-id="34f7c-129">Couple and Synchronize Records Manually</span></span>](admin-how-to-couple-and-synchronize-records-manually.md)  
[<span data-ttu-id="34f7c-130">View the Status of a Synchronisation</span><span class="sxs-lookup"><span data-stu-id="34f7c-130">View the Status of a Synchronization</span></span>](admin-how-to-view-synchronization-status.md)  