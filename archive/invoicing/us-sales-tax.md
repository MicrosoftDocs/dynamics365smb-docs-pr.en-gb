---
title: US tax rates | Invoicing
description: Learn about how to add sales tax in Invoicing. Add a default tax rate based on your own address, and add tax rates for your customers.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: tax rates
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: 180e31d293ae706dd70ffb9e2befe133128a8695
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927895"
---
# <a name="us-tax-rates-in-d365inv_long"></a><span data-ttu-id="42b04-104">US tax rates in [!INCLUDE[d365inv_long](includes/d365inv_long.md)]</span><span class="sxs-lookup"><span data-stu-id="42b04-104">US tax rates in [!INCLUDE[d365inv_long](includes/d365inv_long.md)]</span></span>
> [!Note]
> [!INCLUDE[d365inv_discont](includes/d365inv_discont.md)]

<span data-ttu-id="42b04-105">You can add tax rates on the fly when you create estimates and invoices.</span><span class="sxs-lookup"><span data-stu-id="42b04-105">You can add tax rates on the fly when you create estimates and invoices.</span></span> <span data-ttu-id="42b04-106">You can see the tax rates that you've already added in the settings for Microsoft Invoicing, and you can add new tax rates there as well.</span><span class="sxs-lookup"><span data-stu-id="42b04-106">You can see the tax rates that you've already added in the settings for Microsoft Invoicing, and you can add new tax rates there as well.</span></span>  

<span data-ttu-id="42b04-107">You can also manage the tax rates that you need in the **Settings** page.</span><span class="sxs-lookup"><span data-stu-id="42b04-107">You can also manage the tax rates that you need in the **Settings** page.</span></span> <span data-ttu-id="42b04-108">This is also where you set up your own tax information.</span><span class="sxs-lookup"><span data-stu-id="42b04-108">This is also where you set up your own tax information.</span></span> <span data-ttu-id="42b04-109">The default tax rate is the one that you specify for your business address.</span><span class="sxs-lookup"><span data-stu-id="42b04-109">The default tax rate is the one that you specify for your business address.</span></span>  

<span data-ttu-id="42b04-110">Each tax rate is based on a particular geographic location.</span><span class="sxs-lookup"><span data-stu-id="42b04-110">Each tax rate is based on a particular geographic location.</span></span> <span data-ttu-id="42b04-111">For example, the Miami, Florida, tax rate includes three sales tax jurisdictions: city (Miami), county (Dade), and state (Florida).</span><span class="sxs-lookup"><span data-stu-id="42b04-111">For example, the Miami, Florida, tax rate includes three sales tax jurisdictions: city (Miami), county (Dade), and state (Florida).</span></span>  

<span data-ttu-id="42b04-112">If you set up new tax rates, you must make sure that you fill in the fields correctly.</span><span class="sxs-lookup"><span data-stu-id="42b04-112">If you set up new tax rates, you must make sure that you fill in the fields correctly.</span></span> <span data-ttu-id="42b04-113">In the United States, states, counties, cities, and localities can charge sales tax.</span><span class="sxs-lookup"><span data-stu-id="42b04-113">In the United States, states, counties, cities, and localities can charge sales tax.</span></span> <span data-ttu-id="42b04-114">Companies collect and remit sales tax to these government authorities for products sold to end users.</span><span class="sxs-lookup"><span data-stu-id="42b04-114">Companies collect and remit sales tax to these government authorities for products sold to end users.</span></span> <span data-ttu-id="42b04-115">VAT can also be charged to existing VAT.</span><span class="sxs-lookup"><span data-stu-id="42b04-115">Sales tax can also be charged to existing sales tax.</span></span> <span data-ttu-id="42b04-116">For example, tax can be calculated on a sales invoice amount that already includes the tax from other jurisdictions.</span><span class="sxs-lookup"><span data-stu-id="42b04-116">For example, tax can be calculated on a sales invoice amount that already includes the tax from other jurisdictions.</span></span>  

## <a name="to-add-a-tax-rate-on-an-invoice-or-estimate"></a><span data-ttu-id="42b04-117">To add a tax rate on an invoice or estimate</span><span class="sxs-lookup"><span data-stu-id="42b04-117">To add a tax rate on an invoice or estimate</span></span>

