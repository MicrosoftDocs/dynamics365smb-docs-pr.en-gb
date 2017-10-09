---
title: Design Details - Inventory Costing | Microsoft Docs
description: This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 38a37a6fb1e3b8a58fd28b3d8e678b93a110683b
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="d1c3f-103">Design Details: Inventory Costing</span><span class="sxs-lookup"><span data-stu-id="d1c3f-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="d1c3f-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d1c3f-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="d1c3f-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span><span class="sxs-lookup"><span data-stu-id="d1c3f-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="d1c3f-106">In This Section</span><span class="sxs-lookup"><span data-stu-id="d1c3f-106">In This Section</span></span>  
[<span data-ttu-id="d1c3f-107">Design Details: Costing Methods</span><span class="sxs-lookup"><span data-stu-id="d1c3f-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="d1c3f-108">Design Details: Item Application</span><span class="sxs-lookup"><span data-stu-id="d1c3f-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="d1c3f-109">Design Details: Cost Adjustment</span><span class="sxs-lookup"><span data-stu-id="d1c3f-109">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="d1c3f-110">Design Details: Expected Cost Posting</span><span class="sxs-lookup"><span data-stu-id="d1c3f-110">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="d1c3f-111">Design Details: Average Cost</span><span class="sxs-lookup"><span data-stu-id="d1c3f-111">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="d1c3f-112">Design Details: Variance</span><span class="sxs-lookup"><span data-stu-id="d1c3f-112">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="d1c3f-113">Design Details: Rounding</span><span class="sxs-lookup"><span data-stu-id="d1c3f-113">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="d1c3f-114">Design Details: Cost Components</span><span class="sxs-lookup"><span data-stu-id="d1c3f-114">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="d1c3f-115">Design Details: Inventory Periods</span><span class="sxs-lookup"><span data-stu-id="d1c3f-115">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="d1c3f-116">Design Details: Inventory Posting</span><span class="sxs-lookup"><span data-stu-id="d1c3f-116">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="d1c3f-117">Design Details: Production Order Posting</span><span class="sxs-lookup"><span data-stu-id="d1c3f-117">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="d1c3f-118">Design Details: Assembly Order Posting</span><span class="sxs-lookup"><span data-stu-id="d1c3f-118">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="d1c3f-119">Design Details: Reconciliation with the General Ledger</span><span class="sxs-lookup"><span data-stu-id="d1c3f-119">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="d1c3f-120">Design Details: Accounts in the General Ledger</span><span class="sxs-lookup"><span data-stu-id="d1c3f-120">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="d1c3f-121">Design Details: Revaluation</span><span class="sxs-lookup"><span data-stu-id="d1c3f-121">Design Details: Revaluation</span></span>](design-details-revaluation.md)

