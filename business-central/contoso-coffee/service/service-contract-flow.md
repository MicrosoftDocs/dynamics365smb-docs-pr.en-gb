---
title: Walkthrough of Service Contracts for Service Items
description: This article guides you through various scenarios involving service items and contracts.
author: andreipanko
ms.author: andreipa
ms.topic: how-to
ms.date: 05/31/2023
ms.custom: bap-template
---

# <a name="walkthrough-of-service-contracts-for-service-items"></a>Walkthrough of Service Contracts for Service Items

This walkthrough demonstrates several core processes:

- Creation of Service Items through Sales
- Creating and Invoicing for a Service Contract
- Creating a Service Order for a Service Contract
- Assign a Resource based on Skill and Zone
- Complete the time entry for the Service Order
- Post and Invoice the Contract Service Order

## <a name="creation-of-service-items"></a>Creation of Service Items

### <a name="scenario"></a>Scenario

Susan, the order processor, posts a sales order selling an Item configured to generate a Service Item.  

### <a name="steps"></a>Steps

1. Check that **Item** has **Service Item Group** selected.
   
    1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.  
    2. Select the item *S-100* and open it.
    3. Check the value in the **Service Item Group** field.
       
2. Post the **Sales Order** to create the Service Item for the Customer.  

    1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.  
    2. Select the order for customer 10000. The External Orders No. is *SVC-1*.
    3. Choose the **Post** action to ship the item to the customer.

### <a name="results"></a>Results

- A Service Item will be created for Customer 10000

## <a name="invoicing-a-service-contract"></a>Invoicing a Service Contract

### <a name="scenario-1"></a>Scenario

Charles, the service manager, then creates a Service Contract to invoice for regular maintenance visits.

3. Create the **Service Contract** for the new Service Item
    1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contracts**, and then choose the related link.
    2. Choose the **New** action.  
    3. In the confirmation dialogue, choose **Yes** to create contract using template. 
    4. Select *Non-Prepaid Contract - Monthly*.
    5. On the Service FastTab, in the **Service Order Type**, enter **MAINTEN**.
    6. In the Lines, enter the following information:

    |Service Item No.|Line Value|  
    |----------------|----------|  
    |SV000001|6000|

    7. Choose the **Sign Contract** action and confirm the signing.
    8. Choose **Yes** to confirm creation of a Service Invoice. You'll receive a confirmation message with the Service Invoice number.

3. Post the Service Invoice
   1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Invoices**, and then choose the related link.
   2. Locate the Service Invoice and choose the **Post** action.

### <a name="results-1"></a>Results

- A Signed Service Contract will be created, with Ledger Entries
- A Posted Service Invoice will be created

## <a name="creating-a-service-order-for-a-service-contract-and-assign-resources"></a>Creating a Service Order for a Service Contract and Assign Resources

### <a name="scenario-2"></a>Scenario

Charles, the service manager, will create the Service Orders for regular maintenance orders under Service Contract, then review the Dispatch Board to assign them.

### <a name="steps-1"></a>Steps

1. Run the Service Orders that will fulfil the obligations of active Service Contracts.
   1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create Contract Service Orders**, and then choose the related link.
   2. Enter the beginning and ending dates of the month in the Starting Date and Ending Date fields in the Options FastTab
   3. Choose **OK** to confirm creation of Service Orders. You'll receive a confirmation message with number of created Service Orders.

2. Review the Orders awaiting assignment via the Dispatch Board
   1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Dispatch Board**, and then choose the related link.
   2. The Dispatch Board will show all open Service Orders, along with the **No. of Allocations** to show if the Service Orders have been assigned to a Resource.
   3. Choosing the **Show Documents** action to open a Service Order.  You will see that the Service Item Lines FactBox will show which Resources are skilled at working with this item.

3. Assign a Resource to the Service Order
   1. From the Service Order, choose the Line action **Resource Allocations**
   2. Enter the following information for the Resource Allocation

    |Service Item No.|Resource No.|Allocation Date|Allocated Hours|
    |----------------|------------|---------------|---------------|  
    |SV000001|RESOURCE1|t|1|

    3. The Allocation will be changed to a Status to Active.
    4. Refreshing the Dispatch Board will show the **No of Allocations** changed from 0 to 1 for the Service Order.

### <a name="results-2"></a>Results

- Service Orders will be created for the Service Contracts
- The Service Orders will be allocated to a resource to complete the work

## <a name="complete-the-time-entry-for-the-service-order-and-post-the-service-order"></a>Complete the time entry for the Service Order and Post the Service Order

### <a name="scenario-3"></a>Scenario

The service technician will register their time directly against the Service Order, then mark order as finished.

> [!NOTE]
> Time Entry for Service Orders can be entered via Time Sheets. For more information, see [link to Timesheet if this note makes sense].

### <a name="steps-2"></a>Steps

1. Locate the Service Order and enter the time into the Service Line
   1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Orders**, and then choose the related link.
   2. Locate the Service Order to enter time for.
   3. Choose the Line action **Service Line**.
   4. Enter the following information

    |Type|No.|Quantity|Qty.to Consume|
    |----|---|--------|--------|   
    |Resource|RESOURCE1|2|2|

2. On the Service Order, Post the consumption
   1. Choose the **Post** action to complete the Service Order, select the **Ship and Consume** action, and then choose the **OK** button.

### <a name="results-3"></a>Results

- Service Ledger Entries will be created associated with the Service Item, Service Contract, and Resource

## <a name="see-also"></a>See also
