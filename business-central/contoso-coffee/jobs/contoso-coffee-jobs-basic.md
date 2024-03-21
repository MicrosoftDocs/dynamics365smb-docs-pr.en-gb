---
title: Walkthrough of Basic Jobs
description: This article guides you through several core processes in project management.
author: andreipanko
ms.author: andreipa
ms.topic: how-to
ms.date: 05/31/2023
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# <a name="walkthrough-of-basic-jobs"></a>Walkthrough of Basic Jobs

This walkthrough demonstrates several core processes:

- Adding job tasks to jobs
- Recording time and material expenses to a job
- Invoicing a job

## <a name="adding-a-job-task-to-a-job"></a>Adding a Job Task to a Job

### <a name="scenario"></a>Scenario

Simon, the project manager, wants to be record time spend educating the customer in espresso machine product use to a separate task in the job for installing a commercial machine on-site.

### <a name="steps"></a>Steps

1. Create the Job Task  

    1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.  
    2. Select the Job *J00010*.
    3. In the **Tasks** area, choose the **New Line** action.  Enter the following values:
 
    |Job Task No.|Description|Job Task Type|
    |------------|-----------|-------------|  
    |220|Customer Training|Posting|

2. Indent the Job Tasks
   1. In the Tasks area, locate the **Indent Job Tasks** action
   2. Confirm you wish to indent tasks by selecting **Yes**.

### <a name="results"></a>Results

 - Now time and expenses can be recorded to the new job task

## <a name="record-time-and-material-expenses-to-a-job"></a>Record Time and Material Expenses to a Job

### <a name="scenario-1"></a>Scenario

Edgin, the technician installing the machine, needs to record his time and the materials used during installation to the job for billing.  He has already added the travel and materials, and now needs to add the time for teaching staff how to use the machine.

### <a name="steps-1"></a>Steps

1. Create the additional Job Journal Lines

    1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.  
    2. Select the batch *CONTOSO*.  You will see several lines of Resource and Item types, reflecting the time (for the technician and the vehicle) and materials (the machine and supplies) used.
    3. Create a new line. Enter the following values:
 
    |Job No.|Job Task No.|Type|No.|Description|Quantity|
    |-------|------------|----|---|-----------|--------|  
    |J00010|220|Resource|EDGIN|Customer training|1|

2. Post the time and expense
   1. Choose the **Post** action
   2. Confirm you wish to post the lines by selecting **Yes**.

### <a name="results-1"></a>Results

 - Job Ledger Entries and Resource Ledger Entries of type *Usage* will be created
 - Item Ledger Entries will be created to negatively adjust the inventory
 - On the Job Card, the Costs and Prices in the Tasks area will reflect the new balances waiting to be invoiced
 - On the Job Card, the Job Details FactBox will reflect the totals of the prices

## <a name="creating-a-sales-invoice-for-a-job"></a>Creating a Sales Invoice for a Job

### <a name="scenario-2"></a>Scenario
Simon needs to create and post an invoice to be sent to the customer with the time and expenses from the job.

### <a name="steps-2"></a>Steps
1. Create the Sales Invoice

    1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.  
    2. In the list of Jobs, choose the **Create Job Sales Invoice** action.
    3. Set the **Job No.** filter to *J00010*.
    4. Choose **OK** to generate the Sales Invoice.  You will receive a confirmation of how many invoices are generated

2. Post the time and expense invoice
   1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.  
   2. Select the last invoice to open it for review.
   3. Choose the **Post** action.

### <a name="results-2"></a>Results

 - Job Ledger Entries and Resource Ledger Entries of type *Sales* will be created
 - On the Job Card, the Costs and Prices in the Tasks area will reflect the new Invoiced balances
 - On the Job Card, the Job Details FactBox will reflect the totals of the prices in the Invoiced Price section
