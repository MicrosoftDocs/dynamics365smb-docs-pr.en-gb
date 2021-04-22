---
title: Coupling and Synchronising| Microsoft Docs
description: Synchronising an integration table mapping enables data syncing in all records in a table in Business Central and Dynamics 365 Sales table that are coupled.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 53b12b6ab7e53a20bb1b8fcc659b2f1454e85321
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779939"
---
# <a name="coupling-and-synchronizing"></a>Coupling and Synchronising
This topic describes how to couple one or more records in [!INCLUDE[prod_short](includes/prod_short.md)] with records in Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)]. Coupling records lets you view Dataverse information from [!INCLUDE[prod_short](includes/prod_short.md)], and vice versa. The coupling also enables you to synchronise data between the records. You can couple existing records, or create and couple new records.

> [!Note]
> Coupling and synchronising data is available only if your system administrator has created a connection between [!INCLUDE[prod_short](includes/prod_short.md)] and Dataverse or [!INCLUDE[crm_md](includes/crm_md.md)]. A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action. If the action is available, the apps are connected.   

## <a name="video-example"></a>Video Example

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a>To couple a record  
1.  In [!INCLUDE[prod_short](includes/prod_short.md)], open the card for the record you want to couple. For example, the Customer or Contact card.  

    You can also just open the list page and select the record that you want to couple.  

2.  Choose the **Set Up Coupling** action.  
3.  Fill in the fields, and then choose **OK**.  

## <a name="to-synchronize-a-single-record"></a>To synchronise a single record  
1.  In [!INCLUDE[prod_short](includes/prod_short.md)], open the card for the record you want to couple. For example, the Customer or Contact card.  
2.  Choose the **Synchronise Now** action.  
3.  If a record can be synchronised in one direction, select the option that specifies the direction of data update, and then choose **OK**.  

## <a name="to-synchronize-a-single-record-from-crm_md"></a>To synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)]  
1.  In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple. For example, the Account card or Contact card form.  
2.  Choose the **[!INCLUDE[prod_short](includes/prod_short.md)]** action in the ribbon to open and couple record automatically.

> [!Note]
> You can synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronisation direction is set to Bidirectional or From Integration Table on the **Integration Table Mapping** page for the record. For more information, see [Mapping the Tables and Fields to Synchronise](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).     

## <a name="to-synchronize-multiple-records"></a>To synchronise multiple records  
1.  In [!INCLUDE[prod_short](includes/prod_short.md)], open the list page for the record, such as the Customers or Contacts list pages.  
2.  Select the records that you want to synchronise, and then choose the **Synchronise Now** action.  
3.  If records can be synchronised in one direction, select the option that specifies the direction, and then choose **OK**.  

## <a name="uncoupling-records"></a>Uncoupling Records
You can uncouple one or more records from list pages or the **Coupled Data Synchronisation Errors** page by choosing one or more lines and choosing **Delete Coupling**. You can also remove all couplings for one or more table mappings on the **Integration Table Mappings** page.

## <a name="see-also"></a>See Also  
[Using Dynamics 365 Sales from Business Central](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]