---
author: edupont04
ms.service: dynamics365-accountant
ms.topic: include
ms.date: 10/02/2020
ms.author: edupont
ms.openlocfilehash: 1b9f60eab5b0bcf812343e82389087ac5535301a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749787"
---
<span data-ttu-id="6cb68-101">Before you can set up email logging, you must prepare your Exchange Online with [public folders](/exchange/collaboration/public-folders/public-folders?view=exchserver-2019&preserve-view=true ).</span><span class="sxs-lookup"><span data-stu-id="6cb68-101">Before you can set up email logging, you must prepare your Exchange Online with [public folders](/exchange/collaboration/public-folders/public-folders?view=exchserver-2019&preserve-view=true ).</span></span> <span data-ttu-id="6cb68-102">You can do this in the [Exchange admin centre](/Exchange/architecture/client-access/exchange-admin-center?view=exchserver-2019&preserve-view=true ), or you can use the [Exchange Management Shell](/powershell/exchange/exchange-management-shell?view=exchange-ps&preserve-view=true ).</span><span class="sxs-lookup"><span data-stu-id="6cb68-102">You can do this in the [Exchange admin center](/Exchange/architecture/client-access/exchange-admin-center?view=exchserver-2019&preserve-view=true ), or you can use the [Exchange Management Shell](/powershell/exchange/exchange-management-shell?view=exchange-ps&preserve-view=true ).</span></span>  

