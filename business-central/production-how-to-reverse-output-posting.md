---
title: How to Reverse Output Posting | Microsoft Docs
description: There are times when output posting must be reversed. An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5901ad209149c113497d676a5c86379fc8424a0e
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5392756"
---
# <a name="reverse-output-posting"></a><span data-ttu-id="57578-104">Reverse Output Posting</span><span class="sxs-lookup"><span data-stu-id="57578-104">Reverse Output Posting</span></span>
<span data-ttu-id="57578-105">There are times when output posting must be reversed.</span><span class="sxs-lookup"><span data-stu-id="57578-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="57578-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span><span class="sxs-lookup"><span data-stu-id="57578-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="57578-107">To reverse an output posting</span><span class="sxs-lookup"><span data-stu-id="57578-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="57578-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="57578-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="57578-109">Select your batch.</span><span class="sxs-lookup"><span data-stu-id="57578-109">Select your batch.</span></span>  
2. <span data-ttu-id="57578-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="57578-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="57578-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="57578-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="57578-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span><span class="sxs-lookup"><span data-stu-id="57578-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="57578-113">This reverses the capacity and item ledger entries.</span><span class="sxs-lookup"><span data-stu-id="57578-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="57578-114">Post the reversal by posting the journal.</span><span class="sxs-lookup"><span data-stu-id="57578-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="57578-115">The output journal entries are posted to the item ledger as a positive adjustment.</span><span class="sxs-lookup"><span data-stu-id="57578-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="57578-116">See Also</span><span class="sxs-lookup"><span data-stu-id="57578-116">See Also</span></span>  
 <span data-ttu-id="57578-117">[Manufacturing](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="57578-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="57578-118">Setting Up Manufacturing</span><span class="sxs-lookup"><span data-stu-id="57578-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="57578-119">[Planning](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="57578-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="57578-120">Inventory</span><span class="sxs-lookup"><span data-stu-id="57578-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="57578-121">Purchasing</span><span class="sxs-lookup"><span data-stu-id="57578-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="57578-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="57578-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]