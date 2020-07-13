---
title: Set Up Email Logging| Microsoft Docs
description: Learn how to turn email interactions between salespeople and customers into real sales opportunities.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect, opportunity, email
ms.date: 07/01/2020
ms.author: bholtorf
ms.openlocfilehash: 9ca381bfebcd6db8e67d8153d4d2bc17eeffad81
ms.sourcegitcommit: f9aec4a72172d9270e14e2938c5550d69508f1aa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/02/2020
ms.locfileid: "3532676"
---
# <a name="track-email-message-exchanges-between-salespeople-and-contacts"></a><span data-ttu-id="5acc9-103">Track Email Message Exchanges Between Salespeople and Contacts</span><span class="sxs-lookup"><span data-stu-id="5acc9-103">Track Email Message Exchanges Between Salespeople and Contacts</span></span>

<span data-ttu-id="5acc9-104">Get more out of the communications between salespeople and your existing or potential customers by tracking email exchanges, and then turning them into actionable opportunities.</span><span class="sxs-lookup"><span data-stu-id="5acc9-104">Get more out of the communications between salespeople and your existing or potential customers by tracking email exchanges, and then turning them into actionable opportunities.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="5acc9-105">can work with Exchange Online to keep a log of the inbound and outbound messages.</span><span class="sxs-lookup"><span data-stu-id="5acc9-105">can work with Exchange Online to keep a log of the inbound and outbound messages.</span></span> <span data-ttu-id="5acc9-106">You can view and analyse the contents of each message on the **Interaction Log Entries** page.</span><span class="sxs-lookup"><span data-stu-id="5acc9-106">You can view and analyze the contents of each message on the **Interaction Log Entries** page.</span></span>

## <a name="set-up-public-folders-and-rules-for-email-logging-in-exchange-online"></a><span data-ttu-id="5acc9-107">Set up Public Folders and Rules for Email Logging in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5acc9-107">Set up Public Folders and Rules for Email Logging in Exchange Online</span></span>

[!INCLUDE[admin-setup-email-public-folder](includes/admin-setup-email-public-folder.md)]

<span data-ttu-id="5acc9-108">Next, you connect [!INCLUDE[prodshort](includes/prodshort.md)] with Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5acc9-108">Next, you connect [!INCLUDE[prodshort](includes/prodshort.md)] with Exchange Online.</span></span>

## <a name="setting-up-d365fin-to-log-email-messages"></a><span data-ttu-id="5acc9-109">Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)] to Log Email Messages</span><span class="sxs-lookup"><span data-stu-id="5acc9-109">Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)] to Log Email Messages</span></span>

<span data-ttu-id="5acc9-110">Get started with email logging in two easy steps:</span><span class="sxs-lookup"><span data-stu-id="5acc9-110">Get started with email logging in two easy steps:</span></span>

1. <span data-ttu-id="5acc9-111">Connect [!INCLUDE[d365fin](includes/d365fin_md.md)] with Exchange Online for your Office 365 subscription.</span><span class="sxs-lookup"><span data-stu-id="5acc9-111">Connect [!INCLUDE[d365fin](includes/d365fin_md.md)] with Exchange Online for your Office 365 subscription.</span></span> <span data-ttu-id="5acc9-112">Exchange Online handles your email messages.</span><span class="sxs-lookup"><span data-stu-id="5acc9-112">Exchange Online handles your email messages.</span></span> <span data-ttu-id="5acc9-113">We've made this step easy by providing an assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="5acc9-113">We've made this step easy by providing an assisted setup guide.</span></span> <span data-ttu-id="5acc9-114">You just need your administrator credentials for your administrator account in Office 365.</span><span class="sxs-lookup"><span data-stu-id="5acc9-114">You just need your administrator credentials for your administrator account in Office 365.</span></span> <span data-ttu-id="5acc9-115">To start the guide, go to **Assisted Setup**, and then choose **Set up email logging**.</span><span class="sxs-lookup"><span data-stu-id="5acc9-115">To start the guide, go to **Assisted Setup**, and then choose **Set up email logging**.</span></span>  

