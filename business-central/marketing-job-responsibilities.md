---
title: Setting Up Job Responsibilities for Contacts| Microsoft Docs
description: You can define a job responsibility code and assign it to a contact to indicate the tasks that your contact is responsible for in their company, for example, IT or production.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, to-do, relationship, prospect
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: b531cfcb024444e098363725a4e0098d4651396b
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-job-responsibilities-for-contact-persons"></a>Set Up Job Responsibilities for Contact Persons
You can add information about the job responsibilities of contact persons to indicate what the contact person is responsible for within their company, for example, IT, management, or production. You can use this information when entering information about your contacts.

Using job responsibilities on contacts is a two-step process. First, you define the job responsibility code. You only have to perform this step one time for each job responsibility. Once you have a job responsibility code, you can start to assign the code to contact persons.

## <a name="to-define-a-job-responsibility-code"></a>To define a job responsibility code
The job responsibility code defines the type or category of the job, such a MARKETING or PURCHASE. You can have several job responsibility codes. To define the job responsibility, you use the **Job Responsibilities** window.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Responsibilities**, and then choose the related link.
2. Choose the **New** action, and fill in a code and description. The code can be a maximum of 11 characters, and can be any combination of numbers and letters.

## <a name="to-assign-job-responsibilities-to-a-contact-person"></a>To assign job responsibilities to a contact person
You cannot assign job responsibilities to contact companies.

1. Open the contact person.
2. Choose the **Person** action, and then choose the **Job Responsibilities** action. The **Contact Job Responsibilities** window opens.
3. In the **Job Responsibility Code** field, select the job responsibility that you want to assign.

Repeat these steps to assign as many job responsibilities as you want. You can also assign job responsibilities from the contact list by following the same procedure.

The number of job responsibilities you have assigned to the contact is displayed in the **No. of Job Responsibilities** field in the **Segmentation** section in the **Contact** window.

After you have assigned job responsibilities to your contacts, you can use this information to select contacts for your segments. For more information, see [Add Contacts to Segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>See Also
[Creating Contact Persons](marketing-create-contact-persons.md)  
[Creating Contact Companies](marketing-create-contact-companies.md)  
[Working with Business Central](ui-work-product.md)

