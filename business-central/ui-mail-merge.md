---
title: Using Word Templates for Bulk Communications | Microsoft Docs
description: Word templates can make it easy to bulk create documents that are personalised for specific entities.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: document, mail, merge, Word, template, email
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 118d8db1266bb7150965ec4d1ce44ece77638764
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788604"
---
# <a name="using-word-templates-for-bulk-communication"></a><span data-ttu-id="a46f0-103">Using Word Templates for Bulk Communication</span><span class="sxs-lookup"><span data-stu-id="a46f0-103">Using Word Templates for Bulk Communication</span></span>
<span data-ttu-id="a46f0-104">Microsoft Word templates can make it easier to mass communicate with entities such as customers and vendors.</span><span class="sxs-lookup"><span data-stu-id="a46f0-104">Microsoft Word templates can make it easier to mass communicate with entities such as customers and vendors.</span></span> <span data-ttu-id="a46f0-105">For example, you can create brochures to alert customers about a sales campaign, letters to inform vendors about a new purchasing policy, or invitations to attract contacts to an upcoming event.</span><span class="sxs-lookup"><span data-stu-id="a46f0-105">For example, you can create brochures to alert customers about a sales campaign, letters to inform vendors about a new purchasing policy, or invitations to attract contacts to an upcoming event.</span></span>

<span data-ttu-id="a46f0-106">You can use entities in [!INCLUDE[prod_short](includes/prod_short.md)] as the data source for the template, and add merge fields to personalise documents for each entity.</span><span class="sxs-lookup"><span data-stu-id="a46f0-106">You can use entities in [!INCLUDE[prod_short](includes/prod_short.md)] as the data source for the template, and add merge fields to personalize documents for each entity.</span></span> <span data-ttu-id="a46f0-107">The merge fields come from the entity in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="a46f0-107">The merge fields come from the entity in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="a46f0-108">When you apply a Word template to an entity, data from the merge fields is inserted in the document.</span><span class="sxs-lookup"><span data-stu-id="a46f0-108">When you apply a Word template to an entity, data from the merge fields is inserted in the document.</span></span>

<span data-ttu-id="a46f0-109">On the **Word Templates** page, you can use an assisted setup guide to download a ZIP file that contains a DataSource.txt and a Word template file for an entity.</span><span class="sxs-lookup"><span data-stu-id="a46f0-109">On the **Word Templates** page, you can use an assisted setup guide to download a ZIP file that contains a DataSource.txt and a Word template file for an entity.</span></span> <span data-ttu-id="a46f0-110">After you set up the template and add merge fields, you use the same guide to upload the template.</span><span class="sxs-lookup"><span data-stu-id="a46f0-110">After you set up the template and add merge fields, you use the same guide to upload the template.</span></span> <span data-ttu-id="a46f0-111">You can only use the Word template and data source files that you download from [!INCLUDE[prod_short](includes/prod_short.md)], and you must store the files in the same location.</span><span class="sxs-lookup"><span data-stu-id="a46f0-111">You can only use the Word template and data source files that you download from [!INCLUDE[prod_short](includes/prod_short.md)], and you must store the files in the same location.</span></span>

> [!NOTE]
> <span data-ttu-id="a46f0-112">When you choose an entity for which to create a template, the list shows all entities in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="a46f0-112">When you choose an entity for which to create a template, the list shows all entities in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="a46f0-113">However, you cannot create templates for all entities.</span><span class="sxs-lookup"><span data-stu-id="a46f0-113">However, you cannot create templates for all entities.</span></span> <span data-ttu-id="a46f0-114">If the name of an entity contains special characters, such as **/**, **.**, **_**, or **-**, you cannot create a template for it.</span><span class="sxs-lookup"><span data-stu-id="a46f0-114">If the name of an entity contains special characters, such as **/**, **.**, **_**, or **-**, you cannot create a template for it.</span></span> <span data-ttu-id="a46f0-115">The name of the entity is shown in the **Object Caption** column.</span><span class="sxs-lookup"><span data-stu-id="a46f0-115">The name of the entity is shown in the **Object Caption** column.</span></span>

<span data-ttu-id="a46f0-116">When you are setting up the template in Word, on the **Mailings** tab you can add merge fields by choosing **Insert Merge Field**.</span><span class="sxs-lookup"><span data-stu-id="a46f0-116">When you are setting up the template in Word, on the **Mailings** tab you can add merge fields by choosing **Insert Merge Field**.</span></span>

> [!NOTE]
> <span data-ttu-id="a46f0-117">You cannot use merge fields if the name of the field contains 40 characters or more.</span><span class="sxs-lookup"><span data-stu-id="a46f0-117">You cannot use merge fields if the name of the field contains 40 characters or more.</span></span> <span data-ttu-id="a46f0-118">For example, you cannot use the Company__Information_Customs_Permit_Date field because it has 40 characters.</span><span class="sxs-lookup"><span data-stu-id="a46f0-118">For example, you cannot use the Company__Information_Customs_Permit_Date field because it has 40 characters.</span></span> 

<span data-ttu-id="a46f0-119">When your Word template is ready, on the **Word Templates** page you can choose **Apply** to generate the documents.</span><span class="sxs-lookup"><span data-stu-id="a46f0-119">When your Word template is ready, on the **Word Templates** page you can choose **Apply** to generate the documents.</span></span> <span data-ttu-id="a46f0-120">You can either create one document that contains sections for each entity, or split the operation to create a new document for each entity.</span><span class="sxs-lookup"><span data-stu-id="a46f0-120">You can either create one document that contains sections for each entity, or split the operation to create a new document for each entity.</span></span>

## <a name="to-create-a-word-template"></a><span data-ttu-id="a46f0-121">To create a Word template</span><span class="sxs-lookup"><span data-stu-id="a46f0-121">To create a Word template</span></span>
1. <span data-ttu-id="a46f0-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Word Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a46f0-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Word Templates**, and then choose the related link.</span></span>
2. <span data-ttu-id="a46f0-123">Follow the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="a46f0-123">Follow the steps in the assisted setup guide.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a><span data-ttu-id="a46f0-124">See Also</span><span class="sxs-lookup"><span data-stu-id="a46f0-124">See Also</span></span>
[<span data-ttu-id="a46f0-125">Managing Report and Document Layouts</span><span class="sxs-lookup"><span data-stu-id="a46f0-125">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
