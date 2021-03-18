---
title: Payment Reconciliation With the Envestnet Yodlee Bank Feeds Extension
description: Describes the Envestnet Yodlee Bank Feeds extension, which links to bank accounts so you can and quickly reconcile payments.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 946958669f4554869e171286927bf498fe62a7ed
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5394031"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a><span data-ttu-id="f8bcb-103">The Envestnet Yodlee Bank Feeds Extension</span><span class="sxs-lookup"><span data-stu-id="f8bcb-103">The Envestnet Yodlee Bank Feeds Extension</span></span>

<span data-ttu-id="f8bcb-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span></span> <span data-ttu-id="f8bcb-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span></span>

<span data-ttu-id="f8bcb-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>

> [!NOTE]
> <span data-ttu-id="f8bcb-107">The Envestnet Yodlee Bank Feeds service is only supported in the online version of Business Central.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-107">The Envestnet Yodlee Bank Feeds service is only supported in the online version of Business Central.</span></span> <span data-ttu-id="f8bcb-108">To use this functionality on-premises, you must obtain a cobrand account from Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-108">To use this functionality on-premises, you must obtain a cobrand account from Envestnet Yodlee.</span></span><br /><br />
> <span data-ttu-id="f8bcb-109">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-109">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>
> <span data-ttu-id="f8bcb-110">Only banks residing in these countries are supported, even though banks from other countries may appear in the Envestnet Yodlee Bank Feeds bank selection window in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="f8bcb-110">Only banks residing in these countries are supported, even though banks from other countries may appear in the Envestnet Yodlee Bank Feeds bank selection window in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f8bcb-111">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="f8bcb-111">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="f8bcb-112">We are looking into the possibility of offering this feature again in the future.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-112">We are looking into the possibility of offering this feature again in the future.</span></span>

<span data-ttu-id="f8bcb-113">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span><span class="sxs-lookup"><span data-stu-id="f8bcb-113">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span></span>

* <span data-ttu-id="f8bcb-114">Removes the need for manual entry.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-114">Removes the need for manual entry.</span></span>
* <span data-ttu-id="f8bcb-115">Improves efficiency and accuracy when doing payment reconciliation.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-115">Improves efficiency and accuracy when doing payment reconciliation.</span></span>
* <span data-ttu-id="f8bcb-116">Supports a large number of banks.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-116">Supports a large number of banks.</span></span>
* <span data-ttu-id="f8bcb-117">Allows up-to-date information about bank transactions from within [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="f8bcb-117">Allows up-to-date information about bank transactions from within [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
* <span data-ttu-id="f8bcb-118">Supports manual as well as automatic bank feeds.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-118">Supports manual as well as automatic bank feeds.</span></span>
* <span data-ttu-id="f8bcb-119">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-119">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span></span>

## <a name="available-bank-feeds"></a><span data-ttu-id="f8bcb-120">Available Bank Feeds</span><span class="sxs-lookup"><span data-stu-id="f8bcb-120">Available Bank Feeds</span></span>
<span data-ttu-id="f8bcb-121">You can check whether a bank is supported by setting up and connecting to the Envestnet Yodlee Bank Feeds service.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-121">You can check whether a bank is supported by setting up and connecting to the Envestnet Yodlee Bank Feeds service.</span></span> <span data-ttu-id="f8bcb-122">The bank will appear on the list if it is supported by Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-122">The bank will appear on the list if it is supported by Envestnet Yodlee.</span></span>

<span data-ttu-id="f8bcb-123">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="f8bcb-123">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="f8bcb-124">See Also</span><span class="sxs-lookup"><span data-stu-id="f8bcb-124">See Also</span></span>
<span data-ttu-id="f8bcb-125">[Customising [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="f8bcb-125">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)  </span></span>  
[<span data-ttu-id="f8bcb-126">Applying Payments Automatically and Reconciling Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="f8bcb-126">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
<span data-ttu-id="f8bcb-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f8bcb-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]