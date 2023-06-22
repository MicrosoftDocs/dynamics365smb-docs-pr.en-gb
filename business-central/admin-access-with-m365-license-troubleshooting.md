---
title: Troubleshoot Access with Microsoft 365 Licences
description: Learn how you can fix problems accessing Business Central with only a Microsoft 365 licence.
author: mikebc
ms.author: mikebc
ms.reviewer: jswymer
ms.topic: troubleshooting
ms.date: 02/07/2023
ms.custom: bap-template
ms.search.keywords: 'License, access, Microsoft 365, collaborate, collaboration, Teams, Microsoft Teams'
---

# <a name="troubleshoot-access-with-microsoft--licenses" />Troubleshoot Access with Microsoft 365 Licences

## <a name="this-page-uses-data-from-related-tables-that-you-do-not-have-access-to-error-message" />"This page uses data from related tables that you do not have access to" error message

### <a name="symptoms" />Symptoms

When accessing a record in Teams, you're shown an error message in a tab or card details similar to:

"This page uses data from related tables that you don't have access to. To work with all features of this page, contact your administrator."

### <a name="cause" />Cause

You're most likely missing object permissions for tables that the current page or record links to.

## <a name="microsoft--access-has-been-enabled-but-users-get-a-permission-error" />Microsoft 365 access has been enabled, but users get a permission error

### <a name="symptoms" />Symptoms

Access with Microsoft 365 has been enabled in Business Central admin centre, but users get a permission error when accessing any record.

### <a name="cause" />Cause

If you enable access in the Business Central admin centre, but don't assign permissions in the **Licence Configuration** page, anyone that attempts to access Business Central records in Teams will have their user record provisioned without permission to any objects. Business Central is secure by design: administrators must first configure what data can be accessed in Teams. 

### <a name="resolution" />Resolution

Customising permissions in the Licence Configuration page will only affect newly created users. You must also assign the missing permissions to users that have already been created through the Users list page. 

## <a name="you-shared-a-link-in-teams-but-users-get-a-message-that-they-can-only-view-data" />You shared a link in Teams, but users get a message that they can only view data

### <a name="symptoms" />Symptoms

When you share a link in Teams as a Business Central user, others get the error "When accessing Business Central with a Microsoft 365 licence, you can only view data in Microsoft Teams".

### <a name="cause" />Cause

When sharing a Business Central link to a Teams chat or channels, navigating a link will always navigate out of Microsoft Teams where the data no longer becomes accessible to a person having a Microsoft 365 licence.

### <a name="resolution" />Resolution

When sharing pages or records, either include the link preview as a card, or share data as a tab in the chat or channel.

## <a name="card-from-shared-link-is-minimal-and-doesnt-include-details-button" />Card from shared link is minimal and doesn't include Details button

### <a name="symptoms" />Symptoms

When a Microsoft 365 licence holder without a Business Central licence shares a Business Central link in Teams, it automatically expands into a card that has no useful information and only shows Business Central with no **Details** button.

### <a name="cause" />Cause

Users who have a Microsoft 365 licence but no Business Central licence aren't allowed to share links as cards. If the user has the Business Central app for Teams installed and pastes a link into the compose area, then only a minimal card is displayed. 

## <a name="see-also" />See also

[Business Central Access with Microsoft 365 licences](admin-access-with-m365-license.md#minimum-requirements)  
[Set Up Access with Microsoft 365 Licences](admin-access-with-m365-license-setup.md)  
[Business Central and Microsoft Teams Integration](across-teams-overview.md)
[Sharing Business Central Records and Page Links in Microsoft Teams](across-working-with-teams.md)  
[Troubleshoot Teams Integration](admin-teams-troubleshooting.md)  
