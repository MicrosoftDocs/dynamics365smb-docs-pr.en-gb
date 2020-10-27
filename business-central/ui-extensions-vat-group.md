---
title: The VAT Group Management Extension | Microsoft Docs
description: You can engage with other businesses to form a VAT group, and act as either a member or representative of the group when reporting VAT.
author: bholtorf
manager: annbe
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: VAT, value added tax, report
ms.date: 10/06/2020
ms.author: bholtorf
ms.openlocfilehash: 5dfadee976ce39e7d7ead2c09d907050682b4a7f
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989424"
---
# <a name="the-vat-group-management-extension"></a>The VAT Group Management Extension

You can join one or more businesses in your country to consolidate VAT reporting under a single registration number. This type of arrangement is known as a *VAT group* . You can engage with the group as a member or the group representative.

## <a name="forming-a-vat-group"></a>Forming a VAT Group
VAT group members and the group representative can use the **VAT Group Management Setup** assisted setup guide to define their engagement with the group, and create a connection between their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenants. The group members will use the connection to submit their VAT returns to the group representative. The representative will submit VAT to tax authorities on behalf of the group using a single VAT return. 

## <a name="vat-group-constellations"></a>VAT Group Constellations
Communication happens from group members to the representative. The group representative exposes an API that allows the members to submit their VAT returns to the VAT group representative. 
[!INCLUDE[d365fin](includes/d365fin_md.md)] supports inter-group VAT return submissions for companies using [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises or online, and in any combination. The setup of the communication depends on the constellation. The following sections describe how to set up various group constellations.

The following list shows the recommended order of the steps to set up a VAT group:

1. Create the setup in Azure Active Directory. For more information, see [Requirements for Authentication](ui-extensions-vat-group.md#requirements-for-authentication).
2. Share the technical information that VAT group members and the representative need to connect their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenants.

  Usually, the VAT group representative has this information, such as the name of the VAT group representative environment to which the VAT group members will submit VAT.
3. Create users in the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] that VAT group members can use to authenticate and connect.
4. Run the **Set up VAT Group Management** assisted setup guide to connect the VAT group members.

  The guide requires some information from the VAT group representative. For more information, see the [VAT Group Member Setup](#vat-group-member-setup) section. Make a note of the **Group Member ID** for each VAT group member. The representative needs these IDs to add the companies to the VAT group.
5. Set up the VAT Group Management extension in the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Set up VAT Group Management** assisted setup guide. 

> [!NOTE]
> To connect to the VAT group representative, group members need a user with access to the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)]. The VAT group representative must create at least one user for this, however, for security reasons we recommended that you create a user for each VAT group member. Make sure to distribute the credentials for these users to VAT group members in a secure way.

## <a name="understanding-the-vat-group-management-setup"></a>Understanding the VAT Group Management Setup

The VAT group representative exposes an API that VAT group members can use to connect to their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant and submit VAT returns. VAT group members will often use [!INCLUDE[d365fin](includes/d365fin_md.md)] in separate Azure Active Directory tenants. Therefore, more setup is needed to make a connection between the VAT group member and representative's [!INCLUDE[d365fin](includes/d365fin_md.md)]. 
  
VAT group members connect to the representative by calling a web service on the VAT group representative tenant. The caller must be authenticated using OAuth. When the VAT Group Management extension is set up, you will be asked to authenticate to the VAT group representative to get and save an access token. This access token is used when submitting VAT returns to the VAT group representative. 

Authentication is handled by Azure Active Directory, so your setup must be made in the VAT group representative's Azure Active Directory to allow connections. An Azure Active Directory app registration must be configured with access to the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)]. This is also true if the VAT group representative is using [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises. Additionally, you must configure Single Sign-On if the VAT group representative is using [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises.

