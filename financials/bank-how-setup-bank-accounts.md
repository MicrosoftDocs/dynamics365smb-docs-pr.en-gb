---
title: Set Up Bank Accounts| Microsoft Docs
description: You can reconcile bank accounts in Financials with statements from the bank.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Yodlee, feed, stream
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: f46e95e24ef39a93bc93cfda1b9c575b07273566
ms.contentlocale: en-gb
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-set-up-bank-accounts"></a><span data-ttu-id="029c4-103">How to: Set Up Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="029c4-103">How to: Set Up Bank Accounts</span></span>
<span data-ttu-id="029c4-104">You use bank accounts in the [!INCLUDE[d365fin](includes/d365fin_md.md)] to keep track of your banking transactions.</span><span class="sxs-lookup"><span data-stu-id="029c4-104">You use bank accounts in the [!INCLUDE[d365fin](includes/d365fin_md.md)] to keep track of your banking transactions.</span></span> <span data-ttu-id="029c4-105">Accounts can be denominated in your local currency or in a foreign currency.</span><span class="sxs-lookup"><span data-stu-id="029c4-105">Accounts can be denominated in your local currency or in a foreign currency.</span></span> <span data-ttu-id="029c4-106">After you have set up bank accounts, you can also use the cheque printing option.</span><span class="sxs-lookup"><span data-stu-id="029c4-106">After you have set up bank accounts, you can also use the check printing option.</span></span>

## <a name="to-set-up-bank-accounts"></a><span data-ttu-id="029c4-107">To set up bank accounts</span><span class="sxs-lookup"><span data-stu-id="029c4-107">To set up bank accounts</span></span>
1. <span data-ttu-id="029c4-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="029c4-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="029c4-109">In the **Bank Accounts** window, choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="029c4-109">In the **Bank Accounts** window, choose the **New** action.</span></span>
3. <span data-ttu-id="029c4-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="029c4-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a><span data-ttu-id="029c4-111">To set up your bank account for import or export of bank files</span><span class="sxs-lookup"><span data-stu-id="029c4-111">To set up your bank account for import or export of bank files</span></span>
<span data-ttu-id="029c4-112">Fields on the **Transfer** FastTab in the **Bank Account Card** window are related to import and export of bank feeds and files.</span><span class="sxs-lookup"><span data-stu-id="029c4-112">Fields on the **Transfer** FastTab in the **Bank Account Card** window are related to import and export of bank feeds and files.</span></span> <span data-ttu-id="029c4-113">For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) and [How to: Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="029c4-113">For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) and [How to: Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

1. <span data-ttu-id="029c4-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="029c4-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="029c4-115">Open the card for a bank account that you will export or import bank files for.</span><span class="sxs-lookup"><span data-stu-id="029c4-115">Open the card for a bank account that you will export or import bank files for.</span></span>
3. <span data-ttu-id="029c4-116">On the **Transfer** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="029c4-116">On the **Transfer** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="029c4-117">Different file export services and their formats require different setup values in the **Bank Account Card** window.</span><span class="sxs-lookup"><span data-stu-id="029c4-117">Different file export services and their formats require different setup values in the **Bank Account Card** window.</span></span> <span data-ttu-id="029c4-118">You will be informed about wrong or missing setup values as you try to export the file.</span><span class="sxs-lookup"><span data-stu-id="029c4-118">You will be informed about wrong or missing setup values as you try to export the file.</span></span> <span data-ttu-id="029c4-119">So read the short descriptions of the fields carefully or refer to the related procedure topics.</span><span class="sxs-lookup"><span data-stu-id="029c4-119">So read the short descriptions of the fields carefully or refer to the related procedure topics.</span></span> <span data-ttu-id="029c4-120">For example, exporting a payment file for North American electronic funds transfer (EFT) requires that both the **Last Remittance Advice No.**</span><span class="sxs-lookup"><span data-stu-id="029c4-120">For example, exporting a payment file for North American electronic funds transfer (EFT) requires that both the **Last Remittance Advice No.**</span></span> <span data-ttu-id="029c4-121">field and the **Transit No.**</span><span class="sxs-lookup"><span data-stu-id="029c4-121">field and the **Transit No.**</span></span> <span data-ttu-id="029c4-122">field are filled in.</span><span class="sxs-lookup"><span data-stu-id="029c4-122">field are filled in.</span></span> <span data-ttu-id="029c4-123">For more information, see [How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="029c4-123">For more information, see [How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md).</span></span>

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a><span data-ttu-id="029c4-124">To set up vendor bank accounts for export of bank files</span><span class="sxs-lookup"><span data-stu-id="029c4-124">To set up vendor bank accounts for export of bank files</span></span>
<span data-ttu-id="029c4-125">Fields on the **Transfer** FastTab in the **Vendor Bank Account Card** window are related to export of bank feeds and files.</span><span class="sxs-lookup"><span data-stu-id="029c4-125">Fields on the **Transfer** FastTab in the **Vendor Bank Account Card** window are related to export of bank feeds and files.</span></span> <span data-ttu-id="029c4-126">For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) and [How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="029c4-126">For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md) and [How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md).</span></span>

1. <span data-ttu-id="029c4-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="029c4-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="029c4-128">Open the card for a vendor whose bank account you will export payment bank files to.</span><span class="sxs-lookup"><span data-stu-id="029c4-128">Open the card for a vendor whose bank account you will export payment bank files to.</span></span>
3. <span data-ttu-id="029c4-129">Choose the **Bank Accounts** action.</span><span class="sxs-lookup"><span data-stu-id="029c4-129">Choose the **Bank Accounts** action.</span></span>
3. <span data-ttu-id="029c4-130">In the **Vendor Bank Account Card** window, on the **Transfer** FastTab, fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="029c4-130">In the **Vendor Bank Account Card** window, on the **Transfer** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a><span data-ttu-id="029c4-131">See Also</span><span class="sxs-lookup"><span data-stu-id="029c4-131">See Also</span></span>
[<span data-ttu-id="029c4-132">Setting Up Banking</span><span class="sxs-lookup"><span data-stu-id="029c4-132">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="029c4-133">Managing Bank Accounts</span><span class="sxs-lookup"><span data-stu-id="029c4-133">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
<span data-ttu-id="029c4-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="029c4-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

