---
title: Manage, delete, or compress documents | Microsoft Docs
description: Keep your historical data or delete it.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 5cc49d8b17a56c8f19926cf33e63467005d4788c
ms.contentlocale: en-gb
ms.lasthandoff: 11/26/2018

---
# <a name="manage-documents"></a><span data-ttu-id="20d26-103">Manage Documents</span><span class="sxs-lookup"><span data-stu-id="20d26-103">Manage Documents</span></span>
<span data-ttu-id="20d26-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span><span class="sxs-lookup"><span data-stu-id="20d26-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span></span>  

## <a name="delete-documents"></a><span data-ttu-id="20d26-105">Delete Documents</span><span class="sxs-lookup"><span data-stu-id="20d26-105">Delete Documents</span></span>
<span data-ttu-id="20d26-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span><span class="sxs-lookup"><span data-stu-id="20d26-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="20d26-107">checks that you have fully invoiced the deleted purchase orders.</span><span class="sxs-lookup"><span data-stu-id="20d26-107">checks that you have fully invoiced the deleted purchase orders.</span></span> <span data-ttu-id="20d26-108">You cannot delete orders that you have not fully invoiced and received.</span><span class="sxs-lookup"><span data-stu-id="20d26-108">You cannot delete orders that you have not fully invoiced and received.</span></span>  

<span data-ttu-id="20d26-109">Return orders are usually deleted after they are invoiced.</span><span class="sxs-lookup"><span data-stu-id="20d26-109">Return orders are usually deleted after they are invoiced.</span></span> <span data-ttu-id="20d26-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** page.</span><span class="sxs-lookup"><span data-stu-id="20d26-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** page.</span></span> <span data-ttu-id="20d26-111">If you selected the **Return Shipment on Credit Memo** check box on the **Purchases & Payable Setup** page, then the invoice is transferred to the **Posted Return Shipment** page.</span><span class="sxs-lookup"><span data-stu-id="20d26-111">If you selected the **Return Shipment on Credit Memo** check box on the **Purchases & Payable Setup** page, then the invoice is transferred to the **Posted Return Shipment** page.</span></span> <span data-ttu-id="20d26-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="20d26-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span></span> <span data-ttu-id="20d26-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span><span class="sxs-lookup"><span data-stu-id="20d26-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span></span>  

<span data-ttu-id="20d26-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span><span class="sxs-lookup"><span data-stu-id="20d26-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span></span> <span data-ttu-id="20d26-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="20d26-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span></span>  

<span data-ttu-id="20d26-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span><span class="sxs-lookup"><span data-stu-id="20d26-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="20d26-117">When an invoice is posted, a corresponding entry is created on the **Posted Service Invoices** page.</span><span class="sxs-lookup"><span data-stu-id="20d26-117">When an invoice is posted, a corresponding entry is created on the **Posted Service Invoices** page.</span></span> <span data-ttu-id="20d26-118">The posted document can be viewed on the **Posted Service Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="20d26-118">The posted document can be viewed on the **Posted Service Invoice** page.</span></span>  

<span data-ttu-id="20d26-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="20d26-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** page.</span></span> <span data-ttu-id="20d26-120">Then you may need to delete invoiced orders that were not deleted.</span><span class="sxs-lookup"><span data-stu-id="20d26-120">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="20d26-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="20d26-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="20d26-122">See Also</span><span class="sxs-lookup"><span data-stu-id="20d26-122">See Also</span></span>  
[<span data-ttu-id="20d26-123">Administration</span><span class="sxs-lookup"><span data-stu-id="20d26-123">Administration</span></span>](admin-setup-and-administration.md)  