> [!TIP]
> <span data-ttu-id="6cb68-103">If you want to use the [Exchange Management Shell](/powershell/exchange/exchange-management-shell?view=exchange-ps&preserve-view=true ), you can find inspiration for how to set up your script in a sample script that we published to [the BCTech repo](https://github.com/microsoft/BCTech/tree/master/samples/EmailLogging).</span><span class="sxs-lookup"><span data-stu-id="6cb68-103">If you want to use the [Exchange Management Shell](/powershell/exchange/exchange-management-shell?view=exchange-ps&preserve-view=true ), you can find inspiration for how to set up your script in a sample script that we published to [the BCTech repo](https://github.com/microsoft/BCTech/tree/master/samples/EmailLogging).</span></span>

<span data-ttu-id="6cb68-104">The following list describes the main steps with links to learn more.</span><span class="sxs-lookup"><span data-stu-id="6cb68-104">The following list describes the main steps with links to learn more.</span></span>  

- <span data-ttu-id="6cb68-105">Create an admin role for public folders based on the information in the following table:</span><span class="sxs-lookup"><span data-stu-id="6cb68-105">Create an admin role for public folders based on the information in the following table:</span></span>

  |<span data-ttu-id="6cb68-106">Property</span><span class="sxs-lookup"><span data-stu-id="6cb68-106">Property</span></span>        |<span data-ttu-id="6cb68-107">Value</span><span class="sxs-lookup"><span data-stu-id="6cb68-107">Value</span></span>                     |
  |----------------|--------------------------|
  |<span data-ttu-id="6cb68-108">Name</span><span class="sxs-lookup"><span data-stu-id="6cb68-108">Name</span></span>            |<span data-ttu-id="6cb68-109">Public Folders Management</span><span class="sxs-lookup"><span data-stu-id="6cb68-109">Public Folders Management</span></span> |
  |<span data-ttu-id="6cb68-110">Selected roles</span><span class="sxs-lookup"><span data-stu-id="6cb68-110">Selected roles</span></span>  |<span data-ttu-id="6cb68-111">Public Folders</span><span class="sxs-lookup"><span data-stu-id="6cb68-111">Public Folders</span></span>            |
  |<span data-ttu-id="6cb68-112">Selected members</span><span class="sxs-lookup"><span data-stu-id="6cb68-112">Selected members</span></span>|<span data-ttu-id="6cb68-113">The email of the user account that Business Central will use to run the email logging job</span><span class="sxs-lookup"><span data-stu-id="6cb68-113">The email of the user account that Business Central will use to run the email logging job</span></span>|

  <span data-ttu-id="6cb68-114">For more information, see [Manage role groups](/exchange/permissions/role-groups?view=exchserver-2019&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6cb68-114">For more information, see [Manage role groups](/exchange/permissions/role-groups?view=exchserver-2019&preserve-view=true).</span></span>

- <span data-ttu-id="6cb68-115">Create a new public folder mailbox based on the information in the following table:</span><span class="sxs-lookup"><span data-stu-id="6cb68-115">Create a new public folder mailbox based on the information in the following table:</span></span>

  |<span data-ttu-id="6cb68-116">Property</span><span class="sxs-lookup"><span data-stu-id="6cb68-116">Property</span></span>        |<span data-ttu-id="6cb68-117">Value</span><span class="sxs-lookup"><span data-stu-id="6cb68-117">Value</span></span>                     |
  |----------------|--------------------------|
  |<span data-ttu-id="6cb68-118">Name</span><span class="sxs-lookup"><span data-stu-id="6cb68-118">Name</span></span>            |<span data-ttu-id="6cb68-119">Public MailBox</span><span class="sxs-lookup"><span data-stu-id="6cb68-119">Public MailBox</span></span>            |

  <span data-ttu-id="6cb68-120">For more information, see [Create a public folder mailbox in Exchange Server](/exchange/collaboration/public-folders/create-public-folder-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="6cb68-120">For more information, see [Create a public folder mailbox in Exchange Server](/exchange/collaboration/public-folders/create-public-folder-mailboxes).</span></span>  

- <span data-ttu-id="6cb68-121">Create new public folders</span><span class="sxs-lookup"><span data-stu-id="6cb68-121">Create new public folders</span></span>

  - <span data-ttu-id="6cb68-122">Create a new public folder with the name *Email Logging* in the root so that the full path to the folder becomes ```\Email Logging\```</span><span class="sxs-lookup"><span data-stu-id="6cb68-122">Create a new public folder with the name *Email Logging* in the root so that the full path to the folder becomes ```\Email Logging\```</span></span>
  - <span data-ttu-id="6cb68-123">Create two subfolders so that the the result is the following full paths to the folders:</span><span class="sxs-lookup"><span data-stu-id="6cb68-123">Create two subfolders so that the the result is the following full paths to the folders:</span></span>
    - ```\Email Logging\Queue\```
    - ```\Email Logging\Storage\```

  <span data-ttu-id="6cb68-124">For more information, see [Create a public folder](/exchange/collaboration/public-folders/create-public-folders?view=exchserver-2019&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6cb68-124">For more information, see [Create a public folder](/exchange/collaboration/public-folders/create-public-folders?view=exchserver-2019&preserve-view=true).</span></span>

- <span data-ttu-id="6cb68-125">Mail-enable the *Queue* public folder</span><span class="sxs-lookup"><span data-stu-id="6cb68-125">Mail-enable the *Queue* public folder</span></span>

  <span data-ttu-id="6cb68-126">For more information, see [Mail-enable or mail-disable a public folder](/exchange/collaboration/public-folders/mail-enable-or-disable?view=exchserver-2019&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6cb68-126">For more information, see [Mail-enable or mail-disable a public folder](/exchange/collaboration/public-folders/mail-enable-or-disable?view=exchserver-2019&preserve-view=true)</span></span>

- <span data-ttu-id="6cb68-127">Mail-enable sending emails to the *Queue* public folder using Outlook or the Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="6cb68-127">Mail-enable sending emails to the *Queue* public folder using Outlook or the Exchange Management Shell</span></span>

  <span data-ttu-id="6cb68-128">For more information, see [Allow anonymous users to send email to a mail-enabled public folder](/exchange/collaboration/public-folders/mail-enable-or-disable#allow-anonymous-users-to-send-email-to-a-mail-enabled-public-folder?view=exchserver-2019&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="6cb68-128">For more information, see [Allow anonymous users to send email to a mail-enabled public folder](/exchange/collaboration/public-folders/mail-enable-or-disable#allow-anonymous-users-to-send-email-to-a-mail-enabled-public-folder?view=exchserver-2019&preserve-view=true)</span></span>

- <span data-ttu-id="6cb68-129">Set the email logging user as an owner of both public folders, *Queue* and *Storage* public folders  using Outlook or the Exchange Management Shell based on the information in the following table:</span><span class="sxs-lookup"><span data-stu-id="6cb68-129">Set the email logging user as an owner of both public folders, *Queue* and *Storage* public folders  using Outlook or the Exchange Management Shell based on the information in the following table:</span></span>

  |<span data-ttu-id="6cb68-130">Property</span><span class="sxs-lookup"><span data-stu-id="6cb68-130">Property</span></span>        |<span data-ttu-id="6cb68-131">Value</span><span class="sxs-lookup"><span data-stu-id="6cb68-131">Value</span></span>                     |
  |----------------|--------------------------|
  |<span data-ttu-id="6cb68-132">User</span><span class="sxs-lookup"><span data-stu-id="6cb68-132">User</span></span>            |<span data-ttu-id="6cb68-133">The email of the user account that Business Central will use to run the email logging job</span><span class="sxs-lookup"><span data-stu-id="6cb68-133">The email of the user account that Business Central will use to run the email logging job</span></span>|
  |<span data-ttu-id="6cb68-134">Permission level</span><span class="sxs-lookup"><span data-stu-id="6cb68-134">Permission level</span></span>|<span data-ttu-id="6cb68-135">Owner</span><span class="sxs-lookup"><span data-stu-id="6cb68-135">Owner</span></span>                     |

  <span data-ttu-id="6cb68-136">For more information, see [Assign permissions to the public folder](/exchange/collaboration-exo/public-folders/set-up-public-folders#step-3-assign-permissions-to-the-public-folder).</span><span class="sxs-lookup"><span data-stu-id="6cb68-136">For more information, see [Assign permissions to the public folder](/exchange/collaboration-exo/public-folders/set-up-public-folders#step-3-assign-permissions-to-the-public-folder).</span></span>

- <span data-ttu-id="6cb68-137">Create two mail flow rules based on the information in the following table</span><span class="sxs-lookup"><span data-stu-id="6cb68-137">Create two mail flow rules based on the information in the following table</span></span>

  |<span data-ttu-id="6cb68-138">Purpose</span><span class="sxs-lookup"><span data-stu-id="6cb68-138">Purpose</span></span>  |<span data-ttu-id="6cb68-139">Name</span><span class="sxs-lookup"><span data-stu-id="6cb68-139">Name</span></span> |<span data-ttu-id="6cb68-140">Conditions</span><span class="sxs-lookup"><span data-stu-id="6cb68-140">Conditions</span></span>                        |<span data-ttu-id="6cb68-141">Action</span><span class="sxs-lookup"><span data-stu-id="6cb68-141">Action</span></span>                                       |
  |---------|-----|----------------------------------|---------------------------------------------|
  |<span data-ttu-id="6cb68-142">A rule for incoming email</span><span class="sxs-lookup"><span data-stu-id="6cb68-142">A rule for incoming email</span></span> |<span data-ttu-id="6cb68-143">Log Email Sent to This Organisation</span><span class="sxs-lookup"><span data-stu-id="6cb68-143">Log Email Sent to This Organization</span></span>|<span data-ttu-id="6cb68-144">*The sender* is located *Outside the organisation*, and *the recipient* is located *Inside the organisation*</span><span class="sxs-lookup"><span data-stu-id="6cb68-144">*The sender* is located *Outside the organization*, and *the recipient* is located *Inside the organization*</span></span>|<span data-ttu-id="6cb68-145">BCC the email account that is specified for the *Queue* public folder</span><span class="sxs-lookup"><span data-stu-id="6cb68-145">BCC the email account that is specified for the *Queue* public folder</span></span>|
  |<span data-ttu-id="6cb68-146">A rule for outgoing email</span><span class="sxs-lookup"><span data-stu-id="6cb68-146">A rule for outgoing email</span></span> | <span data-ttu-id="6cb68-147">Log Email Sent from This Organisation</span><span class="sxs-lookup"><span data-stu-id="6cb68-147">Log Email Sent from This Organization</span></span> |<span data-ttu-id="6cb68-148">*The sender* is located *Inside the organisation*, and *the recipient* is located *Outside the organisation*</span><span class="sxs-lookup"><span data-stu-id="6cb68-148">*The sender* is located *Inside the organization*, and *the recipient* is located *Outside the organization*</span></span>|<span data-ttu-id="6cb68-149">BCC the email account that is specified for the *Queue* public folder</span><span class="sxs-lookup"><span data-stu-id="6cb68-149">BCC the email account that is specified for the *Queue* public folder</span></span>|
  
  <span data-ttu-id="6cb68-150">For more information, see [Manage mail flow rules in Exchange Online](/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules) and [Mail flow rule actions in Exchange Online](/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions).</span><span class="sxs-lookup"><span data-stu-id="6cb68-150">For more information, see [Manage mail flow rules in Exchange Online](/exchange/security-and-compliance/mail-flow-rules/manage-mail-flow-rules) and [Mail flow rule actions in Exchange Online](/exchange/security-and-compliance/mail-flow-rules/mail-flow-rule-actions).</span></span>

> [!NOTE]
> <span data-ttu-id="6cb68-151">If you make changes in the Exchange Management Shell, the changes become visible in the Exchange admin centre after a delay.</span><span class="sxs-lookup"><span data-stu-id="6cb68-151">If you make changes in the Exchange Management Shell, the changes become visible in the Exchange admin center after a delay.</span></span> <span data-ttu-id="6cb68-152">Also, the changes made in Exchange will be available in [!INCLUDE[prod_short](prod_short.md)] after a delay.</span><span class="sxs-lookup"><span data-stu-id="6cb68-152">Also, the changes made in Exchange will be available in [!INCLUDE[prod_short](prod_short.md)] after a delay.</span></span>
