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
ms.date: 09/20/2018
ms.author: edupont
ms.openlocfilehash: f9b33875c5831d3caac8ce29140104f570048754
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/08/2019
ms.locfileid: "826177"
---
# <a name="us-tax-rates-in-included365invlongincludesd365invlongmd"></a>US tax rates in [!INCLUDE[d365inv_long](includes/d365inv_long.md)]
You can add tax rates on the fly when you create estimates and invoices. You can see the tax rates that you've already added in the settings for Microsoft Invoicing, and you can add new tax rates there as well.  

You can also manage the tax rates that you need in the **Settings** page. This is also where you set up your own tax information. The default tax rate is the one that you specify for your business address.  

Each tax rate is based on a particular geographic location. For example, the Miami, Florida, tax rate includes three sales tax jurisdictions: city (Miami), county (Dade), and state (Florida).  

If you set up new tax rates, you must make sure that you fill in the fields correctly. In the United States, states, counties, cities, and localities can charge sales tax. Companies collect and remit sales tax to these government authorities for products sold to end users. VAT can also be charged to existing VAT. For example, tax can be calculated on a sales invoice amount that already includes the tax from other jurisdictions.  

## <a name="to-add-a-tax-rate-on-an-invoice-or-estimate"></a>To add a tax rate on an invoice or estimate

1. Create an invoice or estimate. For more information, see [Create an invoice for a new customer](send-invoice.md).  
2. In the **Details** section, if the customer is tax liable, choose the AssistEdit icon > next to the **Customer tax rate** field. This field is already filled in with your default tax rate, but you can choose another.  
3. In the **Tax Rates** window, choose a tax rate or add a new.  
4. Enter the name and rate for both city and state and close the **Tax Rates** window.  
5. You can optionally click or tap **Set as default tax rate**. The default rate is automatically applied to any taxable document or item.  

## <a name="to-add-a-tax-rate-from-the-settings"></a>To add a tax rate from the settings

1. In [!INCLUDE[d365inv](includes/d365inv.md)], in the top right corner, choose the gear symbol, and then choose **My Settings**.  
2. Scroll to the **Tax Rates** section. Click **Add new tax rate** to add a new rate. Click or tap the ellipses to modify an existing tax rate.  
3. Enter the name and rate for both city and state and close the **Tax Rate** form.  

You can optionally click or tap **Set as default tax rate**. The default rate is automatically applied to any taxable document or item.  

If you or your customers are in a country that uses valued added tax (VAT), such as the United Kingdom, see [Add value added tax (VAT) to your invoices](add-vat.md).  

## <a name="see-also"></a>See Also

[Set up your business information](set-up-business-profile.md)  
[Send an invoice to a new customer](send-invoice.md)  
