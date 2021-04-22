---
title: View Table Information
description: Learn how you can view information about the database tables right from the client interface in Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 7a01143dd7928d5996c1620676a758ea634bdf5d
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776898"
---
# <a name="viewing-table-information"></a><span data-ttu-id="a328c-103">Viewing Table Information</span><span class="sxs-lookup"><span data-stu-id="a328c-103">Viewing Table Information</span></span>

<span data-ttu-id="a328c-104">The page **8700 Table Information** provides information about all system and business tables in a Business Central solution.</span><span class="sxs-lookup"><span data-stu-id="a328c-104">The page **8700 Table Information** provides information about all system and business tables in a Business Central solution.</span></span> <span data-ttu-id="a328c-105">In particular, the page displays information about the amount of data the tables contain.</span><span class="sxs-lookup"><span data-stu-id="a328c-105">In particular, the page displays information about the amount of data the tables contain.</span></span>

<span data-ttu-id="a328c-106">This information is useful for troubleshooting performance problems, because let's you see the distribution of data size across tables.</span><span class="sxs-lookup"><span data-stu-id="a328c-106">This information is useful for troubleshooting performance problems, because let's you see the distribution of data size across tables.</span></span>

## <a name="viewing-table-information"></a><span data-ttu-id="a328c-107">Viewing table information</span><span class="sxs-lookup"><span data-stu-id="a328c-107">Viewing table information</span></span>

<span data-ttu-id="a328c-108">To open this page, select the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Table Information**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="a328c-108">To open this page, select the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Table Information**, and then choose the related link.</span></span>

<span data-ttu-id="a328c-109">The following table describes the information provided for each table:</span><span class="sxs-lookup"><span data-stu-id="a328c-109">The following table describes the information provided for each table:</span></span>

|<span data-ttu-id="a328c-110">Column</span><span class="sxs-lookup"><span data-stu-id="a328c-110">Column</span></span>|<span data-ttu-id="a328c-111">Description</span><span class="sxs-lookup"><span data-stu-id="a328c-111">Description</span></span>|
|------|-----------|
|<span data-ttu-id="a328c-112">Company Name</span><span class="sxs-lookup"><span data-stu-id="a328c-112">Company Name</span></span>|<span data-ttu-id="a328c-113">The name of the company, if any, that the table belongs to.</span><span class="sxs-lookup"><span data-stu-id="a328c-113">The name of the company, if any, that the table belongs to.</span></span>|
|<span data-ttu-id="a328c-114">Table Name</span><span class="sxs-lookup"><span data-stu-id="a328c-114">Table Name</span></span>|<span data-ttu-id="a328c-115">The name of the table.</span><span class="sxs-lookup"><span data-stu-id="a328c-115">The name of the table.</span></span>|
|<span data-ttu-id="a328c-116">Table No.</span><span class="sxs-lookup"><span data-stu-id="a328c-116">Table No.</span></span>|<span data-ttu-id="a328c-117">The ID of the table</span><span class="sxs-lookup"><span data-stu-id="a328c-117">The ID of the table</span></span>|
|<span data-ttu-id="a328c-118">No.</span><span class="sxs-lookup"><span data-stu-id="a328c-118">No.</span></span> <span data-ttu-id="a328c-119">of Records</span><span class="sxs-lookup"><span data-stu-id="a328c-119">of Records</span></span>|<span data-ttu-id="a328c-120">The total number of records stored in the table.</span><span class="sxs-lookup"><span data-stu-id="a328c-120">The total number of records stored in the table.</span></span>|
|<span data-ttu-id="a328c-121">Record Size</span><span class="sxs-lookup"><span data-stu-id="a328c-121">Record Size</span></span>|<span data-ttu-id="a328c-122">The average record size in KB/record.</span><span class="sxs-lookup"><span data-stu-id="a328c-122">The average record size in KB/record.</span></span> <span data-ttu-id="a328c-123">The value is calculated using the following formula: 1024(Size)/(No.</span><span class="sxs-lookup"><span data-stu-id="a328c-123">The value is calculated using the following formula: 1024(Size)/(No.</span></span> <span data-ttu-id="a328c-124">of Records)\`.</span><span class="sxs-lookup"><span data-stu-id="a328c-124">of Records)\`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="a328c-125">See Also</span><span class="sxs-lookup"><span data-stu-id="a328c-125">See Also</span></span>

[<span data-ttu-id="a328c-126">Inspecting Pages</span><span class="sxs-lookup"><span data-stu-id="a328c-126">Inspecting Pages</span></span>](across-inspect-page.md)  
[<span data-ttu-id="a328c-127">Performance Articles For Developers</span><span class="sxs-lookup"><span data-stu-id="a328c-127">Performance Articles For Developers</span></span>](/dynamics365/business-central/dev-itpro/performance/performance-developer)  


[!INCLUDE[footer-include](includes/footer-banner.md)]