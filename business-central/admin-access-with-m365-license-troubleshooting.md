---
title: Troubleshoot Access with Microsoft 365 Licences
description: Learn how you can fix problems accessing Business Central with only a Microsoft 365 licence.
author: mikebc
ms.author: mikebc
ms.reviewer: jswymer
ms.service: dynamics365-business-central
ms.topic: troubleshooting
ms.date: 11/03/2022
ms.custom: bap-template
ms.search.keywords: 'License, access, Microsoft 365, collaborate, collaboration, Teams, Microsoft Teams'
---

# Troubleshoot Access with Microsoft 365 Licences

## Symptoms

When accessing a record in Teams, you are shown an error message in a tab or card details similar to:

"This page uses data from related tables that you do not have access to. To work with all features of this page, contact your administrator."

## Cause

You are most likely missing object permissions for tables that the current page or record links to.

## Symptoms

Access has been enabled, but users get a permission error when accessing any record.

## Cause

If you enable access in the Business Central admin centre, but do not assign permissions in the Licence Configuration page, anyone that attempts to access Business Central records in Teams will have their user record provisioned without permission to any objects. Business Central is secure by design: administrators must first configure what data can be accessed in Teams. 

## Resolution

Customising permissions in the Licence Configuration page will only affect newly created users. You must also assign the missing permissions to users that have already been created through the Users list page. 

## Symptoms

When I share a link in Teams, others get the error "When accessing Business Central with a Microsoft 365 licence, you can only view data in Microsoft Teams".

## Cause

When sharing a Business Central link to a Teams chat or channels, navigating a link will always navigate out of Microsoft Teams where the data no longer becomes accessible to a person having a Microsoft 365 licence.

## Resolution

When sharing pages or records, either include the link preview as a card, or share data as a tab in the chat or channel.

## See also 

[Business Central Access with Microsoft 365 licences](admin-access-with-m365-license.md#minimum-requirements)  
[Set Up Access with Microsoft 365 Licences](admin-access-with-m365-license-setup.md)  
[Business Central and Microsoft Teams Integration](across-teams-overview.md)
[Sharing Business Central Records and Page Links in Microsoft Teams](across-working-with-teams.md)  
[Troubleshoot Teams Integration](admin-teams-troubleshooting.md)  