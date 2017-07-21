---
title: Apply and Modify Saved Settings on Reports | Microsoft Docs
description: Describes using predefined options and filters to customise a report, and to generate the correct data.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 06/02/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 9e5f7417579a5ba0629032cf9fa664e0060b9cbf
ms.contentlocale: en-gb
ms.lasthandoff: 07/07/2017


---
# <a name="saved-settings-on-reports"></a>Saved Settings on Reports
Depending on the report that is run, you might be presented with a page that lets you to set certain options and filters for changing the data that is included in the generated report. This page is known as the report request page. A report can include one or more *saved settings* that you can apply to the report from the request page. *Saved settings* are basically predefined options and filters. Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.

You can see the saved settings that are available to you for a report in **Saved Settings** section of the report request page.  

## <a name="to-apply-saved-settings-to-a-report"></a>To apply saved settings to a report
1. Open the report.

   The report request page appears.    
2. In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.

   The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries. The saved settings entry called **Last used options and filters** is always available. These settings are the option and filter values that were used the last time you ran the report.

## <a name="administer-saved-report-settings-for-users"></a>Administer saved report settings for users
If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in company. You can assign saved settings for a report to individual users or all users in the company.

You manage saved settings from page 1506 **Reports Settings**. To open this page, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Settings**, and then choose the related link.

From the **Report Settings** page, you can create a new settings from scratch or you can make a copy and modify existing settings. To modify the options and filters for a settings, choose the **Edit** action.

**Notes:**

* The saved settings feature on reports is only relevant when the SaveValues property of the request page is set to Yes. The SaveValues property property is set in the development environment.
* If you create a saved settings item for all users, and it has the same name as an existing saved settings for a specific user, then that user will not be able to use the saved settings that is assigned to everyone.  In the Saved Settings field on the report request page, the user will see two saved settings options with the same name. However, no matter which option he chooses, the user-specific saved settings will be used.

## <a name="see-also"></a>See Also
[Schedule a Rpeort to Run](ui-schedule-report.md)  

