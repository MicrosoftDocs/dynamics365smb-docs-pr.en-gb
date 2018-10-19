---
title: Import Payroll Transactions| Microsoft Docs
description: To manage salary, you import and post financial transactions from your payroll provider to the general ledger, using a payroll extension such as Ceridian or Quickbooks.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Ceridian, Quickbooks, salary
ms.date: 10/01/2018
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: fbe6a61cb48a4c26ff3fc15eb0dd61c002a59092
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="import-payroll-transactions"></a><span data-ttu-id="e75ab-103">Import Payroll Transactions</span><span class="sxs-lookup"><span data-stu-id="e75ab-103">Import Payroll Transactions</span></span>
<span data-ttu-id="e75ab-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span><span class="sxs-lookup"><span data-stu-id="e75ab-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="e75ab-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span><span class="sxs-lookup"><span data-stu-id="e75ab-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="e75ab-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span><span class="sxs-lookup"><span data-stu-id="e75ab-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="e75ab-107">Lastly, you post the payroll transactions according to the account mapping.</span><span class="sxs-lookup"><span data-stu-id="e75ab-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

> [!NOTE]  
>   <span data-ttu-id="e75ab-108">To use this functionality, an extension for payroll import must be installed and enabled.</span><span class="sxs-lookup"><span data-stu-id="e75ab-108">To use this functionality, an extension for payroll import must be installed and enabled.</span></span> <span data-ttu-id="e75ab-109">The Ceridian Payroll and the Quickbooks Payroll File Import extensions are pre-installed in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e75ab-109">The Ceridian Payroll and the Quickbooks Payroll File Import extensions are pre-installed in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="e75ab-110">For more information, see [Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="e75ab-110">For more information, see [Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md).</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="e75ab-111">To import a payroll file</span><span class="sxs-lookup"><span data-stu-id="e75ab-111">To import a payroll file</span></span>
1. <span data-ttu-id="e75ab-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e75ab-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="e75ab-113">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span><span class="sxs-lookup"><span data-stu-id="e75ab-113">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span> <span data-ttu-id="e75ab-114">An assisted setup guide opens.</span><span class="sxs-lookup"><span data-stu-id="e75ab-114">An assisted setup guide opens.</span></span>
3. <span data-ttu-id="e75ab-115">Follow the steps in the **Import Payroll Transactions** window.</span><span class="sxs-lookup"><span data-stu-id="e75ab-115">Follow the steps in the **Import Payroll Transactions** window.</span></span>

    > [!TIP]  
    >   <span data-ttu-id="e75ab-116">In the step about mapping the external payroll records to your G/L accounts, the mappings that you make will be remembered next time the same records are imported.</span><span class="sxs-lookup"><span data-stu-id="e75ab-116">In the step about mapping the external payroll records to your G/L accounts, the mappings that you make will be remembered next time the same records are imported.</span></span> <span data-ttu-id="e75ab-117">This will save you time as you do not have to manually fill in the **Account No.** field in the general journal every time you have imported recurring payroll transactions.</span><span class="sxs-lookup"><span data-stu-id="e75ab-117">This will save you time as you do not have to manually fill in the **Account No.** field in the general journal every time you have imported recurring payroll transactions.</span></span>   

    <span data-ttu-id="e75ab-118">When you choose the **OK** button in the assisted setup guide, the **General Journal** window is filled with lines representing the transactions that the payroll file contains and with the relevant accounts prefilled in the **G/L Account** fields according to mappings you made in the guide.</span><span class="sxs-lookup"><span data-stu-id="e75ab-118">When you choose the **OK** button in the assisted setup guide, the **General Journal** window is filled with lines representing the transactions that the payroll file contains and with the relevant accounts prefilled in the **G/L Account** fields according to mappings you made in the guide.</span></span>
4. <span data-ttu-id="e75ab-119">Edit or post the journal lines as for any other general ledger transactions.</span><span class="sxs-lookup"><span data-stu-id="e75ab-119">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="e75ab-120">For more information, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="e75ab-120">For more information, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="e75ab-121">See Also</span><span class="sxs-lookup"><span data-stu-id="e75ab-121">See Also</span></span>
[<span data-ttu-id="e75ab-122">Finance</span><span class="sxs-lookup"><span data-stu-id="e75ab-122">Finance</span></span>](finance.md)  
<span data-ttu-id="e75ab-123">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e75ab-123">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="e75ab-124">Working with General Journals</span><span class="sxs-lookup"><span data-stu-id="e75ab-124">Working with General Journals</span></span>](ui-work-general-journals.md)  

