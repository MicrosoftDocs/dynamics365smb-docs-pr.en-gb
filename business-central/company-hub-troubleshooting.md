---
title: Troubleshooting your company hub
description: Learn how to work around any issues when you the company hub in Dynamics 365 Business Central to manage work across multiple companies.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, troubleshoot
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fc015058079e30b2db6989b246dc38498cd7a1f4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786519"
---
# <a name="troubleshooting-your-company-hub"></a><span data-ttu-id="9b518-103">Troubleshooting Your Company Hub</span><span class="sxs-lookup"><span data-stu-id="9b518-103">Troubleshooting Your Company Hub</span></span>

<span data-ttu-id="9b518-104">Adding companies to the company hub dashboard is easy enough, but this article addresses issues that you may have on the way.</span><span class="sxs-lookup"><span data-stu-id="9b518-104">Adding companies to the company hub dashboard is easy enough, but this article addresses issues that you may have on the way.</span></span>  

## <a name="check-errors"></a><span data-ttu-id="9b518-105">Check errors</span><span class="sxs-lookup"><span data-stu-id="9b518-105">Check errors</span></span>

<span data-ttu-id="9b518-106">Use the **Check Errors** action to view a list of recent errors.</span><span class="sxs-lookup"><span data-stu-id="9b518-106">Use the **Check Errors** action to view a list of recent errors.</span></span> <span data-ttu-id="9b518-107">You can see additional details for each error, and you can clean up the log by deleting older entries.</span><span class="sxs-lookup"><span data-stu-id="9b518-107">You can see additional details for each error, and you can clean up the log by deleting older entries.</span></span>  

## <a name="connection-failed"></a><span data-ttu-id="9b518-108">Connection failed</span><span class="sxs-lookup"><span data-stu-id="9b518-108">Connection failed</span></span>

<span data-ttu-id="9b518-109">There can be a couple of reasons why you cannot connect to a company, including the following:</span><span class="sxs-lookup"><span data-stu-id="9b518-109">There can be a couple of reasons why you cannot connect to a company, including the following:</span></span>

- <span data-ttu-id="9b518-110">The URL in the **Environment Link** field is not valid</span><span class="sxs-lookup"><span data-stu-id="9b518-110">The URL in the **Environment Link** field is not valid</span></span>  

  <span data-ttu-id="9b518-111">Go to the **Environment Links** page, open the environment that you cannot connect to, and then choose the **Test the connection** action.</span><span class="sxs-lookup"><span data-stu-id="9b518-111">Go to the **Environment Links** page, open the environment that you cannot connect to, and then choose the **Test the connection** action.</span></span>  
- <span data-ttu-id="9b518-112">The client's company is currently offline, for example if it being upgraded</span><span class="sxs-lookup"><span data-stu-id="9b518-112">The client's company is currently offline, for example if it being upgraded</span></span>

  <span data-ttu-id="9b518-113">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span><span class="sxs-lookup"><span data-stu-id="9b518-113">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span></span> <span data-ttu-id="9b518-114">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span><span class="sxs-lookup"><span data-stu-id="9b518-114">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span></span> <span data-ttu-id="9b518-115">For example, the error message "*The server has rejected the client credentials*" suggests that you do not have access.</span><span class="sxs-lookup"><span data-stu-id="9b518-115">For example, the error message "*The server has rejected the client credentials*" suggests that you do not have access.</span></span>  
- <span data-ttu-id="9b518-116">You do not have access to all companies in the environment that you are trying to connect to</span><span class="sxs-lookup"><span data-stu-id="9b518-116">You do not have access to all companies in the environment that you are trying to connect to</span></span>

  <span data-ttu-id="9b518-117">In [!INCLUDE [prod_short](includes/prod_short.md)], an organisation can have multiple business units called companies and you might not have access to all companies.</span><span class="sxs-lookup"><span data-stu-id="9b518-117">In [!INCLUDE [prod_short](includes/prod_short.md)], an organization can have multiple business units called companies, and you might not have access to all companies.</span></span> <span data-ttu-id="9b518-118">Work with your administrator or client to make sure that you have access to the companies that you have to work in.</span><span class="sxs-lookup"><span data-stu-id="9b518-118">Work with your administrator or client to make sure that you have access to the companies that you have to work in.</span></span>  

## <a name="data-does-not-refresh"></a><span data-ttu-id="9b518-119">Data does not refresh</span><span class="sxs-lookup"><span data-stu-id="9b518-119">Data does not refresh</span></span>

<span data-ttu-id="9b518-120">When you add a company or request a refresh of the data, [!INCLUDE [prod_short](includes/prod_short.md)] fetches the data.</span><span class="sxs-lookup"><span data-stu-id="9b518-120">When you add a company or request a refresh of the data, [!INCLUDE [prod_short](includes/prod_short.md)] fetches the data.</span></span> <span data-ttu-id="9b518-121">But you must refresh the page yourself, such as choosing the **Reload all companies** action, refresh the browser page, navigate away from the dashboard and then back again, or similar.</span><span class="sxs-lookup"><span data-stu-id="9b518-121">But you must refresh the page yourself, such as choosing the **Reload all companies** action, refresh the browser page, navigate away from the dashboard and then back again, or similar.</span></span>  

<span data-ttu-id="9b518-122">If you've added a company but it is not displaying in the list, you can also use the **Reload all companies** action to update the list.</span><span class="sxs-lookup"><span data-stu-id="9b518-122">If you've added a company but it is not displaying in the list, you can also use the **Reload all companies** action to update the list.</span></span>

## <a name="see-also"></a><span data-ttu-id="9b518-123">See also </span><span class="sxs-lookup"><span data-stu-id="9b518-123">See also</span></span>

[<span data-ttu-id="9b518-124">Manage Work across Multiple Companies in the Company Hub</span><span class="sxs-lookup"><span data-stu-id="9b518-124">Manage Work across Multiple Companies in the Company Hub</span></span>](company-hub.md)  
[<span data-ttu-id="9b518-125">Add companies to your company hub</span><span class="sxs-lookup"><span data-stu-id="9b518-125">Add companies to your company hub</span></span>](company-hub-add-company.md)  
[<span data-ttu-id="9b518-126">Accountant Experiences in Business Central</span><span class="sxs-lookup"><span data-stu-id="9b518-126">Accountant Experiences in Business Central</span></span>](finance-accounting.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]