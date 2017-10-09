---
title: Define Business Relation Codes on Contacts| Microsoft Docs
description: Use business relations in Financials to help with marketing and to indicate the business relationship you have with your  prospects, clients, and customers, for example, a bank or service supplier.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, prospect, contact, client, customer
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 7d0f189ac233ea4da72136858a343dfaa7e88883
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-business-relations-on-contact-companies"></a><span data-ttu-id="c6d85-103">Setting Up Business Relations on Contact Companies</span><span class="sxs-lookup"><span data-stu-id="c6d85-103">Setting Up Business Relations on Contact Companies</span></span>
<span data-ttu-id="c6d85-104">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span><span class="sxs-lookup"><span data-stu-id="c6d85-104">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span></span>

<span data-ttu-id="c6d85-105">Using business relations on contacts is a two-step process.</span><span class="sxs-lookup"><span data-stu-id="c6d85-105">Using business relations on contacts is a two-step process.</span></span> <span data-ttu-id="c6d85-106">First, you define the business relation code.</span><span class="sxs-lookup"><span data-stu-id="c6d85-106">First, you define the business relation code.</span></span> <span data-ttu-id="c6d85-107">You only have to perform this step one time for each business relation.</span><span class="sxs-lookup"><span data-stu-id="c6d85-107">You only have to perform this step one time for each business relation.</span></span> <span data-ttu-id="c6d85-108">Once you have a business relation code, you can start to assign the code to contact companies.</span><span class="sxs-lookup"><span data-stu-id="c6d85-108">Once you have a business relation code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="c6d85-109">If you plan to synchronise your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span><span class="sxs-lookup"><span data-stu-id="c6d85-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-a-business-relation-code"></a><span data-ttu-id="c6d85-110">To define a business relation code</span><span class="sxs-lookup"><span data-stu-id="c6d85-110">To define a business relation code</span></span>
<span data-ttu-id="c6d85-111">The business relation code defines a category or type of the business relationship, such as BANK or Law.</span><span class="sxs-lookup"><span data-stu-id="c6d85-111">The business relation code defines a category or type of the business relationship, such as BANK or Law.</span></span> <span data-ttu-id="c6d85-112">You can have several business relation codes.</span><span class="sxs-lookup"><span data-stu-id="c6d85-112">You can have several business relation codes.</span></span> <span data-ttu-id="c6d85-113">To define the business relation, you use the **Business Relations** window.</span><span class="sxs-lookup"><span data-stu-id="c6d85-113">To define the business relation, you use the **Business Relations** window.</span></span>

1. <span data-ttu-id="c6d85-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Business Relations**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="c6d85-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Business Relations**, and then choose the related link.</span></span>
2. <span data-ttu-id="c6d85-115">Choose the **New** action, and fill in a code and description.</span><span class="sxs-lookup"><span data-stu-id="c6d85-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="c6d85-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span><span class="sxs-lookup"><span data-stu-id="c6d85-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <span data-ttu-id="c6d85-117"><a name="AssignBusRelContact"></a> To assign business relations to a contact</span><span class="sxs-lookup"><span data-stu-id="c6d85-117"><a name="AssignBusRelContact"></a> To assign business relations to a contact</span></span>
<span data-ttu-id="c6d85-118">You cannot assign business relations to a contact person - only companies.</span><span class="sxs-lookup"><span data-stu-id="c6d85-118">You cannot assign business relations to a contact person - only companies.</span></span>

1. <span data-ttu-id="c6d85-119">Open the contact.</span><span class="sxs-lookup"><span data-stu-id="c6d85-119">Open the contact.</span></span>
2. <span data-ttu-id="c6d85-120">Choose the **Company** action, and then the **Business Relations** action.</span><span class="sxs-lookup"><span data-stu-id="c6d85-120">Choose the **Company** action, and then the **Business Relations** action.</span></span>

    <span data-ttu-id="c6d85-121">The **Contact Business Relations** window opens.</span><span class="sxs-lookup"><span data-stu-id="c6d85-121">The **Contact Business Relations** window opens.</span></span>
3. <span data-ttu-id="c6d85-122">In the **Business Relation Code** field, select the business relation you want to assign.</span><span class="sxs-lookup"><span data-stu-id="c6d85-122">In the **Business Relation Code** field, select the business relation you want to assign.</span></span>

<span data-ttu-id="c6d85-123">Repeat these steps to assign as many business relations as you want.</span><span class="sxs-lookup"><span data-stu-id="c6d85-123">Repeat these steps to assign as many business relations as you want.</span></span> <span data-ttu-id="c6d85-124">You can also assign business relations from the contact list by following the same procedure.</span><span class="sxs-lookup"><span data-stu-id="c6d85-124">You can also assign business relations from the contact list by following the same procedure.</span></span>

<span data-ttu-id="c6d85-125">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section in the **Contact** window.</span><span class="sxs-lookup"><span data-stu-id="c6d85-125">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="c6d85-126">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span><span class="sxs-lookup"><span data-stu-id="c6d85-126">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="c6d85-127">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="c6d85-127">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="c6d85-128">See Also</span><span class="sxs-lookup"><span data-stu-id="c6d85-128">See Also</span></span>
[<span data-ttu-id="c6d85-129">Creating Contact Companies</span><span class="sxs-lookup"><span data-stu-id="c6d85-129">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="c6d85-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c6d85-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

