---
title: Settle Purchase Invoices Promptly
description: If you need to pay the vendor by cash or cheque, you can have the necessary posting done when you post the invoice.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/06/2020
ms.author: bholtorf
ms.openlocfilehash: 60d3cf3c9e141c8df36eaca2c1975b696fdb105b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5387256"
---
# <a name="settle-purchase-invoices-promptly"></a><span data-ttu-id="63ff8-103">Settle Purchase Invoices Promptly</span><span class="sxs-lookup"><span data-stu-id="63ff8-103">Settle Purchase Invoices Promptly</span></span>

<span data-ttu-id="63ff8-104">If you need to pay the vendor by cash or cheque, you can post the payment when you post the invoice.</span><span class="sxs-lookup"><span data-stu-id="63ff8-104">If you need to pay the vendor by cash or check, you can post the payment when you post the invoice.</span></span>  

> [!NOTE]  
> <span data-ttu-id="63ff8-105">If you frequently pay purchase invoices in cash, by cheque or via bank transfer, it is a good idea to set up a specific payment method with a balancing account and enter this method in the **Payment Method** field on the vendor card.</span><span class="sxs-lookup"><span data-stu-id="63ff8-105">If you frequently pay purchase invoices in cash, check, or bank transfer, it is a good idea to set up a specific payment method with a balancing account and enter this method in the **Payment Method** field on the vendor card.</span></span> <span data-ttu-id="63ff8-106">The balancing account number is inserted automatically on the invoice header every time you create a new invoice.</span><span class="sxs-lookup"><span data-stu-id="63ff8-106">The balancing account number is inserted automatically on the invoice header every time you create a new invoice.</span></span> <span data-ttu-id="63ff8-107">For more information, see [Defining Payment Methods](finance-payment-methods.md).</span><span class="sxs-lookup"><span data-stu-id="63ff8-107">For more information, see [Defining Payment Methods](finance-payment-methods.md).</span></span>  

## <a name="to-settle-purchase-invoices-promptly"></a><span data-ttu-id="63ff8-108">To settle purchase invoices promptly</span><span class="sxs-lookup"><span data-stu-id="63ff8-108">To settle purchase invoices promptly</span></span>

1. <span data-ttu-id="63ff8-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="63ff8-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="63ff8-110">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="63ff8-110">Choose the **New** action.</span></span>  
3. <span data-ttu-id="63ff8-111">To pay either in cash or by bank transfer, enter the number of the general ledger cash account or the bank account in the **Bal. Account No.** field.</span><span class="sxs-lookup"><span data-stu-id="63ff8-111">To pay either in cash or by bank transfer, enter the number of the general ledger cash account or the bank account in the **Bal. Account No.** field.</span></span>  

> [!IMPORTANT]  
> <span data-ttu-id="63ff8-112">The **Bal. Account Type** and **Bal. Account No.** fields are not included in the standard layout of the invoice header.</span><span class="sxs-lookup"><span data-stu-id="63ff8-112">The **Bal. Account Type** and **Bal. Account No.** fields are not included in the standard layout of the invoice header.</span></span> <span data-ttu-id="63ff8-113">In order to post the payment of an invoice, you must contact a Microsoft partner who can add the fields through code.</span><span class="sxs-lookup"><span data-stu-id="63ff8-113">In order to post the payment of an invoice, you must contact a Microsoft partner who can add the fields through code.</span></span>  
>
> <span data-ttu-id="63ff8-114">This customisation is only required if you do not specify balancing accounts on the payment methods as describe above.</span><span class="sxs-lookup"><span data-stu-id="63ff8-114">This customization is only required if you do not specify balancing accounts on the payment methods as describe above.</span></span>

## <a name="see-also"></a><span data-ttu-id="63ff8-115">See Also</span><span class="sxs-lookup"><span data-stu-id="63ff8-115">See Also</span></span>

[<span data-ttu-id="63ff8-116">Managing Payables</span><span class="sxs-lookup"><span data-stu-id="63ff8-116">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="63ff8-117">Purchasing</span><span class="sxs-lookup"><span data-stu-id="63ff8-117">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="63ff8-118">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="63ff8-118">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]