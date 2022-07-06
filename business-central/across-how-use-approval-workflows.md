---
title: Approve or Reject Documents in Workflows| Microsoft Docs
description: Request, reject, or delegate an approval of, for example, a purchase or sales document, as part of a workflow.
author: SorenGP
ms.topic: conceptual
ms.workload: na
ms.search.keywords: reject, delegate, request
ms.date: 09/28/2021
ms.author: edupont
ms.openlocfilehash: 46c81fa887af70e7a2f516df38ec003392b1dabd
ms.sourcegitcommit: 00a8acc82cdc90e0d0db9d1a4f98a908944fd50a
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 06/29/2022
ms.locfileid: "9079357"
---
# <a name="use-approval-workflows"></a>Use Approval Workflows

When a record, such as a purchase document or a customer card, needs to be approved by someone in your organisation, you send an approval request as part of a workflow. Based on how the workflow is set up, the appropriate approver is then notified that the record requires their approval.

You set up approval workflows on the **Workflow** page. You must also set up approval users, including any relevant amount limits, in the **Approval User Setup** page. For more information, see [Setting Up Workflows](across-set-up-workflows.md).  

In addition to approval workflows described in this topic, you can perform various other workflow tasks. For more information, [Use Workflows](across-use-workflows.md).

Core approval workflows for purchases documents, sales documents, payment journals, customer cards, and item cards are ready to start as guides. For more information, see [Getting Ready for Doing Business](ui-get-ready-business.md).

## <a name="to-request-approval-of-a-record"></a>To request approval of a record

The following task is performed by an approval user.

1. On the page that presents the record, choose the **Send Approval Request** action.
2. To see all your approval requests, choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Approval Request Entries**, and then choose the related link.  

The status of the approval entry is updated from **Created** to **Open**. The status of the record, for example a purchase invoice, is updated from **Open** to **Pending Approval** and remains locked for processing until all approvers have approved the record.

When the approver has approved the record, the status changes to **Released**. You can then continue your tasks with the record.

## <a name="to-cancel-requests-for-approval"></a>To cancel requests for approval

The following task is performed by an approval user with approver rights.

A customer may want to change an order after it has been submitted for approval. In this case, you can cancel the approval process and make the necessary changes to the order before you request approval again.

- On the page that displays the record, choose the **Cancel Approval Request** action.

When the approval request has been cancelled, the status of the related approval entry is changed to **Cancelled**. The status of the record is updated from **Pending Approval** to **Open**. The approval process can then start again.

## <a name="to-approve-or-reject-requests-for-approval"></a>To approve or reject requests for approval

The following task is performed by an approval user with approver rights.

You can process approval requests on the **Requests to Approve** page, for example to approve multiple requests at a time. Alternatively, you can process each request on the related record, such as the **Purchase Invoice** page, by choosing the link in the notification that you receive.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requests to Approve**, and then choose the related link.
2. Select one or more lines for the record or records that you want to approve or reject.
3. Choose the **Approve**, **Reject**, or **Delegate** actions.

When a record has been approved or rejected, the approval status in the **Status** field changes to **Approved** or **Rejected**.

If an approver hierarchy is set up, the record status will be **Pending Approval** until all approvers have approved the record. Then the record status will change to **Released**.

At the same time, the approval status changes from **Created** to **Open** as soon as an approval request for the record is created. If the request is rejected, the approval status changes to **Rejected**. The status remains **Open** or **Rejected** until all approvers have approved the request.

## <a name="to-delegate-requests-for-approval"></a>To delegate requests for approval

The following task is performed by an approval user with approver rights.

To prevent documents from piling up or otherwise block the workflow, the approver and the approval administrator can delegate an approval request to a substitute approver. The substitute can either be a designated substitute, the direct approver, or the approval administrator, in that order of priority. You typically use this feature if an approver is out of office and is unable to approve requests before the due date.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Requests to Approve**, and then choose the related link.
2. Select one or more lines for the approval requests that you want to delegate to a substitute approver, and then choose the **Delegate** action.

A notification to approve the request is sent to the substitute approver.

## <a name="to-manage-overdue-approval-requests"></a>To manage overdue approval requests

The following task is performed by an approval user with approver rights.

At regular intervals, you must remind approval workflow users of overdue approval requests that they must react on. You use the **Send Overdue Approval Notifications** function for this.

The **Send Overdue Approval Notifications** function checks for all open approval requests that are currently overdue. Each approver that has at least one overdue approval entry receives a notification with the list of all their overdue approval requests. The notification is also sent to their approver and all the requestors of the overdue approvals. This helps if the overdue approval entry must be delegated to a substitute.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Overdue Approval Requests**, and then choose the related link.
2. On the **Overdue Approval Requests** page, choose the **Send Overdue Approval Notifications** action.

## <a name="see-related-training-at-microsoft-learn"></a>See related training at [Microsoft Learn](/learn/modules/use-approval-workflows/)

## <a name="see-also"></a>See also 

[Set Up Approval Users](across-how-to-set-up-approval-users.md)  
[Sales](sales-manage-sales.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]