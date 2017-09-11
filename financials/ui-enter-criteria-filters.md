---
title: Defining Search Criteria in Filters | Microsoft Docs
description: Describes how to work with filters, such as the Quick Filter, to refine the results you get when you search for data.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 86ca45493081d9dbd229548f7c560e1df4e1c7c3
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017

---
# <a name="entering-criteria-in-filters"></a><span data-ttu-id="482ae-103">Entering Criteria in Filters</span><span class="sxs-lookup"><span data-stu-id="482ae-103">Entering Criteria in Filters</span></span>
<span data-ttu-id="482ae-104">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span><span class="sxs-lookup"><span data-stu-id="482ae-104">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="482ae-105">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span><span class="sxs-lookup"><span data-stu-id="482ae-105">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="482ae-106">In addition, you can use special symbols to further filter the results.</span><span class="sxs-lookup"><span data-stu-id="482ae-106">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="482ae-107">Searching using the Quick Filter</span><span class="sxs-lookup"><span data-stu-id="482ae-107">Searching using the Quick Filter</span></span>
<span data-ttu-id="482ae-108">You can add filters to all pages by using the Quick Filter.</span><span class="sxs-lookup"><span data-stu-id="482ae-108">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="482ae-109">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span><span class="sxs-lookup"><span data-stu-id="482ae-109">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="482ae-110">This filtering type is used for a fast entry of criteria.</span><span class="sxs-lookup"><span data-stu-id="482ae-110">This filtering type is used for a fast entry of criteria.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="482ae-111">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span><span class="sxs-lookup"><span data-stu-id="482ae-111">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="482ae-112">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span><span class="sxs-lookup"><span data-stu-id="482ae-112">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  

* <span data-ttu-id="482ae-113">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span><span class="sxs-lookup"><span data-stu-id="482ae-113">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
* <span data-ttu-id="482ae-114">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-114">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="482ae-115">Quick filter criteria</span><span class="sxs-lookup"><span data-stu-id="482ae-115">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="482ae-116">Search Criteria</span><span class="sxs-lookup"><span data-stu-id="482ae-116">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="482ae-117">Interpreted as...</span><span class="sxs-lookup"><span data-stu-id="482ae-117">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="482ae-118">Returns...</span><span class="sxs-lookup"><span data-stu-id="482ae-118">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="482ae-119">man</span><span class="sxs-lookup"><span data-stu-id="482ae-119">man</span></span></TD>
    <TD><span data-ttu-id="482ae-120">@&#42;man&#42;</span><span class="sxs-lookup"><span data-stu-id="482ae-120">@&#42;man&#42;</span></span></TD>
    <TD><span data-ttu-id="482ae-121">All records that contain the text <b>man</b> and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-121">All records that contain the text <b>man</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="482ae-122">se</span><span class="sxs-lookup"><span data-stu-id="482ae-122">se</span></span></TD>
    <TD><span data-ttu-id="482ae-123">@&#42;se&#42;</span><span class="sxs-lookup"><span data-stu-id="482ae-123">@&#42;se&#42;</span></span></TD>
    <TD><span data-ttu-id="482ae-124">All records that contain the text <b>se</b> and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-124">All records that contain the text <b>se</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="482ae-125">Man&#42;</span><span class="sxs-lookup"><span data-stu-id="482ae-125">Man&#42;</span></span></TD>
    <TD><span data-ttu-id="482ae-126">Starts with <b>Man</b> and case sensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-126">Starts with <b>Man</b> and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="482ae-127">All records that start with the text <b>Man</b>.</span><span class="sxs-lookup"><span data-stu-id="482ae-127">All records that start with the text <b>Man</b>.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="482ae-128">'man'</span><span class="sxs-lookup"><span data-stu-id="482ae-128">'man'</span></span></TD>
    <TD><span data-ttu-id="482ae-129">An exact text and case sensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-129">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="482ae-130">All records that match <b>man</b> exactly.</span><span class="sxs-lookup"><span data-stu-id="482ae-130">All records that match <b>man</b> exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="482ae-131">@man*</span><span class="sxs-lookup"><span data-stu-id="482ae-131">@man*</span></span> </TD>
    <TD><span data-ttu-id="482ae-132">Starts with and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-132">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="482ae-133">All records that start with <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="482ae-133">All records that start with <b>man</b>.</span></span></TD>
  </TR>
    <TR>
    <TD><span data-ttu-id="482ae-134">@&#42;man</span><span class="sxs-lookup"><span data-stu-id="482ae-134">@&#42;man</span></span></TD>
    <TD><span data-ttu-id="482ae-135">Ends with and case insensitive.</span><span class="sxs-lookup"><span data-stu-id="482ae-135">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="482ae-136">All records that end with <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="482ae-136">All records that end with <b>man</b>.</span></span></TD>
  </TR>
</TABLE>

> [!NOTE]  
>   <span data-ttu-id="482ae-137">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span><span class="sxs-lookup"><span data-stu-id="482ae-137">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="482ae-138">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span><span class="sxs-lookup"><span data-stu-id="482ae-138">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="482ae-139">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span><span class="sxs-lookup"><span data-stu-id="482ae-139">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="482ae-140">See Also</span><span class="sxs-lookup"><span data-stu-id="482ae-140">See Also</span></span>
<span data-ttu-id="482ae-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="482ae-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

