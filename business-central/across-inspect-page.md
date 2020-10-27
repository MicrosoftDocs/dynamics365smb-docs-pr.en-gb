---
title: Inspecting Pages in Business Central
description: Use the page inspection feature to zoom into details about the page design and data source. Page inspector is ideal for troubleshooting issues with your data.
ms.custom: na
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: dynamics365-business-central
author: jswymer
ms.author: jswymer
ms.date: 10/01/2020
ms.openlocfilehash: f56dbf4546f5f1b466b23c3bd2794d3c4ffe02c3
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3924710"
---
# <a name="inspecting-pages-in-business-central"></a><span data-ttu-id="8139d-104">Inspecting Pages in Business Central</span><span class="sxs-lookup"><span data-stu-id="8139d-104">Inspecting Pages in Business Central</span></span>

<span data-ttu-id="8139d-105">The page inspection feature enables you to get details about a page, providing insight into the page design, the different elements that comprise the page, and the source behind the data it displays.</span><span class="sxs-lookup"><span data-stu-id="8139d-105">The page inspection feature enables you to get details about a page, providing insight into the page design, the different elements that comprise the page, and the source behind the data it displays.</span></span> <span data-ttu-id="8139d-106">Page inspection is especially designed for administrators, power users, support personnel, and developers.</span><span class="sxs-lookup"><span data-stu-id="8139d-106">Page inspection is especially designed for administrators, power users, support personnel, and developers.</span></span> <span data-ttu-id="8139d-107">It is ideal for learning the data model behind a page and troubleshooting.</span><span class="sxs-lookup"><span data-stu-id="8139d-107">It is ideal for learning the data model behind a page and troubleshooting.</span></span> <span data-ttu-id="8139d-108">For example, if you are experiencing a problem with a page, you could use page inspection to get information to pass on to your system administrator or support personnel.</span><span class="sxs-lookup"><span data-stu-id="8139d-108">For example, if you are experiencing a problem with a page, you could use page inspection to get information to pass on to your system administrator or support personnel.</span></span>

## <a name="working-with-page-inspection"></a><span data-ttu-id="8139d-109">Working with Page Inspection</span><span class="sxs-lookup"><span data-stu-id="8139d-109">Working with Page Inspection</span></span>

<span data-ttu-id="8139d-110">You start page inspection from the **Help & Support** page.</span><span class="sxs-lookup"><span data-stu-id="8139d-110">You start page inspection from the **Help & Support** page.</span></span> <span data-ttu-id="8139d-111">Choose the question mark in the top right corner, choose **Help & Support** , and then choose **Inspect pages and data** .</span><span class="sxs-lookup"><span data-stu-id="8139d-111">Choose the question mark in the top right corner, choose **Help & Support** , and then choose **Inspect pages and data** .</span></span> <span data-ttu-id="8139d-112">Or, you can just use the keyboard shortcut **Ctrl+Alt+F1** .</span><span class="sxs-lookup"><span data-stu-id="8139d-112">Or, you can just use the keyboard shortcut **Ctrl+Alt+F1** .</span></span>

<span data-ttu-id="8139d-113">The **Page inspection** pane opens on the side.</span><span class="sxs-lookup"><span data-stu-id="8139d-113">The **Page inspection** pane opens on the side.</span></span> <span data-ttu-id="8139d-114">The following figure illustrates the **Page Inspection** pane on the **Sales Order** page.</span><span class="sxs-lookup"><span data-stu-id="8139d-114">The following figure illustrates the **Page Inspection** pane on the **Sales Order** page.</span></span>

![Page Inspection](media/page-inspection-example.png)

<span data-ttu-id="8139d-116">When the **Page Inspection** pane first opens, it shows information that pertains to the main page object.</span><span class="sxs-lookup"><span data-stu-id="8139d-116">When the **Page Inspection** pane first opens, it shows information that pertains to the main page object.</span></span>

