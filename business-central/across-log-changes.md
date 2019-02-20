---
title: Track User Activity in a Change Log| Microsoft Docs
description: You can activate a user log so that you have a history of any changes made to data in tracked tables.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 11/14/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 59afb06e9d43bdadc5ceacf563a9e6faf7439b7b
ms.openlocfilehash: bc56e07a540c24f53b88651ad2b2ff5e1e56a571
ms.contentlocale: en-gb
ms.lasthandoff: 12/05/2018

---
# <a name="auditing-changes-in-business-central"></a>Auditing Changes in Business Central

You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities. The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables. The change log collects all changes that are made to the table.

> [!Important]
> A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:
<br />
> * The session expired and was refreshed.
> * The user selected another company or Role Centre.
> * The user signed out and back in.

## <a name="working-with-the-change-log"></a>Working with the Change Log

A common problem in many financial systems is to locate the origin of errors and changes in data. It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger. The change log lets you track all direct modifications a user makes to data in the database. You must specify each table and field that you want the system to log, and then you must activate the change log.  

You activate and deactivate the change log on the **Change Log Setup** page. When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.

On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.

After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page. If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.  

## <a name="see-also"></a>See Also
[Changing Basic Settings](ui-change-basic-settings.md)  
[Sorting](ui-sorting.md)  
[Using Search for Page or Report](ui-search.md)  
[Managing Users and Permissions](ui-how-users-permissions.md)    
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

