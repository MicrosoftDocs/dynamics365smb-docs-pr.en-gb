---
title: Post SEPA Direct Debit Payments | Microsoft Docs
description: When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: finance-collect-payments-with-sepa-direct-debit
ms.openlocfilehash: 6d24df38b980542b1c77d737b8f661fac0df29fa
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "809473"
---
# <a name="post-sepa-direct-debit-payment-receipts"></a><span data-ttu-id="39daf-103">Post SEPA Direct Debit Payment Receipts</span><span class="sxs-lookup"><span data-stu-id="39daf-103">Post SEPA Direct Debit Payment Receipts</span></span>
<span data-ttu-id="39daf-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span><span class="sxs-lookup"><span data-stu-id="39daf-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span></span> <span data-ttu-id="39daf-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="39daf-105">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

<span data-ttu-id="39daf-106">You can post the payment receipt directly from the **Direct Debit Collections** page or the **Direct Debit Collect. Entries** page.</span><span class="sxs-lookup"><span data-stu-id="39daf-106">You can post the payment receipt directly from the **Direct Debit Collections** page or the **Direct Debit Collect. Entries** page.</span></span> <span data-ttu-id="39daf-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span><span class="sxs-lookup"><span data-stu-id="39daf-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span></span>  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-page"></a><span data-ttu-id="39daf-108">To post a direct-debit payment receipt from the Direct Debit Collections page</span><span class="sxs-lookup"><span data-stu-id="39daf-108">To post a direct-debit payment receipt from the Direct Debit Collections page</span></span>  
1. <span data-ttu-id="39daf-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Direct Debit Collections**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="39daf-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="39daf-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span><span class="sxs-lookup"><span data-stu-id="39daf-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span></span> <span data-ttu-id="39daf-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="39daf-111">For more information, see [Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  
3. <span data-ttu-id="39daf-112">Choose the **Post Payment Receipts** action.</span><span class="sxs-lookup"><span data-stu-id="39daf-112">Choose the **Post Payment Receipts** action.</span></span>  
4. <span data-ttu-id="39daf-113">On the **Post Direct Debit Collection** page, fill in the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="39daf-113">On the **Post Direct Debit Collection** page, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="39daf-114">Field</span><span class="sxs-lookup"><span data-stu-id="39daf-114">Field</span></span>|<span data-ttu-id="39daf-115">Description</span><span class="sxs-lookup"><span data-stu-id="39daf-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="39daf-116">**Direct Debit Collection No.**</span><span class="sxs-lookup"><span data-stu-id="39daf-116">**Direct Debit Collection No.**</span></span>|<span data-ttu-id="39daf-117">Specify the direct debit collection that you want to post payment receipt for.</span><span class="sxs-lookup"><span data-stu-id="39daf-117">Specify the direct debit collection that you want to post payment receipt for.</span></span>|  
    |<span data-ttu-id="39daf-118">**General Journal Template**</span><span class="sxs-lookup"><span data-stu-id="39daf-118">**General Journal Template**</span></span>|<span data-ttu-id="39daf-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span><span class="sxs-lookup"><span data-stu-id="39daf-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span></span>|  
    |<span data-ttu-id="39daf-120">**General Journal Batch Name**</span><span class="sxs-lookup"><span data-stu-id="39daf-120">**General Journal Batch Name**</span></span>|<span data-ttu-id="39daf-121">Specify which general journal batch to use for posting the payment receipt.</span><span class="sxs-lookup"><span data-stu-id="39daf-121">Specify which general journal batch to use for posting the payment receipt.</span></span>|  
    |<span data-ttu-id="39daf-122">**Create Journal Only**</span><span class="sxs-lookup"><span data-stu-id="39daf-122">**Create Journal Only**</span></span>|<span data-ttu-id="39daf-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="39daf-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span></span> <span data-ttu-id="39daf-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span><span class="sxs-lookup"><span data-stu-id="39daf-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span></span>|  

5. <span data-ttu-id="39daf-125">Choose the **OK** button.</span><span class="sxs-lookup"><span data-stu-id="39daf-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="39daf-126">See Also</span><span class="sxs-lookup"><span data-stu-id="39daf-126">See Also</span></span>  
 <span data-ttu-id="39daf-127">[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="39daf-127">[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
 [<span data-ttu-id="39daf-128">Sales</span><span class="sxs-lookup"><span data-stu-id="39daf-128">Sales</span></span>](sales-manage-sales.md)
