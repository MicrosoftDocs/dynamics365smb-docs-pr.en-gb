---
title: Business Central accountant experience | Microsoft Docs
description: Learn about the accountant portal for Business Central and the Accountant Role Centre that supports internal and external accountants in the client company.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 05/02/2019
ms.author: edupont
ms.openlocfilehash: f088e1319684b9a18a2b0c8ab5305f73747f6889
ms.sourcegitcommit: dac212009aadf3227e54c99976c438f6e56f182a
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 05/02/2019
ms.locfileid: "1446929"
---
# <a name="accountant-experiences-in-included365finlongincludesd365finlongmdmd"></a>Accountant Experiences in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]
Any business must do its books and sign off on the accounting. Some businesses employ an external accountant, and others have an accountant on staff. No matter which type of accountant you are, you can use the **Accountant** Role Center as your Home in [!INCLUDE[d365fin](includes/d365fin_md.md)]. From here, you can access all pages that you need in your work.  

## <a name="accountant-role-center"></a>Accountant Role Centre
The Role Centre is a dashboard with activity tiles that show you real-time key figures and give you quick access to data. In the ribbon at the top of the page, you have access to more actions, such as opening the most commonly used financial reports and statements in Excel. In the navigation bar at the top, you can quickly switch between the lists you use most often. Here, you will see other areas, such as **Posted Documents** with the various types of documents that the company has posted.  

If you are new to [!INCLUDE[d365fin](includes/d365fin_md.md)], you can launch a list of videos right from your Role Centre. You can also launch a **Getting Started** tour that points out key areas.  

## <a name="accountant-hub"></a>Accountant Hub
If you are an accountant with several clients, you can use [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)] for a better overview of your clients. From there, you can access each client's tenant in [!INCLUDE[d365fin](includes/d365fin_md.md)] and use the Accountant Role Centre as described above. For more information see [Welcome to [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]](/dynamics365/accountants/index).

## <a name="inviting-your-external-accountant-to-your-included365finincludesd365finmdmd"></a>Inviting Your External Accountant to Your [!INCLUDE[d365fin](includes/d365fin_md.md)]
If you use an external accountant to manage your books and financial reporting, you can invite them to your [!INCLUDE[d365fin](includes/d365fin_md.md)] so they can work with you on your fiscal data.

Once your accountant has gained access to your [!INCLUDE[d365fin](includes/d365fin_md.md)], they can use the **Accountant** Role Centre that gives easy access to the most relevant pages for their work.  

We have made it easy for you to invite your external accountant. Simply open the **Users** page, and then choose the **Invite External Accountant** action in the ribbon. An email is made ready for you, just add your accountant's work email, and send the invitation.  

![Invite your accountant](./media/finance-invite-accountant/invite-accountant.png)

> [!TIP]  
>  This requires that you have set up SMTP email. You can do this yourself or ask your [!INCLUDE[d365fin](includes/d365fin_md.md)] partner. Also, you must be logged in to [!INCLUDE[d365fin](includes/d365fin_md.md)] as a user administrator, not as the business owner or other users. Finally, you must have left the trial company so that you have an Azure Active Directory administrator.  

> [!IMPORTANT]  
> The accountant's email address must be a work address that is based on Azure Active Directory. If the accountant uses another type of email, then the invitation cannot be sent.  

### <a name="separate-license"></a>Separate Licence
Behind the scenes, the accountant is added to your Active Directory tenant. Your administrator can verify that the accountant accepts the invitation and is assigned the correct licence. The steps for doing this depends on the type of account that you used when you signed up for [!INCLUDE[d365fin](includes/d365fin_md.md)]. This topic is based on the use of an Office 365 account, which uses Microsoft Azure Active Directory.  

If you have activated your subscription of [!INCLUDE[d365fin](includes/d365fin_md.md)] and are no longer using the evaluation company, you have an Azure Active Directory tenant. Your administrator or [!INCLUDE[d365fin](includes/d365fin_md.md)] partner manages this tenant in the [Azure portal](https://portal.azure.com). This is where new users are added and licences are applied and removed. For more information, see the [Microsoft Azure portal overview](https://docs.microsoft.com/en-us/azure/azure-portal-overview).  

One of the licence types for [!INCLUDE[d365fin](includes/d365fin_md.md)] is the *External Accountant* licence. This licence type is intended for use by users such as external accountants. This means that you do not have to buy an extra seat in your current Active Directory or use one of your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] user accounts on your external accountant. For example, if your current Office 365 subscription includes 10 users for [!INCLUDE[d365fin](includes/d365fin_md.md)], and you are currently using 10 *Full User* licences, your administrator can simply add your external accountant as a guest user in the Azure portal and assign this user the *External Accountant* licence at no additional cost. However, you can only have one user with the *External Accountant* license. If you want to add more users, you must update your Office 365 subscription accordingly.

## <a name="see-also"></a>See Also
[Finance](finance.md)  
[Setting Up Finance](finance-setup-finance.md)  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Closing Years and Periods](year-close-years-periods.md)  
[Working with Dimensions](finance-dimensions.md)  
[Analysing Financial Statements in Excel](finance-analyze-excel.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Setting Up Cash Flow Analysis](finance-setup-cash-flow-analyses.md)  
[Welcome to [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]](/dynamics365/accountants/index)  
[Dynamics 365 - Accountant Hub on Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  
