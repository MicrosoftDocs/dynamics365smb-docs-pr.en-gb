---
title: FAQ for technical details
description: Implementation details related to the Shopify connector.
ms.date: 05/27/2022
ms.topic: article
ms.service: dynamics365-business-central
author: AndreiPanko
ms.author: andreipa
ms.openlocfilehash: 534b4aa47820bc3738a8ffc22a02151efef64863
ms.sourcegitcommit: bb6ecb20cbd82fdb5235e3cb426fc73c29c0a7ae
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 11/23/2022
ms.locfileid: "9802910"
---
# <a name="faq-for-technical-details"></a>FAQ for Technical Details

This article answers frequently asked questions about the Shopify connector.

## <a name="what-is-shopify"></a>What is Shopify? 

Shopify is a subscription-based software that allows anyone to set up an online store and sell their products. The Shopify platform offers online retailers a suite of services including payments, marketing, shipping, and customer engagement tools. 

## <a name="what-is-the-microsoft-dynamics-365-business-central-shopify-connector"></a>What is the Microsoft Dynamics 365 Business Central Shopify connector? 

With the Shopify connector, businesses can link their Shopify store (or stores) with [!INCLUDE[prod_short](../includes/prod_short.md)] to maximise business productivity. Using the Shopify connector, they can manage and view insights from their business and their Shopify online store as one unit. 

### <a name="capabilities"></a>Capabilities

- Support for more than one Shopify shop
  - Each shop has its own setup, including a collection of products, locations used to calculate inventory, and price lists.  
- Bi-directional synchronisation of items or products
  - The connector will synchronise images, item variants, barcodes, vendor item numbers, extended texts, and tags.  
  - Export item attributes to Shopify.  
  - Use selected customer price groups and discounts to define prices exported to Shopify.  
  - Decide whether items can be created automatically or only allow updates to existing products.  
- Synchronisation of inventory levels
  - Choose some or all of the available locations in [!INCLUDE [prod_short](../includes/prod_short.md)].  
  - Update inventory levels on multiple locations in Shopify.  
- Bi-directional synchronisation of customers
  - Smart-map customers by phone and email.  
  - Use country-specific templates when creating customers, which helps ensure that tax settings are correct.  
- Import of orders from Shopify
  - Include orders created in various sales channels, such as Online store or **Shopify POS**. 
  - Shipping costs, gift cards, tips, shipping and payment methods, transactions, and risk of fraud.  
  - During the import, you can automatically create customers in [!INCLUDE [prod_short](../includes/prod_short.md)] or decide to manage the customers in Shopify.  
  - Receive payout information from Shopify Payments. 
- Track fulfillment information
  - Optionally, choose to transfer item tracking information from [!INCLUDE [prod_short](../includes/prod_short.md)] to Shopify.  

## <a name="why-did-microsoft-and-shopify-form-this-partnership"></a>Why did Microsoft and Shopify form this partnership? 

[!INCLUDE[prod_short](../includes/prod_long.md)] is teaming up with Shopify to help our customers create a better shopping experience. While Shopify provides merchants with an easy-to-use commerce solution, [!INCLUDE[prod_short](../includes/prod_short.md)] offers comprehensive business management across finance, sales, service, and operations teams within a single application. Seamless connection between the two systems synchronises orders, stock and customer information so merchants can fulfil orders faster and better serve customers.

## <a name="what-microsoft-products-is-the-shopify-connector-available-for"></a>What Microsoft products is the Shopify connector available for?

This feature is available only for [!INCLUDE[prod_short](../includes/prod_short.md)] online, starting with version 20.1. It isn't available for on-premises deployments. The app with the connector is pre-installed for new environments. Organisations with existing environments can download and install the app from AppSource. The organisation must have both a Business Central licence and a Shopify licence to use the connector. Learn more about supported countries, languages, and editions of [!INCLUDE[prod_short](../includes/prod_short.md)] at [Shopify Connector on the AppSource](https://go.microsoft.com/fwlink/?linkid=2196238).

The Shopify connector doesn't work for [Embed App](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview), where the client URL has the format: `https://[application name].bc.dynamics.com`. 

## <a name="what-support-is-offered-for-the-shopify-connector"></a>What support is offered for the Shopify connector?

### [!INCLUDE[prod_short](../includes/prod_short.md)]

The Shopify connector is covered by the current support model. Learn more at [Technical Support](/dynamics365/business-central/dev-itpro/administration//manage-technical-support) (in English only). 

Get help from a consultant that knows the Shopify connector for [!INCLUDE[prod_short](../includes/prod_short.md)], to meet your unique business-specific requirements.
 
Search in [Consultancy Services](https://aka.ms/BCShopifyConsultant).

### <a name="shopify"></a>Shopify

Get help with Shopify by starting with [General Shopify Help Centre](https://help.shopify.com/) or [24/7 Support for your store as a Shopify merchant](https://help.shopify.com/questions#/). 

You can also explore [Experts Marketplace](https://experts.shopify.com/) to find the right experts who offer services for Shopify merchants.

## <a name="currently-not-supported-features-however-were-tracking-them-and-may-consider-adding-them-in-the-future"></a>Currently not supported features, however, we're tracking them and may consider adding them in the future:

- B2B features, including Companies, company price lists, payment terms
- Markets
  - Multiple translations of master data. You can choose one language that will be used for product information export.
  - Prices per country/region. One price list is available for the selected currency. The conversion to other currencies will be handled by Shopify.

## <a name="is-the-shopify-connector-extensible"></a>Is the Shopify connector extensible?

Currently, this app is non-extensible with plans to make it extensible in 2023. 

## <a name="is-the-shopify-connector-open-for-contribution"></a>Is the Shopify connector open for contribution

Yes, this extension is open for contribution by the community. You can find the [source code](https://github.com/microsoft/ALAppExtensions/tree/main/Apps/W1/Shopify) in the Microsoft AL application add-ons repository.


## <a name="see-also"></a>See Also

[Get Started with the Connector for Shopify](get-started.md)  
