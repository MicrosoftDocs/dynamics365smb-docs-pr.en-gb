---
title: Manage Interactions With Your Contacts| Microsoft Docs
description: You can manage all types of communication or interactions between your company and your contacts, for example, letters, phone calls, meetings, and so on.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: d72025a95f6d12ab64ba6ec29de754bb9c318ab0
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6435804"
---
# <a name="record-interactions-with-contacts"></a>Record Interactions With Contacts
Setting up your application to record interactions consists of these tasks:

* Setting up interaction templates  
* Creating interactions on contacts or segments  
* View and manage recorded interactions  

##  <a name="setting-up-interaction-templates"></a>Setting up Interaction Templates
Before you can create and record interactions, you must set up interaction templates. When creating interactions, you must specify the interaction templates they are based on. An interaction template is a model that defines the basic characteristics of an interaction.
You set up an interaction template on the **Interaction Templates** page.

After you have entered information about the interaction template, you can create an attachment, for example, a Microsoft Word document. Repeat the steps to set up as many interaction templates as you want.  

## <a name="creating-interactions"></a>Creating Interactions
There are two ways of recording interactions:

* You can manually create interactions that are linked to a single contact or to a segment. For more information, see [Create Interactions on Contacts and Segments](marketing-how-create-interactions.md).  
* You can automatically record interactions when you perform actions in the application, for example, when you print an invoice, or quote. For more information, see [Automatically Record Interactions with Contacts](marketing-auto-record-interactions.md).

## <a name="viewing-and-managing-recorded-interactions"></a>Viewing and Managing Recorded Interactions
You can view all the recorded interactions that have not been deleted on the **Interaction Log Entries** page. You can open this page by:

* Using the **Search for Page or Report** icon to search on **Interaction Log Entries**.
* Choosing the **Interaction Log Entries** action on a contact or segment.
  The **Interaction Log Entry** page contains the interactions you create manually and the interactions that the application records automatically.

In this page, you can:

* View the status of interactions.
* Mark interactions as cancelled.

You can delete interaction log entries that have been cancelled. To delete interaction log entries, choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete cancelled Interaction Log Entries**, and then choose the related link, and then fill in the information.

## <a name="see-also"></a>See Also
[Managing Contacts](marketing-contacts.md)  
[Managing Sales Opportunities](marketing-manage-sales-opportunities.md)  
[Working with Business Central](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]