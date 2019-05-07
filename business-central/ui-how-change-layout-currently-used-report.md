---
title: Change the Way a Report Looks by Selecting a Different Layout | Microsoft Docs
description: You can use different layouts for a report, and switch between layouts to change how a report looks.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 04/01/2019
ms.author: jswymer
ms.openlocfilehash: f24f1cd24a31ddbd0b455b876821ae0173a677c3
ms.sourcegitcommit: addfb47612cc2e4e98dfd7e338b6f41cde405d5c
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/16/2019
ms.locfileid: "969816"
---
# <a name="change-which-layout-is-currently-used-on-a-report"></a><span data-ttu-id="918d5-103">Change Which Layout is Currently Used on a Report</span><span class="sxs-lookup"><span data-stu-id="918d5-103">Change Which Layout is Currently Used on a Report</span></span>
<span data-ttu-id="918d5-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span><span class="sxs-lookup"><span data-stu-id="918d5-104">A report can be set up with more than one report layout, which you can then switch among as needed.</span></span>

<span data-ttu-id="918d5-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span><span class="sxs-lookup"><span data-stu-id="918d5-105">Depending on the layouts that are available for a report, you can choose to use a built-in RDLC report layout, a built-in Word report layout, or a custom layout.</span></span> <span data-ttu-id="918d5-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span><span class="sxs-lookup"><span data-stu-id="918d5-106">For more information about RDLC and Word report layouts, built-in and custom layouts, and more, see [Manage Report Layouts](ui-manage-report-layouts.md).</span></span>

> [!TIP]  
> <span data-ttu-id="918d5-107">Document reports (not lists) that use a Word report layout are typically faster than those that use an RDLC report layout.</span><span class="sxs-lookup"><span data-stu-id="918d5-107">Document reports (not lists) that use a Word report layout are typically faster than those that use an RDLC report layout.</span></span> <span data-ttu-id="918d5-108">So if you have the option to choose between a Word or RDLC report layout for a document report, use the Word report layout for the best performance.</span><span class="sxs-lookup"><span data-stu-id="918d5-108">So if you have the option to choose between a Word or RDLC report layout for a document report, use the Word report layout for the best performance.</span></span>  

## <a name="to-change-the-layout-that-is-used-on-a-report"></a><span data-ttu-id="918d5-109">To change the layout that is used on a report</span><span class="sxs-lookup"><span data-stu-id="918d5-109">To change the layout that is used on a report</span></span>
1. <span data-ttu-id="918d5-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="918d5-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Layout Selection**, and then choose the related link.</span></span>  
   <span data-ttu-id="918d5-111">The **Report Layout Selection** page lists all the reports that are available for the company that is specified in the Company field at the top of the page.</span><span class="sxs-lookup"><span data-stu-id="918d5-111">The **Report Layout Selection** page lists all the reports that are available for the company that is specified in the Company field at the top of the page.</span></span> <span data-ttu-id="918d5-112">The Selected Layout field specifies the layout that is currently used on the report.</span><span class="sxs-lookup"><span data-stu-id="918d5-112">The Selected Layout field specifies the layout that is currently used on the report.</span></span>
