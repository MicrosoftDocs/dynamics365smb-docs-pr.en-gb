---
title: Set Up Organisational Levels for Contact Persons| Microsoft Docs
description: You can define an organisational level and assign it to your contact to indicate the position they have in their company, for example, top management.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, client, prospect
ms.date: 04/01/2019
ms.author: jswymer
redirect_url: marketing-setup-contacts
ms.openlocfilehash: 68f20af84652f684eaa0d69c98e0dc3cb722ee91
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "931345"
---
# <a name="set-up-organizational-levels-for-contact-persons"></a>Set Up Organisational Levels for Contact Persons
You can use organisational levels on your contacts to specify which position they have in the company, for example, top management. You can use this information when entering information about your contacts.

Using organisational levels on contacts is a two-step process. First, you define the organisational level code. You only have to perform this step one time for each organisational level. Once you have an organisational level code, you can start to assign the code to contact persons.

## <a name="to-define-an-organizational-level-code"></a>To define an organisational level code
The organisational level code defines the type or category of the organisational level, such a CEO  or CFO. You can have several organisational level codes. To define the organisational level, you use the **Organisational Levels** page.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Organisational Levels**, and then choose the related link.
2. Choose the **New** action, and fill in a code and description. The code can be a maximum of 11 characters, and can be any combination of numbers and letters.

## <a name="to-assign-organizational-levels-to-a-contact-person"></a>To assign organisational levels to a contact person
You can assign organisational levels to contact persons only, not contact companies. You can only assign one organisational level to each contact.

1. Open the contact.
2. In the **Organisational Levels** field, select the code you want to assign.

After you have assigned organisational levels to your contacts, you can use this information to create segments.

After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments. For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>See Also
[Creating Contacts](marketing-create-contact-companies.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
