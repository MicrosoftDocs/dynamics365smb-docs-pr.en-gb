---
title: Viewing and Editing in Excel From Business Central
description: Learn about how you can open the pages in Microsoft Excel from Business Central for better data analysis.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 7e3abf36444c4701229ffaac7ceade11bb1879cc
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786939"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="eb985-103">Viewing and Editing in Excel From Business Central</span><span class="sxs-lookup"><span data-stu-id="eb985-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="eb985-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="eb985-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="eb985-105">To do this, you have two options.</span><span class="sxs-lookup"><span data-stu-id="eb985-105">To do this, you have two options.</span></span> <span data-ttu-id="eb985-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span><span class="sxs-lookup"><span data-stu-id="eb985-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="eb985-107">The differences between the two actions are as follows:</span><span class="sxs-lookup"><span data-stu-id="eb985-107">The differences between the two actions are as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="eb985-108">Open in Excel</span><span class="sxs-lookup"><span data-stu-id="eb985-108">Open in Excel</span></span>

- <span data-ttu-id="eb985-109">With this action, Excel respects any filters on the page that limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="eb985-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="eb985-110">The Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="eb985-110">The Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

- <span data-ttu-id="eb985-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="eb985-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="eb985-112">You can only save the changes to Excel file on your computer.</span><span class="sxs-lookup"><span data-stu-id="eb985-112">You can only save the changes to Excel file on your computer.</span></span>

- <span data-ttu-id="eb985-113">This action works on both on Windows and macOS.</span><span class="sxs-lookup"><span data-stu-id="eb985-113">This action works on both on Windows and macOS.</span></span>

> [!NOTE]
> <span data-ttu-id="eb985-114">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Open in Excel** action is available by default.</span><span class="sxs-lookup"><span data-stu-id="eb985-114">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="eb985-115">However, if you set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span><span class="sxs-lookup"><span data-stu-id="eb985-115">However, if you set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="eb985-116">Edit in Excel</span><span class="sxs-lookup"><span data-stu-id="eb985-116">Edit in Excel</span></span>

- <span data-ttu-id="eb985-117">With this action, Excel respects most filters on the page that limit the records shown, so the Excel workbook will contain almost the same records and columns.</span><span class="sxs-lookup"><span data-stu-id="eb985-117">With this action, Excel respects most filters on the page that limit the records shown, so the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="eb985-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="eb985-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

- <span data-ttu-id="eb985-119">It only works on Windows; not macOS.</span><span class="sxs-lookup"><span data-stu-id="eb985-119">It only works on Windows; not macOS.</span></span>

- <span data-ttu-id="eb985-120">You can switch the company that you are working with.</span><span class="sxs-lookup"><span data-stu-id="eb985-120">You can switch the company that you are working with.</span></span> <span data-ttu-id="eb985-121">To switch company, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span><span class="sxs-lookup"><span data-stu-id="eb985-121">To switch company, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span></span>  

    > [!IMPORTANT]
    > <span data-ttu-id="eb985-122">When changing the company, make sure that the **Environment** field is not empty.</span><span class="sxs-lookup"><span data-stu-id="eb985-122">When changing the company, make sure that the **Environment** field is not empty.</span></span> <span data-ttu-id="eb985-123">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span><span class="sxs-lookup"><span data-stu-id="eb985-123">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span></span>  

<span data-ttu-id="eb985-124">If you make changes to the add-in, you must reload it to update the connection.</span><span class="sxs-lookup"><span data-stu-id="eb985-124">If you make changes to the add-in, you must reload it to update the connection.</span></span> <span data-ttu-id="eb985-125">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span><span class="sxs-lookup"><span data-stu-id="eb985-125">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span></span> <span data-ttu-id="eb985-126">If you cannot load the add-in, talk to your administrator.</span><span class="sxs-lookup"><span data-stu-id="eb985-126">If you cannot load the add-in, talk to your administrator.</span></span> <span data-ttu-id="eb985-127">If you are the administrator, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="eb985-127">If you are the administrator, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

> [!NOTE]
> <span data-ttu-id="eb985-128">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span><span class="sxs-lookup"><span data-stu-id="eb985-128">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span></span> <span data-ttu-id="eb985-129">For administrators, if you want to learn how to install the Excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="eb985-129">For administrators, if you want to learn how to install the Excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="eb985-130">See the differences between the options</span><span class="sxs-lookup"><span data-stu-id="eb985-130">See the differences between the options</span></span>
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="eb985-131">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="eb985-131">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="eb985-132">See Also</span><span class="sxs-lookup"><span data-stu-id="eb985-132">See Also</span></span>

[<span data-ttu-id="eb985-133">Analysing Financial Statements in Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="eb985-133">Analyzing Financial Statements in Microsoft Excel</span></span>](finance-analyze-excel.md)  
[<span data-ttu-id="eb985-134">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="eb985-134">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="eb985-135">Enhancements to Excel integration in 2019 release wave 2</span><span class="sxs-lookup"><span data-stu-id="eb985-135">Enhancements to Excel integration in 2019 release wave 2</span></span>](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  


[!INCLUDE[footer-include](includes/footer-banner.md)]