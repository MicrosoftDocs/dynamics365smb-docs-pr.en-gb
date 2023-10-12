---
title: FAQ for technical details
description: Implementation details related to the Shopify connector.
ms.date: 03/27/2023
ms.topic: article
ms.service: dynamics365-business-central
author: brentholtorf
ms.author: bholtorf
---

# <a name="faq-for-technical-details"></a>FAQ for Technical Details

This article answers frequently asked questions about the Shopify connector.

## <a name="what-is-shopify"></a>What is Shopify?

Shopify is a subscription-based application that allows anyone to set up an online store and sell products. The Shopify platform offers online retailers a suite of services for payments, marketing, shipping, and customer engagement.

## <a name="what-is-the-microsoft-dynamics-365-business-central-shopify-connector"></a>What is the Microsoft Dynamics 365 Business Central Shopify connector?

With the Shopify connector, businesses can link their Shopify store (or stores) with [!INCLUDE[prod_short](../includes/prod_short.md)] to maximise business productivity. Using the Shopify connector, they can access and manage insights from their business and their Shopify online store as one unit.

### <a name="capabilities"></a>Capabilities

- Support for more than one Shopify shop
  - Each shop has its own setup, including a collection of products and locations used to calculate inventory and price lists.  
- Bi-directional synchronisation of items or products
  - The connector synchronises images, item variants, bar codes, vendor item numbers, extended texts, and tags.  
  - Export item attributes to Shopify.  
  - Use selected customer price groups and discounts to define prices exported to Shopify.  
  - Decide whether items can be created automatically or only allow updates to existing products.  
- Synchronisation of inventory levels
  - Choose some or all of the available locations in [!INCLUDE [prod_short](../includes/prod_short.md)].  
  - Update inventory levels on multiple locations in Shopify.  
- Bi-directional synchronisation of customers
  - Smart-map customers by phone and email.  
  - Use specific country/region templates when creating customers, which helps ensure that tax settings are correct.  
- Import orders from Shopify
  - Include orders created in various sales channels, such as Online store or **Shopify POS**.
  - Shipping costs, gift cards, tips, shipping and payment methods, transactions, and risk of fraud.  
  - During import, you can automatically create customers in [!INCLUDE [prod_short](../includes/prod_short.md)] or decide to manage the customers in Shopify.  
  - Receive payout information from Shopify Payments.
- Track fulfillment information
  - Optionally, choose to transfer item tracking information from [!INCLUDE [prod_short](../includes/prod_short.md)] to Shopify.  

## <a name="why-did-microsoft-and-shopify-form-this-partnership"></a>Why did Microsoft and Shopify form this partnership?

[!INCLUDE[prod_short](../includes/prod_long.md)] is teaming up with Shopify to help our customers create a better shopping experience. While Shopify provides merchants with an easy-to-use commerce solution, [!INCLUDE[prod_short](../includes/prod_short.md)] offers comprehensive business management across finance, sales, service, and operations teams. Use the seamless connection between the applications to synchronise orders, stock, and customer information to fulfil orders faster, and better serve customers.

## <a name="which-microsoft-products-are-the-shopify-connector-available-for"></a>Which Microsoft products are the Shopify connector available for?

This feature is available only for [!INCLUDE[prod_short](../includes/prod_short.md)] online, starting with version 20.1. It isn't available for on-premises deployments. The connector is pre-installed for new environments. Organisations with existing environments can download and install the connector from AppSource. The organisation must have both a [!INCLUDE [prod_short](../includes/prod_short.md)] licence and a Shopify licence to use the connector. To learn more about supported countries/regions, languages, and editions of [!INCLUDE[prod_short](../includes/prod_short.md)], go to [Shopify Connector on the AppSource](https://go.microsoft.com/fwlink/?linkid=2196238).

The Shopify connector doesn't work for [Embed App](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview), where the client URL has the `https://[application name].bc.dynamics.com` format.

## <a name="what-support-is-offered-for-the-shopify-connector"></a>What support is offered for the Shopify connector?

### [!INCLUDE[prod_short](../includes/prod_short.md)]

The Shopify connector is covered by the current support model. Learn more at [Technical Support](/dynamics365/business-central/dev-itpro/administration//manage-technical-support) (in English only).

Get help from a consultant who knows the Shopify connector for [!INCLUDE[prod_short](../includes/prod_short.md)], to meet your unique business-specific requirements. Search in [Consultancy Services](https://aka.ms/BCShopifyConsultant).

### <a name="shopify"></a>Shopify

Get help with Shopify from the [General Shopify Help Centre](https://help.shopify.com/), or from [24/7 Support for your store as a Shopify merchant](https://help.shopify.com/questions#/).

You can also explore [Experts Marketplace](https://experts.shopify.com/) to find the right experts who offer services for Shopify merchants.

## <a name="currently-unsupported-features-however-were-tracking-them-and-may-consider-adding-them"></a>Currently unsupported features, however, we're tracking them and may consider adding them

- B2B features, including companies, company price lists, and payment terms
  - It is currently possible to import orders created via B2B. If you have multiple buyers linked to company, you should not enable automatic creation of customers, but link each Shopify buyer to a respective customer manually.
  - You will need to maintain company price lists in Shopify.
- Markets
  - Multiple translations of master data. You can choose one language that will be used for product information export.
  - Prices per country/region. One price list is available for the selected currency. Shopify handles the conversion to other currencies.
- Draft orders

## <a name="is-the-shopify-connector-extensible"></a>Is the Shopify connector extensible?

Yes, the Shopify connector is extensible. Check GitHub to access the [list of extensibility points](https://github.com/microsoft/ALAppExtensions/tree/main/Apps/W1/Shopify) and explore some [examples](https://github.com/microsoft/ALAppExtensions/blob/main/Apps/W1/Shopify/extensibility_examples.md).

## <a name="is-the-shopify-connector-open-for-contribution"></a>Is the Shopify connector open for contribution

Yes, this extension is open for contributions from our community. You can find the [source code](https://github.com/microsoft/ALAppExtensions/tree/main/Apps/W1/Shopify) in the Microsoft AL application add-ons repository.

## <a name="see-also"></a>See Also

[Get Started with the Connector for Shopify](get-started.md)  