2. <span data-ttu-id="5acc9-116">Make sure that valid email addresses have been entered in [!INCLUDE[d365fin](includes/d365fin_md.md)] for your sales people and contacts, depending on whether they are potential or existing customers.</span><span class="sxs-lookup"><span data-stu-id="5acc9-116">Make sure that valid email addresses have been entered in [!INCLUDE[d365fin](includes/d365fin_md.md)] for your sales people and contacts, depending on whether they are potential or existing customers.</span></span> <span data-ttu-id="5acc9-117">To do that, for each customer or salesperson, open the **Contact** or **Salesperson/Purchaser** card and have a look in the **Email** field.</span><span class="sxs-lookup"><span data-stu-id="5acc9-117">To do that, for each customer or salesperson, open the **Contact** or **Salesperson/Purchaser** card and have a look in the **Email** field.</span></span>

> [!Tip]
> <span data-ttu-id="5acc9-118">After you complete the steps in the guide you can check whether the connection was successful.</span><span class="sxs-lookup"><span data-stu-id="5acc9-118">After you complete the steps in the guide you can check whether the connection was successful.</span></span> <span data-ttu-id="5acc9-119">Search for **Marketing Setup**, choose **Process**, then **Functions**, and then **Validate Email Logging Setup**.</span><span class="sxs-lookup"><span data-stu-id="5acc9-119">Search for **Marketing Setup**, choose **Process**, then **Functions**, and then **Validate Email Logging Setup**.</span></span>

## <a name="viewing-email-message-exchanges-in-the-interaction-log"></a><span data-ttu-id="5acc9-120">Viewing Email Message Exchanges in the Interaction Log</span><span class="sxs-lookup"><span data-stu-id="5acc9-120">Viewing Email Message Exchanges in the Interaction Log</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="5acc9-121">creates an entry on the **Interaction Log** page each time a salesperson and a contact exchange an email message.</span><span class="sxs-lookup"><span data-stu-id="5acc9-121">creates an entry on the **Interaction Log** page each time a salesperson and a contact exchange an email message.</span></span> <span data-ttu-id="5acc9-122">To view the interaction log, open the **Contact** or **Salesperson\*Purchaser** card for the person, and then choose **Navigate**, **History**, and then choose **Interaction Log Entries**.</span><span class="sxs-lookup"><span data-stu-id="5acc9-122">To view the interaction log, open the **Contact** or **Salesperson\*Purchaser** card for the person, and then choose **Navigate**, **History**, and then choose **Interaction Log Entries**.</span></span> <span data-ttu-id="5acc9-123">There are a few things we can do with each entry in the log, for example:</span><span class="sxs-lookup"><span data-stu-id="5acc9-123">There are a few things we can do with each entry in the log, for example:</span></span>

- <span data-ttu-id="5acc9-124">View the content of the email message that was exchanged by clicking the **Show Attachments** action.</span><span class="sxs-lookup"><span data-stu-id="5acc9-124">View the content of the email message that was exchanged by clicking the **Show Attachments** action.</span></span>
- <span data-ttu-id="5acc9-125">Turn an email exchange into a sales opportunity - If an entry looks promising, you can turn it into an opportunity and then manage its progress toward a sale.</span><span class="sxs-lookup"><span data-stu-id="5acc9-125">Turn an email exchange into a sales opportunity - If an entry looks promising, you can turn it into an opportunity and then manage its progress toward a sale.</span></span> <span data-ttu-id="5acc9-126">To do that, choose the entry, and then choose the **Create Opportunity** action.</span><span class="sxs-lookup"><span data-stu-id="5acc9-126">To do that, choose the entry, and then choose the **Create Opportunity** action.</span></span> <span data-ttu-id="5acc9-127">For more information, see [Managing Sales Opportunities](marketing-manage-sales-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="5acc9-127">For more information, see [Managing Sales Opportunities](marketing-manage-sales-opportunities.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="5acc9-128">See Also</span><span class="sxs-lookup"><span data-stu-id="5acc9-128">See Also</span></span>
[<span data-ttu-id="5acc9-129">Managing Relationships</span><span class="sxs-lookup"><span data-stu-id="5acc9-129">Managing Relationships</span></span>](marketing-relationship-management.md)

