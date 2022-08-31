---
title: Synchronisation and Data Integration | Microsoft Docs
description: The synchronisation copies data between Microsoft Dataverse tables and Business Central records, and keeps the data in both systems up-to-date.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Dataverse, integration, sync, synchronize, mapping
ms.date: 06/14/2021
ms.author: bholtorf
ms.openlocfilehash: 7c03e4491519a31aeaf11c4d52555ab222701c32
ms.sourcegitcommit: 5a02f8527faecdffcc54f9c5c70cefe8c4b3b3f4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/04/2022
ms.locfileid: "8383092"
---
# <a name="synchronizing-data-in-business-central-with-microsoft-dataverse"></a>Synchronising Data in Business Central with Microsoft Dataverse


When you integrate [!INCLUDE[prod_short](includes/cds_long_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)], you can decide whether to synchronise data in selected fields of [!INCLUDE[prod_short](includes/prod_short.md)] (such as customers, contacts, and sales people) with equivalent rows in [!INCLUDE[prod_short](includes/cds_long_md.md)] (such as accounts, contacts, and users). Depending on the type of row, you can synchronise data from [!INCLUDE[prod_short](includes/cds_long_md.md)] to [!INCLUDE[prod_short](includes/prod_short.md)], or vice versa. For more information, see [Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Synchronisation uses the following elements:

* Integration table mappings
* Integration field mappings
* Synchronisation rules
* Coupled records

When synchronisation is set up you can couple [!INCLUDE[prod_short](includes/prod_short.md)] records to [!INCLUDE[prod_short](includes/cds_long_md.md)] rows to synchronise their data. You can start a synchronisation manually, or based on a schedule. The following table provides an overview of the ways you can synchronise.  

|  Type  |  Method  |  See  |  
|--------|----------|-------|  
|Manual synchronisation|Synchronise on a row-by-row basis.<br /><br /> You can synchronise individual records in [!INCLUDE[prod_short](includes/prod_short.md)], such as a customer, with a corresponding [!INCLUDE[prod_short](includes/cds_long_md.md)] row, such as an account. This is typically how users will work with [!INCLUDE[prod_short](includes/cds_long_md.md)] data in [!INCLUDE[prod_short](includes/prod_short.md)].|[Couple and Synchronise Records Manually](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Synchronise on a table mapping basis.<br /><br /> You can synchronise all records in a [!INCLUDE[prod_short](includes/prod_short.md)] table with an table [!INCLUDE[prod_short](includes/cds_long_md.md)] table.|[Synchronise Individual Table Mappings](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Synchronise all modified records for all table mappings.<br /><br /> You can synchronise all of the records that have been modified in [!INCLUDE[prod_short](includes/prod_short.md)] tables since the last synchronisation.|[Synchronising All Modified Records](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Full synchronisation of all data for all table mappings.<br /><br /> You can synchronise all of the data in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] tables that are mapped, and create new records or rows in the destination solution for uncoupled records in the source solution.<br /><br /> Full synchronisation synchronises all data and ignores coupling. Typically, you do a full synchronisation when you set up the integration and only one of solutions contains data. A full synchronisation can also be useful in a demonstration environment.|[Run a Full Synchronisation](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Scheduled synchronisation|Synchronise all changes to data for all table mappings.<br /><br /> You can synchronise [!INCLUDE[prod_short](includes/prod_short.md)] with [!INCLUDE[prod_short](includes/cds_long_md.md)] on scheduled intervals by setting up jobs in the job queue.|[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

> [!NOTE]
> The synchronisation between [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)] is based on the scheduled execution of job queue entries and does not guarantee real time data consistency between two services. For real time data conistency you should explore [Business Central Virtual Tables](/dynamics365/business-central/dev-itpro/powerplatform/powerplat-overview) or Business Central APIs.   


## <a name="standard-table-mapping-for-synchronization"></a>Standard Table Mapping for Synchronisation
Tables in [!INCLUDE[prod_short](includes/cds_long_md.md)], such as accounts, are integrated with equivalent types of tables in [!INCLUDE[prod_short](includes/prod_short.md)], such as customers. To work with [!INCLUDE[prod_short](includes/cds_long_md.md)] data you set up links, called couplings, between tables in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)].

The following table lists the standard mapping between tables in [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)].

> [!TIP]
> You can reset configuration changes made to integration table and field mappings to their default settings by selecting the mappings, then choosing **Use Default synchronisation Setup**.

| [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] | Synchronisation Direction | Default Filter |
|---------------------------------------------|----------------------------------------------|---------------------------|----------------|
| Salesperson/Purchaser | User | [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] contact filter: **Status** is **No**, **User Licensed** is **Yes**, Integration user mode is **No** |
| Customer | Account | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] account filter: **Relationship Type** is **Customer** and **Status** is **Active**. [!INCLUDE[prod_short](includes/prod_short.md)] filter: **Blocked** is blank (Customer is not blocked). |
| Vendor | Account | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] account filter: **Relationship Type** is **Vendor** and **Status** is **Active**. [!INCLUDE[prod_short](includes/prod_short.md)] filter: **Blocked** is blank (Vendor is not blocked). |
| Contact | Contact | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/prod_short.md)] contact filter: **Type** is **Person** and the contact is assigned to a company. [!INCLUDE[prod_short](includes/cds_long_md.md)] contact filter: The contact is assigned to a company and the parent customer type is **Customer**. |
| Currency | Transaction Currency | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] |  |

> [!NOTE]
> The **Dataverse** actions will not be available on pages, for example, the Customer Card page, for records that do not respect the table filter on the integration table mapping.

### <a name="tip-for-admins-viewing-table-mappings"></a>Tip for Admins: Viewing Table Mappings
You can view the mapping between the tables in [!INCLUDE[prod_short](includes/cds_long_md.md)] and [!INCLUDE[prod_short](includes/prod_short.md)] on the **Integration Table Mappings** page, where you can also apply filters. You define the mapping between the fields in [!INCLUDE[prod_short](includes/prod_short.md)] tables and the columns in [!INCLUDE[prod_short](includes/cds_long_md.md)] tables on the **Integration Field Mapping** page, where you can add additional mapping logic. For example, this can be useful if you need to troubleshoot synchronisation.

## <a name="see-also"></a>See Also  
[Couple and Synchronise Records Manually](admin-how-to-couple-and-synchronize-records-manually.md)   
[Schedule a Synchronisation](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Integrating with Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
