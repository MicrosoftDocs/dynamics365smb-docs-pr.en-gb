---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 01/25/2021
ms.author: edupont
ms.openlocfilehash: 539ee2eb2c9e4a71eacfb78d95320870128fb1d9
ms.sourcegitcommit: cb06aa973f5c767df774b0e1e199c6fbe0e85b88
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/17/2021
ms.locfileid: "5470294"
---
<span data-ttu-id="865fe-101">When all the items have been entered on the sales lines, you can calculate the invoice discount for the entire document by choosing the **Calculate Invoice Discount** action.</span><span class="sxs-lookup"><span data-stu-id="865fe-101">When all the items have been entered on the sales lines, you can calculate the invoice discount for the entire document by choosing the **Calculate Invoice Discount** action.</span></span>

<span data-ttu-id="865fe-102">The discount is calculated based on all the lines in the sales document for items where the **Allow Invoice Disc.** field on the sales order line contains **Yes**.</span><span class="sxs-lookup"><span data-stu-id="865fe-102">The discount is calculated based on all the lines in the sales document for items where the **Allow Invoice Disc.** field on the sales order line contains **Yes**.</span></span> <span data-ttu-id="865fe-103">This is the default setting for items.</span><span class="sxs-lookup"><span data-stu-id="865fe-103">This is the default setting for items.</span></span> <span data-ttu-id="865fe-104">Lines with item charges, for example, are not included in the calculation of the invoice discount.</span><span class="sxs-lookup"><span data-stu-id="865fe-104">Lines with item charges, for example, are not included in the calculation of the invoice discount.</span></span> <span data-ttu-id="865fe-105">If you want to apply a discount to such lines, you must set the **Line Discount %** field on the relevant lines.</span><span class="sxs-lookup"><span data-stu-id="865fe-105">If you want to apply a discount to such lines, you must set the **Line Discount %** field on the relevant lines.</span></span>  

> [!TIP]
> <span data-ttu-id="865fe-106">If the **Calc. Inv. Discount** field is selected in the **Sales and Receivables Setup** page, then the invoice discount is calculated automatically when you do either of the following on a sales document:</span><span class="sxs-lookup"><span data-stu-id="865fe-106">If the **Calc. Inv. Discount** field is selected in the **Sales and Receivables Setup** page, then the invoice discount is calculated automatically when you do either of the following on a sales document:</span></span>
>
> * <span data-ttu-id="865fe-107">View statistics</span><span class="sxs-lookup"><span data-stu-id="865fe-107">View statistics</span></span>
> * <span data-ttu-id="865fe-108">View a test report</span><span class="sxs-lookup"><span data-stu-id="865fe-108">View a test report</span></span>
> * <span data-ttu-id="865fe-109">Print</span><span class="sxs-lookup"><span data-stu-id="865fe-109">Print</span></span>
> * <span data-ttu-id="865fe-110">Post</span><span class="sxs-lookup"><span data-stu-id="865fe-110">Post</span></span>

<span data-ttu-id="865fe-111">The invoice discount terms for a customer are defined in the **Cust. Invoice Discounts** page for the customer.</span><span class="sxs-lookup"><span data-stu-id="865fe-111">The invoice discount terms for a customer are defined in the **Cust. Invoice Discounts** page for the customer.</span></span> <span data-ttu-id="865fe-112">The currency code on the sales document is used to find the invoice discount terms in the corresponding currency.</span><span class="sxs-lookup"><span data-stu-id="865fe-112">The currency code on the sales document is used to find the invoice discount terms in the corresponding currency.</span></span>

<span data-ttu-id="865fe-113">If invoice discounts have not been defined for foreign currencies, then the invoice discount terms defined in the **Cust. Invoice Discounts** page with amounts in your local currency and the exchange rate on the posting date on the sales document are used to calculate the invoice discount in the foreign currency.</span><span class="sxs-lookup"><span data-stu-id="865fe-113">If invoice discounts have not been defined for foreign currencies, then the invoice discount terms defined in the **Cust. Invoice Discounts** page with amounts in your local currency and the exchange rate on the posting date on the sales document are used to calculate the invoice discount in the foreign currency.</span></span>
