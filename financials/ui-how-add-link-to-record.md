---
title: How to Link from Records to External Information or Programs | Microsoft Docs
description: Attach a hyperlink to a document or website to a specific record, such as a customer or document.
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 8eee2a93a56c33fd5cefb70c475e237166017606
ms.contentlocale: en-gb
ms.lasthandoff: 11/10/2017

---
# <a name="adding-links-to-websites-documents-or-programs-on-records"></a><span data-ttu-id="ab0df-103">Adding Links to Websites, Documents, or Programs on Records</span><span class="sxs-lookup"><span data-stu-id="ab0df-103">Adding Links to Websites, Documents, or Programs on Records</span></span>
<span data-ttu-id="ab0df-104">On a specific record, such as a customer, document, or sales order, you can add a link to an external document, website, or programme.</span><span class="sxs-lookup"><span data-stu-id="ab0df-104">On a specific record, such as a customer, document, or sales order, you can add a link to an external document, website, or program.</span></span> <span data-ttu-id="ab0df-105">Or, you may want a link that opens a new empty email to a specific recipient when you select it.</span><span class="sxs-lookup"><span data-stu-id="ab0df-105">Or, you may want a link that opens a new empty email to a specific recipient when you select it.</span></span> <span data-ttu-id="ab0df-106">The card page for some records, such as customer and vendor cards, include a **Home Page** field where you can enter an Internet address (URL).</span><span class="sxs-lookup"><span data-stu-id="ab0df-106">The card page for some records, such as customer and vendor cards, include a **Home Page** field where you can enter an Internet address (URL).</span></span> <span data-ttu-id="ab0df-107">To include other links, you can use the method described in this article.</span><span class="sxs-lookup"><span data-stu-id="ab0df-107">To include other links, you can use the method described in this article.</span></span>

<span data-ttu-id="ab0df-108">Another example could be when you receive printed invoices from vendors.</span><span class="sxs-lookup"><span data-stu-id="ab0df-108">Another example could be when you receive printed invoices from vendors.</span></span> <span data-ttu-id="ab0df-109">You can scan them and store them as .pdf files on a SharePoint site.</span><span class="sxs-lookup"><span data-stu-id="ab0df-109">You can scan them and store them as .pdf files on a SharePoint site.</span></span> <span data-ttu-id="ab0df-110">Then you can make a link from a purchase invoice in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] to the corresponding invoice on  SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ab0df-110">Then you can make a link from a purchase invoice in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] to the corresponding invoice on  SharePoint.</span></span> <span data-ttu-id="ab0df-111">Or, you can make a link from an item card to the corresponding page in your vendor's online catalogue.</span><span class="sxs-lookup"><span data-stu-id="ab0df-111">Or, you can make a link from an item card to the corresponding page in your vendor's online catalog.</span></span>

## <a name="to-add-a-link-on-a-record"></a><span data-ttu-id="ab0df-112">To add a link on a record</span><span class="sxs-lookup"><span data-stu-id="ab0df-112">To add a link on a record</span></span>   

1.  <span data-ttu-id="ab0df-113">Open the record that you want to attach the link to, such as a customer card or sales order.</span><span class="sxs-lookup"><span data-stu-id="ab0df-113">Open the record that you want to attach the link to, such as a customer card or sales order.</span></span> <span data-ttu-id="ab0df-114">If you want to attach the link to a specific line, such as a journal line, select the line.</span><span class="sxs-lookup"><span data-stu-id="ab0df-114">If you want to attach the link to a specific line, such as a journal line, select the line.</span></span>  

2.  <span data-ttu-id="ab0df-115">Choose the **Links** action to open the **Links** windows that shows all the current links that are added to the record.</span><span class="sxs-lookup"><span data-stu-id="ab0df-115">Choose the **Links** action to open the **Links** windows that shows all the current links that are added to the record.</span></span>

3. <span data-ttu-id="ab0df-116">To add a new link, choose **+new**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-116">To add a new link, choose **+new**.</span></span>

