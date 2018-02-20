---
title: Manage, delete, or compress documents | Microsoft Docs
description: Keep your historical data or delete it.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 60438f0b6f0d5da60925b5b9c309cc359a8422e3
ms.contentlocale: en-gb
ms.lasthandoff: 01/30/2018

---
# <a name="manage-documents"></a><span data-ttu-id="685d6-103">Manage Documents</span><span class="sxs-lookup"><span data-stu-id="685d6-103">Manage Documents</span></span>
<span data-ttu-id="685d6-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span><span class="sxs-lookup"><span data-stu-id="685d6-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span></span>  

## <a name="delete-documents"></a><span data-ttu-id="685d6-105">Delete Documents</span><span class="sxs-lookup"><span data-stu-id="685d6-105">Delete Documents</span></span>
<span data-ttu-id="685d6-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span><span class="sxs-lookup"><span data-stu-id="685d6-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="685d6-107"> checks that you have fully invoiced the deleted purchase orders.</span><span class="sxs-lookup"><span data-stu-id="685d6-107"> checks that you have fully invoiced the deleted purchase orders.</span></span> <span data-ttu-id="685d6-108">You cannot delete orders that you have not fully invoiced and received.</span><span class="sxs-lookup"><span data-stu-id="685d6-108">You cannot delete orders that you have not fully invoiced and received.</span></span>  

<span data-ttu-id="685d6-109">Return orders are usually deleted after they are invoiced.</span><span class="sxs-lookup"><span data-stu-id="685d6-109">Return orders are usually deleted after they are invoiced.</span></span> <span data-ttu-id="685d6-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** window.</span><span class="sxs-lookup"><span data-stu-id="685d6-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** window.</span></span> <span data-ttu-id="685d6-111">If you selected the **Return Shipment on Credit Memo** check box in the **Purchases & Payable Setup** window, then the invoice is transferred to the **Posted Return Shipment** window.</span><span class="sxs-lookup"><span data-stu-id="685d6-111">If you selected the **Return Shipment on Credit Memo** check box in the **Purchases & Payable Setup** window, then the invoice is transferred to the **Posted Return Shipment** window.</span></span> <span data-ttu-id="685d6-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="685d6-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span></span> <span data-ttu-id="685d6-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span><span class="sxs-lookup"><span data-stu-id="685d6-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span></span>  

<span data-ttu-id="685d6-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span><span class="sxs-lookup"><span data-stu-id="685d6-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span></span> <span data-ttu-id="685d6-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="685d6-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span></span>  

<span data-ttu-id="685d6-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span><span class="sxs-lookup"><span data-stu-id="685d6-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="685d6-117">When an invoice is posted, a corresponding entry is created in the **Posted Service Invoices** window.</span><span class="sxs-lookup"><span data-stu-id="685d6-117">When an invoice is posted, a corresponding entry is created in the **Posted Service Invoices** window.</span></span> <span data-ttu-id="685d6-118">The posted document can be viewed in the **Posted Service Invoice** window.</span><span class="sxs-lookup"><span data-stu-id="685d6-118">The posted document can be viewed in the **Posted Service Invoice** window.</span></span>  

<span data-ttu-id="685d6-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** window.</span><span class="sxs-lookup"><span data-stu-id="685d6-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** window.</span></span> <span data-ttu-id="685d6-120">Then you may need to delete invoiced orders that were not deleted.</span><span class="sxs-lookup"><span data-stu-id="685d6-120">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="685d6-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="685d6-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="685d6-122">See Also</span><span class="sxs-lookup"><span data-stu-id="685d6-122">See Also</span></span>  
[<span data-ttu-id="685d6-123">Setup and Administration in Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="685d6-123">Setup and Administration in Finance and Operations, Business edition</span></span>](admin-setup-and-administration.md)  

