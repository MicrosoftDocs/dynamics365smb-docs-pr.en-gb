---
title: How to Link from Records to External Information or Programs | Microsoft Docs
description: Attach a hyperlink to a document or website to a specific record, such as a customer or document.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/12/2019
ms.author: jswymer
ms.openlocfilehash: 781f43daf6482c7e29696dc7a03aa021550cde7d
ms.sourcegitcommit: f2e3b571eab6e01d9f5aa8ef47056b6bd313dcbd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/13/2019
ms.locfileid: "1629764"
---
# <a name="add-links-to-websites-documents-or-programs-on-records"></a><span data-ttu-id="2431e-103">Add Links to Websites, Documents, or Programmes on Records</span><span class="sxs-lookup"><span data-stu-id="2431e-103">Add Links to Websites, Documents, or Programs on Records</span></span>
<span data-ttu-id="2431e-104">On a specific record, such as a customer, document, or sales order, you can add a link to an external document, website, or programme.</span><span class="sxs-lookup"><span data-stu-id="2431e-104">On a specific record, such as a customer, document, or sales order, you can add a link to an external document, website, or program.</span></span> <span data-ttu-id="2431e-105">Or, you may want a link that opens a new empty email to a specific recipient when you select it.</span><span class="sxs-lookup"><span data-stu-id="2431e-105">Or, you may want a link that opens a new empty email to a specific recipient when you select it.</span></span> <span data-ttu-id="2431e-106">The card page for some records, such as customer and vendor cards, include a **Home Page** field where you can enter an Internet address (URL).</span><span class="sxs-lookup"><span data-stu-id="2431e-106">The card page for some records, such as customer and vendor cards, include a **Home Page** field where you can enter an Internet address (URL).</span></span> <span data-ttu-id="2431e-107">To include other links, you can use the method described in this article.</span><span class="sxs-lookup"><span data-stu-id="2431e-107">To include other links, you can use the method described in this article.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="2431e-108">Currently, this capability is available only in [!INCLUDE [prodshort](includes/prodshort.md)] on-premises deployments with the legacy Dynamics NAV Windows client.</span><span class="sxs-lookup"><span data-stu-id="2431e-108">Currently, this capability is available only in [!INCLUDE [prodshort](includes/prodshort.md)] on-premises deployments with the legacy Dynamics NAV Windows client.</span></span>  

<span data-ttu-id="2431e-109">Another example could be when you receive printed invoices from vendors.</span><span class="sxs-lookup"><span data-stu-id="2431e-109">Another example could be when you receive printed invoices from vendors.</span></span> <span data-ttu-id="2431e-110">You can scan them and store them as .pdf files on a SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="2431e-110">You can scan them and store them as .pdf files on a SharePoint site.</span></span> <span data-ttu-id="2431e-111">Then you can make a link from a purchase invoice in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] to the corresponding invoice on  SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2431e-111">Then you can make a link from a purchase invoice in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] to the corresponding invoice on  SharePoint.</span></span> <span data-ttu-id="2431e-112">Or, you can make a link from an item card to the corresponding page in your vendor's online catalogue.</span><span class="sxs-lookup"><span data-stu-id="2431e-112">Or, you can make a link from an item card to the corresponding page in your vendor's online catalog.</span></span>

## <a name="to-add-a-link-on-a-record"></a><span data-ttu-id="2431e-113">To add a link on a record</span><span class="sxs-lookup"><span data-stu-id="2431e-113">To add a link on a record</span></span>   

1.  <span data-ttu-id="2431e-114">Open the record that you want to attach the link to, such as a customer card or sales order.</span><span class="sxs-lookup"><span data-stu-id="2431e-114">Open the record that you want to attach the link to, such as a customer card or sales order.</span></span> <span data-ttu-id="2431e-115">If you want to attach the link to a specific line, such as a journal line, select the line.</span><span class="sxs-lookup"><span data-stu-id="2431e-115">If you want to attach the link to a specific line, such as a journal line, select the line.</span></span>  

2.  <span data-ttu-id="2431e-116">Choose the **Links** action to open the **Links** pages that shows all the current links that are added to the record.</span><span class="sxs-lookup"><span data-stu-id="2431e-116">Choose the **Links** action to open the **Links** pages that shows all the current links that are added to the record.</span></span>

