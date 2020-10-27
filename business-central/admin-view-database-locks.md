---
title: View Database Locks
description: Learn how you can view information about any database locks right from the client interface in Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 6880ffa9a2ab42c1af7c22f9cace64697c9f905b
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922324"
---
# <a name="viewing-database-locks"></a>Viewing Database Locks

Database locking controls access by multiple users to the same data at the same time. To protect a transaction against other transactions modifying the same data, the first transaction puts a lock on the data. The lock remains until the transaction's done.

Users may be blocked from completing transactions on the locked data. They'll typically get a message that indicates the lock condition.

## <a name="to-view-database-locks"></a>To view database locks

Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Database Locks** , and then choose the related link.

The **Database Locks** page gives snapshot of all current database locks.

For more information about database locking, see [Monitoring Database Locks](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) in the Business Central Developer and IT Pro help.

## <a name="see-also"></a>See Also

[Monitor Database Locks](/dynamics365/business-central/dev-itpro/administration/monitor-database-locks) 
