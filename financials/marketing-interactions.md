---
title: Interactions | Microsoft Docs
description: Describes using interactions with contacts in Financials
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: a423f5581f6803b60a0351d0b91f2c08ebafeba7
ms.contentlocale: en-gb
ms.lasthandoff: 05/04/2017


---
# <a name="managing-interactions-with-contacts"></a>Managing Interactions With Contacts
In [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)], interactions are all types of communications between your company and your contacts. For example, communications can be by letter, fax, email, telephone, meetings, and so on.

The relationship management area enables you to record all the interactions you have with your contacts in order to keep track of the sales and marketing efforts you have directed at your contacts and to improve your future business interactions with them. Setting up your application to record interactions consists of these tasks:

* Setting up interaction templates  
* Creating interactions on contacts or segments  
* View and manage recorded interactions  

##  <a name="set-up-interaction-templates"></a>Set up Interaction Templates
Before you can create and record interactions, you must set up interaction templates. When creating interactions, you must specify the interaction templates they are based on. An interaction template is a model that defines the basic characteristics of an interaction.
You set up an interaction template in the **Interaction Templates** window.  

## <a name="create-interactions"></a>Create Interactions
There are two ways of recording interactions:

* You can manually create interactions that are linked to a single contact or to a segment. For more information, see [How to: Create Interactions on Contacts and Segments](marketing-how-create-interactions.md).  
* You can automatically record interactions when you perform actions in the application, for example, when you print an invoice, or quote. For more information, see [Automatically Record Interactions with Contacts](marketing-auto-record-interactions.md).

## <a name="view-and-manage-recorded-interactions"></a>View and manage recorded Interactions
You can view all the recorded interactions that have not been deleted in the **Interaction Log Entries** window. You can open this window by:

* Using the **Search for Page or Report** icon to search on **Interaction Log Entries**.
* Choosing the **Interaction Log Entries** action on a contact or segment.
  The **Interaction Log Entry** window contains the interactions you create manually and the interactions that the application records automatically.

In this window, you can:

* View the status of interactions.
* Mark interactions as cancelled.

You can delete interaction log entries that have been cancelled. To delete interaction log entries, in the top right corner, choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), enter **Delete Canceled Interaction Log Entries**, and then choose the related link, and then fill in the information.

## <a name="see-also"></a>See Also
[Managing Contacts](marketing-contacts.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Working With Financials](ui-work-product.md)  

