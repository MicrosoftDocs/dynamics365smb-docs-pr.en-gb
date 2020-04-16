---
title: Manage, delete, or compress documents | Microsoft Docs
description: Keep your historical data or delete it.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 54cccb9df4daee3ad0811139dc2180d8a3072deb
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3186963"
---
# <a name="manage-documents"></a><span data-ttu-id="817e0-103">Manage Documents</span><span class="sxs-lookup"><span data-stu-id="817e0-103">Manage Documents</span></span>
<span data-ttu-id="817e0-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span><span class="sxs-lookup"><span data-stu-id="817e0-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span></span>  

## <a name="delete-documents"></a><span data-ttu-id="817e0-105">Delete Documents</span><span class="sxs-lookup"><span data-stu-id="817e0-105">Delete Documents</span></span>
<span data-ttu-id="817e0-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span><span class="sxs-lookup"><span data-stu-id="817e0-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="817e0-107">checks that you have fully invoiced the deleted purchase orders.</span><span class="sxs-lookup"><span data-stu-id="817e0-107">checks that you have fully invoiced the deleted purchase orders.</span></span> <span data-ttu-id="817e0-108">You cannot delete orders that you have not fully invoiced and received.</span><span class="sxs-lookup"><span data-stu-id="817e0-108">You cannot delete orders that you have not fully invoiced and received.</span></span>  

<span data-ttu-id="817e0-109">Return orders are usually deleted after they are invoiced.</span><span class="sxs-lookup"><span data-stu-id="817e0-109">Return orders are usually deleted after they are invoiced.</span></span> <span data-ttu-id="817e0-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** page.</span><span class="sxs-lookup"><span data-stu-id="817e0-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** page.</span></span> <span data-ttu-id="817e0-111">If you selected the **Return Shipment on Credit Memo** check box on the **Purchases & Payable Setup** page, then the invoice is transferred to the **Posted Return Shipment** page.</span><span class="sxs-lookup"><span data-stu-id="817e0-111">If you selected the **Return Shipment on Credit Memo** check box on the **Purchases & Payable Setup** page, then the invoice is transferred to the **Posted Return Shipment** page.</span></span> <span data-ttu-id="817e0-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="817e0-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span></span> <span data-ttu-id="817e0-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span><span class="sxs-lookup"><span data-stu-id="817e0-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span></span>  

<span data-ttu-id="817e0-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span><span class="sxs-lookup"><span data-stu-id="817e0-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span></span> <span data-ttu-id="817e0-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="817e0-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span></span>  

<span data-ttu-id="817e0-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span><span class="sxs-lookup"><span data-stu-id="817e0-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="817e0-117">When an invoice is posted, a corresponding entry is created on the **Posted Service Invoices** page.</span><span class="sxs-lookup"><span data-stu-id="817e0-117">When an invoice is posted, a corresponding entry is created on the **Posted Service Invoices** page.</span></span> <span data-ttu-id="817e0-118">The posted document can be viewed on the **Posted Service Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="817e0-118">The posted document can be viewed on the **Posted Service Invoice** page.</span></span>  

<span data-ttu-id="817e0-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** page.</span><span class="sxs-lookup"><span data-stu-id="817e0-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** page.</span></span> <span data-ttu-id="817e0-120">Then you may need to delete invoiced orders that were not deleted.</span><span class="sxs-lookup"><span data-stu-id="817e0-120">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="817e0-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span><span class="sxs-lookup"><span data-stu-id="817e0-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="817e0-122">See Also</span><span class="sxs-lookup"><span data-stu-id="817e0-122">See Also</span></span>  
[<span data-ttu-id="817e0-123">Administration</span><span class="sxs-lookup"><span data-stu-id="817e0-123">Administration</span></span>](admin-setup-and-administration.md)  
