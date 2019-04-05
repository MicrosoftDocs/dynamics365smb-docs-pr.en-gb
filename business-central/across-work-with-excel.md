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
ms.date: 12/07/2018
ms.author: jswymer
ms.openlocfilehash: 27c137ea6309d40cddc94bc676ec7ea27d5c01fa
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "808916"
---
# <a name="viewing-and-editing-in-excel-from-business-central"></a><span data-ttu-id="0b3ae-103">Viewing and Editing in Excel From Business Central</span><span class="sxs-lookup"><span data-stu-id="0b3ae-103">Viewing and Editing in Excel From Business Central</span></span> 

<span data-ttu-id="0b3ae-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-104">With pages that display a list of records in rows and columns, like a list of customers, sale orders, or invoices, you can also view the records using Microsoft Excel.</span></span> <span data-ttu-id="0b3ae-105">To do this, you have two options.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-105">To do this, you have two options.</span></span> <span data-ttu-id="0b3ae-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-106">You can either select the **Open in Excel** action or the **Edit in Excel** action on the page.</span></span> <span data-ttu-id="0b3ae-107">The differences between the two actions is as follows:</span><span class="sxs-lookup"><span data-stu-id="0b3ae-107">The differences between the two actions is as follows:</span></span>  

## <a name="open-in-excel"></a><span data-ttu-id="0b3ae-108">Open in Excel</span><span class="sxs-lookup"><span data-stu-id="0b3ae-108">Open in Excel</span></span>

-    <span data-ttu-id="0b3ae-109">With this action, Excel respects any filters on the page the limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-109">With this action, Excel respects any filters on the page the limit the records shown.</span></span> <span data-ttu-id="0b3ae-110">This means that the Excel workbook will contain the same rows and columns that appear on the the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="0b3ae-110">This means that the Excel workbook will contain the same rows and columns that appear on the the page in [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

-    <span data-ttu-id="0b3ae-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="0b3ae-111">You can make changes to the records in Excel, but you cannot publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="0b3ae-112">You can only save the changes to Excel file on your computer.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-112">You can only save the changes to Excel file on your computer.</span></span> 

-    <span data-ttu-id="0b3ae-113">This action works on both on Windows and macOS.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-113">This action works on both on Windows and macOS.</span></span> 

>[!NOTE]
><span data-ttu-id="0b3ae-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is not available if the **Edit in Excel** action is.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-114">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Open in Excel** action is not available if the **Edit in Excel** action is.</span></span>

## <a name="edit-in-excel"></a><span data-ttu-id="0b3ae-115">Edit in Excel</span><span class="sxs-lookup"><span data-stu-id="0b3ae-115">Edit in Excel</span></span>

-    <span data-ttu-id="0b3ae-116">With this action, the Excel workbook does not respect filters on the page the limit the records shown.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-116">With this action, the Excel workbook does not respect filters on the page the limit the records shown.</span></span> <span data-ttu-id="0b3ae-117">This means that the Excel workbook will contain all the available records and columns, regardless of what is shown on the page.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-117">This means that the Excel workbook will contain all the available records and columns, regardless of what is shown on the page.</span></span> 

-    <span data-ttu-id="0b3ae-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="0b3ae-118">The advantage of the **Edit in Excel** action is that it lets you make changes to records in Excel and then publish the changes back to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>

-    <span data-ttu-id="0b3ae-119">It only works on Windows; not macOS.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-119">It only works on Windows; not macOS.</span></span>

>[!NOTE]
><span data-ttu-id="0b3ae-120">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been installed by your administrator.</span><span class="sxs-lookup"><span data-stu-id="0b3ae-120">For [!INCLUDE[prodshort](includes/prodshort.md)] on-premises, the **Edit in Excel** action is only available if the Excel add-in has been installed by your administrator.</span></span> <span data-ttu-id="0b3ae-121">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span><span class="sxs-lookup"><span data-stu-id="0b3ae-121">For administrators, if you want to learn how to install the excel add-in, see [Setting up the Excel Add-In](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/configuring-excel-addin).</span></span>

## <a name="see-also"></a><span data-ttu-id="0b3ae-122">See Also</span><span class="sxs-lookup"><span data-stu-id="0b3ae-122">See Also</span></span>

[<span data-ttu-id="0b3ae-123">Working with Business Central</span><span class="sxs-lookup"><span data-stu-id="0b3ae-123">Working with Business Central</span></span>](ui-work-product.md)  
