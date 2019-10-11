---
title: Payment Reconciliation With the Envestnet Yodlee Bank Feeds Extension | Microsoft Docs
description: Describes the Envestnet Yodlee Bank Feeds extension, which links to bank accounts so you can and quickly reconcile payments.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: d79ef7c076ec3a529aeb0c679b8b61658ef65af5
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2019
ms.locfileid: "2315355"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a><span data-ttu-id="7b0fc-103">The Envestnet Yodlee Bank Feeds Extension</span><span class="sxs-lookup"><span data-stu-id="7b0fc-103">The Envestnet Yodlee Bank Feeds Extension</span></span>
<span data-ttu-id="7b0fc-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span></span> <span data-ttu-id="7b0fc-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span></span>

<span data-ttu-id="7b0fc-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>

> [!NOTE]
> <span data-ttu-id="7b0fc-107">This functionality is only supported in the online version of Business Central.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-107">This functionality is only supported in the online version of Business Central.</span></span> <span data-ttu-id="7b0fc-108">To use this functionality on-premise, you must obtain a cobrand account from Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-108">To use this functionality on-premise, you must obtain a cobrand account from Envestnet Yodlee.</span></span><br /><br />

> [!IMPORTANT]
> <span data-ttu-id="7b0fc-109">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7b0fc-109">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="7b0fc-110">We are looking into the possibility of offering this feature again in the future.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-110">We are looking into the possibility of offering this feature again in the future.</span></span>

<span data-ttu-id="7b0fc-111">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span><span class="sxs-lookup"><span data-stu-id="7b0fc-111">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span></span>

* <span data-ttu-id="7b0fc-112">Removes the need for manual entry.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-112">Removes the need for manual entry.</span></span>
* <span data-ttu-id="7b0fc-113">Improves efficiency and accuracy when doing payment reconciliation.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-113">Improves efficiency and accuracy when doing payment reconciliation.</span></span>
* <span data-ttu-id="7b0fc-114">Supports a large number of banks.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-114">Supports a large number of banks.</span></span>
* <span data-ttu-id="7b0fc-115">Allows up-to-date information about bank transactions from within [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="7b0fc-115">Allows up-to-date information about bank transactions from within [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
* <span data-ttu-id="7b0fc-116">Supports manual as well as automatic bank feeds.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-116">Supports manual as well as automatic bank feeds.</span></span>
* <span data-ttu-id="7b0fc-117">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span><span class="sxs-lookup"><span data-stu-id="7b0fc-117">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span></span>

<span data-ttu-id="7b0fc-118">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="7b0fc-118">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="7b0fc-119">See Also</span><span class="sxs-lookup"><span data-stu-id="7b0fc-119">See Also</span></span>
<span data-ttu-id="7b0fc-120">[Customising [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="7b0fc-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
[<span data-ttu-id="7b0fc-121">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="7b0fc-121">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
<span data-ttu-id="7b0fc-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7b0fc-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
