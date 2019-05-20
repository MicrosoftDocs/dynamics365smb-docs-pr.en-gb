---
title: Set Up Service Contracts | Microsoft Docs
description: Learn how to set up service contracts.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, cost, service order
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 697de344a439bb0a91b1f74acc3d8b93d2f6d5d3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/29/2019
ms.locfileid: "1252143"
---
# <a name="set-up-service-contracts"></a><span data-ttu-id="18ffc-103">Set Up Service Contracts</span><span class="sxs-lookup"><span data-stu-id="18ffc-103">Set Up Service Contracts</span></span>
<span data-ttu-id="18ffc-104">Before you can work with contracts, you must set up the following:</span><span class="sxs-lookup"><span data-stu-id="18ffc-104">Before you can work with contracts, you must set up the following:</span></span> 

* <span data-ttu-id="18ffc-105">**Service contract groups**, which gather service contracts that are related in some way.</span><span class="sxs-lookup"><span data-stu-id="18ffc-105">**Service contract groups**, which gather service contracts that are related in some way.</span></span>
* <span data-ttu-id="18ffc-106">**Service contract account groups**, which are used to group the service contract accounts together for service invoices created for service contracts.</span><span class="sxs-lookup"><span data-stu-id="18ffc-106">**Service contract account groups**, which are used to group the service contract accounts together for service invoices created for service contracts.</span></span> <span data-ttu-id="18ffc-107">You assign these groups to service contracts.</span><span class="sxs-lookup"><span data-stu-id="18ffc-107">You assign these groups to service contracts.</span></span>  
* <span data-ttu-id="18ffc-108">**Contract templates** that define contract layouts of contracts that include the most commonly used service contract details.</span><span class="sxs-lookup"><span data-stu-id="18ffc-108">**Contract templates** that define contract layouts of contracts that include the most commonly used service contract details.</span></span> <span data-ttu-id="18ffc-109">When you create service contract quotes, you can create them by using templates.</span><span class="sxs-lookup"><span data-stu-id="18ffc-109">When you create service contract quotes, you can create them by using templates.</span></span> <span data-ttu-id="18ffc-110">When you create a contract quote, the fields automatically contain the contents of the template fields.</span><span class="sxs-lookup"><span data-stu-id="18ffc-110">When you create a contract quote, the fields automatically contain the contents of the template fields.</span></span>
* <span data-ttu-id="18ffc-111">**Customer templates** that let you create quotes for contacts or potential customers who are not registered as customers in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="18ffc-111">**Customer templates** that let you create quotes for contacts or potential customers who are not registered as customers in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-set-up-a-service-contract-group"></a><span data-ttu-id="18ffc-112">To set up a service contract group</span><span class="sxs-lookup"><span data-stu-id="18ffc-112">To set up a service contract group</span></span>  
1. <span data-ttu-id="18ffc-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contract Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18ffc-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contract Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18ffc-114">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="18ffc-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="18ffc-115">Choose the **Disc. on Contr. Orders Only** check box if you want contract or service discounts to be valid only for contract service orders, such as maintenance.</span><span class="sxs-lookup"><span data-stu-id="18ffc-115">Choose the **Disc. on Contr. Orders Only** check box if you want contract or service discounts to be valid only for contract service orders, such as maintenance.</span></span>  

## <a name="to-set-up-a-service-contract-account-group"></a><span data-ttu-id="18ffc-116">To set up a service contract account group</span><span class="sxs-lookup"><span data-stu-id="18ffc-116">To set up a service contract account group</span></span>  
1. <span data-ttu-id="18ffc-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Serv. Contract Account Groups**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18ffc-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Serv. Contract Account Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18ffc-118">Create a new service contract account group.</span><span class="sxs-lookup"><span data-stu-id="18ffc-118">Create a new service contract account group.</span></span>   
3. <span data-ttu-id="18ffc-119">Fill in the **Code** and **Description** fields.</span><span class="sxs-lookup"><span data-stu-id="18ffc-119">Fill in the **Code** and **Description** fields.</span></span> <span data-ttu-id="18ffc-120">These fields describe the service account group.</span><span class="sxs-lookup"><span data-stu-id="18ffc-120">These fields describe the service account group.</span></span>  
4. <span data-ttu-id="18ffc-121">Fill in the **Non-Prepaid Contract Acc.** field, choose general ledger account number for the non-prepaid account.</span><span class="sxs-lookup"><span data-stu-id="18ffc-121">Fill in the **Non-Prepaid Contract Acc.** field, choose general ledger account number for the non-prepaid account.</span></span>  
5. <span data-ttu-id="18ffc-122">In the **Prepaid Contract Acc.** field, choose the general ledger account number for the prepaid account.</span><span class="sxs-lookup"><span data-stu-id="18ffc-122">In the **Prepaid Contract Acc.** field, choose the general ledger account number for the prepaid account.</span></span>  

