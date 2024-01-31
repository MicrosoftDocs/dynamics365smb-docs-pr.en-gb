---
title: Setting Up Cost Accounting
description: 'Before you start working with cost accounting, you must setup. Each cost entry must have a cost type assigned and a cost centre code or a cost object assigned.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.form: '1100, 1112, 1113, 1122'
ms.date: 10/09/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Setting Up Cost Accounting

Before you start working with cost accounting, you must perform setup tasks.

## Balances Between Cost Type, Cost Centre, and Cost Object

When you set up cost accounting, you must make sure that all entries are assigned to a cost type as well as a cost centre or a cost object. The means that each cost entry must have a cost type assigned and a cost centre code or a cost object assigned. This rule ensures that each cost entry appears in either the cost centres or the cost objects, but never in both places.  

By doing this, you create the following accounting equation:  

*Cost Type Balance* = *Cost Centre Balance* + *Cost Object Balance*  

When you print the chart of cost type, the chart of cost centres, and the chart of cost objects reports, you can analyse this relationship.

## Setting Up Cost Types

The chart of cost types is similar to the chart of accounts in the general ledger. You can set up the chart of cost types in the following ways:  

- Structure the chart of cost types similar to the income statement accounts in the general ledger chart of accounts. Then, you can transfer the general ledger chart of accounts to the chart of cost types. You can make any necessary adjustments after the transfer.  
- Create new chart of cost types or add new cost types to existing chart of cost types. You must create each new cost type individually.  

### To transfer the general ledger chart of accounts to the chart of cost types

