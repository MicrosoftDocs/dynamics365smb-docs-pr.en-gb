---
title: Post SEPA Direct Debit Payments | Microsoft Docs
description: When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 2daa52e1ee4546356ecb7d94b5c01ab9e22bbbd6
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="post-sepa-direct-debit-payment-receipts"></a><span data-ttu-id="f56e0-103">Post SEPA Direct Debit Payment Receipts</span><span class="sxs-lookup"><span data-stu-id="f56e0-103">Post SEPA Direct Debit Payment Receipts</span></span>
<span data-ttu-id="f56e0-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span><span class="sxs-lookup"><span data-stu-id="f56e0-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span></span> <span data-ttu-id="f56e0-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="f56e0-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

<span data-ttu-id="f56e0-106">You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window.</span><span class="sxs-lookup"><span data-stu-id="f56e0-106">You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window.</span></span> <span data-ttu-id="f56e0-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span><span class="sxs-lookup"><span data-stu-id="f56e0-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span></span>  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-window"></a><span data-ttu-id="f56e0-108">To post a direct-debit payment receipt from the Direct Debit Collections window</span><span class="sxs-lookup"><span data-stu-id="f56e0-108">To post a direct-debit payment receipt from the Direct Debit Collections window</span></span>  
1. <span data-ttu-id="f56e0-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f56e0-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f56e0-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span><span class="sxs-lookup"><span data-stu-id="f56e0-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span></span> <span data-ttu-id="f56e0-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="f56e0-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  
3. <span data-ttu-id="f56e0-112">Choose the **Post Payment Receipts** action.</span><span class="sxs-lookup"><span data-stu-id="f56e0-112">Choose the **Post Payment Receipts** action.</span></span>  
4. <span data-ttu-id="f56e0-113">In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="f56e0-113">In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="f56e0-114">Field</span><span class="sxs-lookup"><span data-stu-id="f56e0-114">Field</span></span>|<span data-ttu-id="f56e0-115">Description</span><span class="sxs-lookup"><span data-stu-id="f56e0-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="f56e0-116">**Direct Debit Collection No.**</span><span class="sxs-lookup"><span data-stu-id="f56e0-116">**Direct Debit Collection No.**</span></span>|<span data-ttu-id="f56e0-117">Specify the direct debit collection that you want to post payment receipt for.</span><span class="sxs-lookup"><span data-stu-id="f56e0-117">Specify the direct debit collection that you want to post payment receipt for.</span></span>|  
    |<span data-ttu-id="f56e0-118">**General Journal Template**</span><span class="sxs-lookup"><span data-stu-id="f56e0-118">**General Journal Template**</span></span>|<span data-ttu-id="f56e0-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span><span class="sxs-lookup"><span data-stu-id="f56e0-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span></span>|  
    |<span data-ttu-id="f56e0-120">**General Journal Batch Name**</span><span class="sxs-lookup"><span data-stu-id="f56e0-120">**General Journal Batch Name**</span></span>|<span data-ttu-id="f56e0-121">Specify which general journal batch to use for posting the payment receipt.</span><span class="sxs-lookup"><span data-stu-id="f56e0-121">Specify which general journal batch to use for posting the payment receipt.</span></span>|  
    |<span data-ttu-id="f56e0-122">**Create Journal Only**</span><span class="sxs-lookup"><span data-stu-id="f56e0-122">**Create Journal Only**</span></span>|<span data-ttu-id="f56e0-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="f56e0-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span></span> <span data-ttu-id="f56e0-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span><span class="sxs-lookup"><span data-stu-id="f56e0-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span></span>|  

5. <span data-ttu-id="f56e0-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="f56e0-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f56e0-126">See Also</span><span class="sxs-lookup"><span data-stu-id="f56e0-126">See Also</span></span>  
 <span data-ttu-id="f56e0-127">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="f56e0-127">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
 [<span data-ttu-id="f56e0-128">Sales</span><span class="sxs-lookup"><span data-stu-id="f56e0-128">Sales</span></span>](sales-manage-sales.md)