## <a name="to-set-up-a-contract-template"></a><span data-ttu-id="18ffc-123">To set up a contract template</span><span class="sxs-lookup"><span data-stu-id="18ffc-123">To set up a contract template</span></span>  
1. <span data-ttu-id="18ffc-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contract Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18ffc-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Contract Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18ffc-125">Create a new service contract template.</span><span class="sxs-lookup"><span data-stu-id="18ffc-125">Create a new service contract template.</span></span>  
3. <span data-ttu-id="18ffc-126">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="18ffc-126">In the **No.**</span></span> <span data-ttu-id="18ffc-127">field, enter a number for the contract template.</span><span class="sxs-lookup"><span data-stu-id="18ffc-127">field, enter a number for the contract template.</span></span>  
  
     <span data-ttu-id="18ffc-128">Alternatively, if you have set up number series for contract templates on the **Service Mgt. Setup** page, you can press the Enter key to enter the next available contract template number.</span><span class="sxs-lookup"><span data-stu-id="18ffc-128">Alternatively, if you have set up number series for contract templates on the **Service Mgt. Setup** page, you can press the Enter key to enter the next available contract template number.</span></span> <span data-ttu-id="18ffc-129">Fill in the other fields if appropriate.</span><span class="sxs-lookup"><span data-stu-id="18ffc-129">Fill in the other fields if appropriate.</span></span>  
  
4. <span data-ttu-id="18ffc-130">On the **Invoice** FastTab, fill in the **Serv. Contract Acc. Group Code** field, the **Invoice Period**, and so on.</span><span class="sxs-lookup"><span data-stu-id="18ffc-130">On the **Invoice** FastTab, fill in the **Serv. Contract Acc. Group Code** field, the **Invoice Period**, and so on.</span></span> <span data-ttu-id="18ffc-131">Fill in the other fields if appropriate.</span><span class="sxs-lookup"><span data-stu-id="18ffc-131">Fill in the other fields if appropriate.</span></span>  
5. <span data-ttu-id="18ffc-132">Choose the **Service Discounts** action to add contract discounts.</span><span class="sxs-lookup"><span data-stu-id="18ffc-132">Choose the **Service Discounts** action to add contract discounts.</span></span>  

## <a name="to-set-up-a-customer-template"></a><span data-ttu-id="18ffc-133">To set up a customer template</span><span class="sxs-lookup"><span data-stu-id="18ffc-133">To set up a customer template</span></span>  
1. <span data-ttu-id="18ffc-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Templates**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="18ffc-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customer Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18ffc-135">Create a new customer template card.</span><span class="sxs-lookup"><span data-stu-id="18ffc-135">Create a new customer template card.</span></span>  
3. <span data-ttu-id="18ffc-136">On the **General** FastTab, enter a code and a description for the customer template in the **Code** and **Description** fields respectively.</span><span class="sxs-lookup"><span data-stu-id="18ffc-136">On the **General** FastTab, enter a code and a description for the customer template in the **Code** and **Description** fields respectively.</span></span> 
4. <span data-ttu-id="18ffc-137">To define search criteria, fill in the other fields, such as **Country/Region Code**, **Territory Code**, and **Language Code**.</span><span class="sxs-lookup"><span data-stu-id="18ffc-137">To define search criteria, fill in the other fields, such as **Country/Region Code**, **Territory Code**, and **Language Code**.</span></span>  
5. <span data-ttu-id="18ffc-138">Fill in the **Gen. Bus. Posting Group** and **Customer Posting Group** fields.</span><span class="sxs-lookup"><span data-stu-id="18ffc-138">Fill in the **Gen. Bus. Posting Group** and **Customer Posting Group** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="18ffc-139">See Also</span><span class="sxs-lookup"><span data-stu-id="18ffc-139">See Also</span></span>
[<span data-ttu-id="18ffc-140">Setting Up Service Management</span><span class="sxs-lookup"><span data-stu-id="18ffc-140">Setting Up Service Management</span></span>](service-setup-service.md)