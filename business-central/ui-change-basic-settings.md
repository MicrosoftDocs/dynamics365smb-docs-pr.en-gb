---
title: Change basic settings for the current user
description: Learn how to change some basic settings, for example, your Role Centre, company, or work date.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: change Role Center, notification, change company, change work date
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a0a504aa7c06c08d2e9f4251128e4203f0f90dee
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787459"
---
# <a name="change-basic-settings"></a>Change Basic Settings

On the **My Settings** page, you can see and change basic settings for your [!INCLUDE[prod_short](includes/prod_short.md)]. The changes that you make will only affect your workspace, not the workspaces of other users.  

## <a name="role"></a><a name="role-center"></a>Role

The role determines the home page, a starting screen that is designed for the needs of a specific role in an organisation. Depending on your role, the home page, or role centre, gives you an overview of the business, your department, or your personal tasks. It also helps you navigate to your daily tasks and find work that is assigned to you.

* At the top, the navigation allows you to switch between customers, vendors, items, and other important lists of information. Similarly, actions allow you to initiate tasks, such as create a new sales invoice, directly from the home page.

* In the centre, you find the **Activities** area, which shows current data and can be clicked or tapped to view more detailed information. Key performance indicators (KPIs) can be set up to display a selected chart for a visual representation of, for example, cash flow or income and expenses. You can also build up a list of favourite customers on the home page for business accounts that you do business with often or need to pay special attention to.

### <a name="to-change-the-role"></a>To change the role

The default role is **Business Manager**, but you can select another role to use a role centre that fits your needs better.  

1. In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role centre"), and then choose the **My Settings** action.
2. On the **My Settings** page, in the **Role** field, select the role that you want to use by default. For example, select **Accountant**.
3. Choose the **OK** button.

## <a name="company"></a><a name="company"></a>Company

A company functions as a container for data in [!INCLUDE[prod_short](includes/prod_short.md)]. There can be multiple companies in a database, but only one can be selected at a time.

The default company is called CRONUS and contains demonstration data only. You can create a new company with custom data. For more information, see [Creating New Companies](about-new-company.md).

### <a name="to-change-the-company-name"></a>To change the company name

The company name is always displayed at the top left corner and works as an action that you can choose to go back to the Role Centre. You can change this name on the **Company Information** page.

1. Choose the ![Sprocket icon to open the Settings menu](media/ui-experience/settings_icon_small.png) icon, and then choose the **Company Information** action.
2. In the **Name** field, enter the new company name.
3. Leave the page. The system restarts and displays the new company in the top-left corner.

### <a name="to-display-a-company-badge-for-quick-access-to-company-information"></a><a name="badge"></a>To display a company badge for quick access to company information

You can add a customised badge in the top-right corner, which you can choose to quickly view company name and tenant information in a pop-up box. The company badge is also useful when [!INCLUDE[prod_short](includes/prod_short.md)] is embedded in another application, like Microsoft Teams or in some other web application. In these cases, because the [!INCLUDE[web_client](includes/web_client.md)] displays less surrounding contextual information, the company badge serves as the only way to determine which company or environment a record belongs to.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Company Information**, and then choose the related link.
2. On the **Company Badge** FastTab, fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

> [!NOTE]
> If a company badge is defined, then you cannot change the company name as described in [To change the company name](ui-change-basic-settings.md#to-change-the-company-name)

## <a name="work-date"></a><a name="work-date"></a>Work date
The most commonly used work date is today's date. You may have to temporarily change the work date to be able to perform tasks, such as completing transactions for a date that is not today's date.

> [!TIP]  
> In all date fields, type **t** to quickly enter today's date, and type **w** to quickly enter the work date, which is the value in the **Work Date** field on the **My Settings** page.

> [!IMPORTANT]  
> After you change the work date, if you sign out or switch to another company, the work data reverts to the default work date. So the next time you sign in or switch back to the original company, you may have to set the work date again.

### <a name="work-date-indication"></a>Work date indication

The work date is critical on pages that can be edited. Whenever the work date isn't set to today's date on an editable page, then two types of indicators appear on the page:

* A reminder appears at the top of the page that tells you what the work date is set to. The reminder provides a direct link to the work date setting on the **My Settings** page so you change the date if you want. From the reminder, you can also choose to dismiss the reminder for the rest of your session. Unless you change the work date to "today", the reminder will appear the next time you sign in.

* If you dismiss the reminder, the work date will appear in the title of the page.  

If the work date isn't set to the current day (today), then on all pages where you can edit data, the current work date appears in the upper-left corner.

## <a name="region"></a><a name="region"></a> Region

The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.

## <a name="language"></a><a name="language"></a> Language

Changes the display language. This field appears only when there's more than one language to choose from.

The initial language is either determined by the administrator or by your browser settings when you sign up for [!INCLUDE[prod_short](includes/prod_short.md)]. The language that you set will be used on all devices that you sign in from, such as a phone or tablet.

Additional languages for [!INCLUDE[prod_short](includes/prod_short.md)] can be installed from AppSource. While all supported display languages are shown in the list, the administrator must install the relevant language app to the tenant before users can switch to the new language in [!INCLUDE[prod_short](includes/prod_short.md)].  

## <a name="time-zone"></a>Time zone

Defines the time zone where you are located. When you first sign into [!INCLUDE [prod_short](includes/prod_short.md)], the time zone is set based on your company's address. Change it if it doesn't fit your physical location.  

## <a name="notifications"></a>Notifications

Choose the *Change when I receive notifications* link to view or change the notifications that you get about certain events or changes in status, such as when you are about to invoice a customer who has an overdue balance, or the available inventory is lower than the quantity you are about to sell. For more information, see [Managing Notifications](ui-smart-notifications.md).

## <a name="teaching-tips"></a>Teaching tips

[!INCLUDE [ua-teachingtips](includes/ua-teachingtips.md)]

## <a name="see-related-training-at-microsoft-learn"></a>See Related Training at [Microsoft Learn](/learn/modules/personalize-ui-dynamics-365-business-central/index)

## <a name="see-also"></a>See Also

[Creating New Companies](about-new-company.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Change Which Features are Displayed](ui-experiences.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
