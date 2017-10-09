---
title: How to Quote an Assemble-to-Order Sale | Microsoft Docs
description: "You can use assembly management to customise an assembly item to a customer’s request during the sales process."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7602b067e4b3fc99815a581c851138d7cc3ff41e
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a><span data-ttu-id="6567f-103">How to: Quote an Assemble-to-Order Sale</span><span class="sxs-lookup"><span data-stu-id="6567f-103">How to: Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="6567f-104">You can use assembly management to customise an assembly item to a customer’s request during the sales process.</span><span class="sxs-lookup"><span data-stu-id="6567f-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="6567f-105">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="6567f-105">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="6567f-106">As when you sell any other type of item, you can also create a sales quote for a customised assembly item before converting it to a sales order.</span><span class="sxs-lookup"><span data-stu-id="6567f-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="6567f-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span><span class="sxs-lookup"><span data-stu-id="6567f-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="6567f-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span><span class="sxs-lookup"><span data-stu-id="6567f-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="6567f-109">To create a sales quote for an assemble-to-order item</span><span class="sxs-lookup"><span data-stu-id="6567f-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="6567f-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="6567f-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6567f-111">Create a sales quote line with one line for an assembly item.</span><span class="sxs-lookup"><span data-stu-id="6567f-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="6567f-112">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="6567f-112">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="6567f-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span><span class="sxs-lookup"><span data-stu-id="6567f-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="6567f-114">You should not quote a partial quantity.</span><span class="sxs-lookup"><span data-stu-id="6567f-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="6567f-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span><span class="sxs-lookup"><span data-stu-id="6567f-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="6567f-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span><span class="sxs-lookup"><span data-stu-id="6567f-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="6567f-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span><span class="sxs-lookup"><span data-stu-id="6567f-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="6567f-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span><span class="sxs-lookup"><span data-stu-id="6567f-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="6567f-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span><span class="sxs-lookup"><span data-stu-id="6567f-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="6567f-120">You cannot change the contents of most fields, and you cannot post.</span><span class="sxs-lookup"><span data-stu-id="6567f-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="6567f-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span><span class="sxs-lookup"><span data-stu-id="6567f-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="6567f-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span><span class="sxs-lookup"><span data-stu-id="6567f-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="6567f-123">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="6567f-123">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span> <span data-ttu-id="6567f-124">The linked assembly quote and any customisations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span><span class="sxs-lookup"><span data-stu-id="6567f-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6567f-125">See Also</span><span class="sxs-lookup"><span data-stu-id="6567f-125">See Also</span></span>  
[<span data-ttu-id="6567f-126">Assembly Management</span><span class="sxs-lookup"><span data-stu-id="6567f-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="6567f-127">How to: Work with Bills of Material</span><span class="sxs-lookup"><span data-stu-id="6567f-127">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="6567f-128">Inventory</span><span class="sxs-lookup"><span data-stu-id="6567f-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="6567f-129">Design Details: Warehouse Management</span><span class="sxs-lookup"><span data-stu-id="6567f-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="6567f-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6567f-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