> [!NOTE]
> For a limited time, authentication using a web service access key is also supported. For more information, see [Deprecated Features in 2021 release wave 1](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1#deprecated-features-in-2021-release-wave-1).

## <a name="requirements-for-authentication"></a>Requirements for Authentication 
When the VAT group representative is using [!INCLUDE[d365fin](includes/d365fin_md.md)] online or on-premises, VAT group members use Azure Active Directory to authenticate when they submit VAT returns to the VAT group representative. If the VAT group members are also using [!INCLUDE[d365fin](includes/d365fin_md.md)] online, the VAT group member can authenticate using the designated user credentials and the endpoint information. For more information, see [VAT Group Member Setup](ui-extensions-vat-group.md#vat-group-member-setup).

VAT group members who have [!INCLUDE[d365fin](includes/d365fin_md.md)] on-premises must set up an app registration in Azure Active Directory for the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant. The app registration will enable the VAT group representative's [!INCLUDE[d365fin](includes/d365fin_md.md)] online to authenticate the group member. For more information, see [Quickstart: Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app).

When you create the app registration in Azure Active Directory, you must specify the following.

* In the **Authentication** section, add **Web** as a platform, and use the following **Redirect URL** : https://businesscentral.dynamics.com/OAuthLanding.htm.
* In the **Authentication** section, in the option to select **Supported account types** , select **Accounts in any organisational directory (Any Azure AD directory - Multitenant)** .
* In the **Certificates & secrets** section, create a new client secret and note the value. The VAT group members will need the secret when they set up the connection to the group representative.
* In the **API permissions** section, add permissions to [!INCLUDE[d365fin](includes/d365fin_md.md)]. Enable delegated access to **Financials.ReadWrite.All** and **user_impersonation** .
* In the **Overview** section, note the **Application (client) ID** . The VAT group members will need the ID when they set up the connection to the group representative. 

## <a name="vat-group-member-setup"></a>VAT Group Member Setup
Set up the VAT group member by starting the **Set up VAT Group Management** assisted setup guide. 

> [!NOTE]
> Before you get started, contact the VAT group representative for the following information about their [!INCLUDE[d365fin](includes/d365fin_md.md)] tenant:
>
> * The API URL
> * The name of their company 
> * Client ID
> * Client secret
> * Sign in credentials for the dedicated user 

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Group** , and then choose the related link.
2. To define the company's VAT group role, choose **Member** , and then choose **Next** .
3. Copy the value of the **Group Member ID** field, and then share it with the VAT group representative so they can add your company as an approved member of the group.
4. Add the **API URL** from the VAT group representative. Typically, the URL is formatted as follows: `https://api.businesscentral.dynamics.com/v2.0/[TENANT-ID]/[ENVIRONMENTNAME]`. For example, `https://api.businesscentral.dynamics.com/v2.0/907869c3-b252-4aca-b9cb-17a15d25477b/UKRepresentative`. 
5. Add the [!INCLUDE[d365fin](includes/d365fin_md.md)] company name of the VAT group representative, such as *CRONUS UK Ltd* .
6. Choose **Authentication Type** , choose **OAuth2** , and then choose **Next** .
7. In the **Client ID** field, enter the ID provided by the VAT group representative.
8. In the **Client Secret provided by the VAT Group representative** field, enter the secret provided by the VAT group representative.
9. In the **OAuth 2.0 Authority Endpoint** field, enter *https://login.microsoftonline.com/common/oauth2* .
10. In the **OAuth 2.0 Resource URL** field, enter *https://api.businesscentral.dynamics.com/* .
11. In the **OAuth 2.0 Redirect URL** field, enter *https://businesscentral.dynamics.com/OAuthLanding.htm* . 
12. When you have specified the various fields, choose **Next** , and then enter the user credentials that were provided by the VAT group representative.
13. Choose the VAT report configuration that you use to report VAT to authorities in your country.

  For example, in the United Kingdom, the VAT report configuration would be set up to report VAT to HMRC. The VAT Group Management extension copies this setup but replaces the submission codeunit with one that supports submission to the VAT group representative rather than the tax authorities. The codeunit is provided by Microsoft. When done, choose **Next** .

## <a name="using-the-vat-group-management-features"></a>Using the VAT Group Management Features

VAT group members use the standard processes to prepare VAT returns. The only difference is to choose the **VATGROUP** report version, which submits the VAT return to the VAT group representative rather than the authorities. For more information, see [About the VAT Return Report](/business-central/finance-how-report-vat#about-the-vat-return-report).

The following sections describe the tasks that VAT group representatives must perform.

### <a name="vat-group-submissions"></a>VAT Group Submissions

The **VAT Group Submissions** page lists the VAT returns that members have submitted. The page serves as a draft location for the submissions until the VAT group representative includes them in a VAT return for the group. You can open the submissions to review the VAT for the individual boxes reported by the VAT group member.

### <a name="creating-a-group-vat-return"></a>Creating a Group VAT Return

To report VAT on behalf of the group, on the **VAT Returns** page, create a VAT return for your company only. Afterward, include the most recent VAT submissions from VAT group members by choosing the **Include Group VAT** action.  

When the VAT Group representative's VAT Return has been submitted to the authorities on behalf of the entire group, you will normally run the **Calculate and Post VAT Settlement** action. This action closes open VAT Entries and transfers amounts to the VAT Settlement account. Currently, this action does not take the group submissions into account. This means that only the VAT Entries of the VAT Group representative company will be posted. The VAT Group member submission amounts must be posted to the VAT settlement amount manually, so that the VAT Group representative's VAT Settlement account will reflect the liability of what was reported to authorities. This behaviour will change in an upcoming update of [!INCLUDE[d365fin](includes/d365fin_md.md)], so the entire group VAT (the Total Amount on Report Lines on the VAT Return) will be settled. 

> [!NOTE]
> VAT group members can correct submitted VAT returns as long as the group representative has not released the VAT return for the group. To make a correction, the VAT group member must create a new VAT return for the VAT return period and submit it to the VAT group representative. On the VAT group representative's side, the latest VAT return will be included on the **VAT Returns** page. 

## <a name="see-also"></a>See Also
[Work with VAT on Sales and Purchases](finance-work-with-vat.md)  
[Set Up Value-Added Tax](finance-setup-vat.md)
