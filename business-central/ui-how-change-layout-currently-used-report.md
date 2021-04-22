---
title: Change the Way a Report Looks by Selecting a Different Layout | Microsoft Docs
description: You can use different layouts for a report, and switch between layouts to change how a report looks.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: ad5dd28d10df38fbd780ec4df5d4a87056670b99
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771092"
---
# <a name="change-the-current-report-layout"></a><span data-ttu-id="3daa3-103">Change the Current Report Layout</span><span class="sxs-lookup"><span data-stu-id="3daa3-103">Change the Current Report Layout</span></span>
<span data-ttu-id="3daa3-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span><span class="sxs-lookup"><span data-stu-id="3daa3-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span></span>

<span data-ttu-id="3daa3-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span><span class="sxs-lookup"><span data-stu-id="3daa3-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span></span> <span data-ttu-id="3daa3-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="3daa3-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span></span>

<span data-ttu-id="3daa3-107">When custom report layouts are defined, you can select them from customer and vendor cards to specify that the selected layouts will be used for documents that you crate for the customer or vendor in question.</span><span class="sxs-lookup"><span data-stu-id="3daa3-107">When custom report layouts are defined, you can select them from customer and vendor cards to specify that the selected layouts will be used for documents that you crate for the customer or vendor in question.</span></span> <span data-ttu-id="3daa3-108">For more information, see [Define Document Layouts for Customers and Vendors](ui-define-customer-vendor-document-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="3daa3-108">For more information, see [Define Document Layouts for Customers and Vendors](ui-define-customer-vendor-document-layouts.md).</span></span>

> [!TIP]  
> <span data-ttu-id="3daa3-109">Document reports (not lists) that use a Word report layout are typically faster than those that use an RDLC report layout.</span><span class="sxs-lookup"><span data-stu-id="3daa3-109">Document reports (not lists) that use a Word report layout are typically faster than those that use an RDLC report layout.</span></span> <span data-ttu-id="3daa3-110">So if you have the option to choose between a Word or RDLC report layout for a document report, use the Word report layout for the best performance.</span><span class="sxs-lookup"><span data-stu-id="3daa3-110">So if you have the option to choose between a Word or RDLC report layout for a document report, use the Word report layout for the best performance.</span></span>

## <a name="to-change-which-report-layout-to-use-for-a-report-or-document"></a><span data-ttu-id="3daa3-111">To change which report layout to use for a report or document</span><span class="sxs-lookup"><span data-stu-id="3daa3-111">To change which report layout to use for a report or document</span></span>
1. <span data-ttu-id="3daa3-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="3daa3-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  
   <span data-ttu-id="3daa3-113">The **Report Layout Selection** page lists all the reports that are available for the company that is specified in the **Company** field at the top of the page.</span><span class="sxs-lookup"><span data-stu-id="3daa3-113">The **Report Layout Selection** page lists all the reports that are available for the company that is specified in the **Company** field at the top of the page.</span></span> <span data-ttu-id="3daa3-114">The **Selected Layout** field specifies the layout that is currently used on the report.</span><span class="sxs-lookup"><span data-stu-id="3daa3-114">The **Selected Layout** field specifies the layout that is currently used on the report.</span></span>
2. <span data-ttu-id="3daa3-115">Set the **Company** field at the top of the page to the company that includes the report.</span><span class="sxs-lookup"><span data-stu-id="3daa3-115">Set the **Company** field at the top of the page to the company that includes the report.</span></span>
3. <span data-ttu-id="3daa3-116">To change the layout that is used by a report, on the row for the report, set the **Selected Layout** field to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="3daa3-116">To change the layout that is used by a report, on the row for the report, set the **Selected Layout** field to one of the following options:</span></span>
   * <span data-ttu-id="3daa3-117">**RDLC (built-in)**, uses the built-in RDLC report layout on the report.</span><span class="sxs-lookup"><span data-stu-id="3daa3-117">**RDLC (built-in)**, uses the built-in RDLC report layout on the report.</span></span>
   * <span data-ttu-id="3daa3-118">**Word (built-in)**, uses the built-in Word report layout on the report.</span><span class="sxs-lookup"><span data-stu-id="3daa3-118">**Word (built-in)**, uses the built-in Word report layout on the report.</span></span>
   * <span data-ttu-id="3daa3-119">**Custom**, uses a custom layout on the report.</span><span class="sxs-lookup"><span data-stu-id="3daa3-119">**Custom**, uses a custom layout on the report.</span></span>  

> [!NOTE]
> <span data-ttu-id="3daa3-120">If you choose a report layout of type **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span><span class="sxs-lookup"><span data-stu-id="3daa3-120">If you choose a report layout of type **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span></span> <span data-ttu-id="3daa3-121">See the next procedure.</span><span class="sxs-lookup"><span data-stu-id="3daa3-121">See the next procedure.</span></span>

<span data-ttu-id="3daa3-122">If you selected a built-in RDLC or Word report layout, then no further action is required, and the layout will be used the next time the report is run.</span><span class="sxs-lookup"><span data-stu-id="3daa3-122">If you selected a built-in RDLC or Word report layout, then no further action is required, and the layout will be used the next time the report is run.</span></span>

## <a name="to-change-the-custom-layout-to-use-for-a-report-layout"></a><span data-ttu-id="3daa3-123">To change the custom layout to use for a report layout</span><span class="sxs-lookup"><span data-stu-id="3daa3-123">To change the custom layout to use for a report layout</span></span>
<span data-ttu-id="3daa3-124">You may also want to change the currently used custom layout.</span><span class="sxs-lookup"><span data-stu-id="3daa3-124">You may also want to change the currently used custom layout.</span></span> <span data-ttu-id="3daa3-125">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="3daa3-125">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

<span data-ttu-id="3daa3-126">All custom report layouts that exist for report layouts in a company are listed on the **Custom Report Layouts** page.</span><span class="sxs-lookup"><span data-stu-id="3daa3-126">All custom report layouts that exist for report layouts in a company are listed on the **Custom Report Layouts** page.</span></span> <span data-ttu-id="3daa3-127">On the **Report Layout Selection** page, you can see which custom layouts are available for each report in the **Custom Layouts** FactBox.</span><span class="sxs-lookup"><span data-stu-id="3daa3-127">On the **Report Layout Selection** page, you can see which custom layouts are available for each report in the **Custom Layouts** FactBox.</span></span>

1. <span data-ttu-id="3daa3-128">On the **Report Layout Selection** page, on the line for the report layout that you want to change, choose the lookup button in the **Custom Layout Description** field.</span><span class="sxs-lookup"><span data-stu-id="3daa3-128">On the **Report Layout Selection** page, on the line for the report layout that you want to change, choose the lookup button in the **Custom Layout Description** field.</span></span>
2. <span data-ttu-id="3daa3-129">On the **Custom Report Layouts** page, select the row for the custom layout that you want to use, and then choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="3daa3-129">On the **Custom Report Layouts** page, select the row for the custom layout that you want to use, and then choose the **OK** button.</span></span>

<span data-ttu-id="3daa3-130">The name of the selected custom layout is now shown in the **Custom Layout Description** field and will be used the next time the report or document is previewed, printed, or sent.</span><span class="sxs-lookup"><span data-stu-id="3daa3-130">The name of the selected custom layout is now shown in the **Custom Layout Description** field and will be used the next time the report or document is previewed, printed, or sent.</span></span>

<span data-ttu-id="3daa3-131">You can now go to your customer and vendor cards to specify which of the layouts to use for different documents that you crate for the customer or vendor in question, such as order confirmations or payment reminders.</span><span class="sxs-lookup"><span data-stu-id="3daa3-131">You can now go to your customer and vendor cards to specify which of the layouts to use for different documents that you crate for the customer or vendor in question, such as order confirmations or payment reminders.</span></span> <span data-ttu-id="3daa3-132">For more information, see [Define Document Layouts for Customers and Vendors](ui-define-customer-vendor-document-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="3daa3-132">For more information, see [Define Document Layouts for Customers and Vendors](ui-define-customer-vendor-document-layouts.md).</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="3daa3-133">See Related Training at [Microsoft Learn](/learn/modules/change-documents-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="3daa3-133">See Related Training at [Microsoft Learn](/learn/modules/change-documents-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="3daa3-134">See Also</span><span class="sxs-lookup"><span data-stu-id="3daa3-134">See Also</span></span>
[<span data-ttu-id="3daa3-135">Managing Report Layouts</span><span class="sxs-lookup"><span data-stu-id="3daa3-135">Managing Report Layouts</span></span>](ui-manage-report-layouts.md)  
<span data-ttu-id="3daa3-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3daa3-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]