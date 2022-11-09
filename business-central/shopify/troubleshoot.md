---
title: Troubleshooting the Shopify and Business Central Synchronisation
description: Learn what to do if something goes wrong during the synchronisation of data between Shopify and Business Central
ms.date: 08/19/2022
ms.topic: article
ms.service: dynamics365-business-central
ms.search.form: 30118, 30119, 30120,
author: edupont04
ms.author: andreipa
ms.reviewer: solsen
ms.openlocfilehash: 37fb8069f6149cc89c1c53f671eafe3788f54ccf
ms.sourcegitcommit: 5bb13966e9ba8d7a3c2f00dd32f167acccf90b82
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/28/2022
ms.locfileid: "9728364"
---
# <a name="troubleshooting-the-shopify-and-business-central-synchronization"></a>Troubleshooting the Shopify and Business Central Synchronisation

It's possible to run into situations where you need to troubleshoot issues when synchronising data between Shopify and [!INCLUDE[prod_short](../includes/prod_short.md)]. This page defines troubleshooting steps for some common scenarios that may occur.

## <a name="logs"></a>Logs

If a synchronisation task fails, you can activate logging by enabling the **Log Enable** toggle on the **Shopify Shop Card** page. Then you can manually trigger the synchronisation task and review logs.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify Log Entries**, and choose the related link.
2. Select the related log entry and open the **Shopify Log Entry** page.
3. Review the request, status code and description, and response values.

Later, remember to switch logging off to avoid negative performance impacts and increases in database size.

From the **Shopify Log Entries** page, you can trigger the deletion of all log entries or ones older than seven days.

## <a name="data-capture"></a>Data capture

Regardless of the **Log Activated** settings, some Shopify responses always get logged so you can inspect or download them using the **Data Capture List** page.

Choose the **Retrieved Shopify Data** action on one of the following pages:

- **Shopify order**
- **Shopify order fulfillments**
- **Shopify order shipping costs**
- **Shopify order transactions**
- **Shopify payouts**
- **Shopify payment transactions**
- **Shopify transactions**

## <a name="reset-sync"></a>Reset sync

For optimal performance, the connector imports only customers, products, and orders created or changed since the last synchronisation. On the **Shopify Shop Card** page, there are functions that change the date/time of the last synchronisation or completely reset it. This function ensures that when the sync is run, all data is synced rather than just the changes since the last sync.

This function only applies to syncs from Shopify to [!INCLUDE[prod_short](../includes/prod_short.md)]. It can be useful if you need to restore deleted data such as products, customers, or deleted orders.

## <a name="request-the-access-token"></a>Request the access token

If [!INCLUDE[prod_short](../includes/prod_short.md)] won't connect to your Shopify account, try to request the access token from Shopify. This request might be needed if there is a rotation of security keys or changes in required permissions (scopes).

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify shops**, and choose the related link.
2. Select the shop for which you want to get the access token to open the **Shopify Shop Card** page.
3. Choose the **Request Access** action.
4. If prompted, sign in to your Shopify account.

The **Has AccessKey** toggle will be activated.

### <a name="verify-and-enable-permissions-to-make-http-requests-when-running-in-a-non-production-environment"></a>Verify and enable permissions to make http requests when running in a non-production environment

To work correctly, the Shopify Connector extension requires permission to make http requests. When testing in a sandbox, the http requests are prohibited for all extensions.

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **extension management**, and choose the related link.
2. Select the **Shopify Connector** extension.
3. Choose the **Configure** action to open the **Extension Setting** page.
4. Make sure that the **Allow HTTPClient Requests** toggle is enabled.

## <a name="rotate-the-shopify-access-token"></a>Rotate the Shopify access token

The following procedures describe how to rotate the access token used by the Shopify connector to access your Shopify online shop.

### <a name="in-shopify"></a>In Shopify

1. From your **Shopify Admin**, go to [Apps](https://www.shopify.com/admin/apps).
2. Select **Delete** in the row with the **Dynamics 365 Business Central** app.
3. Select **Delete** in the message that appears.

### <a name="in-prod_short"></a>In [!INCLUDE[prod_short](../includes/prod_short.md)]

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shopify shops**, and choose the related link.
2. Select the shop for which you want to rotate the access token to open the **Shopify Shop Card** page.
3. Choose the **Request Access** action.
4. If prompted, sign in to your Shopify account, review privacy and permissions, and then choose the **Install App** button.

## <a name="known-issues"></a>Known issues

### <a name="the-gen-bus-posting-group-cannot-be-zero-or-empty-there-must-be-a-value-in-the-customer-field"></a>The *Gen. Bus. Posting Group* cannot be zero or empty; there must be a value in the customer field

On the **Shopify Shop Card** page, fill in the **Customer Template Code** field with the template that has **Gen. Bus. Posting Group** populated. The customer template is used not only for the creation of customers but also for the calculation of the sales price and during the creation of sales documents.

### <a name="importing-data-to-your-shopify-shop-isnt-enabled-go-to-the-shop-card-to-enable-it"></a>Importing data to your Shopify shop isn't enabled. Go to the shop card to enable it

On the **Shopify Shop Card** window, turn on the **Allow Data Sync to Shopify** toggle. This toggle is intended to protect the online shop from getting demo data from [!INCLUDE[prod_short](../includes/prod_short.md)].

### <a name="oauth-error-invalid_request-could-not-find-shopify-api-application-with-api_key"></a>Oauth error invalid_request: Could not find Shopify API application with api_key

It seems you use the [Embed App](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview), where the client URL has the format: `https://[application name].bc.dynamics.com`. The Shopify connector doesn't work for Embed Apps. For more information, see [What Microsoft products is the Shopify connector available for](shopify-faq.md#what-microsoft-products-is-the-shopify-connector-available-for).

## <a name="see-also"></a>See also 

[Get Started with the Connector for Shopify](get-started.md)
