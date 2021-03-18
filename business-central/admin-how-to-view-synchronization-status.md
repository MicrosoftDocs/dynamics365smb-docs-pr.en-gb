---
title: View the Status of Synchronisation Jobs | Microsoft Docs
description: Learn how to view the status after synchronising coupled records.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: a54ce7805deafa5d67c3e25b89606a1a40634ad6
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5378155"
---
# <a name="view-the-status-of-synchronization-jobs"></a><span data-ttu-id="ea854-103">View the Status of Synchronisation Jobs</span><span class="sxs-lookup"><span data-stu-id="ea854-103">View the Status of Synchronization Jobs</span></span>
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

<span data-ttu-id="ea854-104">Use the **Coupled Data Synchronisation Errors** page to view the status of synchronisation jobs that have been run for coupled records in a Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)] integrations.</span><span class="sxs-lookup"><span data-stu-id="ea854-104">Use the **Coupled Data Synchronization Errors** page to view the status of synchronization jobs that have been run for coupled records in a Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)] integrations.</span></span> <span data-ttu-id="ea854-105">This includes jobs that were run from the job queue and manual synchronisation jobs that ran on records from [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ea854-105">This includes jobs that were run from the job queue and manual synchronization jobs that ran on records from [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="ea854-106">For example, viewing their status is helpful when troubleshooting because it gives you access to details about errors related to coupled records.</span><span class="sxs-lookup"><span data-stu-id="ea854-106">For example, viewing their status is helpful when troubleshooting because it gives you access to details about errors related to coupled records.</span></span> <span data-ttu-id="ea854-107">Typically, these types of errors are caused by user actions, for example, when:</span><span class="sxs-lookup"><span data-stu-id="ea854-107">Typically, these types of errors are caused by user actions, for example, when:</span></span>  

* <span data-ttu-id="ea854-108">Two people made a change to the same data in both business apps.</span><span class="sxs-lookup"><span data-stu-id="ea854-108">Two people made a change to the same data in both business apps.</span></span>
* <span data-ttu-id="ea854-109">Someone deleted data in one of the apps, but not both.</span><span class="sxs-lookup"><span data-stu-id="ea854-109">Someone deleted data in one of the apps, but not both.</span></span>

> [!Note]
> <span data-ttu-id="ea854-110">The **Coupled Data Synchronisation Errors** page shows information about jobs related to coupled records.</span><span class="sxs-lookup"><span data-stu-id="ea854-110">The **Coupled Data Synchronization Errors** page shows information about jobs related to coupled records.</span></span> <span data-ttu-id="ea854-111">If you resolve all of the errors but records are still not synchronising, it might have something to do with a setting for the integration.</span><span class="sxs-lookup"><span data-stu-id="ea854-111">If you resolve all of the errors but records are still not synchronizing, it might have something to do with a setting for the integration.</span></span> <span data-ttu-id="ea854-112">Typically, your administrator will need to resolve those types of errors.</span><span class="sxs-lookup"><span data-stu-id="ea854-112">Typically, your administrator will need to resolve those types of errors.</span></span>   

<!--

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098171]

-->

## <a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a><span data-ttu-id="ea854-113">To view and resolve synchronisation errors for coupled records</span><span class="sxs-lookup"><span data-stu-id="ea854-113">To view and resolve synchronization errors for coupled records</span></span>
1. <span data-ttu-id="ea854-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronisation Errors**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ea854-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Coupled Data Synchronization Errors**, and then choose the related link.</span></span>
2. <span data-ttu-id="ea854-115">The **Coupled Data Synchronisation Errors** page shows issues that occurred when you synchronised coupled records.</span><span class="sxs-lookup"><span data-stu-id="ea854-115">The **Coupled Data Synchronization Errors** page shows issues that occurred when you synchronized coupled records.</span></span> <span data-ttu-id="ea854-116">The following table includes actions that you can use to resolve issues one by one:</span><span class="sxs-lookup"><span data-stu-id="ea854-116">The following table includes actions that you can use to resolve issues one by one:</span></span>

