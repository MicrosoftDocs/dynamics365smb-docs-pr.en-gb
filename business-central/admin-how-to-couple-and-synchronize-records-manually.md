---
title: Coupling and Synchronising (contains video)
description: Synchronising an integration table mapping enables data syncing in all records in a table in Business Central and Dynamics 365 Sales table that are coupled.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.topic: conceptual
ms.date: 03/31/2023
ms.custom: bap-template
ms.search.keywords: 'crm, sales, couple, decouple, synchronize'
ms.search.form: '6250,'
---

# <a name="couple-and-synchronize-records-between-dataverse-and-business-central"></a><a name="couple-and-synchronize-records-between-dataverse-and-business-central"></a><a name="couple-and-synchronize-records-between-dataverse-and-business-central"></a>Couple and Synchronise Records between Dataverse and Business Central

This topic describes how to couple one or more records in [!INCLUDE[prod_short](includes/prod_short.md)] with records in Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)]. Coupling records lets you view Dataverse information from [!INCLUDE[prod_short](includes/prod_short.md)], and vice versa. The coupling also enables you to synchronise data between the records. You can couple existing records, or create and couple new records.

> [!NOTE]
> Coupling and synchronising data is available only if your system administrator has created a connection between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)]. A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action. If the action is available, the apps are connected.

## <a name="video-example"></a><a name="video-example"></a><a name="video-example"></a>Video Example

This video shows coupling and synchronising data in the context of an integration with [!INCLUDE[crm_md](includes/crm_md.md)].

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a><a name="to-couple-a-record"></a><a name="to-couple-a-record"></a>To couple a record

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the card for the record you want to couple. For example, the Customer or Contact card.  

    You can also just open the list page and select the record that you want to couple.  

2. Choose the **Set Up Coupling** action.  
3. Fill in the fields, and then choose **OK**.  

## <a name="to-synchronize-a-single-record"></a><a name="to-synchronize-a-single-record"></a><a name="to-synchronize-a-single-record"></a>To synchronise a single record

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the card for the record you want to couple. For example, the Customer or Contact card.  
2. Choose the **Synchronise Now** action.  
3. If a record can be synchronised in one direction, select the option that specifies the direction of data update, and then choose **OK**.  

## <a name="to-synchronize-a-single-record-from-"></a><a name="to-synchronize-a-single-record-from-"></a><a name="to-synchronize-a-single-record-from-"></a>To synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)]

1. In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple. For example, the Account card or Contact card form.  
2. Choose the **[!INCLUDE[prod_short](includes/prod_short.md)]** action in the ribbon to open and couple record automatically.

    > [!Note]
    > You can synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronisation direction is set to **Bidirectional** or **From Integration Table** on the **Integration Table Mapping** page for the record. For more information, see [Mapping the Tables and Fields to Synchronise](admin-how-to-modify-table-mappings-for-synchronization.md#create-new-records).

## <a name="to-couple-multiple-records-using-match-based-coupling"></a><a name="to-couple-multiple-records-using-match-based-coupling"></a><a name="to-couple-multiple-records-using-match-based-coupling"></a>To couple multiple records using match-based coupling

Specify the data to synchronise for an entity, such as a customer or contact, by coupling records based on matches. Refine the matches by making the search case sensitive, and assigning a priority for each match. If no match is found, you can also specify that you want to create the entity in Dataverse. For more information, go to [Customise the match-based coupling](admin-how-to-set-up-a-dynamics-crm-connection.md#customize-the-match-based-coupling).  

> [!NOTE]
> The match-based coupling process skips records that are already matched. To include those records when you run match-based coupling, uncouple the records and then try again. To learn more about uncoupling records, go to [Uncoupling Records](#uncoupling-records).

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the list page for the record, such as the Customers or Contacts list pages.
2. Choose the **Match-Based Coupling** action.
3. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-synchronize-multiple-records"></a><a name="to-synchronize-multiple-records"></a><a name="to-synchronize-multiple-records"></a>To synchronise multiple records

1. In [!INCLUDE[prod_short](includes/prod_short.md)], open the list page for the record, such as the Customers or Contacts pages.  
2. Select the records that you want to synchronise, and then choose the **Synchronise Now** action.  
3. If records can be synchronised in one direction, select the option that specifies the direction, and then choose **OK**.  

## <a name="bulk-insert-and-couple-records"></a><a name="bulk-insert-and-couple-records"></a><a name="bulk-insert-and-couple-records"></a>Bulk-insert and couple records

If you have a large number of Dataverse entities that correspond to records in [!INCLUDE [prod_short](includes/prod_short.md)], you can insert and couple them in-bulk. For example, you might want to bulk-insert and couple records when you're setting up synchronisation for the first time.

You'll use the **Data import wizard** in the **Microsoft Power Platform admin centre**.

The following example describes how to bulk-insert and couple customers with accounts in Dataverse. Use the same process for other types of entities, such as vendors, items, and resources.

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.
2. Choose the **Open in Excel** action to open customer data in Excel. <!--Don't they need to choose the customers that they want to import to Dataverse?-->
3. To map and import data to the **Account** entity in Dataverse, follow the steps described in [Import data (all record types) from multiple sources](/power-platform/admin/import-data-all-record-types).  

    If the Account entity has a **bcbi_companyid** column, when you map the data columns make sure that the import assigns the appropriate company ID in the column for every imported record. To find the company ID in [!INCLUDE [prod_short](includes/prod_short.md)], follow these steps:

    1. Open the **Integration Table Mappings** page.
    2. Choose the **CUSTOMER** mapping, and then choose **Edit List**.
    3. Scroll to the right, and choose the assist edit :::image type="icon" source="media/assist-edit-icon.png" border="false"::: button in the **Integration Table Filter** field. This shows the default filter for customer mapping, and it contains the company ID. The company ID is the first part of the value. Copy only that part, and disregard the 0s. The following example highlights the part to copy.

    :::image type="content" source="media/dataverse-company-id-guid.png" alt-text="Shows the part of the company ID to copy.":::

    > [!NOTE]
    > Not all of the names of Dataverse entities and Business Central records match. Depending on what you're importing, double-check that the following columns have the following values after you import:
    >
    >* For customers, the **CustomerTypeCode** column should contain **Customer**.
    >* For vendors, the **CustomerTypeCode** column should contain **Vendors**. 
    >* For items, **ProductTypeCode** column should contain **Sales Inventory**.
    >* For resources, the **ProductTypeCode** column should contain **Service**.
 
4. After you import data to the Dataverse environment, in [!INCLUDE [prod_short](includes/prod_short.md)], follow the steps [To couple multiple records using match-based coupling](#to-couple-multiple-records-using-match-based-coupling) to couple the Dataverse entities with [!INCLUDE [prod_short](includes/prod_short.md)] records. 

## <a name="uncoupling-records"></a><a name="uncoupling-records"></a><a name="uncoupling-records"></a>Uncoupling Records

You can uncouple one or more records from list pages or the **Coupled Data Synchronisation Errors** page by choosing one or more lines and choosing **Delete Coupling**. You can also remove all couplings for one or more table mappings on the **Integration Table Mappings** page.

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>See Also

[Use Dynamics 365 Sales from Business Central](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
