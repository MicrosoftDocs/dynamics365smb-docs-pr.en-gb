---
title: How to Create a New Company | Microsoft Docs
description: To use RapidStart Services tables and pages are created, but there is no data in them.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7583837e515a4fd5fb415fe1b482512e7edf6b5a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4754012"
---
# <a name="create-a-new-company"></a>Create a New Company
To use RapidStart Services for [!INCLUDE[prod_short](includes/prod_short.md)], you first create a new company for which you want to perform a customer implementation. When you create a new company, the standard [!INCLUDE[prod_short](includes/prod_short.md)] tables and pages are created, but there is no data in them.

In addition, you can apply specific setup data to your company after you initialise it. The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.  

Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company. Use the following procedures to use the example configuration package with a new company.  

## <a name="to-use-the-sample-basicconfig-configuration-package"></a>To use the sample BASICCONFIG configuration package  
1. Open the CRONUS International Ltd. company. For more information, see [Change Basic Settings](ui-change-basic-settings.md).
2. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.  
3. Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.  

Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.  

## <a name="to-create-a-new-company"></a>To create a new company  
1. Create a new company. For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).
2. From the RapidStart Services Implementer Role Centre, you can now import the configuration package that you exported from the CRONUS International Ltd. company.

After you create a new company, some tables are automatically filled in, even if no company template is applied. For example, you can review the standard codes for posting and batch transactions on the **Source Code** page. If you provide a local version of [!INCLUDE[prod_short](includes/prod_short.md)], you should review this table and consider any local language issues.

## <a name="about-data-tables"></a>About Data Tables
[!INCLUDE[prod_short](includes/prod_short.md)], data tables come in two basic types: Master and Setup. When you are setting up a company configuration, you can use these types to focus your configuration strategy.  

### <a name="master-data-tables"></a>Master Data Tables  
The following table lists some of the master data tables. When you initialise a new company, these tables are empty.  

|Table No.|Table Name|  
|-------------------|--------------------|  
|15|G/L Account|  
|18|Customer|  
|23|Vendor|  
|27|Item|  
|5050|Contact|  

### <a name="setup-data-tables"></a>Setup Data Tables  
The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire. These tables contain baseline information when the company is created.  

|Table No.|Table Name|  
|-------------------|--------------------|  
|98|General Ledger Setup|  
|311|Sales & Receivables Setup|  
|312|Purchases & Payables Setup|  
|313|Inventory Setup|  

In addition to setup data tables, [!INCLUDE[prod_short](includes/prod_short.md)] also has setup-type data tables that specify core information about the company and its business processes. The following table lists some of them.  

|Table No.|Table Name|  
|-------------------|--------------------|  
|3|Payment Terms|  
|4|Currency|  
|6|Customer Price Groups|  
|5700|Stockkeeping Unit|

  

## <a name="see-also"></a>See Also  
[Apply Configurations to New Companies](admin-apply-configuration-to-new-companies.md)  
[Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Administration](admin-setup-and-administration.md)
