---
title: Viewing and Editing in Excel From Business Central
description: Learn about how you can open the pages in Microsoft Excel from Business Central for better data analysis.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 11/06/2020
ms.author: jswymer
ms.openlocfilehash: cb172cd1d3285128e871fedb44ccd70fb84a669a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754174"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="51727-103">Viewing and Editing in Excel From Business Central</span><span class="sxs-lookup"><span data-stu-id="51727-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="51727-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="51727-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="51727-105">To do this, you have two options.</span><span class="sxs-lookup"><span data-stu-id="51727-105">To do this, you have two options.</span></span> <span data-ttu-id="51727-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span><span class="sxs-lookup"><span data-stu-id="51727-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="51727-107">The differences between the two actions are as follows:</span><span class="sxs-lookup"><span data-stu-id="51727-107">The differences between the two actions are as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="51727-108">Open in Excel</span><span class="sxs-lookup"><span data-stu-id="51727-108">Open in Excel</span></span>

- <span data-ttu-id="51727-109">With this action, Excel respects any filters on the page that limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="51727-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="51727-110">The Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="51727-110">The Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

- <span data-ttu-id="51727-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="51727-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="51727-112">You can only save the changes to Excel file on your computer.</span><span class="sxs-lookup"><span data-stu-id="51727-112">You can only save the changes to Excel file on your computer.</span></span>

- <span data-ttu-id="51727-113">This action works on both on Windows and macOS.</span><span class="sxs-lookup"><span data-stu-id="51727-113">This action works on both on Windows and macOS.</span></span>

> [!NOTE]
> <span data-ttu-id="51727-114">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Open in Excel** action is available by default.</span><span class="sxs-lookup"><span data-stu-id="51727-114">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="51727-115">However, if you set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span><span class="sxs-lookup"><span data-stu-id="51727-115">However, if you set up [!INCLUDE[prod_short](includes/prod_short.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="51727-116">Edit in Excel</span><span class="sxs-lookup"><span data-stu-id="51727-116">Edit in Excel</span></span>

- <span data-ttu-id="51727-117">With this action, Excel respects most filters on the page that limit the records shown, so the Excel workbook will contain almost the same records and columns.</span><span class="sxs-lookup"><span data-stu-id="51727-117">With this action, Excel respects most filters on the page that limit the records shown, so the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="51727-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="51727-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

- <span data-ttu-id="51727-119">It only works on Windows; not macOS.</span><span class="sxs-lookup"><span data-stu-id="51727-119">It only works on Windows; not macOS.</span></span>

- <span data-ttu-id="51727-120">You can switch the company that you are working with.</span><span class="sxs-lookup"><span data-stu-id="51727-120">You can switch the company that you are working with.</span></span> <span data-ttu-id="51727-121">To switch company, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span><span class="sxs-lookup"><span data-stu-id="51727-121">To switch company, select the **Options** icon ![Excel add-in options](media/cogwheel.png "Excel add-in options") in the Excel Add-in pane, then select the company from the **Company** field.</span></span>  

    > [!IMPORTANT]
    > <span data-ttu-id="51727-122">When changing the company, make sure that the **Environment** field is not empty.</span><span class="sxs-lookup"><span data-stu-id="51727-122">When changing the company, make sure that the **Environment** field is not empty.</span></span> <span data-ttu-id="51727-123">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span><span class="sxs-lookup"><span data-stu-id="51727-123">If it is, then set it to one of the available options; otherwise, the add-in will not work correctly.</span></span>  

<span data-ttu-id="51727-124">If you make changes to the add-in, you must reload it to update the connection.</span><span class="sxs-lookup"><span data-stu-id="51727-124">If you make changes to the add-in, you must reload it to update the connection.</span></span> <span data-ttu-id="51727-125">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span><span class="sxs-lookup"><span data-stu-id="51727-125">To reload, use the ![Excel add-in menu](media/excel-addin-menu.png "Excel add-in menu") menu in the top-right corner of the add-in.</span></span> <span data-ttu-id="51727-126">If you cannot load the add-in, talk to your administrator.</span><span class="sxs-lookup"><span data-stu-id="51727-126">If you cannot load the add-in, talk to your administrator.</span></span> <span data-ttu-id="51727-127">If you are the administrator, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="51727-127">If you are the administrator, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

> [!NOTE]
> <span data-ttu-id="51727-128">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span><span class="sxs-lookup"><span data-stu-id="51727-128">For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator, and only available for the Web client.</span></span> <span data-ttu-id="51727-129">For administrators, if you want to learn how to install the Excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="51727-129">For administrators, if you want to learn how to install the Excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="51727-130">See the differences between the options</span><span class="sxs-lookup"><span data-stu-id="51727-130">See the differences between the options</span></span>
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="51727-131">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="51727-131">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="51727-132">See Also</span><span class="sxs-lookup"><span data-stu-id="51727-132">See Also</span></span>

[<span data-ttu-id="51727-133">Analysing Financial Statements in Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="51727-133">Analyzing Financial Statements in Microsoft Excel</span></span>](finance-analyze-excel.md)  
[<span data-ttu-id="51727-134">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="51727-134">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="51727-135">Enhancements to Excel integration in 2019 release wave 2</span><span class="sxs-lookup"><span data-stu-id="51727-135">Enhancements to Excel integration in 2019 release wave 2</span></span>](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration)  
