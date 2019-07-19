---
title: Specify the Layout of a Cheque| Microsoft Docs
description: You can design and print your cheques in different formats to conform with standards.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 06/24/2019
ms.author: edupont
ms.openlocfilehash: 6ba5b6f0f91e207ec8ffedf5b45003a5787b9e0f
ms.sourcegitcommit: 0854c074b500c3031eaf86fde9d452f93f238081
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/24/2019
ms.locfileid: "1701136"
---
# <a name="select-a-check-layout"></a><span data-ttu-id="00326-103">Select a Cheque Layout</span><span class="sxs-lookup"><span data-stu-id="00326-103">Select a Check Layout</span></span>
<span data-ttu-id="00326-104">You can design your cheques to conform with the standards set by the local authorities.</span><span class="sxs-lookup"><span data-stu-id="00326-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="00326-105">Cheque images can be printed in English, French, or Spanish.</span><span class="sxs-lookup"><span data-stu-id="00326-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="00326-106">Cheques are designed to print in both the United States and Canadian cheque image formats in either a cheque-stub-cheque format or a stub-stub-cheque format.</span><span class="sxs-lookup"><span data-stu-id="00326-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-select-a-check-layout"></a><span data-ttu-id="00326-107">To select a cheque layout</span><span class="sxs-lookup"><span data-stu-id="00326-107">To select a check layout</span></span>
1. <span data-ttu-id="00326-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="00326-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="00326-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Cheque**.</span><span class="sxs-lookup"><span data-stu-id="00326-109">On the **Report Selection - Bank Acc.** page, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="00326-110">Select one of the following report IDs.</span><span class="sxs-lookup"><span data-stu-id="00326-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="00326-111">Report ID</span><span class="sxs-lookup"><span data-stu-id="00326-111">Report ID</span></span> | <span data-ttu-id="00326-112">Report Name</span><span class="sxs-lookup"><span data-stu-id="00326-112">Report Name</span></span> | <span data-ttu-id="00326-113">Description</span><span class="sxs-lookup"><span data-stu-id="00326-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="00326-114">1401</span><span class="sxs-lookup"><span data-stu-id="00326-114">1401</span></span> |<span data-ttu-id="00326-115">Cheque</span><span class="sxs-lookup"><span data-stu-id="00326-115">Check</span></span> |<span data-ttu-id="00326-116">This is the default report.</span><span class="sxs-lookup"><span data-stu-id="00326-116">This is the default report.</span></span> |
| <span data-ttu-id="00326-117">10411</span><span class="sxs-lookup"><span data-stu-id="00326-117">10411</span></span> |<span data-ttu-id="00326-118">Cheque (Stub/Stub/Cheque)</span><span class="sxs-lookup"><span data-stu-id="00326-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="00326-119">This report is designed to print cheques in a stub/stub/cheque format.</span><span class="sxs-lookup"><span data-stu-id="00326-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="00326-120">10412</span><span class="sxs-lookup"><span data-stu-id="00326-120">10412</span></span> |<span data-ttu-id="00326-121">Cheque (Stub/Cheque/Stub)</span><span class="sxs-lookup"><span data-stu-id="00326-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="00326-122">This report is designed to print cheques in a stub/cheque/stub format.</span><span class="sxs-lookup"><span data-stu-id="00326-122">This report is designed to print checks in a stub/check/stub format.</span></span> |
| <span data-ttu-id="00326-123">10413</span><span class="sxs-lookup"><span data-stu-id="00326-123">10413</span></span> |<span data-ttu-id="00326-124">Three Cheques per Page</span><span class="sxs-lookup"><span data-stu-id="00326-124">Three Checks per Page</span></span> |<span data-ttu-id="00326-125">This report is designed to print three cheques on each page.</span><span class="sxs-lookup"><span data-stu-id="00326-125">This report is designed to print three checks on each page.</span></span> |

<span data-ttu-id="00326-126">When you have set up cheque layouts, you can print cheques from the **Payment Journal** page.</span><span class="sxs-lookup"><span data-stu-id="00326-126">When you have set up check layouts, you can print checks from the **Payment Journal** page.</span></span> <span data-ttu-id="00326-127">For more information, see [Work with Cheques](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="00326-127">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

<span data-ttu-id="00326-128">To change one of these default cheque layouts, use either the Word or the RDLC integration to do so.</span><span class="sxs-lookup"><span data-stu-id="00326-128">To change one of these default check layouts, use either the Word or the RDLC integration to do so.</span></span> <span data-ttu-id="00326-129">For more information, see [Create and Modify a Custom Report or Document Layout](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="00326-129">For more information, see [Create and Modify a Custom Report or Document Layout](ui-how-create-custom-report-layout.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="00326-130">See Also</span><span class="sxs-lookup"><span data-stu-id="00326-130">See Also</span></span>
[<span data-ttu-id="00326-131">Create and Modify a Custom Report or Document Layout</span><span class="sxs-lookup"><span data-stu-id="00326-131">Create and Modify a Custom Report or Document Layout</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="00326-132">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="00326-132">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="00326-133">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="00326-133">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="00326-134">Completing Period-End Processes</span><span class="sxs-lookup"><span data-stu-id="00326-134">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="00326-135">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="00326-135">[Working with [!INCLUDE[prodshort](includes/prodshort.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="00326-136">General Business Functionality</span><span class="sxs-lookup"><span data-stu-id="00326-136">General Business Functionality</span></span>](ui-across-business-areas.md)
