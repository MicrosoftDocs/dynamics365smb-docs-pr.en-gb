---
title: Share contacts between Business Central and Outlook| Microsoft Docs
description: This service has deep integration with Office 365 so you can share contacts between Outlook and Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: contacts, Office 365
ms.date: 10/01/2019
ms.author: edupont
ms.openlocfilehash: c28118ad9aa894678e4630800c638cf252c4f524
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2307773"
---
# <a name="synchronize-contacts-in-business-central-with-contacts-in-microsoft-outlook"></a>Synchronise Contacts in Business Central with Contacts in Microsoft Outlook
You can see the same contacts in [!INCLUDE[d365fin](includes/d365fin_md.md)] as you see in Outlook if you set up contact synchronisation. For example, if you are a sales person, you might do some of your work in Outlook and some of your work in [!INCLUDE[d365fin](includes/d365fin_md.md)]. If the contacts are the same in both places, your work is more straightforward.  

A dedicated folder in Outlook makes contacts easy to find, and you can set a filter to synchronise only the contacts from [!INCLUDE[d365fin](includes/d365fin_md.md)] that you want to see in Outlook. Once the contact synchronisation is set up, you can start synchronisation manually or set up an automatic synchronisation that will keep the contacts in sync on a scheduled basis.  

## <a name="set-up-synchronization"></a>Set Up Synchronisation
You set up how you want to synchronise contacts with Outlook on the **Exchange Sync. Setup** page in [!INCLUDE[d365fin](includes/d365fin_md.md)]. As a prerequisite, your user profile in [!INCLUDE[d365fin](includes/d365fin_md.md)] must specify your Office 365 email account. You can check this in the **Office 365 Authentication** section of your user profile in the **Users** list.  

Then, on the **Exchange Sync. Setup** page, you can validate that the connection to Exchange is working and then set up contact synchronisation. Open the **Contact Sync. Setup** page and start the synchronisation. Optionally, set a filter for which contacts to synchronise between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Outlook. For example, you can set a filter on name, type, company, or similar. You can also change the default name of the folder that the contacts will synchronise to in Outlook. The default name is *Business Central*.  

Once this synchronisation has been set up, any changes to that you make to the contact in either Outlook or in [!INCLUDE[d365fin](includes/d365fin_md.md)] is synchronised to the other.  

Each of your coworkers can also set up their own Exchange synchronisation and set their own filter on which contacts to synchronise.  

## <a name="synchronize-contacts"></a>Synchronise Contacts
If you are used to working with contacts in [!INCLUDE[d365fin](includes/d365fin_md.md)], then you will find it easy to start the synchronisation manually whenever it suits you from the **Contacts** list. Simply choose the **Sync with Office 365** action, and then decide if you want to change the filter that you have set up. When you choose the OK button, the synchronisation starts immediately, and the latest changes are applied to your contacts in Outlook.  

In the **Contacts** list, you can synchronise contacts in two ways:

* **Sync with Office 365**

  This action synchronises all changes from [!INCLUDE[d365fin](includes/d365fin_md.md)] to Office 365 since the previous synchronisation, based on the last modified date. Any new contacts from Office 365 will be synchronised back to [!INCLUDE[d365fin](includes/d365fin_md.md)] as well. This is typically faster than doing a full sync.  

* **Full Sync with Office 365**

  This action synchronises all contacts in both directions regardless of the last sync date and last modified date.  

In both cases, contacts are only synchronised from Outlook if they have the required fields filled in. The required fields to synchronise to Office 365 are **Name**, **Email address** and they must be of type Person. [!INCLUDE[d365fin](includes/d365fin_md.md)] is the master of the contact information, so the [!INCLUDE[d365fin](includes/d365fin_md.md)] contact information will be saved in the event of duplicates.  

In Outlook, the contacts from [!INCLUDE[d365fin](includes/d365fin_md.md)] are shown in a folder under **Other contacts** in the **People**  view. If you are not familiar with the People view in Outlook, then you can get to it from the navigation options in the bottom left corner of Outlook.  

## <a name="see-also"></a>See Also
[Getting Started](product-get-started.md)  
[Finance](finance.md)  
[Sales](sales-manage-sales.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Using contacts (People) in Outlook on the web](https://support.office.com/en-us/article/Using-contacts-People-in-Outlook-on-the-web-1e3438c7-26b2-420c-87de-3cea9d31b5cb?appver=OWB150)  