2. <span data-ttu-id="918d5-113">Set the **Company** field at the top of the page to the company that includes the report.</span><span class="sxs-lookup"><span data-stu-id="918d5-113">Set the **Company** field at the top of the page to the company that includes the report.</span></span>
3. <span data-ttu-id="918d5-114">To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:</span><span class="sxs-lookup"><span data-stu-id="918d5-114">To change the layout that is used by a report, in the row for the report in the list, set the **Selected Layout** field to one of the following options:</span></span>
   * <span data-ttu-id="918d5-115">RDLC (built-in), uses the built-in RDLC report layout on the report.</span><span class="sxs-lookup"><span data-stu-id="918d5-115">RDLC (built-in), uses the built-in RDLC report layout on the report.</span></span>
   * <span data-ttu-id="918d5-116">Word (built-in), uses the built-in Word report layout on the report.</span><span class="sxs-lookup"><span data-stu-id="918d5-116">Word (built-in), uses the built-in Word report layout on the report.</span></span>
   * <span data-ttu-id="918d5-117">Custom, uses a custom layout on the report.</span><span class="sxs-lookup"><span data-stu-id="918d5-117">Custom, uses a custom layout on the report.</span></span>  
     <span data-ttu-id="918d5-118">You can see which custom layouts are available for the report in the Report Layouts Part FactBox.</span><span class="sxs-lookup"><span data-stu-id="918d5-118">You can see which custom layouts are available for the report in the Report Layouts Part FactBox.</span></span> <span data-ttu-id="918d5-119">If there are no custom layouts for the report, then you will have to create one first.</span><span class="sxs-lookup"><span data-stu-id="918d5-119">If there are no custom layouts for the report, then you will have to create one first.</span></span> <span data-ttu-id="918d5-120">If you choose this option, go to the next procedure to specify the custom layout that you want to use.</span><span class="sxs-lookup"><span data-stu-id="918d5-120">If you choose this option, go to the next procedure to specify the custom layout that you want to use.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="918d5-121">If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span><span class="sxs-lookup"><span data-stu-id="918d5-121">If you choose **RDLC (built-in)** or **Word (built-in)** and you get an error message that the report does not have a layout of the specified type, then you must choose another layout option or create a custom report layout of the type that you want to use.</span></span>

<span data-ttu-id="918d5-122">If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.</span><span class="sxs-lookup"><span data-stu-id="918d5-122">If you selected a built-in RDLC or Word report layout, then no further action is required and the layout will be used the next time the report is run.</span></span>

## <a name="to-specify-a-custom-layout-on-a-report"></a><span data-ttu-id="918d5-123">To specify a custom layout on a report</span><span class="sxs-lookup"><span data-stu-id="918d5-123">To specify a custom layout on a report</span></span>
1. <span data-ttu-id="918d5-124">You specify which custom layout to use on the report from the **Custom Report Layouts** page.</span><span class="sxs-lookup"><span data-stu-id="918d5-124">You specify which custom layout to use on the report from the **Custom Report Layouts** page.</span></span> <span data-ttu-id="918d5-125">If the **Custom Report Layouts** page is not open, then in the **Report Layout Description** field, choose the lookup button.</span><span class="sxs-lookup"><span data-stu-id="918d5-125">If the **Custom Report Layouts** page is not open, then in the **Report Layout Description** field, choose the lookup button.</span></span>
2. <span data-ttu-id="918d5-126">On the **Custom Report Layouts** page, select the row for custom layout that you want to use, and then close the page.</span><span class="sxs-lookup"><span data-stu-id="918d5-126">On the **Custom Report Layouts** page, select the row for custom layout that you want to use, and then close the page.</span></span>

<span data-ttu-id="918d5-127">You return to the **Report Layout Selection** page.</span><span class="sxs-lookup"><span data-stu-id="918d5-127">You return to the **Report Layout Selection** page.</span></span> <span data-ttu-id="918d5-128">The name of the selected custom layout displays in the **Custom Layout Description** field.</span><span class="sxs-lookup"><span data-stu-id="918d5-128">The name of the selected custom layout displays in the **Custom Layout Description** field.</span></span> <span data-ttu-id="918d5-129">The custom layout will be used the next time that you run the report.</span><span class="sxs-lookup"><span data-stu-id="918d5-129">The custom layout will be used the next time that you run the report.</span></span>

## <a name="see-also"></a><span data-ttu-id="918d5-130">See Also</span><span class="sxs-lookup"><span data-stu-id="918d5-130">See Also</span></span>
[<span data-ttu-id="918d5-131">Managing Report Layouts</span><span class="sxs-lookup"><span data-stu-id="918d5-131">Managing Report Layouts</span></span>](ui-manage-report-layouts.md)  
<span data-ttu-id="918d5-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="918d5-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