|<span data-ttu-id="ea854-117">Action</span><span class="sxs-lookup"><span data-stu-id="ea854-117">Action</span></span>|<span data-ttu-id="ea854-118">Description</span><span class="sxs-lookup"><span data-stu-id="ea854-118">Description</span></span>|
|----|----|
|<span data-ttu-id="ea854-119">**Remove Coupling**</span><span class="sxs-lookup"><span data-stu-id="ea854-119">**Remove Coupling**</span></span>|<span data-ttu-id="ea854-120">Uncouples the records and they will no longer synchronise.</span><span class="sxs-lookup"><span data-stu-id="ea854-120">Uncouples the records and they will no longer synchronize.</span></span> <span data-ttu-id="ea854-121">To restart the synchronisation you must couple them again.</span><span class="sxs-lookup"><span data-stu-id="ea854-121">To restart the synchronization you must couple them again.</span></span> |
|<span data-ttu-id="ea854-122">**Retry** and **Retry All**</span><span class="sxs-lookup"><span data-stu-id="ea854-122">**Retry** and **Retry All**</span></span>|<span data-ttu-id="ea854-123">For each record where an error is found, synchronisation is skipped unless you fix the issue.</span><span class="sxs-lookup"><span data-stu-id="ea854-123">For each record where an error is found, synchronization is skipped unless you fix the issue.</span></span> <span data-ttu-id="ea854-124">Retry will include the selected record in the next synchronisation and **Retry All** includes all of the records.</span><span class="sxs-lookup"><span data-stu-id="ea854-124">Retry will include the selected record in the next synchronization, and **Retry All** includes all of the records.</span></span>|
|<span data-ttu-id="ea854-125">**Synchronise**</span><span class="sxs-lookup"><span data-stu-id="ea854-125">**Synchronize**</span></span>|<span data-ttu-id="ea854-126">The app will try to resolve a conflict where data was changed in both business apps.</span><span class="sxs-lookup"><span data-stu-id="ea854-126">The app will try to resolve a conflict where data was changed in both business apps.</span></span> <span data-ttu-id="ea854-127">You can choose the data to use.</span><span class="sxs-lookup"><span data-stu-id="ea854-127">You can choose the data to use.</span></span>|
|<span data-ttu-id="ea854-128">**Restore Records** and **Delete Records**</span><span class="sxs-lookup"><span data-stu-id="ea854-128">**Restore Records** and **Delete Records**</span></span>|<span data-ttu-id="ea854-129">These are useful when a record was deleted in one of the business apps.</span><span class="sxs-lookup"><span data-stu-id="ea854-129">These are useful when a record was deleted in one of the business apps.</span></span> <span data-ttu-id="ea854-130">Delete Records deletes the record or row in the app where it still exists.</span><span class="sxs-lookup"><span data-stu-id="ea854-130">Delete Records deletes the record or row in the app where it still exists.</span></span> <span data-ttu-id="ea854-131">Restore Records recreates the record or row in the business app where it was deleted.</span><span class="sxs-lookup"><span data-stu-id="ea854-131">Restore Records recreates the record or row in the business app where it was deleted.</span></span>|

> [!NOTE]
> <span data-ttu-id="ea854-132">To reduce the number of conflicts you need to resolve, you can set up your integration table mappings to apply these actions automatically.</span><span class="sxs-lookup"><span data-stu-id="ea854-132">To reduce the number of conflicts you need to resolve, you can set up your integration table mappings to apply these actions automatically.</span></span> <span data-ttu-id="ea854-133">For more information, [Mapping Integration Tables](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).</span><span class="sxs-lookup"><span data-stu-id="ea854-133">For more information, [Mapping Integration Tables](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).</span></span>

## <a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a><span data-ttu-id="ea854-134">To view the synchronisation log for a specific (manually synchronised) record</span><span class="sxs-lookup"><span data-stu-id="ea854-134">To view the synchronization log for a specific (manually synchronized) record</span></span>
1. <span data-ttu-id="ea854-135">Open, for example, a customer, item or any other record that is synchronising data between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ea854-135">Open, for example, a customer, item or any other record that is synchronizing data between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span>
2. <span data-ttu-id="ea854-136">Choose the **Synchronisation Log** action to view the synchronisation log for a selected record.</span><span class="sxs-lookup"><span data-stu-id="ea854-136">Choose the **Synchronization Log** action to view the synchronization log for a selected record.</span></span> <span data-ttu-id="ea854-137">For example, a specific customer you synchronised manually.</span><span class="sxs-lookup"><span data-stu-id="ea854-137">For example, a specific customer you synchronized manually.</span></span>

## <a name="see-also"></a><span data-ttu-id="ea854-138">See Also</span><span class="sxs-lookup"><span data-stu-id="ea854-138">See Also</span></span>  
[<span data-ttu-id="ea854-139">Setting Up User Accounts for Integrating with Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="ea854-139">Setting Up User Accounts for Integrating with Dynamics 365 Sales</span></span>](admin-setting-up-integration-with-dynamics-sales.md)  
[<span data-ttu-id="ea854-140">Using Dynamics 365 Sales from Business Central</span><span class="sxs-lookup"><span data-stu-id="ea854-140">Using Dynamics 365 Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]