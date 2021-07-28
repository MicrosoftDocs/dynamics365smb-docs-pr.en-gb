---
title: Power BI FAQ
description: Get answers for some typical questions about working with Power BI and Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Power BI, reports, faq, errors
ms.date: 04/22/2021
ms.author: jswymer
ms.openlocfilehash: ef63963c7c37f36db34e3e8292e73d64c1b67538
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6438759"
---
# <a name="power-bi--faq"></a>Power BI  FAQ

This article answers some of the questions you may have about working with Power BI and [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[General](#tab/general)
<!-- 26 -->
### <a name="ive-selected-a-report-for-my-role-center-in-business-central-if-i-later-make-changes-to-the-reports-visuals-online-will-the-role-center-automatically-update-to-my-changes"></a>I've selected a report for my role centre in Business Central. If I later make changes to the report's visuals online, will the role centre automatically update to my changes?

Yes, because the reports are embedded from Power BI.

<!-- 3 -->
### <a name="are-the-business-central-apps-for-power-bi-available-in-languages-other-than-english"></a>Are the Business Central apps for Power BI available in languages other than English?

No. These apps are currently only available in English.

<!-- 24 -->
### <a name="once-a-report-is-published-on-mypowerbicomworkspace-can-i-download-its-pbix"></a>Once a report is published on my powerbi.com workspace, can I download its pbix? 

Yes. For more information, see [Download a report from the Power BI service to Power BI Desktop](/power-bi/create-reports/service-export-to-pbix).  

<!-- 27 -->
### <a name="can-i-download-the-apps-as-pbix-files"></a>Can I download the apps as pbix files? 

No. Currently, we don’t offer downloading pbix files for the official Power BI apps, because they're published on AppSource.

## <a name="license"></a>[Licence](#tab/license)

<!-- 14 -->
### <a name="do-i-need-a-power-bi-pro-license-to-publish-reports"></a>Do I need a Power BI Pro licence to publish reports? 

<!-- todo What does " or for every user that consults the published report" mean? fixed -->
No. A Pro licence isn't needed to publish reports. The standard (free) Power BI licence is enough. For more information, see [Power BI Licensing](admin-powerbi-setup.md#license).

<!-- 15 -->
### <a name="is-there-anything-i-cant-do-with-the-free-license"></a>Is there anything I can't do with the free licence?

You can't share reports or install the Business Central apps for Power BI. Other than that, the free licence allows you to create almost all variations of charts and reports.

<!-- 16 -->
### <a name="if-someone-shares-a-report-with-another-person-then-that-person-needs-a-pro-license-to-see-the-report-are-there-plans-to-make-this-capability-possible-with-the-free-license"></a>If someone shares a report with another person, then that person needs a Pro licence to see the report. Are there plans to make this capability possible with the free licence?

We don't have control over this requirement. This requirement is set by Power BI. For more information, see [Share Power BI dashboards and reports with coworkers and others](/power-bi/collaborate-share/service-share-dashboards).  

## <a name="designer"></a>[Designer](#tab/designer)

<!-- 7 -->
### <a name="does-the-connector-work-with-api-pages"></a>Does the connector work with API pages?

Yes. Starting in June 2021, the new Power BI connector supports both Business Central web services and API pages. For more information, see [Enable Power BI connector to work with Business Central APIs, instead of with web services only](/dynamics365-release-plan/2021wave1/smb/dynamics365-business-central/enable-power-bi-connector-work-business-central-apis-instead-web-services-only).

### <a name="can-i-build-a-power-bi-report-using-the-sales-invoice-lines-or-journal-lines-apis"></a>Can I build a Power BI report using the Sales Invoice Lines or Journal Lines APIs?

The most commonly used line records are available in the [Business Central APIs v2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/)). So you can use them to build reports in Power BI by selecting them in the **Dynamics 365 Business Central** connector. However, the **Lines** APIs are designed to be used only with some very specific filters, and might not work in your scenario. You might get an error similar to "You must specify an Id or a Document Id to get the lines". To fix this problem, do the following steps when getting data from Business Central for the report in Power BI Desktop:

1. Instead of including the data source for the lines entity, add the parent data source. For example, add **Sales Invoice** instead of **Sales Invoice Lines**.
2. Select **Transform Data** in the Power BI Desktop action bar.
3. Select the query you just added, for example **Sales Invoices**.
4. Apply any needed filtering on the records to reduce the amount of records loaded in your report.
5. Scroll to the right until you find a column named as the lines, for example **SalesInvoiceLines**.
6. Select the expand button in the header of the column, next to the column name.

   :::image type="content" source="media/saleinvoicelines.png" alt-text="Shows the SalesInvoiceLines column in Power BI Desktop.":::
<!-- 11 --> 
### <a name="is-it-possible-to-choose-which-business-central-environment-to-get-data-from-for-power-bi-for-example-like-a-sandbox-or-production-environment"></a>Is it possible to choose which Business Central environment to get data from for Power BI, for example, like a sandbox or production environment? 

Yes. It can be easily chosen. When you connect to Business Central using the connector, you have to choose the environment and company name.

<!-- 6 --> 
### <a name="can-i-merge-data-from-several-production-environments-of-the-same-tenant"></a>Can I merge data from several production environments of the same tenant?

Yes. In Power BI, just run the get data operation again and choose the environment you want.

<!-- 25 -->
### <a name="which-pages-in-business-central-have-the-power-bi-report-part"></a>Which pages in Business Central have the Power BI Report part?  

Currently, there are a few selected pages that have a FactBox with a **Power BI Reports** part for displaying a report. 

On list pages, the **Power BI Reports** part is filtered to show reports that pertain to data in the list. Here's the list type pages that include the **Power BI Reports** part:

|Page ID|Name|
|-------|----|
|22|Customer List|
|27|Supplier List|
|31|Item List|
|9305|Sales Order List|
|9308|Purchase Invoices|

Here are other pages that contain the larger, non-filtered **Power BI Reports** part:

|Page ID|Name|
|-------|----|
|1156|Company Detail|
|4013|Intelligent Cloud Insights |
|9006|Order Processor Role Centre|
|9008|Whse. Basic Role Centre|
|9010|Production Planner Role Centre|
|9015|Job Project Manager RC|
|9016|Service Dispatcher Role Centre|
|9022|Business Manager Role Centre|
|9024|Security Admin Role Centre|
|9026|Sales & Relationship Mgr. RC|
|9027|Accountant Role Centre|

> [!TIP]
> We don't have plans to add it to all list pages at the moment. However, you can create a simple page extension that adds the **Power BI Reports** part in a FactBox. For more information, see [Adding Power BI Report Parts to Pages](/dynamics365/business-central/dev-itpro/developer/devenv-power-bi-report-parts) in the Developer and IT Pro help.

<!-- 5 -->
### <a name="is-there-any-way-to-filter-a-dataset-from-business-central-before-i-pull-it-into-power-bi-instead-of-applying-filters-afterwards"></a>Is there any way to filter a dataset from Business Central *before* I pull it into Power BI, instead of applying filters afterwards?

To filter larger datasets, the easiest way is to set a filter on your Power BI report by editing directly the Power Query formula. Most of the filters you set this way will be passed on to Business Central through query folding. See [Incremental refresh for datasets](/power-bi/admin/service-premium-incremental-refresh).

There's currently no way of setting a filter for the web service data from within Business Central. If your application needs to set a filter from within Business Central, you'll have to create a custom Business Central App for this purpose.

<!-- 8 and 9 -->

### <a name="for-embedding-reports-in-business-central-pages-right-now-its-only-possible-to-get-reports-from-my-workspace-in-power-bi-are-there-plans-to-make-it-possible-to-get-them-from-custom-workspaces"></a>For embedding reports in Business Central pages, right now it's only possible to get reports from *My Workspace* in Power BI. Are there plans to make it possible to get them from custom workspaces?

Yes. We have it in our plans to add support for shared workspaces, but we don't yet have a timeline to give you.  

<!-- 10 -->
### <a name="from-power-bi-besides-using-a-query-is-there-another-way-to-get-data-from-business-central-tables-that-dont-have-an-associated-page-for-example-like-the-item-attributes-value-mapping-table"></a>From Power BI, besides using a query, is there another way to get data from Business Central tables that don't have an associated page? For example, like the *Item Attributes Value Mapping* table.

No. Not at this point.

<!-- 12 --> 
### <a name="are-published-queries-faster-to-use-than-published-pages"></a>Are published queries faster to use than published pages?

When it comes to web services, published queries are usually faster than equivalent published pages. The reason is that queries are optimised for reading data and don’t contain expensive triggers like OnAfterGetRecord.

When the new connector is available in June 2021, you're encouraged to use API pages over queries published as web services.

<!-- 13 --> 
### <a name="is-there-a-way-for-an-end-user-to-create-a-web-service-with-a-column-thats-in-a-business-central-table-but-not-a-page-or-will-the-developer-have-to-create-a-custom-query"></a>Is there a way for an end user to create a web service with a column that's in a Business Central table, but not a page? Or will the developer have to create a custom query? 

Yes. With the release of the new connector in June 2021, a developer can create a new API page to meet this requirement. 

<!-- 28 --> 
### <a name="can-i-connect-power-bi-to-a-read-only-database-server-of-business-central-online"></a>Can I connect Power BI to a read-only database server of Business Central online? 

No. But we have this feature on our long-term roadmap. 

### <a name="how-do-i-change-or-clear-the-user-account-im-currently-using-to-connect-to-business-central-from-power-bi-desktop"></a><a name="perms"></a>How do I change or clear the user account I'm currently using to connect to Business Central from Power BI Desktop?

In Power BI Desktop, do the following steps:

1. In the File menu, select **Options and settings** > **Data source settings**.
2. Select **Dynamics Business Central** from the list, then select **Clear permissions** > **Delete**.

Then next time you connect to Business Central to get data, you'll be asked to sign in.

## <a name="performance"></a>[Performance](#tab/performance)

<!-- 17 -->

### <a name="is-it-faster-to-get-data-using-api-pages-than-using-web-services"></a>Is it faster to get data using API pages than using web services?

Yes. Our tests indicate that API pages are up to 25% more performant than web services.

<!-- 18 -->
### <a name="are-there-plans-to-have-a-mirror-on-the-azure-sql-database-instance-which-i-can-connect-to-directly"></a>Are there plans to have a mirror on the Azure SQL Database instance, which I can connect to directly?

No. Not at this point. You can only communicate with Business Central through APIs.

<!-- 19 -->
### <a name="loading-data-from-business-central-web-services-seems-slow-is-there-any-way-to-get-data-directly-from-the-sql-database-table"></a>Loading data from Business Central web services seems slow. Is there any way to get data directly from the SQL database table?

No. Direct access to the database isn't possible, but switching to API pages (when the new connector available) will help greatly.

## <a name="advanced"></a>[Advanced](#tab/advanced)
<!-- 1 -->

### <a name="are-there-plans-for-the-power-bi-connector-to-support-the-incremental-refresh-features-in-the-power-bi-service"></a>Are there plans for the Power BI connector to support the incremental refresh features in the Power BI Service?

Yes. It's on our roadmap.

<!-- 2 -->
### <a name="if-a-business-central-on-premises-solution-doesnt-have-internet-access-can-i-still-use-power-bi"></a>If a Business Central on-premises solution doesn't have internet access, can I still use Power BI?
<!-- todo: please explain this one-->

Yes. In this case, you use Power BI Desktop locally and connect to the Business Central on-premises. Once connected, can create and view reports, but you just can't publish them to the Power BI Service. 
<!-- 20 -->
### <a name="are-there-any-plans-to-make-it-possible-to-replicate-business-central-online-databases-so-theyre-accessible-for-read-only-sql-queries-this-capability-would-support-incremental-refresh-and-be-a-lot-faster-than-apis-or-web-services"></a>Are there any plans to make it possible to replicate Business Central online databases so they're accessible for read-only SQL queries? This capability would support incremental refresh and be a lot faster than API's or web services.

<!-- todo: what does "BC-Saas-DB-replicated DB accessible" mean? fixe-->
Yes. We have this feature on our long-term roadmap. 

<!-- 21 -->
### <a name="if-i-use-azure-data-factory-to-get-data-from-business-central-and-consume-it-on-power-bi-will-that-help-in-increase-in-performance"></a>If I use Azure Data Factory to get data from Business Central and consume it on Power BI, will that help in increase in performance? 

Yes. This advanced scenario will help Business Central stay performant, because the data access would be done via the Azure Data Factory.

<!-- 22 -->
### <a name="are-there-any-plans-to-support-power-bi-deployment-pipelines-or-a-way-to-build-deployment-pipelines-for-pbi-reports-similar-to-extensions-or-maybe-even-a-simple-api-in-the-business-admin-center"></a>Are there any plans to support Power BI deployment pipelines or a way to build deployment pipelines for PBI reports, similar to extensions? Or maybe even a simple API in the Business Admin Centre? 

We're looking into this feature. Power BI offers rich APIs to control report deployments. For more information, see [Introduction to deployment pipelines](/power-bi/create-reports/deployment-pipelines-overview).

### <a name="ive-tried-the-preview-of-the-new-connector-which-will-be-live-in-june-2021-i-see-some-values-like-_x0020_-when-connecting-to-api-v20-what-are-these-values"></a>I've tried the preview of the new connector, which will be live in June 2021. I see some values like "_x0020_" when connecting to API v2.0. What are these values?

The upcoming version of the Power BI connector enables you to connect to the Business Central API pages, including API v2.0. These pages include a few fields based on [AL Enum objects](/dynamics365/business-central/dev-itpro/developer/devenv-extensible-enums). Fields based on AL Enum objects must have names that are consistent and always the same, so that filters on the report always work&mdash;no matter the language or operating system you're using. For this reason, the fields based on AL Enums aren't translated and are encoded to avoid any special character, including the space. In particular, whenever there's an empty option in the AL Enum object, it's encoded to "_x0020_". You can always apply a transformation to your data on Power BI if you want to display some different value for these fields, for example "Empty".


---

## <a name="see-also"></a>See Also

[Power BI Licensing](admin-powerbi-setup.md#license)
[Business Central and Power BI Introduction](admin-powerbi.md)  
[Power BI Integration Overview](admin-powerbi-overview.md)  
[Enabling Power BI in Business Central](admin-powerbi-setup.md)  
[Working with Power BI Reports in Business Central](across-working-with-powerbi.md)  
[Working with Business Central Data in Power BI](across-working-with-business-central-in-powerbi.md)  
[Building Power BI Reports to Display Business Central Data](across-how-use-financials-data-source-powerbi.md)    
[Power BI documentation](/power-bi/)  


[!INCLUDE[footer-include](includes/footer-banner.md)]