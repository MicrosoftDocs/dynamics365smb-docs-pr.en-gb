---
title: How to Create Service Quotes | Microsoft Docs
description: You can use the **Service Quote** page to create documents where you enter information about a service, such as repairs and maintenance, on service items by customer request. You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 0d4c8bba7814e33eb353ea39b3681aa52be53f40
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3189874"
---
# <a name="create-service-quotes"></a><span data-ttu-id="77524-104">Create Service Quotes</span><span class="sxs-lookup"><span data-stu-id="77524-104">Create Service Quotes</span></span>
<span data-ttu-id="77524-105">You can think of service quotes as the basis for service orders.</span><span class="sxs-lookup"><span data-stu-id="77524-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="77524-106">In fact, they are almost identical.</span><span class="sxs-lookup"><span data-stu-id="77524-106">In fact, they are almost identical.</span></span> <span data-ttu-id="77524-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span><span class="sxs-lookup"><span data-stu-id="77524-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="77524-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span><span class="sxs-lookup"><span data-stu-id="77524-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="77524-109">To create a service quote</span><span class="sxs-lookup"><span data-stu-id="77524-109">To create a service quote</span></span>  
1. <span data-ttu-id="77524-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="77524-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="77524-111">Create a new service quote.</span><span class="sxs-lookup"><span data-stu-id="77524-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="77524-112">In the **No.**</span><span class="sxs-lookup"><span data-stu-id="77524-112">In the **No.**</span></span> <span data-ttu-id="77524-113">field, enter a number for the service quote.</span><span class="sxs-lookup"><span data-stu-id="77524-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="77524-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span><span class="sxs-lookup"><span data-stu-id="77524-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="77524-115">In the **Customer No.**</span><span class="sxs-lookup"><span data-stu-id="77524-115">In the **Customer No.**</span></span>  <span data-ttu-id="77524-116">field, select the relevant customer from the list.</span><span class="sxs-lookup"><span data-stu-id="77524-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="77524-117">The customer fields are filled in automatically with information from the **Customer** card.</span><span class="sxs-lookup"><span data-stu-id="77524-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="77524-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span><span class="sxs-lookup"><span data-stu-id="77524-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="77524-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span><span class="sxs-lookup"><span data-stu-id="77524-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="77524-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span><span class="sxs-lookup"><span data-stu-id="77524-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="77524-121">Fill in the service item lines.</span><span class="sxs-lookup"><span data-stu-id="77524-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="77524-122">Register estimated costs on the service lines.</span><span class="sxs-lookup"><span data-stu-id="77524-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="77524-123">See Also</span><span class="sxs-lookup"><span data-stu-id="77524-123">See Also</span></span>  
[<span data-ttu-id="77524-124">Create Service Orders</span><span class="sxs-lookup"><span data-stu-id="77524-124">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="77524-125">Work on Service tasks</span><span class="sxs-lookup"><span data-stu-id="77524-125">Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 