4.  <span data-ttu-id="ab0df-117">In the **Link Address** field, enter</span><span class="sxs-lookup"><span data-stu-id="ab0df-117">In the **Link Address** field, enter</span></span>

    -   <span data-ttu-id="ab0df-118">To link to a file on your computer or network, enter the full path and file name, such as  **C:My Documentsinvoice1.doc**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-118">To link to a file on your computer or network, enter the full path and file name, such as  **C:My Documentsinvoice1.doc**.</span></span>
    -   <span data-ttu-id="ab0df-119">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-119">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span></span>
    -   <span data-ttu-id="ab0df-120">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-120">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span></span>
    -   <span data-ttu-id="ab0df-121">To link to a programme, enter a specific string to open the programme.</span><span class="sxs-lookup"><span data-stu-id="ab0df-121">To link to a program, enter a specific string to open the program.</span></span> <span data-ttu-id="ab0df-122">For example, to open OneNote with a specific page, enter **onenote:///C:My Documentstest.one**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-122">For example, to open OneNote with a specific page, enter **onenote:///C:My Documentstest.one**.</span></span> <span data-ttu-id="ab0df-123">Or, to open Outlook with a new empty email to a specific alias, enter **mailto:testalias**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-123">Or, to open Outlook with a new empty email to a specific alias, enter **mailto:testalias**.</span></span>  

5.  <span data-ttu-id="ab0df-124">Fill in the **Description** field with information about the link.</span><span class="sxs-lookup"><span data-stu-id="ab0df-124">Fill in the **Description** field with information about the link.</span></span>  

6.  <span data-ttu-id="ab0df-125">Choose the **Save** button.</span><span class="sxs-lookup"><span data-stu-id="ab0df-125">Choose the **Save** button.</span></span>  

## <a name="to-delete-a-link-from-a-record"></a><span data-ttu-id="ab0df-126">To delete a link from a record</span><span class="sxs-lookup"><span data-stu-id="ab0df-126">To delete a link from a record</span></span>  

<span data-ttu-id="ab0df-127">To delete a link, in the **Links** window, you can select **...** and then **Delete**.</span><span class="sxs-lookup"><span data-stu-id="ab0df-127">To delete a link, in the **Links** window, you can select **...** and then **Delete**.</span></span>

<span data-ttu-id="ab0df-128">If you delete a single record, such as a sales order line, a sales order, or a customer, then all the links attached to the record are deleted.</span><span class="sxs-lookup"><span data-stu-id="ab0df-128">If you delete a single record, such as a sales order line, a sales order, or a customer, then all the links attached to the record are deleted.</span></span> <span data-ttu-id="ab0df-129">However, if you delete records using a batch job, such as the **Delete Invoiced Sales Orders** batch job, then the links are still stored in the database.</span><span class="sxs-lookup"><span data-stu-id="ab0df-129">However, if you delete records using a batch job, such as the **Delete Invoiced Sales Orders** batch job, then the links are still stored in the database.</span></span> <span data-ttu-id="ab0df-130">To delete the links from the database, run the **Delete Orphaned Record Links** codeunit.</span><span class="sxs-lookup"><span data-stu-id="ab0df-130">To delete the links from the database, run the **Delete Orphaned Record Links** codeunit.</span></span> <span data-ttu-id="ab0df-131">To do this, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Orphaned Record Links**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="ab0df-131">To do this, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Orphaned Record Links**, and then choose the related link.</span></span>   

<!-- ### To run delete orphaned record links  

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Deletion**, and then choose the related link.  

2.  On the **Data Deletion** page, choose **Tasks**, and then choose **Delete Orphaned Record Links**.  -->

## <a name="see-also"></a><span data-ttu-id="ab0df-132">See Also</span><span class="sxs-lookup"><span data-stu-id="ab0df-132">See Also</span></span>  
<span data-ttu-id="ab0df-133">[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ab0df-133">[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  

