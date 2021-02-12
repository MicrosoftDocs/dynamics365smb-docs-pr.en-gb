---
title: Working with Business Central Data in Microsoft Teams| Microsoft Docs
description: Learn how to use the Business Central app for Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 01/20/2021
ms.author: jswymer
ms.openlocfilehash: 0f7c1e8016a1bc1915d7d6a54a183aa0e8cea2ea
ms.sourcegitcommit: 36a32c997b201ff32ed8c1cff8179b36e2468c47
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/22/2021
ms.locfileid: "5046461"
---
# <a name="working-with-business-central-data-in-microsoft-teams"></a><span data-ttu-id="ee3c2-103">Working with Business Central Data in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ee3c2-103">Working with Business Central Data in Microsoft Teams</span></span>

[!INCLUDE [online_only](includes/online_only.md)]

<span data-ttu-id="ee3c2-104">[!INCLUDE [prod_short](includes/prod_short.md)] offers an app that connects Microsoft Teams to your business data in [!INCLUDE [prod_short](includes/prod_short.md)], so you can quickly share details across team members and respond faster to inquiries.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-104">[!INCLUDE [prod_short](includes/prod_short.md)] offers an app that connects Microsoft Teams to your business data in [!INCLUDE [prod_short](includes/prod_short.md)], so you can quickly share details across team members and respond faster to inquiries.</span></span> <span data-ttu-id="ee3c2-105">In this article, you'll learn how to use the app to share [!INCLUDE [prod_short](includes/prod_short.md)] data with coworkers in a Teams conversation.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-105">In this article, you'll learn how to use the app to share [!INCLUDE [prod_short](includes/prod_short.md)] data with coworkers in a Teams conversation.</span></span>

## <a name="overview"></a><span data-ttu-id="ee3c2-106">Overview</span><span class="sxs-lookup"><span data-stu-id="ee3c2-106">Overview</span></span>

<span data-ttu-id="ee3c2-107">The [!INCLUDE [prod_short](includes/prod_short.md)] app lets you:</span><span class="sxs-lookup"><span data-stu-id="ee3c2-107">The [!INCLUDE [prod_short](includes/prod_short.md)] app lets you:</span></span>

- <span data-ttu-id="ee3c2-108">Copy a link to any Business Central record and paste it into a Teams conversation to share with your coworkers.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-108">Copy a link to any Business Central record and paste it into a Teams conversation to share with your coworkers.</span></span> <span data-ttu-id="ee3c2-109">The app will then expand the link into a compact, interactive card that displays information about the record.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-109">The app will then expand the link into a compact, interactive card that displays information about the record.</span></span>
- <span data-ttu-id="ee3c2-110">Once in the conversation, you and coworkers can view more details about the record, edit data, and take action&mdash;without leaving Teams.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-110">Once in the conversation, you and coworkers can view more details about the record, edit data, and take action&mdash;without leaving Teams.</span></span>

