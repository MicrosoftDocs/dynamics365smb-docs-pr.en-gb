---
title: OneDrive for Business FAQ
description: Get answers for some typical questions about working with OneDrive for Business and Business Central.
author: brentholtorf
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OneDrive, integration, share, browser
ms.date: 05/19/2021
ms.author: bholtorf
ms.openlocfilehash: 2ab3005c7958e6ce7cd112c495ba6bb1d0ae2366
ms.sourcegitcommit: 5a02f8527faecdffcc54f9c5c70cefe8c4b3b3f4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/04/2022
ms.locfileid: "8381974"
---
# <a name="onedrive-for-business-faq"></a>OneDrive for Business FAQ

[!INCLUDE [online_only](includes/online_only.md)]

This article answers some of the questions you may have about working with OneDrive and [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="does-this-work-with-all-prod_short-clients"></a>Does this work with all [!INCLUDE[prod_short](includes/prod_short.md)] clients?

Yes. You can open files in OneDrive from the [!INCLUDE[prod_short](includes/prod_short.md)] mobile apps, when viewing card details in Microsoft Teams, or even from the Outlook add-in.  

## <a name="is-onedrive-the-same-as-sharepoint-for-storing-files"></a>Is OneDrive the same as SharePoint for storing files?

As part of your Microsoft 365 subscription, your organisation provides you with OneDrive, your file storage in the cloud. OneDrive is private by default, where you organise your content and choose which files or folders to share and with whom. SharePoint on the other hand, provides a file repository in the cloud that is shared with others in your organisation.  

## <a name="does-prod_short-support-consumer-onedrive"></a>Does [!INCLUDE[prod_short](includes/prod_short.md)] support consumer OneDrive?

No. This integration is exclusively intended for OneDrive for Business and only supports your work account. 

## <a name="are-all-onedrive-for-business-plans-supported"></a>Are all OneDrive for Business plans supported?

[!INCLUDE[prod_short](includes/prod_short.md)] does not support standalone plans for OneDrive for Business. OneDrive must be purchased as part of a Microsoft 365 business or enterprise plan. For more information, see [Compare OneDrive cloud storage pricing and plans](https://www.microsoft.com/microsoft-365/onedrive/compare-onedrive-plans?market=af&activetab=tab:primaryr2).  

## <a name="where-can-i-see-onedrive-service-health"></a>Where can I see OneDrive service health?

Administrators can access the Service health dashboard as part of the Microsoft 365 admin centre. The dashboard includes OneDrive’s service availability. 
 
## <a name="is-onedrive-integration-available-to-prod_short-on-premises"></a>Is OneDrive integration available to [!INCLUDE[prod_short](includes/prod_short.md)] on premises?

Yes, but unlike [!INCLUDE[prod_short](includes/prod_short.md)] online, it does require additional setup. For more information, see [Configuring Business Central On-Premises](admin-onedrive-integration.md#configuring-business-central-on-premises).  

## <a name="does-prod_short-on-premises-connect-with-sharepoint-server"></a>Does [!INCLUDE[prod_short](includes/prod_short.md)] on premises connect with SharePoint Server?

No. This deployment combination is not supported, even if SharePoint Server has enabled My Sites.  

## <a name="does-prod_short-online-connect-with-sharepoint-server"></a>Does [!INCLUDE[prod_short](includes/prod_short.md)] online connect with SharePoint Server?

No. This deployment combination is not supported, even if SharePoint Server has enabled My Sites.  

## <a name="how-does-this-work-in-an-organization-with-multiple-environments"></a>How does this work in an organisation with multiple environments?

The integration assumes that company names are unique across [!INCLUDE[prod_short](includes/prod_short.md)] environments. When company names are unique across the organisation, opening a file in OneDrive will copy the file to a folder named after the current company. If company names are not unique across environments, files may from identical company names will be placed together in the same folder.  

## <a name="weve-changed-company-name-what-happens-to-my-previous-files"></a>We’ve changed company name. What happens to my previous files?

[!INCLUDE[prod_short](includes/prod_short.md)] does not automatically migrate files you opened earlier in OneDrive to the new folder. After renaming your company, the Open in OneDrive action will copy files to a folder that has the new company name.   

## <a name="when-attaching-files-to-prod_short-how-do-i-pick-a-file-from-onedrive"></a>When attaching files to [!INCLUDE[prod_short](includes/prod_short.md)], how do I pick a file from OneDrive? 
[!INCLUDE[prod_short](includes/prod_short.md)] does not provide a cloud file picker. You must download the file from OneDrive to your device, and then upload it to [!INCLUDE[prod_short](includes/prod_short.md)]. 

## <a name="i-want-to-open-files-in-sharepoint-instead-how-do-i-do-this"></a>I want to open files in SharePoint instead. How do I do this?

[!INCLUDE[prod_short](includes/prod_short.md)] does not provide features to copy files to SharePoint and open them from a SharePoint library. Contact your Microsoft partner to understand your options, or search for apps on AppSource.  

## <a name="how-do-i-turn-off-integration-to-onedrive"></a>How do I turn off integration to OneDrive?

[!INCLUDE[prod_short](includes/prod_short.md)] online does not provide a way to enable or disable integration to OneDrive.  

## <a name="should-i-use-the-sharepoint-connection-setup-page-to-connect-to-sharepoint"></a>Should I use the SharePoint Connection Setup page to connect to SharePoint?

This is a legacy feature where all [!INCLUDE[prod_short](includes/prod_short.md)] files from all users are sent to a single SharePoint folder. We recommend that you do not configure the Shared Documents FastTab on the SharePoint Connection Setup page because we are working towards deprecating this feature.  

## <a name="which-version-of-prod_short-supports-onedrive"></a>Which version of [!INCLUDE[prod_short](includes/prod_short.md)] supports OneDrive?

Integration with OneDrive became available in 2021 release wave 2.  

## <a name="will-microsoft-continue-to-improve-the-integration-to-onedrive"></a>Will Microsoft continue to improve the integration to OneDrive?

At Microsoft, we're constantly listening to feedback from our diverse user community and acting upon the top suggestions. To learn about what's next for integrations with Microsoft 365 apps, see the [Dynamics 365 release plan](/dynamics365-release-plan/2021wave1).  

If you want to participate in improving OneDrive integration, or have an idea that would improve file sharing and collaboration in [!INCLUDE[prod_short](includes/prod_short.md)], add an idea or vote for existing ideas at [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="troubleshooting"></a>Troubleshooting

This section provides information about how to identify and fix problems you might experience when using OneDrive with [!INCLUDE[prod_short](includes/prod_short.md)].  

### <a name="i-have-to-sign-in-each-time-i-open-a-file"></a>I have to sign in each time I open a file

Sorry, that's a known issue and we're working on it. We expect to provide a smoother experience in an upcoming update.  

### <a name="business-central-cant-find-my-onedrive"></a>Business Central can't find my OneDrive

When this message displays, “Could not determine the location of your OneDrive for Business, contact your partner to set this up.”, check whether the user has accessed their OneDrive at least one time. If they haven't, ask the person to go to portal.office.com/onedrive to set it up. That can take a while. If the message still displays after 24 hours, contact Support.  
 

## <a name="see-also"></a>See Also
[Business Central and OneDrive Integration](across-onedrive-overview.md)  
[Managing OneDrive Integration with Business Central](admin-onedrive-integration.md)  
[Opening Business Central Files in OneDrive](across-share-onedrive.md)  
