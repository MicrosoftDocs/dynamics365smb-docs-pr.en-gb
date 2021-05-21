---
title: Searching for Contacts from Microsoft Teams
description: Learn how to look up Business Central customers, suppliers, and other contacts from Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, contacts, search, messaging extensions
ms.date: 04/12/2021
ms.author: jswymer
ms.openlocfilehash: 6d094e365ad0c7da73467e5a3160d926902c45d9
ms.sourcegitcommit: c11ad91a389ed72532f5513654fdc7909b20aed9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/22/2021
ms.locfileid: "5935168"
---
# <a name="searching-for-customers-vendors-and-other-contacts-from-microsoft-teams"></a><span data-ttu-id="b96e6-103">Searching for Customers, Suppliers, and Other Contacts from Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b96e6-103">Searching for Customers, Vendors, and Other Contacts from Microsoft Teams</span></span>

<span data-ttu-id="b96e6-104">[!INCLUDE [online_only](includes/online_only.md)].</span><span class="sxs-lookup"><span data-stu-id="b96e6-104">[!INCLUDE [online_only](includes/online_only.md)].</span></span> <span data-ttu-id="b96e6-105">Introduced in 2021 release wave 1.</span><span class="sxs-lookup"><span data-stu-id="b96e6-105">Introduced in 2021 release wave 1.</span></span>