1. <span data-ttu-id="42b04-118">Create an invoice or estimate.</span><span class="sxs-lookup"><span data-stu-id="42b04-118">Create an invoice or estimate.</span></span> <span data-ttu-id="42b04-119">For more information, see [Create an invoice for a new customer](send-invoice.md).</span><span class="sxs-lookup"><span data-stu-id="42b04-119">For more information, see [Create an invoice for a new customer](send-invoice.md).</span></span>  
2. <span data-ttu-id="42b04-120">In the **Details** section, if the customer is tax liable, choose the AssistEdit icon > next to the **Customer tax rate** field.</span><span class="sxs-lookup"><span data-stu-id="42b04-120">In the **Details** section, if the customer is tax liable, choose the AssistEdit icon > next to the **Customer tax rate** field.</span></span> <span data-ttu-id="42b04-121">This field is already filled in with your default tax rate, but you can choose another.</span><span class="sxs-lookup"><span data-stu-id="42b04-121">This field is already filled in with your default tax rate, but you can choose another.</span></span>  
3. <span data-ttu-id="42b04-122">In the **Tax Rates** window, choose a tax rate or add a new.</span><span class="sxs-lookup"><span data-stu-id="42b04-122">In the **Tax Rates** window, choose a tax rate or add a new.</span></span>  
4. <span data-ttu-id="42b04-123">Enter the name and rate for both city and state and close the **Tax Rates** window.</span><span class="sxs-lookup"><span data-stu-id="42b04-123">Enter the name and rate for both city and state and close the **Tax Rates** window.</span></span>  
5. <span data-ttu-id="42b04-124">You can optionally click or tap **Set as default tax rate** .</span><span class="sxs-lookup"><span data-stu-id="42b04-124">You can optionally click or tap **Set as default tax rate** .</span></span> <span data-ttu-id="42b04-125">The default rate is automatically applied to any taxable document or item.</span><span class="sxs-lookup"><span data-stu-id="42b04-125">The default rate is automatically applied to any taxable document or item.</span></span>  

## <a name="to-add-a-tax-rate-from-the-settings"></a><span data-ttu-id="42b04-126">To add a tax rate from the settings</span><span class="sxs-lookup"><span data-stu-id="42b04-126">To add a tax rate from the settings</span></span>

1. <span data-ttu-id="42b04-127">In [!INCLUDE[d365inv](includes/d365inv.md)], in the top right corner, choose the gear symbol, and then choose **My Settings** .</span><span class="sxs-lookup"><span data-stu-id="42b04-127">In [!INCLUDE[d365inv](includes/d365inv.md)], in the top right corner, choose the gear symbol, and then choose **My Settings** .</span></span>  
2. <span data-ttu-id="42b04-128">Scroll to the **Tax Rates** section.</span><span class="sxs-lookup"><span data-stu-id="42b04-128">Scroll to the **Tax Rates** section.</span></span> <span data-ttu-id="42b04-129">Click **Add new tax rate** to add a new rate.</span><span class="sxs-lookup"><span data-stu-id="42b04-129">Click **Add new tax rate** to add a new rate.</span></span> <span data-ttu-id="42b04-130">Click or tap the ellipses to modify an existing tax rate.</span><span class="sxs-lookup"><span data-stu-id="42b04-130">Click or tap the ellipses to modify an existing tax rate.</span></span>  
3. <span data-ttu-id="42b04-131">Enter the name and rate for both city and state and close the **Tax Rate** form.</span><span class="sxs-lookup"><span data-stu-id="42b04-131">Enter the name and rate for both city and state and close the **Tax Rate** form.</span></span>  

<span data-ttu-id="42b04-132">You can optionally click or tap **Set as default tax rate** .</span><span class="sxs-lookup"><span data-stu-id="42b04-132">You can optionally click or tap **Set as default tax rate** .</span></span> <span data-ttu-id="42b04-133">The default rate is automatically applied to any taxable document or item.</span><span class="sxs-lookup"><span data-stu-id="42b04-133">The default rate is automatically applied to any taxable document or item.</span></span>  

<span data-ttu-id="42b04-134">If you or your customers are in a country that uses valued added tax (VAT), such as the United Kingdom, see [Add value added tax (VAT) to your invoices](add-vat.md).</span><span class="sxs-lookup"><span data-stu-id="42b04-134">If you or your customers are in a country that uses valued added tax (VAT), such as the United Kingdom, see [Add value added tax (VAT) to your invoices](add-vat.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="42b04-135">See Also</span><span class="sxs-lookup"><span data-stu-id="42b04-135">See Also</span></span>

[<span data-ttu-id="42b04-136">Set up your business information</span><span class="sxs-lookup"><span data-stu-id="42b04-136">Set up your business information</span></span>](set-up-business-profile.md)  
[<span data-ttu-id="42b04-137">Send an invoice to a new customer</span><span class="sxs-lookup"><span data-stu-id="42b04-137">Send an invoice to a new customer</span></span>](send-invoice.md)  