<span data-ttu-id="ee3c2-111">[![Teams integration with Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ee3c2-111">[![Teams integration with Business Central](media/teams-intro-v3.png)](media/teams-intro-v3.png#lightbox)</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee3c2-112">Prerequisites</span><span class="sxs-lookup"><span data-stu-id="ee3c2-112">Prerequisites</span></span>

- <span data-ttu-id="ee3c2-113">You have access to Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-113">You have access to Microsoft Teams.</span></span>
- <span data-ttu-id="ee3c2-114">You've installed the [!INCLUDE [prod_short](includes/prod_short.md)] app in Teams.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-114">You've installed the [!INCLUDE [prod_short](includes/prod_short.md)] app in Teams.</span></span> <span data-ttu-id="ee3c2-115">For more information, see [Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="ee3c2-115">For more information, see [Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>

> [!NOTE]
> <span data-ttu-id="ee3c2-116">All participants in a Teams conversation will be able to view cards for Business Central records that you submit to the conversation.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-116">All participants in a Teams conversation will be able to view cards for Business Central records that you submit to the conversation.</span></span> <span data-ttu-id="ee3c2-117">But to view more details about records, by using the **Details** or **Pop out** buttons on a card, they'll need access to [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ee3c2-117">But to view more details about records, by using the **Details** or **Pop out** buttons on a card, they'll need access to [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="ee3c2-118">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span><span class="sxs-lookup"><span data-stu-id="ee3c2-118">For more information, see [Managing Microsoft Teams Integration](admin-teams-integration.md#minimum-requirements-1).</span></span>

## <a name="include-a-business-central-card-in-a-teams-conversation"></a><span data-ttu-id="ee3c2-119">Include a Business Central card in a Teams conversation</span><span class="sxs-lookup"><span data-stu-id="ee3c2-119">Include a Business Central card in a Teams conversation</span></span>

1. <span data-ttu-id="ee3c2-120">Sign in to [!INCLUDE [prod_short](includes/prod_short.md)] using your browser.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-120">Sign in to [!INCLUDE [prod_short](includes/prod_short.md)] using your browser.</span></span>
2. <span data-ttu-id="ee3c2-121">Open the record that you want to share.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-121">Open the record that you want to share.</span></span>

    <span data-ttu-id="ee3c2-122">The app is designed to display card type pages from [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ee3c2-122">The app is designed to display card type pages from [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="ee3c2-123">So open a page that displays a single record, like an item, customer, or sales order.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-123">So open a page that displays a single record, like an item, customer, or sales order.</span></span> <span data-ttu-id="ee3c2-124">You can't use it for role centres or pages that display several records in a list.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-124">You can't use it for role centers or pages that display several records in a list.</span></span>

3. <span data-ttu-id="ee3c2-125">Copy the entire URL from the browser's address bar.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-125">Copy the entire URL from the browser's address bar.</span></span>

   ![Copy Business Central URL from browser](media/teams-url-v2.png)
4. <span data-ttu-id="ee3c2-127">Go to Teams and start a conversation, which can be chat with a person, group of persons, or a team channel.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-127">Go to Teams and start a conversation, which can be chat with a person, group of persons, or a team channel.</span></span>

    <!--Teams imposes a few limitations here eg. you cannot unfurl a link during a Voice/Video call :/ We should probably only mention this in a Troubleshooting section (and i hope it will also be fixed soon)-->
5. <span data-ttu-id="ee3c2-128">Paste the URL in the message box where you compose a message.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-128">Paste the URL in the message box where you compose a message.</span></span>

   ![Paste Business Central URL in Teams](media/teams-paste-url-v2.png)
6. <span data-ttu-id="ee3c2-130">The first time you paste a link into a conversation, you'll be asked to sign in to [!INCLUDE [prod_short](includes/prod_short.md)] and give consent for the app to retrieve data.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-130">The first time you paste a link into a conversation, you'll be asked to sign in to [!INCLUDE [prod_short](includes/prod_short.md)] and give consent for the app to retrieve data.</span></span> <span data-ttu-id="ee3c2-131">Just follow the on-screen instructions.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-131">Just follow the on-screen instructions.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ee3c2-132">You'll only have to do this step once.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-132">You'll only have to do this step once.</span></span>

7. <span data-ttu-id="ee3c2-133">Wait a moment while a card is generated in the message box.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-133">Wait a moment while a card is generated in the message box.</span></span>

8. <span data-ttu-id="ee3c2-134">When the card appears, review the contents of the card carefully for any sensitive information before sending the message.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-134">When the card appears, review the contents of the card carefully for any sensitive information before sending the message.</span></span> <span data-ttu-id="ee3c2-135">This step is important because once you send the message, everyone in the conversation can see the card.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-135">This step is important because once you send the message, everyone in the conversation can see the card.</span></span>

9. <span data-ttu-id="ee3c2-136">If the card looks good, select **Send** to submit it to the conversation.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-136">If the card looks good, select **Send** to submit it to the conversation.</span></span>

    > [!TIP]
    > <span data-ttu-id="ee3c2-137">After the card appears, and before you select **Send**, you can delete the pasted URL if you like.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-137">After the card appears, and before you select **Send**, you can delete the pasted URL if you like.</span></span>

10. <span data-ttu-id="ee3c2-138">To view more details or make changes to the record shown in the card, select **Details**.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-138">To view more details or make changes to the record shown in the card, select **Details**.</span></span> <span data-ttu-id="ee3c2-139">For more information, see the next section.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-139">For more information, see the next section.</span></span>

## <a name="view-card-details"></a><span data-ttu-id="ee3c2-140">View card details</span><span class="sxs-lookup"><span data-stu-id="ee3c2-140">View card details</span></span>

<span data-ttu-id="ee3c2-141">Once a card's been sent to a conversation, all participants with the [proper permissions](admin-teams-integration.md#permissions) can select **Details** to open a window that displays more information about the record&mdash;and possibly make changes to the record.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-141">Once a card's been sent to a conversation, all participants with the [proper permissions](admin-teams-integration.md#permissions) can select **Details** to open a window that displays more information about the record&mdash;and possibly make changes to the record.</span></span> <span data-ttu-id="ee3c2-142">It doesn't matter if you're the one sending the card or the one receiving the card.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-142">It doesn't matter if you're the one sending the card or the one receiving the card.</span></span> <span data-ttu-id="ee3c2-143">The **Details** feature is especially useful to recipients, because it quickly provides them with concise, targeted information about the record, as opposed to having to scan the full record.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-143">The **Details** feature is especially useful to recipients, because it quickly provides them with concise, targeted information about the record, as opposed to having to scan the full record.</span></span>

<span data-ttu-id="ee3c2-144">The details window is similar to what you'd see in [!INCLUDE [prod_short](includes/prod_short.md)] the record.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-144">The details window is similar to what you'd see in [!INCLUDE [prod_short](includes/prod_short.md)] the record.</span></span> <span data-ttu-id="ee3c2-145">But it's slightly trimmed for Teams.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-145">But it's slightly trimmed for Teams.</span></span> <span data-ttu-id="ee3c2-146">When you're finished viewing and making changes, close the window to return to the Teams conversation.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-146">When you're finished viewing and making changes, close the window to return to the Teams conversation.</span></span>

<span data-ttu-id="ee3c2-147">Here are a couple things to keep in mind when working with the card details:</span><span class="sxs-lookup"><span data-stu-id="ee3c2-147">Here are a couple things to keep in mind when working with the card details:</span></span>

- <span data-ttu-id="ee3c2-148">To open the card details, users must have permission on the page and its data in [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ee3c2-148">To open the card details, users must have permission on the page and its data in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span>
- <span data-ttu-id="ee3c2-149">Cards in Teams chats aren't automatically updated to changes.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-149">Cards in Teams chats aren't automatically updated to changes.</span></span> <span data-ttu-id="ee3c2-150">Any changes you save to a record in the details window are saved in [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ee3c2-150">Any changes you save to a record in the details window are saved in [!INCLUDE [prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="ee3c2-151">But the card in Teams won't show the changes in the conversion, until you paste the link again.</span><span class="sxs-lookup"><span data-stu-id="ee3c2-151">But the card in Teams won't show the changes in the conversion, until you paste the link again.</span></span>

<span data-ttu-id="ee3c2-152">To learn more about working with cards and card details, see [Teams FAQ](teams-faq.md).</span><span class="sxs-lookup"><span data-stu-id="ee3c2-152">To learn more about working with cards and card details, see [Teams FAQ](teams-faq.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="ee3c2-153">See Also</span><span class="sxs-lookup"><span data-stu-id="ee3c2-153">See Also</span></span>

[<span data-ttu-id="ee3c2-154">Business Central and Microsoft Teams Integration Overview</span><span class="sxs-lookup"><span data-stu-id="ee3c2-154">Business Central and Microsoft Teams Integration Overview</span></span>](across-teams-overview.md)  
<span data-ttu-id="ee3c2-155">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span><span class="sxs-lookup"><span data-stu-id="ee3c2-155">[Install the [!INCLUDE [prod_short](includes/prod_short.md)] App for Microsoft Teams](across-install-app-for-teams.md)</span></span>  
[<span data-ttu-id="ee3c2-156">Teams FAQ</span><span class="sxs-lookup"><span data-stu-id="ee3c2-156">Teams FAQ</span></span>](teams-faq.md)  
[<span data-ttu-id="ee3c2-157">Troubleshooting Teams</span><span class="sxs-lookup"><span data-stu-id="ee3c2-157">Troubleshooting Teams</span></span>](admin-teams-troubleshooting.md)  
[<span data-ttu-id="ee3c2-158">Developing for Teams Integration</span><span class="sxs-lookup"><span data-stu-id="ee3c2-158">Developing for Teams Integration</span></span>](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  