1. Choose the ![Lightbulb that opens the Tell Me feature 1.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Types**, and then choose the related link.  
2. Choose the **Get Cost Types from Chart of Accounts** action. In the dialogue box, choose the **Yes** button to confirm the transfer. The function uses the chart of accounts to create a chart of cost types.  

    The chart of cost types now contain all income statement accounts in the general ledger and include headings and subtotals. You can change the chart of cost types, as necessary. For example, you can delete duplicate existing cost types.  

    > [!IMPORTANT]  
    >  The **Register Cost Types in Chart of Accounts** function updates the relationship between the chart of accounts and the chart of cost types. The **No.** field is filled and verified to make sure that each general ledger account is related to only one cost type. The function runs automatically before transferring general ledger entries to cost accounting.  

### To set up new cost types in the Chart of Cost Types page

1. Open the **Chart of Cost Types** page in edit mode.  
2. Fill in the fields as described as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    >  You can set up and maintain cost types in either the **Cost Type Card** page or on the **Chart of Cost Types** page. In this procedure, you set up cost types on the **Chart of Cost Types** page.

3. After you have created all cost types, choose the **Indent Cost Types** action. In the dialogue box, choose the **Yes** button.  
4. Link the new cost type to the corresponding general ledger account.  

    > [!IMPORTANT]  
    >  If you have entered definitions in the **Totalling** fields for the line type of **End-Total** before you run the **Indent Cost Types** function, then you must enter the definitions again because the function overwrites the values in all **End-Total** fields.  

### To update cost types

1. On the **Cost Accounting Setup** page, select if you want the chart of cost types to be automatically updated when the chart of accounts is changed.  
2. In the **Align G/L Account** field, you can choose from the following options.  

- **No Alignment** - There is no corresponding change in the chart of cost types when you change the chart of accounts.  
- **Automatic** - A corresponding change is made in the chart of cost types when you change the chart of accounts.  
- **Prompt** - A message is displayed asking if you want to make a corresponding change in the chart of cost types when you change the chart of accounts.

## Defining the Relationship Between Cost Types and General Ledger Accounts

The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.  

- The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.  
- The **Cost Type No.** field in the chart of accounts establishes which cost type a general ledger account belongs to.  

These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.  

### Relationship Between General Ledger Accounts and Cost Types

There is an n:1 relationship between general ledger accounts and cost types. Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type. The following table describes the details in the relationship.  

|Relationship|**G/L Account Range**|**Cost Type No.**|  
|------------------|------------------------------------------------|-------------------------------------------|  
|One general ledger account for each cost type|One general ledger account|One cost type|  
|Several general ledger accounts for one cost type|General ledger account range, for example, 7110..7193 for each general ledger account|For each general ledger account in the range, there is only one cost type|  
|Cost types without corresponding general ledger accounts|\<Empty\>||  
|General ledger accounts whose entries will not be transferred||\<Empty\>|  

### Cost Types Without a Relationship to the General Ledger

A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:  

- Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.  
- Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[prod_short](includes/prod_short.md)] database, are used as credit and debit accounts for allocations.  
- The helping account, 9920 in the [!INCLUDE[prod_short](includes/prod_short.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.

## Setting Up Cost Centres

Cost centres are departments that are responsible for costs and income. The chart of cost centres is similar to the dimension information for the general ledger. You can set up the chart of cost centres in the following ways:  

- Transfer dimension values in the general ledger to the chart of cost centres. You can make any necessary adjustments after the transfer.  
- Create a new chart of cost centre that is independent of the general ledger or add a new cost centre to an existing chart of cost centre. You must create each cost centre individually.  

### To transfer dimension values in the general ledger to the chart of cost centres

1. Set up a dimension to be the cost centre dimension on the **Cost Accounting Setup** page. Only the values from this dimension are transferred.
You can choose **Actions** > **Functions** > **Update Cost Acctg. Dimensions** action to update cost accounting dimensions.
1. Choose the ![Lightbulb that opens the Tell Me feature 2.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centres**, and then choose the related link.  
1. On the **Actions** tab, in the **Functions** group, choose **Get Cost Centres from Dimension** to transfer dimension values to the chart of cost centres. The function transfers the dimension values that you defined in step 1.  

    > [!NOTE]  
    >  You can set up the **Align Cost Centre Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost centres. You cannot define a synchronisation of the chart of cost centres to dimension values from the general ledger.  

The chart of cost centres now contains all specified dimension values from the general ledger and includes titles and subtotals.  

### To create new cost centres in the Chart of Cost Centres page

You can set up and maintain cost centres in either the **Cost Centre Card** card or on the **Chart of Cost Centres** page. In this procedure, you set up cost centres on the **Chart of Cost Centres** page.  

1. Open the **Chart of Cost Centres** page in edit mode.  
2. In the **Code** field, enter the cost center code. All cost centres must have a code.  
3. In the **Name** field, enter the cost center name.  
4. Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost centre.  

    - For cost centres of the **Total** type, you must fill in the **Totalling** field. Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centres.  
    - For cost centres of the **End-Total** line type, this field is filled in automatically when you use the indent function.  
5. Fill in the **Sorting Order** and **Cost Subtype** fields.  
6. Choose the next empty line to create a new cost centre, and then repeat steps 2 through 5.  
7. After you have set up all the cost centres, choose the **Indent Cost Centres** action. Choose the **Yes** button.  

> [!IMPORTANT]  
> If you have entered definitions in the **Totalling** fields for **End-Total** cost centres before you run the indent function, then you must enter them again. The function overwrites the values in all **End-Total** fields.

## Setting Up Cost Objects

Cost objects are projects, products, or services of a company. The chart of cost objects is similar to the dimension information for the general ledger. You can set up the chart of cost objects in the following ways:  

* Transfer dimension values in the general ledger to the chart of cost objects. You can make any necessary adjustments after the transfer.  
* Create a new chart of cost object that is independent of the general ledger or add a new cost object to an existing chart of cost objects. You must create each cost object individually.  

### To transfer dimension values from the general ledger to the chart of cost objects

1.  Set a dimension to be the cost object dimension on the **Update CA Dimensions** page. Only the values from this dimension are transferred.  
2.  Choose the ![Lightbulb that opens the Tell Me feature 3.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Objects**, and then choose the related link.  
3.  Choose the **Get Cost Objects from Dimension** action to transfer dimension values to the chart of cost objects. The function transfers the dimension values that you defined in step 1.  

    > [!NOTE]  
    >  You can set up the **Align Cost Object Dimension**  field to define a one-way synchronisation of dimension values from the general ledger to the chart of cost objects. You cannot define a synchronisation of the chart of cost objects to dimension values from the general ledger.  

The chart of cost objects now contains all specified dimension values from the general ledger and includes titles and subtotals.  

### To create new cost objects in the Chart of Cost Objects page

You can set up and maintain cost objects in either the **Cost Object Card** card or on the **Chart of Cost Objects** page. In this procedure, you set up cost objects on the **Chart of Cost Objects** page.  

1.  Open the **Chart of Cost Objects** page in edit mode.  
2.  In the **Code** field, enter the cost object code. All cost objects must have a code.  
3.  In the **Name** field, enter the cost object name.  
4.  Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost object.  

    * For cost objects of the **Total** line type, fill in the **Total From/To** field. Use the **or** operator, which is a vertical line (**&#124;**), to set ranges of cost objects.  
    * For cost objects of the **End-Total** line type, this field is filled in automatically when you use  the indent function.  
5.  Fill in the **Sorting Order** field.  
6.  Chose the next empty line to create a new cost object, and then repeat steps 2 through 5.  
7.  After you have set up all the cost objects, choose the **Indent Cost Objects** action. Choose the **Yes** button.  

> [!IMPORTANT]  
>  If you have entered definitions in the **Total From/To** fields for **End-Total** cost objects before you run the indent function, then you must enter them again. The function overwrites the values in all **End-Total** fields.

## Defining Cost Centres and Cost Objects for Chart of Accounts

You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job. When you do the transfer, [!INCLUDE[prod_short](includes/prod_short.md)] only transfers the entries that are already linked to a cost center or a cost object. To establish a meaningful transfer, you must ensure that the cost centres and cost objects are correctly defined.  

### Defining Default Dimension Values for General Ledger Accounts

For each general ledger account, you can define default dimension values in the **Default Dimension** table. The following example shows how to define that there should always be a DEPARTMENT cost centre, but never be a PROJECT cost object when posting to a general ledger account.  

|**Dimension Code**|**Value Posting**|  
|------------------------------------------|-----------------------------------------|  
|Department|Code Mandatory|  
|Project|No Code|  

### Defining Dimension Values for Overhead Costs and Direct Costs

 You can transfer overhead costs to a cost centre and direct costs to a cost object. The following table shows the optimal combination of the dimension setup values.  

|Transfer To|Cost Centre Posting|Cost Object Posting|  
|-----------------|-------------------------|-------------------------|  
|Cost Centre|Code Mandatory|No Code|  
|Cost Object|No Code|Code Mandatory|  

> [!NOTE]  
>  To make sure that the predefined cost centre and cost object that you set up in the general ledger are automatically carried over to cost accounting, select the **Check G/L Postings** check box in the Cost Accounting Setup page.

## See also 

[Accounting for Costs](finance-manage-cost-accounting.md)  
[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md)  
[Defining and Allocating Costs](finance-define-and-allocate-costs.md)  
[Work with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
