---
title: Enable Customer Payments Through Payment Services| Microsoft Docs
description: Make it easier for customers to pay their invoices by enabling payment services.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3bcfac75d1d161a4163fda466e320b0efd408655
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4758274"
---
# <a name="enable-customer-payments-through-payment-services"></a><span data-ttu-id="166b4-103">Enable Customer Payments Through Payment Services</span><span class="sxs-lookup"><span data-stu-id="166b4-103">Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="166b4-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span><span class="sxs-lookup"><span data-stu-id="166b4-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span></span>  

<span data-ttu-id="166b4-105">After you enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)], a link to the service is available on sales documents that you send by email to your customers.</span><span class="sxs-lookup"><span data-stu-id="166b4-105">After you enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="166b4-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span><span class="sxs-lookup"><span data-stu-id="166b4-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="166b4-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span><span class="sxs-lookup"><span data-stu-id="166b4-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="166b4-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[prod_short](includes/prod_short.md)], and are ready for you to enable.</span><span class="sxs-lookup"><span data-stu-id="166b4-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[prod_short](includes/prod_short.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-prod_short"></a><span data-ttu-id="166b4-109">To enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="166b4-109">To enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>
1. <span data-ttu-id="166b4-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="166b4-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="166b4-111">On the **Payment Services** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="166b4-111">On the **Payment Services** page, choose the **New** action.</span></span>  
3. <span data-ttu-id="166b4-112">Select the payment service, and then close the page.</span><span class="sxs-lookup"><span data-stu-id="166b4-112">Select the payment service, and then close the page.</span></span>  
4. <span data-ttu-id="166b4-113">On the **Payment Services** page, choose the **Setup** action.</span><span class="sxs-lookup"><span data-stu-id="166b4-113">On the **Payment Services** page, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="166b4-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="166b4-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="166b4-115">Close the page.</span><span class="sxs-lookup"><span data-stu-id="166b4-115">Close the page.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="166b4-116">To select a payment service on a sales invoice</span><span class="sxs-lookup"><span data-stu-id="166b4-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="166b4-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="166b4-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="166b4-118">Open the sales invoice that you want to pay by using the payment service.</span><span class="sxs-lookup"><span data-stu-id="166b4-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="166b4-119">In the **Payment Service** field, choose the payment service.</span><span class="sxs-lookup"><span data-stu-id="166b4-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="166b4-120">The **Payment Service** field is available only if you've enabled the payment service.</span><span class="sxs-lookup"><span data-stu-id="166b4-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="166b4-121">See Also</span><span class="sxs-lookup"><span data-stu-id="166b4-121">See Also</span></span>  
[<span data-ttu-id="166b4-122">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="166b4-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="166b4-123">Sales</span><span class="sxs-lookup"><span data-stu-id="166b4-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="166b4-124">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="166b4-124">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="166b4-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="166b4-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
