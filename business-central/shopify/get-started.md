---
title: Getting started with connector for Shopify
description: First steps when configuring connection between Business Central and Shopify
ms.date: 05/16/2022
ms.topic: article
ms.service: dynamics365-business-central
ms.reviewer: solsen
author: AndreiPanko
ms.author: andreipa
ms.openlocfilehash: 2b88995cad8cfe0c3688ca062643f2d339fed9bf
ms.sourcegitcommit: f071aef3660cc3202006e00f2f790faff849a240
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/18/2022
ms.locfileid: "8768203"
---
# <a name="get-started-with-the-shopify-connector"></a>Get Started with the Shopify Connector

[!INCLUDE [prod_short](../includes/prod_short.md)] gives you the flexibility to connect your Shopify store (or stores) with it to maximise your business productivity. You can manage and view insights from your business and your Shopify online store as one unit by using the Shopify connector. To use Shopify with [!INCLUDE [prod_short](../includes/prod_short.md)], you need to follow some steps. This page serves as a guide to complete the integration of your Shopify store with [!INCLUDE [prod_short](../includes/prod_short.md)].

## <a name="prerequisites-for-shopify"></a>Prerequisites for Shopify

You must have:

- A Shopify account
- A Shopify online store

To create a new Shopify account or sign-up for a free 14-day trial, navigate to [Shopify](https://www.shopify.com/). For more information on how to create and personalise your online store, see [Shopify Help Centre](https://help.shopify.com/).
  
- Other sales channels are supported, for example, Shopify POS.

### <a name="recommended-settings"></a>Recommended settings

- Deactivate **Automatically archive the order** in the **Order Processing** section of the [**Checkout**](https://www.shopify.com/admin/settings/checkout) settings in your **Shopify admin**.

To know more about Shopify settings for demo and trial scenarios, see [Test and training scenarios](/dynamics365/business-central/dev-itpro/administration/admin-shopify-connector#preparation).

## <a name="prerequisites-for-business-central"></a>Prerequisites for Business Central

- Make sure that the **Connect to Shopify for [!INCLUDE[prod_short](../includes/prod_short.md)]** extension is installed.

The extension is pre-installed for all new sign ups and trials. If you need to install extensions from the Market place, visit [Installing and Uninstalling Extensions](../ui-extensions-install-uninstall.md#install). Follow the steps listed below if you don't have [!INCLUDE[prod_short](../includes/prod_short.md)].
<!--
## Installing the **Dynamics 365 Business Central** app to your Shopify online store

For existing [!INCLUDE[prod_short](../includes/prod_short.md)], this step is optional and can be skipped.

1. Locate the [Dynamics 365 Business Central](https://apps.shopify.com/dynamics-365-business-central) app on the [Shopify AppStore](https://apps.shopify.com/)
2. Choose the **Add App** button. Sign-in into your Shopify account if prompted. Select the required online shop if you've more than one.
3. After reviewing privacy and permissions, choose the **Install App** button.
  You can find and open the installed **Dynamics 365 Business Central** app in the **Apps** section on the sidebar of **Shopify admin**.
4. Choose **Sign up now** to start [!INCLUDE[prod_short](../includes/prod_short.md)] trial or **Sign in** if you already have [!INCLUDE[prod_short](../includes/prod_short.md)]. You'll be redirected to your [!INCLUDE[prod_short](../includes/prod_short.md)] at [Business Central](https://businesscentral.dynamics.com).
5. The next steps should be done in [!INCLUDE[prod_short](../includes/prod_short.md)].
-->
## <a name="connecting-business-central-to-the-shopify-online-store"></a>Connecting Business Central to the Shopify online store

1. Go to search ![Lightbulb that opens the Tell Me feature.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Shop** and choose the related link.
2. Choose the **New** action.  
3. In the **Code** field, enter the desired code.  
4. In **Shopify URL** field, type URL of your online shop, which needs to be connected.
5. Activate **Enabled** toggle, review and accept the terms and conditions.
6. If prompted, sign-in into your Shopify account, review privacy and permissions, and then choose the **Install App** button.

Repeat steps 2-6 for all online shops that you want to connect.

### <a name="next-steps"></a>Next steps

Now your online shop is connected to [!INCLUDE[prod_short](../includes/prod_short.md)]. In the next steps, you'll define how and what to synchronise.

- [Synchronise Items](synchronize-items.md)
- [Synchronise Customers](synchronize-customers.md)
- [Synchronise Orders](synchronize-orders.md)

## <a name="see-also"></a>See Also

[Test and training scenarios](/dynamics365/business-central/dev-itpro/administration/admin-shopify-connector).

