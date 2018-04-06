---
title: Set Up Organisational Levels for Contact Persons| Microsoft Docs
description: You can define an organisational level and assign it to your contact to indicate the position they have in their company, for example, top management.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 974133ffb0324cf6bc3ed37436adb9fb237f5e4d
ms.contentlocale: en-gb
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-organizational-levels-for-contact-persons"></a>Set Up Organisational Levels for Contact Persons
You can use organisational levels on your contacts to specify which position they have in the company, for example, top management. You can use this information when entering information about your contacts.

Using organisational levels on contacts is a two-step process. First, you define the organisational level code. You only have to perform this step one time for each organisational level. Once you have an organisational level code, you can start to assign the code to contact persons.

## <a name="to-define-an-organizational-level-code"></a>To define an organisational level code
The organisational level code defines the type or category of the organisational level, such a CEO  or CFO. You can have several organisational level codes. To define the organisational level, you use the **Organisational Levels** window.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Organizational Levels**, and then choose the related link.
2. Choose the **New** action, and fill in a code and description. The code can be a maximum of 11 characters, and can be any combination of numbers and letters.

## <a name="to-assign-organizational-levels-to-a-contact-person"></a>To assign organisational levels to a contact person
You can assign organisational levels to contact persons only, not contact companies. You can only assign one organisational level to each contact.

1. Open the contact.
2. In the **Organisational Levels** field, select the code you want to assign.

After you have assigned organisational levels to your contacts, you can use this information to create segments.

After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments. For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>See Also
[Creating Contact Companies](marketing-create-contact-companies.md)  
[Creating Contact Persons](marketing-create-contact-persons.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

