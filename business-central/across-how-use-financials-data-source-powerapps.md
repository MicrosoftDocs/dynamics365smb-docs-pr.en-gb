---
title: Use Your Data to Create an App| Microsoft Docs
description: You can make your Business Central data available as a data source and specify an OData URL of your web services to build a business app using Power Apps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OData, Power App, SOAP
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 25607473e20bca8cec8cd65e2e808e12dda47869
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774543"
---
# <a name="connecting-to-your-business-central-data-to-build-a-business-app-using-power-apps"></a>Connecting to Your Business Central Data to Build a Business App Using Power Apps

You can make your [!INCLUDE[prod_short](includes/prod_short.md)] data available as a data source in Power Apps.  

> [!NOTE]  
> You must have a valid account with [!INCLUDE[prod_short](includes/prod_short.md)] and with Power Apps.  

## <a name="to-add-prod_short-as-a-data-source-in-power-apps"></a>To add [!INCLUDE[prod_short](includes/prod_short.md)] as a data source in Power Apps

1. In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/), and then sign in.
2. On the Home page, in the **Start from data** section, choose the **Other data sources** tile.  

    This opens Power Apps Studio. On first login, you must specify the country/region.  
3. In the list of available connections, choose **Business Central**, and then choose the **Create** button.

    Power Apps will connect to your [!INCLUDE[prod_short](includes/prod_short.md)] using the credentials that you are signed in with. If you are not an administrator of your [!INCLUDE[prod_short](includes/prod_short.md)], you may have to sign in with another account.  

4. Power Apps will display a list of *Environments and companies* that are available from [!INCLUDE[prod_short](includes/prod_short.md)]. Choose the environment and company that contains the data you want to connect to, such as *PRODUCTION - My Company*.  

5. Next, you will be presented with a list of tables that are exposed as part of the API for your environment. Select the table that you want to connect to, and then choose **Connect**.

These so-called tables are exposed as endpoints by the [!INCLUDE[prod_short](includes/prod_short.md)] connector for Power Apps.  

> [!NOTE]
> If you want to include data from other tables in [!INCLUDE[prod_short](includes/prod_short.md)] in your app, then you must work with a developer to define a custom API in [!INCLUDE[prod_short](includes/prod_short.md)] and then consume that custom API through a custom connector in Power Apps. For more information, see [Create a custom connector from scratch](/connectors/custom-connectors/define-blank).  

At this point, you have successfully connected to your [!INCLUDE[prod_short](includes/prod_short.md)] data and are ready to begin building your PowerApp. You can add additional screens and connect to additional data from your [!INCLUDE[prod_short](includes/prod_short.md)]. For more information, see [Create a canvas app from a sample in Power Apps](/powerapps/maker/canvas-apps/open-and-run-a-sample-app).  

When you have designed and built your app, you can share it with your colleagues. For more information, see [Save and publish a canvas app in Power Apps](/powerapps/maker/canvas-apps/save-publish-app).  

> [!NOTE]
> If you want to connect to [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, then you must choose the **Business Central (on-premises)** connector in step 3.  

## <a name="see-also"></a>See Also

[Create a canvas app from a template in Power Apps](/powerapps/maker/canvas-apps/get-started-test-drive)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Getting Started Developing Connect Apps for Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-connect-apps)  


[!INCLUDE[footer-include](includes/footer-banner.md)]