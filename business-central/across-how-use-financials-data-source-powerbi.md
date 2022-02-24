---
title: Use Business Central in Power BI reports | Microsoft Docs
description: Make your data available as a data source in Power BI and build powerful reports of the state of your business.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 4f140303f037ea4a914cba1ded44fd453bcdfabb
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3187899"
---
# <a name="using-prodlong-as-power-bi-data-source-for-building-reports"></a>Using [!INCLUDE [prodlong](includes/prodlong.md)] as Power BI Data Source for Building Reports

You can make your [!INCLUDE[prodlong](includes/prodlong.md)] data available as a data source in Power BI and build powerful reports of the state of your business.  

You must have a valid account with [!INCLUDE[prodshort](includes/prodshort.md)] and with Power BI. You must also download [Power BI Desktop](https://powerbi.microsoft.com/desktop/). For more information, see [Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data).  

## <a name="to-add-prodshort-as-a-data-source-in-power-bi-desktop"></a>To add [!INCLUDE[prodshort](includes/prodshort.md)] as a data source in Power BI Desktop

1. In Power BI Desktop, in the left navigation pane, choose **Get Data**.
2. On the **Get Data** page, choose **Online Services**, choose **Microsoft Dynamics 365 Business Central**, and then choose the **Connect** button.
3. Power BI displays a wizard that will guide you through the connection process, including signing into [!INCLUDE [prodshort](includes/prodshort.md)]. Choose **Sign in**, and then choose the relevant account. Use the same account that you sign into [!INCLUDE [prodshort](includes/prodshort.md)] with.
4. Choose the **Connect** button to continue. The Power BI wizard shows a list of Microsoft [!INCLUDE[d365fin](includes/d365fin_md.md)] environments, companies, and data sources. These data sources represent all the web services that you have published from [!INCLUDE [prodshort](includes/prodshort.md)].

    You can also create a new web service URL in [!INCLUDE [prodshort](includes/prodshort.md)] instead. Choose one of the following methods:

      - Use the **Create Data Set** action on the **Web Services** page
      - Use the **Set Up Reporting** Assisted Setup guide
      - Choose the **Edit in Excel** action in any lists

5. Specify the data you want to add to your data model, and then choose the **Load** button.
6. Repeat the previous steps to add additional [!INCLUDE [prodshort](includes/prodshort.md)], or other data, to your Power BI data model.

> [!NOTE]  
> Once you have successfully connected to [!INCLUDE [prodshort](includes/prodshort.md)], you will not be prompted again to sign in.

Once the data is loaded, you can see it in the right navigation on the page. You have successfully connected to your [!INCLUDE [prodshort](includes/prodshort.md)] data, and you can begin building your Power BI report.  

Before building your report, we recommend that you import the [!INCLUDE [prodshort](includes/prodshort.md)] theme file.  The theme file will create a colour palette so that you can build reports with the same colour styling as the [!INCLUDE [prodshort](includes/prodshort.md)] apps without requiring you to define custom colours for each visual.

For more information, see the [Power BI documentation](/power-bi/consumer/).

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Enabling Your Business Data for Power BI](admin-powerbi.md)  
[Business Intelligence](bi.md)  
[Getting Started](product-get-started.md)  
[Importing Business Data from Other Finance Systems](across-import-data-configuration-packages.md)  
[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Finance](finance.md)  
[Quickstart: Connect to data in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
