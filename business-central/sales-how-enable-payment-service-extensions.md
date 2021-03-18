---
title: Enable Customer Payments Through Payment Services| Microsoft Docs
description: Make it easier for customers to pay their invoices by enabling payment services.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5fa58c177629fdf386bca0ebfce2b668a55cbc8f
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5393356"
---
# <a name="enable-customer-payments-through-payment-services"></a><span data-ttu-id="47f85-103">Enable Customer Payments Through Payment Services</span><span class="sxs-lookup"><span data-stu-id="47f85-103">Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="47f85-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span><span class="sxs-lookup"><span data-stu-id="47f85-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as Microsoft Pay, PayPal, or WorldPay.</span></span>  

<span data-ttu-id="47f85-105">After you enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)], a link to the service is available on sales documents that you send by email to your customers.</span><span class="sxs-lookup"><span data-stu-id="47f85-105">After you enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="47f85-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span><span class="sxs-lookup"><span data-stu-id="47f85-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="47f85-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span><span class="sxs-lookup"><span data-stu-id="47f85-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="47f85-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[prod_short](includes/prod_short.md)], and are ready for you to enable.</span><span class="sxs-lookup"><span data-stu-id="47f85-108">The Microsoft Pay, PayPal Payments Standard, and WorldPay Payments Standard extensions are installed in [!INCLUDE[prod_short](includes/prod_short.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-prod_short"></a><span data-ttu-id="47f85-109">To enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="47f85-109">To enable a payment service in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>
1. <span data-ttu-id="47f85-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="47f85-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="47f85-111">On the **Payment Services** page, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="47f85-111">On the **Payment Services** page, choose the **New** action.</span></span>  
3. <span data-ttu-id="47f85-112">Select the payment service, and then close the page.</span><span class="sxs-lookup"><span data-stu-id="47f85-112">Select the payment service, and then close the page.</span></span>  
4. <span data-ttu-id="47f85-113">On the **Payment Services** page, choose the **Setup** action.</span><span class="sxs-lookup"><span data-stu-id="47f85-113">On the **Payment Services** page, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="47f85-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="47f85-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="47f85-115">Close the page.</span><span class="sxs-lookup"><span data-stu-id="47f85-115">Close the page.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="47f85-116">To select a payment service on a sales invoice</span><span class="sxs-lookup"><span data-stu-id="47f85-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="47f85-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="47f85-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="47f85-118">Open the sales invoice that you want to pay by using the payment service.</span><span class="sxs-lookup"><span data-stu-id="47f85-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="47f85-119">In the **Payment Service** field, choose the payment service.</span><span class="sxs-lookup"><span data-stu-id="47f85-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="47f85-120">The **Payment Service** field is available only if you've enabled the payment service.</span><span class="sxs-lookup"><span data-stu-id="47f85-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="47f85-121">See Also</span><span class="sxs-lookup"><span data-stu-id="47f85-121">See Also</span></span>  
[<span data-ttu-id="47f85-122">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="47f85-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="47f85-123">Sales</span><span class="sxs-lookup"><span data-stu-id="47f85-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="47f85-124">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="47f85-124">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="47f85-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="47f85-125">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]