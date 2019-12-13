---
title: Viewing and Editing in Excel From Business Central | Microsoft Docs
description: Learn about how you can open the pages in Microsoft Excel from Business Central for better data analysis.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 10/24/2019
ms.author: jswymer
ms.openlocfilehash: 99fe339426b755b70983d8ec9345858357043347
ms.sourcegitcommit: 893e13fa75b2d04dedd4a29abda216e3e54b24ae
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 11/15/2019
ms.locfileid: "2808752"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="b93a1-103">Viewing and Editing in Excel From Business Central</span><span class="sxs-lookup"><span data-stu-id="b93a1-103">Viewing and Editing in Excel From Business Central</span></span>

<span data-ttu-id="b93a1-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="b93a1-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="b93a1-105">To do this, you have two options.</span><span class="sxs-lookup"><span data-stu-id="b93a1-105">To do this, you have two options.</span></span> <span data-ttu-id="b93a1-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span><span class="sxs-lookup"><span data-stu-id="b93a1-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="b93a1-107">The differences between the two actions is as follows:</span><span class="sxs-lookup"><span data-stu-id="b93a1-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="b93a1-108">Open in Excel</span><span class="sxs-lookup"><span data-stu-id="b93a1-108">Open in Excel</span></span>

- <span data-ttu-id="b93a1-109">With this action, Excel respects any filters on the page that limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="b93a1-109">With this action, Excel respects any filters on the page that limit the records shown.</span></span> <span data-ttu-id="b93a1-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b93a1-110">This means that the Excel workbook will contain the same rows and columns that appear on the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="b93a1-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b93a1-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="b93a1-112">You can only save the changes to Excel file on your computer.</span><span class="sxs-lookup"><span data-stu-id="b93a1-112">You can only save the changes to Excel file on your computer.</span></span> 

- <span data-ttu-id="b93a1-113">This action works on both on Windows and macOS.</span><span class="sxs-lookup"><span data-stu-id="b93a1-113">This action works on both on Windows and macOS.</span></span> 

> [!NOTE]
> <span data-ttu-id="b93a1-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span><span class="sxs-lookup"><span data-stu-id="b93a1-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is available by default.</span></span> <span data-ttu-id="b93a1-115">However, if you set up [!INCLUDE [prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span><span class="sxs-lookup"><span data-stu-id="b93a1-115">However, if you set up [!INCLUDE [prodshort](includes/prodshort.md)] on-premises for editing data in Excel, then the **Open in Excel** action is replaced by the **Edit in Excel** action.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="b93a1-116">Edit in Excel</span><span class="sxs-lookup"><span data-stu-id="b93a1-116">Edit in Excel</span></span>

- <span data-ttu-id="b93a1-117">With this action, Excel respects most filters on the page that limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="b93a1-117">With this action, Excel respects most filters on the page that limit the records shown.</span></span> <span data-ttu-id="b93a1-118">This means that the Excel workbook will contain almost the same records and columns.</span><span class="sxs-lookup"><span data-stu-id="b93a1-118">This means that the Excel workbook will contain almost the same records and columns.</span></span>

- <span data-ttu-id="b93a1-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="b93a1-119">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

- <span data-ttu-id="b93a1-120">It only works on Windows; not macOS.</span><span class="sxs-lookup"><span data-stu-id="b93a1-120">It only works on Windows; not macOS.</span></span>

<span data-ttu-id="b93a1-121">This was enhanced in 2019 release wave 2.</span><span class="sxs-lookup"><span data-stu-id="b93a1-121">This was enhanced in 2019 release wave 2.</span></span> <span data-ttu-id="b93a1-122">For more information, see [Enhancements to Excel integration](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).</span><span class="sxs-lookup"><span data-stu-id="b93a1-122">For more information, see [Enhancements to Excel integration](/dynamics365-release-plan/2019wave2/dynamics365-business-central/enhancements-excel-integration).</span></span>

> [!NOTE]
> <span data-ttu-id="b93a1-123">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator.</span><span class="sxs-lookup"><span data-stu-id="b93a1-123">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been configured by your administrator.</span></span> <span data-ttu-id="b93a1-124">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="b93a1-124">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In for Editing Business Central Data](/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

> [!NOTE]
> <span data-ttu-id="b93a1-125">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, this feature is only available for the Web client.</span><span class="sxs-lookup"><span data-stu-id="b93a1-125">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, this feature is only available for the Web client.</span></span>

### <a name="see-the-differences-between-the-options"></a><span data-ttu-id="b93a1-126">See the differences between the options</span><span class="sxs-lookup"><span data-stu-id="b93a1-126">See the differences between the options</span></span> 
<br><br>  

> [!Video https://go.microsoft.com/fwlink/?linkid=2086039]

## <a name="see-also"></a><span data-ttu-id="b93a1-127">See Also</span><span class="sxs-lookup"><span data-stu-id="b93a1-127">See Also</span></span>
[<span data-ttu-id="b93a1-128">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="b93a1-128">Working with Business Central</span></span>](ui-work-product.md)  
