---
title: Tips and Tricks - RapidStart Services | Microsoft Docs
description: When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: e301d788fdedacf0fc2ac3ce29946df965bed711
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777073"
---
# <a name="tips-and-tricks-rapidstart-services"></a><span data-ttu-id="b404c-103">Tips and Tricks: RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="b404c-103">Tips and Tricks: RapidStart Services</span></span>

<span data-ttu-id="b404c-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span><span class="sxs-lookup"><span data-stu-id="b404c-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span></span>  

## <a name="take-advantage-of-configuration-templates"></a><span data-ttu-id="b404c-105">Take advantage of configuration templates</span><span class="sxs-lookup"><span data-stu-id="b404c-105">Take advantage of configuration templates</span></span>

<span data-ttu-id="b404c-106">Configuration templates can help you streamline your implementation process.</span><span class="sxs-lookup"><span data-stu-id="b404c-106">Configuration templates can help you streamline your implementation process.</span></span> <span data-ttu-id="b404c-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span><span class="sxs-lookup"><span data-stu-id="b404c-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span></span> <span data-ttu-id="b404c-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span><span class="sxs-lookup"><span data-stu-id="b404c-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span></span>  

## <a name="configuration-questionnaires"></a><span data-ttu-id="b404c-109">Configuration questionnaires</span><span class="sxs-lookup"><span data-stu-id="b404c-109">Configuration questionnaires</span></span>

<span data-ttu-id="b404c-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span><span class="sxs-lookup"><span data-stu-id="b404c-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span></span>  

## <a name="batch-creation-of-journal-lines"></a><span data-ttu-id="b404c-111">Batch creation of journal lines</span><span class="sxs-lookup"><span data-stu-id="b404c-111">Batch creation of journal lines</span></span>

<span data-ttu-id="b404c-112">We recommend that you use the data migration tools provided to migrate journal entries.</span><span class="sxs-lookup"><span data-stu-id="b404c-112">We recommend that you use the data migration tools provided to migrate journal entries.</span></span> <span data-ttu-id="b404c-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span><span class="sxs-lookup"><span data-stu-id="b404c-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span></span> <span data-ttu-id="b404c-114">The rest of the journal then has to be completed manually.</span><span class="sxs-lookup"><span data-stu-id="b404c-114">The rest of the journal then has to be completed manually.</span></span>  

## <a name="migrating-transactions"></a><span data-ttu-id="b404c-115">Migrating transactions</span><span class="sxs-lookup"><span data-stu-id="b404c-115">Migrating transactions</span></span>

<span data-ttu-id="b404c-116">We recommend that you migrate opening balances in the following order.</span><span class="sxs-lookup"><span data-stu-id="b404c-116">We recommend that you migrate opening balances in the following order.</span></span> <!--Be aware that you cannot insert ledger entries directly. Instead you must use journals to post the journal lines-->

1. <span data-ttu-id="b404c-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span><span class="sxs-lookup"><span data-stu-id="b404c-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span></span> <span data-ttu-id="b404c-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span><span class="sxs-lookup"><span data-stu-id="b404c-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span></span> <span data-ttu-id="b404c-119">Set up the offsetting accounts to enable direct postings.</span><span class="sxs-lookup"><span data-stu-id="b404c-119">Set up the offsetting accounts to enable direct postings.</span></span>  
2. <span data-ttu-id="b404c-120">Migrate open customer ledger entries.</span><span class="sxs-lookup"><span data-stu-id="b404c-120">Migrate open customer ledger entries.</span></span>  <!--work on these-->
3. <span data-ttu-id="b404c-121">Migrate open item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="b404c-121">Migrate open item ledger entries.</span></span>  
4. <span data-ttu-id="b404c-122">Migrate open fixed asset entries.</span><span class="sxs-lookup"><span data-stu-id="b404c-122">Migrate open fixed asset entries.</span></span>  

## <a name="make-each-package-manageable"></a><span data-ttu-id="b404c-123">Make each package manageable</span><span class="sxs-lookup"><span data-stu-id="b404c-123">Make each package manageable</span></span>

<span data-ttu-id="b404c-124">When you use configuration packages to migrate data, separate the data into separate packages for easier portability.</span><span class="sxs-lookup"><span data-stu-id="b404c-124">When you use configuration packages to migrate data, separate the data into separate packages for easier portability.</span></span> <span data-ttu-id="b404c-125">For example, if you want to migrate 20 years of ledger entries, the import might take many hours and days.</span><span class="sxs-lookup"><span data-stu-id="b404c-125">For example, if you want to migrate 20 years of ledger entries, the import might take many hours and days.</span></span> <span data-ttu-id="b404c-126">Instead, split the data up so that each package becomes more manageable.</span><span class="sxs-lookup"><span data-stu-id="b404c-126">Instead, split the data up so that each package becomes more manageable.</span></span> <span data-ttu-id="b404c-127">Currently, there are no firm rules for what makes a package performant, but if you see problems importing or exporting a package, try making it smaller and see if that helps.</span><span class="sxs-lookup"><span data-stu-id="b404c-127">Currently, there are no firm rules for what makes a package performant, but if you see problems importing or exporting a package, try making it smaller and see if that helps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b404c-128">See Also</span><span class="sxs-lookup"><span data-stu-id="b404c-128">See Also</span></span>

[<span data-ttu-id="b404c-129">Setting Up a Company With RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="b404c-129">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="b404c-130">Administration</span><span class="sxs-lookup"><span data-stu-id="b404c-130">Administration</span></span>](admin-setup-and-administration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]