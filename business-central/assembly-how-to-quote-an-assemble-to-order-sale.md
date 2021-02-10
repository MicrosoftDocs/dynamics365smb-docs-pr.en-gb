---
title: How to Quote an Assemble-to-Order Sale | Microsoft Docs
description: You can use assembly management to customise an assembly item to a customer’s request during the sales process.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: kit, kitting
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 323466061d845e04a38ba660b38dd21483bcb8c1
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749600"
---
# <a name="quote-an-assemble-to-order-sale"></a><span data-ttu-id="7d903-103">Quote an Assemble-to-Order Sale</span><span class="sxs-lookup"><span data-stu-id="7d903-103">Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="7d903-104">You can use assembly management to customise an assembly item to a customer’s request during the sales process.</span><span class="sxs-lookup"><span data-stu-id="7d903-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="7d903-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="7d903-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="7d903-106">As when you sell any other type of item, you can also create a sales quote for a customised assembly item before converting it to a sales order.</span><span class="sxs-lookup"><span data-stu-id="7d903-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="7d903-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span><span class="sxs-lookup"><span data-stu-id="7d903-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="7d903-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span><span class="sxs-lookup"><span data-stu-id="7d903-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="7d903-109">To create a sales quote for an assemble-to-order item</span><span class="sxs-lookup"><span data-stu-id="7d903-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="7d903-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Quote**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="7d903-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="7d903-111">Create a sales quote line with one line for an assembly item.</span><span class="sxs-lookup"><span data-stu-id="7d903-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="7d903-112">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="7d903-112">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="7d903-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span><span class="sxs-lookup"><span data-stu-id="7d903-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="7d903-114">You should not quote a partial quantity.</span><span class="sxs-lookup"><span data-stu-id="7d903-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="7d903-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span><span class="sxs-lookup"><span data-stu-id="7d903-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="7d903-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span><span class="sxs-lookup"><span data-stu-id="7d903-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="7d903-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span><span class="sxs-lookup"><span data-stu-id="7d903-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="7d903-118">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the quote that the customer is requesting.</span><span class="sxs-lookup"><span data-stu-id="7d903-118">On the **Assemble-to-Order Lines** page, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="7d903-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span><span class="sxs-lookup"><span data-stu-id="7d903-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="7d903-120">You cannot change the contents of most fields, and you cannot post.</span><span class="sxs-lookup"><span data-stu-id="7d903-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="7d903-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** page to return to the **Sales Quote** page.</span><span class="sxs-lookup"><span data-stu-id="7d903-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** page to return to the **Sales Quote** page.</span></span>  
7.  <span data-ttu-id="7d903-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span><span class="sxs-lookup"><span data-stu-id="7d903-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="7d903-123">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="7d903-123">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span> <span data-ttu-id="7d903-124">The linked assembly quote and any customisations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span><span class="sxs-lookup"><span data-stu-id="7d903-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7d903-125">See Also</span><span class="sxs-lookup"><span data-stu-id="7d903-125">See Also</span></span>  
[<span data-ttu-id="7d903-126">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="7d903-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="7d903-127">Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="7d903-127">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="7d903-128">Inventory</span><span class="sxs-lookup"><span data-stu-id="7d903-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="7d903-129">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="7d903-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="7d903-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7d903-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
