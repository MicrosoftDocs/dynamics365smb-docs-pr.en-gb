---
title: Troubleshoot Your Automated Workflows
description: Learn how to troubleshoot the connection between Business Central and Power Automate when you build an automated workflow.
author: jswymer
ms.topic: conceptual
ms.search.keywords: 'workflow, OData, Power App, SOAP, Entity set not found, workflowWebhookSubscriptions, Power Automate,'
ms.date: 07/03/2023
ms.author: jswymer
ms.reviewer: jswymer
ms.service: d365-business-central
---

# <a name="troubleshoot-your--automated-workflows"></a>Troubleshoot Your [!INCLUDE[prod_short](includes/prod_short.md)] Automated Workflows

When you connect [!INCLUDE [prod_short](includes/prod_short.md)] with Power Automate to create automated workflows, you might run into error messages. This article provides suggested solutions to recurring problems.

## <a name="flow-doesnt-run-on-all-records-created-or-changed"></a>Flow doesn't run on all records created or changed

### <a name="problem"></a>Problem

If an event creates or changes many records, the flow doesn't run on some or all records.

### <a name="possible-cause"></a>Possible cause

Currently, there's a limit on how many records a flow can process. If more than 1000 records are created or changed within 30 seconds, the flow isn't triggered.

> [!NOTE]
> For developers, the flow triggering is done via webhook notifications, and this limitation is due to the way the Business Central connector handles `collection` notifications. Learn more at [Working with Webhooks in Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/api-reference/v2.0/dynamics-subscriptions#notes-for-power-automate-flows) in the Developer and Admin help.

## <a name="the-response-from-the-business-central-service-is-too-large-error"></a>"The response from the Business Central service is too large" error

### <a name="problem-1"></a>Problem

When using an action that interacts with records (such as *Create record (V3)* and *Get record (V3)*), Power Automate might display an error similar to this one:

`The response from the Business Central service is too large`

### <a name="possible-cause-1"></a>Possible cause

Even though Business Central has no set limit on the size of records returned by APIs, the Dynamics 365 Business Central connector for Power Automate can handle only records up to 8 MB.

All the Business Central APIs provided by Microsoft return records under this limit, but APIs provided by partners might not. If you see an error "The response from the Business Central service is too large", reach out to the partner who created the API you're using.

## <a name="entity-set-not-found-error"></a>"Entity set not found" error

### <a name="problem-2"></a>Problem

When you create a new Power Automate flow using a [!INCLUDE[prod_short](includes/prod_short.md)] approval trigger, such as *When a purchase document approval is requested*, you might get an error message similar to this one:

`Entity set not found: \<name\>`

The placeholder, `\<name\>`, is the service name of the missing web service, such as *workflowWebhookSubscriptions* or *workflowPurchaseDocumentLines*.

### <a name="possible-cause-2"></a>Possible cause

Using Power Automate for approvals requires certain page and codeunit objects to be published as web services. By default, most of the required objects are published as web services. But in some cases, your environment may have been customised so these objects are no longer published.

### <a name="fix"></a>Fix

Go to the **Web Services** page and make sure the following objects are published as web services. There should be an entry in the list for each object, with the **Published** check box selected.  

| Object Type | Object ID | Object Name | Service Name |
|--|--|--|--|
| Codeunit | 1544 | WorkflowWebhookSubscription | WorkflowActionResponse |
| Page | 6408 | workflowCustomers | workflowCustomers |
| Page | 6406 | workflowGenJournalBatches | workflowGenJournalBatches |
| Page | 6407 | workflowGenJournalLines | workflowGenJournalLines |
| Page | 6409 | workflowItems | workflowItems |
| Page | 6405 | Purchase Document Line Entity | workflowPurchaseDocumentLines |
| Page | 6404 | workflowPurchaseDocuments | workflowPurchaseDocuments |
| Page | 6403 | Sales Document Line Entity | workflowSalesDocumentLines |
| Page | 6402 | workflowSalesDocuments | workflowSalesDocuments |
| Page | 6410 | workflowVendors | workflowVendors |
| Page | 831 | workflowWebhookSubscriptions | workflowWebhookSubscriptions |

> [!NOTE]
> The **Service Name** value must be exactly as shown in the table. Don't change or translate the service name.

Learn more about publishing web services at [Publish a Web Service](across-how-publish-web-service.md).

## <a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/use-power-automate/).

## <a name="see-also"></a>See also

[Use Power Automate Flows in [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-flow.md)  
[Workflow](across-workflow.md)  
[Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  
[Switch on Instant Flows](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)  
[Manage Power Automate Flows](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