3. <span data-ttu-id="2431e-117">To add a new link, choose **+new**.</span><span class="sxs-lookup"><span data-stu-id="2431e-117">To add a new link, choose **+new**.</span></span>

4.  <span data-ttu-id="2431e-118">In the **Link Address** field, enter</span><span class="sxs-lookup"><span data-stu-id="2431e-118">In the **Link Address** field, enter</span></span>

    -   <span data-ttu-id="2431e-119">To link to a file on your computer or network, enter the full path and file name, such as  **C:\My Documents\invoice1.doc**.</span><span class="sxs-lookup"><span data-stu-id="2431e-119">To link to a file on your computer or network, enter the full path and file name, such as  **C:\My Documents\invoice1.doc**.</span></span>
    -   <span data-ttu-id="2431e-120">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span><span class="sxs-lookup"><span data-stu-id="2431e-120">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span></span>
    -   <span data-ttu-id="2431e-121">To link to a programme, enter a specific string to open the programme.</span><span class="sxs-lookup"><span data-stu-id="2431e-121">To link to a program, enter a specific string to open the program.</span></span> <span data-ttu-id="2431e-122">For example, to open OneNote with a specific page, enter **onenote:///C:\My Documents/test.one**.</span><span class="sxs-lookup"><span data-stu-id="2431e-122">For example, to open OneNote with a specific page, enter **onenote:///C:\My Documents/test.one**.</span></span> <span data-ttu-id="2431e-123">Or, to open Outlook with a new empty email to a specific alias, enter **mailto:testalias**.</span><span class="sxs-lookup"><span data-stu-id="2431e-123">Or, to open Outlook with a new empty email to a specific alias, enter **mailto:testalias**.</span></span>  

5.  <span data-ttu-id="2431e-124">Fill in the **Description** field with information about the link.</span><span class="sxs-lookup"><span data-stu-id="2431e-124">Fill in the **Description** field with information about the link.</span></span>  

6.  <span data-ttu-id="2431e-125">Choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="2431e-125">Choose the **Save** button.</span></span>  

## <a name="to-delete-a-link-from-a-record"></a><span data-ttu-id="2431e-126">To delete a link from a record</span><span class="sxs-lookup"><span data-stu-id="2431e-126">To delete a link from a record</span></span>  

<span data-ttu-id="2431e-127">To delete a link, on the **Links** page, you can select **...** and then **Delete**.</span><span class="sxs-lookup"><span data-stu-id="2431e-127">To delete a link, on the **Links** page, you can select **...** and then **Delete**.</span></span>

<span data-ttu-id="2431e-128">If you delete a single record, such as a sales order line, a sales order, or a customer, then all the links attached to the record are deleted.</span><span class="sxs-lookup"><span data-stu-id="2431e-128">If you delete a single record, such as a sales order line, a sales order, or a customer, then all the links attached to the record are deleted.</span></span> <span data-ttu-id="2431e-129">However, if you delete records using a batch job, such as the **Delete Invoiced Sales Orders** batch job, then the links are still stored in the database.</span><span class="sxs-lookup"><span data-stu-id="2431e-129">However, if you delete records using a batch job, such as the **Delete Invoiced Sales Orders** batch job, then the links are still stored in the database.</span></span> <span data-ttu-id="2431e-130">To delete the links from the database, run the **Delete Orphaned Record Links** codeunit.</span><span class="sxs-lookup"><span data-stu-id="2431e-130">To delete the links from the database, run the **Delete Orphaned Record Links** codeunit.</span></span> <span data-ttu-id="2431e-131">To do this, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Orphaned Record Links**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="2431e-131">To do this, choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Orphaned Record Links**, and then choose the related link.</span></span>   

<!-- ### To run delete orphaned record links  

1.  Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Deletion**, and then choose the related link.  

2.  On the **Data Deletion** page, choose **Tasks**, and then choose **Delete Orphaned Record Links**.  -->

## <a name="see-also"></a><span data-ttu-id="2431e-132">See Also</span><span class="sxs-lookup"><span data-stu-id="2431e-132">See Also</span></span>  
<span data-ttu-id="2431e-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2431e-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