<span data-ttu-id="8139d-117">Use the keyboard or pointing device to move focus to different elements on the page.</span><span class="sxs-lookup"><span data-stu-id="8139d-117">Use the keyboard or pointing device to move focus to different elements on the page.</span></span> <span data-ttu-id="8139d-118">When you select a FactBox or a part on the main page, the bounding area is highlighted by a border, and the **Page Inspection** pane shows information about the selected element.</span><span class="sxs-lookup"><span data-stu-id="8139d-118">When you select a FactBox or a part on the main page, the bounding area is highlighted by a border, and the **Page Inspection** pane shows information about the selected element.</span></span> <span data-ttu-id="8139d-119">For example, the previous figure shows information about the list part in the **Sales Order** page.</span><span class="sxs-lookup"><span data-stu-id="8139d-119">For example, the previous figure shows information about the list part in the **Sales Order** page.</span></span> <span data-ttu-id="8139d-120">As you navigate to other pages in the application, the **Page Inspection** pane will automatically update with page information as you move along.</span><span class="sxs-lookup"><span data-stu-id="8139d-120">As you navigate to other pages in the application, the **Page Inspection** pane will automatically update with page information as you move along.</span></span>

<span data-ttu-id="8139d-121">For more information about what is shown in page inspection, see [Inspecting and Troubleshooting Pages](/dynamics365/business-central/dev-itpro/developer/devenv-inspecting-pages) in the Business Central Developer and IT Pro help.</span><span class="sxs-lookup"><span data-stu-id="8139d-121">For more information about what is shown in page inspection, see [Inspecting and Troubleshooting Pages](/dynamics365/business-central/dev-itpro/developer/devenv-inspecting-pages) in the Business Central Developer and IT Pro help.</span></span>

<span data-ttu-id="8139d-122">If you do not see the details that you expect to see in the **Page Inspection** pane, you probably do not have the required permissions, as described in the next section.</span><span class="sxs-lookup"><span data-stu-id="8139d-122">If you do not see the details that you expect to see in the **Page Inspection** pane, you probably do not have the required permissions, as described in the next section.</span></span>

## <a name="controlling-access-to-page-inspection-details"></a><span data-ttu-id="8139d-123">Controlling Access to Page Inspection Details</span><span class="sxs-lookup"><span data-stu-id="8139d-123">Controlling Access to Page Inspection Details</span></span>

<span data-ttu-id="8139d-124">As an administrator, you can control access to the full details that are shown in the **Page Inspection** pane by configuring the permissions that users have.</span><span class="sxs-lookup"><span data-stu-id="8139d-124">As an administrator, you can control access to the full details that are shown in the **Page Inspection** pane by configuring the permissions that users have.</span></span> <span data-ttu-id="8139d-125">To grant a user permission to the full details, give users **Execute** permission on the **System** object **5330** .</span><span class="sxs-lookup"><span data-stu-id="8139d-125">To grant a user permission to the full details, give users **Execute** permission on the **System** object **5330** .</span></span> <span data-ttu-id="8139d-126">You can grant this permission by using a permission set (such as **D365 Troubleshoot** ) or a user group (such as **D365 Troubleshoot** ).</span><span class="sxs-lookup"><span data-stu-id="8139d-126">You can grant this permission by using a permission set (such as **D365 Troubleshoot** ) or a user group (such as **D365 Troubleshoot** ).</span></span> <span data-ttu-id="8139d-127">For more information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="8139d-127">For more information about permissions, see [Assign Permissions to Users and Groups](ui-define-granular-permissions.md).</span></span>

<span data-ttu-id="8139d-128">Users who are not granted permissions on **System object 5330** can still access the **Page Inspection** pane, but they will only see the **Page** and **Table** fields, which display basic details that they can pass on to their support team.</span><span class="sxs-lookup"><span data-stu-id="8139d-128">Users who are not granted permissions on **System object 5330** can still access the **Page Inspection** pane, but they will only see the **Page** and **Table** fields, which display basic details that they can pass on to their support team.</span></span>

## <a name="see-also"></a><span data-ttu-id="8139d-129">See Also</span><span class="sxs-lookup"><span data-stu-id="8139d-129">See Also</span></span>

<span data-ttu-id="8139d-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8139d-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