<span data-ttu-id="b96e6-106">[!INCLUDE [prod_short](includes/prod_short.md)] has a comprehensive business contact management system that is essential for users in sales, operations, or other departmental roles.</span><span class="sxs-lookup"><span data-stu-id="b96e6-106">[!INCLUDE [prod_short](includes/prod_short.md)] has a comprehensive business contact management system that is essential for users in sales, operations, or other departmental roles.</span></span> <span data-ttu-id="b96e6-107">If you're a user in one of these roles, you'll often need to look up, meet, or start a conversation with your suppliers, customers, and other contacts.</span><span class="sxs-lookup"><span data-stu-id="b96e6-107">If you're a user in one of these roles, you'll often need to look up, meet, or start a conversation with your vendors, customers, and other contacts.</span></span> <span data-ttu-id="b96e6-108">With the [!INCLUDE [prod_short](includes/prod_short.md)] app for Teams, you can do these tasks directly from Teams, without having to switch to [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b96e6-108">With the [!INCLUDE [prod_short](includes/prod_short.md)] app for Teams, you can do these tasks directly from Teams, without having to switch to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b96e6-109">From within Teams, you can:</span><span class="sxs-lookup"><span data-stu-id="b96e6-109">From within Teams, you can:</span></span>

- <span data-ttu-id="b96e6-110">Look up [!INCLUDE [prod_short](includes/prod_short.md)] contacts from the Teams command box or from the message compose area.</span><span class="sxs-lookup"><span data-stu-id="b96e6-110">Look up [!INCLUDE [prod_short](includes/prod_short.md)] contacts from the Teams command box or from the message compose area.</span></span> <span data-ttu-id="b96e6-111">Contacts can include prospects, suppliers, customers, or other business relationships.</span><span class="sxs-lookup"><span data-stu-id="b96e6-111">Contacts can include prospects, vendors, customers, or other business relationships.</span></span>
- <span data-ttu-id="b96e6-112">Share a contact as a card in a Teams conversation.</span><span class="sxs-lookup"><span data-stu-id="b96e6-112">Share a contact as a card in a Teams conversation.</span></span>
- <span data-ttu-id="b96e6-113">View details about the contact, interaction history, and other insights like outstanding payments or open documents.</span><span class="sxs-lookup"><span data-stu-id="b96e6-113">View details about the contact, interaction history, and other insights like outstanding payments or open documents.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b96e6-114">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="b96e6-114">Prerequisites</span></span>

- <span data-ttu-id="b96e6-115">You have access to Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b96e6-115">You have access to Microsoft Teams.</span></span>
- <span data-ttu-id="b96e6-116">You've installed the [!INCLUDE [prod_short](includes/prod_short.md)] app in Teams.</span><span class="sxs-lookup"><span data-stu-id="b96e6-116">You've installed the [!INCLUDE [prod_short](includes/prod_short.md)] app in Teams.</span></span> <span data-ttu-id="b96e6-117">For more information, see [Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="b96e6-117">For more information, see [Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>
- <span data-ttu-id="b96e6-118">You've got a [!INCLUDE [prod_short](includes/prod_short.md)] account with access to contacts in at least one company.</span><span class="sxs-lookup"><span data-stu-id="b96e6-118">You've got a [!INCLUDE [prod_short](includes/prod_short.md)] account with access to contacts in at least one company.</span></span>

> [!NOTE]
> <span data-ttu-id="b96e6-119">Whether you searching from the command box or message compose box, you may be asked to sign in or set up the app the first time.</span><span class="sxs-lookup"><span data-stu-id="b96e6-119">Whether you searching from the command box or message compose box, you may be asked to sign in or set up the app the first time.</span></span> <span data-ttu-id="b96e6-120">This step is necessary to search for contacts in the right Business Central company.</span><span class="sxs-lookup"><span data-stu-id="b96e6-120">This step is necessary to search for contacts in the right Business Central company.</span></span> <span data-ttu-id="b96e6-121">For information about setting up the app to choose your company, see [Changing Company and Other Settings in Teams](across-teams-settings.md).</span><span class="sxs-lookup"><span data-stu-id="b96e6-121">For information about setting up the app to choose your company, see [Changing Company and Other Settings in Teams](across-teams-settings.md).</span></span>

## <a name="look-up-contacts-from-the-command-box"></a><span data-ttu-id="b96e6-122">Look up contacts from the command box</span><span class="sxs-lookup"><span data-stu-id="b96e6-122">Look up contacts from the command box</span></span>

<span data-ttu-id="b96e6-123">The command box is at the top of every screen in Teams.</span><span class="sxs-lookup"><span data-stu-id="b96e6-123">The command box is at the top of every screen in Teams.</span></span> <span data-ttu-id="b96e6-124">It lets you search, take quick actions, or launch apps, like the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span><span class="sxs-lookup"><span data-stu-id="b96e6-124">It lets you search, take quick actions, or launch apps, like the [!INCLUDE [prod_short](includes/prod_short.md)] app.</span></span> <span data-ttu-id="b96e6-125">Searching from the command box is great for quickly looking up contacts and their related data for your own use.</span><span class="sxs-lookup"><span data-stu-id="b96e6-125">Searching from the command box is great for quickly looking up contacts and their related data for your own use.</span></span> <span data-ttu-id="b96e6-126">For example, suppose you want to look up an email address of a supplier to set up a calendar meeting.</span><span class="sxs-lookup"><span data-stu-id="b96e6-126">For example, suppose you want to look up an email address of a vendor to set up a calendar meeting.</span></span> <span data-ttu-id="b96e6-127">Or maybe you want to look up interaction history during a meeting with a customer.</span><span class="sxs-lookup"><span data-stu-id="b96e6-127">Or maybe you want to look up interaction history during a meeting with a customer.</span></span>

1. <span data-ttu-id="b96e6-128">In the command box, type **@Business Central**, then select the Business Central app from the results.</span><span class="sxs-lookup"><span data-stu-id="b96e6-128">In the command box, type **@Business Central**, then select the Business Central app from the results.</span></span>

    ![Open Business Central app  to search for contacts from command box](media/teams-contacts-command-1.png)

2. <span data-ttu-id="b96e6-130">In the **Business Central** box, start typing search text, like a name, address, or phone number.</span><span class="sxs-lookup"><span data-stu-id="b96e6-130">In the **Business Central** box, start typing search text, like a name, address, or phone number.</span></span>

    <span data-ttu-id="b96e6-131">As you type, matching results will appear.</span><span class="sxs-lookup"><span data-stu-id="b96e6-131">As you type, matching results will appear.</span></span>

    ![Search Business Central contacts from command box in Teams](media/teams-contacts-command-2.png)
3. <span data-ttu-id="b96e6-133">Select a contact from the results.</span><span class="sxs-lookup"><span data-stu-id="b96e6-133">Select a contact from the results.</span></span>

    <span data-ttu-id="b96e6-134">The contact card appears beneath the command box.</span><span class="sxs-lookup"><span data-stu-id="b96e6-134">The contact card appears beneath the command box.</span></span>

4. <span data-ttu-id="b96e6-135">If you want to add the contact card into a conversation, go to the upper right corner of the card, select **... (More options)** > **Copy**.</span><span class="sxs-lookup"><span data-stu-id="b96e6-135">If you want to add the contact card into a conversation, go to the upper right corner of the card, select **... (More options)** > **Copy**.</span></span> <span data-ttu-id="b96e6-136">Then, paste the copy in the message compose box of a conversation.</span><span class="sxs-lookup"><span data-stu-id="b96e6-136">Then, paste the copy in the message compose box of a conversation.</span></span>  

<span data-ttu-id="b96e6-137">For more general information about the command box in Teams, see [Teams - Use the command box](https://support.microsoft.com/en-us/office/use-the-command-box-13c4e429-7324-4886-b377-5dbed539193b).</span><span class="sxs-lookup"><span data-stu-id="b96e6-137">For more general information about the command box in Teams, see [Teams - Use the command box](https://support.microsoft.com/en-us/office/use-the-command-box-13c4e429-7324-4886-b377-5dbed539193b).</span></span>

## <a name="look-up-contacts-from-the-message-compose-box"></a><span data-ttu-id="b96e6-138">Look up contacts from the message compose box</span><span class="sxs-lookup"><span data-stu-id="b96e6-138">Look up contacts from the message compose box</span></span>

<span data-ttu-id="b96e6-139">The advantage of using the message compose box is that you can add a contact card directly to a conversation, for others to see.</span><span class="sxs-lookup"><span data-stu-id="b96e6-139">The advantage of using the message compose box is that you can add a contact card directly to a conversation, for others to see.</span></span>

1. <span data-ttu-id="b96e6-140">Beneath to message compose box, select the **Business Central** icon to launch the app.</span><span class="sxs-lookup"><span data-stu-id="b96e6-140">Beneath to message compose box, select the **Business Central** icon to launch the app.</span></span>

    <span data-ttu-id="b96e6-141">If you don't see the **Business Central** icon, select **... (Messaging extensions)**.</span><span class="sxs-lookup"><span data-stu-id="b96e6-141">If you don't see the **Business Central** icon, select **... (Messaging extensions)**.</span></span>

    ![Open Business Central app to search for contacts from message box](media/teams-contacts-message-box.png)

2. <span data-ttu-id="b96e6-143">In the **Business Central** box, start typing search text, like a name, address, or phone number.</span><span class="sxs-lookup"><span data-stu-id="b96e6-143">In the **Business Central** box, start typing search text, like a name, address, or phone number.</span></span>

    <span data-ttu-id="b96e6-144">As you type, matching results will appear.</span><span class="sxs-lookup"><span data-stu-id="b96e6-144">As you type, matching results will appear.</span></span>

    ![Search for Business Central contacts from message box](media/teams-contacts-5.png)
3. <span data-ttu-id="b96e6-146">Select a contact from the results.</span><span class="sxs-lookup"><span data-stu-id="b96e6-146">Select a contact from the results.</span></span>

    <span data-ttu-id="b96e6-147">The contact card appears in the message compose box.</span><span class="sxs-lookup"><span data-stu-id="b96e6-147">The contact card appears in the message compose box.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b96e6-148">The contact card isn't sent to the conversation right away for others to see.</span><span class="sxs-lookup"><span data-stu-id="b96e6-148">The contact card isn't sent to the conversation right away for others to see.</span></span> <span data-ttu-id="b96e6-149">You have the opportunity to review the contents of the card, and add text before or after it as you like.</span><span class="sxs-lookup"><span data-stu-id="b96e6-149">You have the opportunity to review the contents of the card, and add text before or after it as you like.</span></span> <span data-ttu-id="b96e6-150">Then, send your message to the chat when ready.</span><span class="sxs-lookup"><span data-stu-id="b96e6-150">Then, send your message to the chat when ready.</span></span>

### <a name="heres-another-way"></a><span data-ttu-id="b96e6-151">Here's another way</span><span class="sxs-lookup"><span data-stu-id="b96e6-151">Here's another way</span></span>

1. <span data-ttu-id="b96e6-152">Instead of using the **Business Central** icon, type **@Business Central** directly in the message compose box.</span><span class="sxs-lookup"><span data-stu-id="b96e6-152">Instead of using the **Business Central** icon, type **@Business Central** directly in the message compose box.</span></span>
2. <span data-ttu-id="b96e6-153">Enter your search terms in the box.</span><span class="sxs-lookup"><span data-stu-id="b96e6-153">Enter your search terms in the box.</span></span>
3. <span data-ttu-id="b96e6-154">Use the up and down arrow keys on the keyboard to choose a contact, then press Enter to select it.</span><span class="sxs-lookup"><span data-stu-id="b96e6-154">Use the up and down arrow keys on the keyboard to choose a contact, then press Enter to select it.</span></span>

## <a name="viewing-contact-card-details"></a><span data-ttu-id="b96e6-155">Viewing contact card details</span><span class="sxs-lookup"><span data-stu-id="b96e6-155">Viewing contact card details</span></span>

<span data-ttu-id="b96e6-156">The contact card in Teams gives you a quick overview of the customer, supplier, or contact.</span><span class="sxs-lookup"><span data-stu-id="b96e6-156">The contact card in Teams gives you a quick overview of the customer, vendor, or contact.</span></span> <span data-ttu-id="b96e6-157">The card is interactive&mdash;meaning you can view more information or even modify a contact by using the **Details** or **Pop-out** buttons.</span><span class="sxs-lookup"><span data-stu-id="b96e6-157">The card is interactive&mdash;meaning you can view more information or even modify a contact by using the **Details** or **Pop-out** buttons.</span></span>

<span data-ttu-id="b96e6-158">The **Details** button opens a window within Teams that displays more information about the contact, but not as much as you'd see in [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b96e6-158">The **Details** button opens a window within Teams that displays more information about the contact, but not as much as you'd see in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b96e6-159">To see all the information about a contact in [!INCLUDE [prod_short](includes/prod_short.md)], select **Pop-out**.</span><span class="sxs-lookup"><span data-stu-id="b96e6-159">To see all the information about a contact in [!INCLUDE [prod_short](includes/prod_short.md)], select **Pop-out**.</span></span>

<span data-ttu-id="b96e6-160">The contact card works just like cards for records, like items, customers, or sales orders.</span><span class="sxs-lookup"><span data-stu-id="b96e6-160">The contact card works just like cards for records, like items, customers, or sales orders.</span></span> <span data-ttu-id="b96e6-161">For more information about cards, see [View card details](across-working-with-teams.md#view-card-details).</span><span class="sxs-lookup"><span data-stu-id="b96e6-161">For more information about cards, see [View card details](across-working-with-teams.md#view-card-details).</span></span>

> [!NOTE]
> <span data-ttu-id="b96e6-162">All participants in a Teams conversation will be able to view cards for Business Central contact that you submit to a conversation.</span><span class="sxs-lookup"><span data-stu-id="b96e6-162">All participants in a Teams conversation will be able to view cards for Business Central contact that you submit to a conversation.</span></span> <span data-ttu-id="b96e6-163">But to view more details about records, by using the **Details** or **Pop out** buttons on a card, they'll need access to [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b96e6-163">But to view more details about records, by using the **Details** or **Pop out** buttons on a card, they'll need access to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b96e6-164">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span><span class="sxs-lookup"><span data-stu-id="b96e6-164">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span></span>

## <a name="see-also"></a><span data-ttu-id="b96e6-165">See Also</span><span class="sxs-lookup"><span data-stu-id="b96e6-165">See Also</span></span>

[<span data-ttu-id="b96e6-166">Business Central and Microsoft Teams Integration Overview</span><span class="sxs-lookup"><span data-stu-id="b96e6-166">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="b96e6-167">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="b96e6-167">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="b96e6-168">Teams FAQ</span><span class="sxs-lookup"><span data-stu-id="b96e6-168">Teams FAQ</span></span>](teams-faq.md)  
[<span data-ttu-id="b96e6-169">Troubleshooting Teams</span><span class="sxs-lookup"><span data-stu-id="b96e6-169">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  
[<span data-ttu-id="b96e6-170">Developing for Teams Integration</span><span class="sxs-lookup"><span data-stu-id="b96e6-170">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]