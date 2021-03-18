---
title: Microsoft Pay Standard| Microsoft Docs
description: Provides information about the Microsoft Pay extension
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: a8811f6a05b380ce4e4b18b9caf28528a49b99d0
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5386156"
---
# <a name="the-microsoft-pay-extension"></a><span data-ttu-id="7ee96-103">The Microsoft Pay Extension</span><span class="sxs-lookup"><span data-stu-id="7ee96-103">The Microsoft Pay Extension</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7ee96-104">Effective February 8 2020, changes in the Microsoft Pay service will affect the Microsoft Pay extension in Microsoft [!INCLUDE[prod_short](includes/prod_long.md)].</span><span class="sxs-lookup"><span data-stu-id="7ee96-104">Effective February 8 2020, changes in the Microsoft Pay service will affect the Microsoft Pay extension in Microsoft [!INCLUDE[prod_short](includes/prod_long.md)].</span></span> <span data-ttu-id="7ee96-105">Due to the changes, after February 8, the **Pay now** payment links that the Microsoft Pay extension generates for invoices in [!INCLUDE[prod_short](includes/prod_short.md)] will not open Microsoft Pay.</span><span class="sxs-lookup"><span data-stu-id="7ee96-105">Due to the changes, after February 8, the **Pay now** payment links that the Microsoft Pay extension generates for invoices in [!INCLUDE[prod_short](includes/prod_short.md)] will not open Microsoft Pay.</span></span> <span data-ttu-id="7ee96-106">Customers who are using the extension should change their Payment Services setup to start using the PayPal extension instead.</span><span class="sxs-lookup"><span data-stu-id="7ee96-106">Customers who are using the extension should change their Payment Services setup to start using the PayPal extension instead.</span></span><br /></br>
>
> <span data-ttu-id="7ee96-107">From January 8, we will display a notification in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="7ee96-107">From January 8, we will display a notification in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="7ee96-108">The notification will contain a link to the settings that you need to change and to more information.</span><span class="sxs-lookup"><span data-stu-id="7ee96-108">The notification will contain a link to the settings that you need to change and to more information.</span></span> <span data-ttu-id="7ee96-109">After February 8, the Microsoft Pay extension will no longer be available in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="7ee96-109">After February 8, the Microsoft Pay extension will no longer be available in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span><br /></br>
>
> <span data-ttu-id="7ee96-110">The changes impact the following versions of Business Central:</span><span class="sxs-lookup"><span data-stu-id="7ee96-110">The changes impact the following versions of Business Central:</span></span>
> - <span data-ttu-id="7ee96-111">Microsoft Dynamics 365 Business Central October 2018</span><span class="sxs-lookup"><span data-stu-id="7ee96-111">Microsoft Dynamics 365 Business Central October 2018</span></span>
> - <span data-ttu-id="7ee96-112">Microsoft Dynamics 365 Business Central April 2019</span><span class="sxs-lookup"><span data-stu-id="7ee96-112">Microsoft Dynamics 365 Business Central April 2019</span></span>
> - <span data-ttu-id="7ee96-113">Microsoft Dynamics 365 Business Central 2019 Release Wave 2</span><span class="sxs-lookup"><span data-stu-id="7ee96-113">Microsoft Dynamics 365 Business Central 2019 Release Wave 2</span></span>

<span data-ttu-id="7ee96-114">Customers continuously require higher customer service, both in terms of the quality of product but also in terms of delivery and payment services.</span><span class="sxs-lookup"><span data-stu-id="7ee96-114">Customers continuously require higher customer service, both in terms of the quality of product but also in terms of delivery and payment services.</span></span> <span data-ttu-id="7ee96-115">The Microsoft Pay service helps you increase your customer service.</span><span class="sxs-lookup"><span data-stu-id="7ee96-115">The Microsoft Pay service helps you increase your customer service.</span></span>

<span data-ttu-id="7ee96-116">The Microsoft Pay extension adds a Microsoft Pay link to your sales documents so customers can easily pay using Microsoft Pay.</span><span class="sxs-lookup"><span data-stu-id="7ee96-116">The Microsoft Pay extension adds a Microsoft Pay link to your sales documents so customers can easily pay using Microsoft Pay.</span></span> <span data-ttu-id="7ee96-117">Then you can send the documents by email to provide higher customer service and shorten the time it takes for customers’ payments to arrive on your bank account.</span><span class="sxs-lookup"><span data-stu-id="7ee96-117">Then you can send the documents by email to provide higher customer service and shorten the time it takes for customers’ payments to arrive on your bank account.</span></span>

<span data-ttu-id="7ee96-118">The Microsoft Pay extension provides the following benefits:</span><span class="sxs-lookup"><span data-stu-id="7ee96-118">The Microsoft Pay extension provides the following benefits:</span></span>
- <span data-ttu-id="7ee96-119">Customer payments appear faster on your bank account.</span><span class="sxs-lookup"><span data-stu-id="7ee96-119">Customer payments appear faster on your bank account.</span></span>
- <span data-ttu-id="7ee96-120">Customers have more ways to pay invoices.</span><span class="sxs-lookup"><span data-stu-id="7ee96-120">Customers have more ways to pay invoices.</span></span>
- <span data-ttu-id="7ee96-121">Microsoft Pay offers a trustworthy payment service, which customers prefer to entering credit card information on unknown web sites.</span><span class="sxs-lookup"><span data-stu-id="7ee96-121">Microsoft Pay offers a trustworthy payment service, which customers prefer to entering credit card information on unknown web sites.</span></span>
- <span data-ttu-id="7ee96-122">Microsoft Pay offers multiple ways of handling payments, including credit card processing, such as PayPal and Stripe.</span><span class="sxs-lookup"><span data-stu-id="7ee96-122">Microsoft Pay offers multiple ways of handling payments, including credit card processing, such as PayPal and Stripe.</span></span>
- <span data-ttu-id="7ee96-123">The Microsoft Pay link can be embedded automatically on every invoice document or by the user.</span><span class="sxs-lookup"><span data-stu-id="7ee96-123">The Microsoft Pay link can be embedded automatically on every invoice document or by the user.</span></span>
- <span data-ttu-id="7ee96-124">Because this functionality is built as an extension, it gives you full control to enable it when and if your business processes require it.</span><span class="sxs-lookup"><span data-stu-id="7ee96-124">Because this functionality is built as an extension, it gives you full control to enable it when and if your business processes require it.</span></span>

<span data-ttu-id="7ee96-125">Enabling payment service extensions is free in [!INCLUDE[prod_short](includes/prod_short.md)], however, you will need to contact the payment service to get an account.</span><span class="sxs-lookup"><span data-stu-id="7ee96-125">Enabling payment service extensions is free in [!INCLUDE[prod_short](includes/prod_short.md)], however, you will need to contact the payment service to get an account.</span></span> <span data-ttu-id="7ee96-126">For more information, see [Enable Customer Payment Through Payment Services](sales-how-enable-payment-service-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="7ee96-126">For more information, see [Enable Customer Payment Through Payment Services](sales-how-enable-payment-service-extensions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="7ee96-127">See Also</span><span class="sxs-lookup"><span data-stu-id="7ee96-127">See Also</span></span>
<span data-ttu-id="7ee96-128">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="7ee96-128">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="7ee96-129">Setting Up Sales</span><span class="sxs-lookup"><span data-stu-id="7ee96-129">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="7ee96-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7ee96-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]