---
title: Couple and Synchronise Records Manually| Microsoft Docs
description: Synchronising an integration table mapping enables data syncing in all records in a table in Business Central and Dynamics 365 Sales entity that are coupled.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: fdc407ef26d238ba54a2566cdd9003c29da2eeb3
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196670"
---
# <a name="couple-and-synchronize-records-manually"></a><span data-ttu-id="4e484-103">Couple and Synchronise Records Manually</span><span class="sxs-lookup"><span data-stu-id="4e484-103">Couple and Synchronize Records Manually</span></span>
<span data-ttu-id="4e484-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4e484-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="4e484-105">Coupling records lets you view Common Data Service information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span><span class="sxs-lookup"><span data-stu-id="4e484-105">Coupling records lets you view Common Data Service information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span></span> <span data-ttu-id="4e484-106">The coupling also enables you to synchronise data between the records.</span><span class="sxs-lookup"><span data-stu-id="4e484-106">The coupling also enables you to synchronize data between the records.</span></span> <span data-ttu-id="4e484-107">You can couple existing records, or create and couple new records.</span><span class="sxs-lookup"><span data-stu-id="4e484-107">You can couple existing records, or create and couple new records.</span></span>

> [!Note]
> <span data-ttu-id="4e484-108">Coupling and synchronising data is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4e484-108">Coupling and synchronizing data is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="4e484-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span><span class="sxs-lookup"><span data-stu-id="4e484-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span></span> <span data-ttu-id="4e484-110">If the action is available, the apps are connected.</span><span class="sxs-lookup"><span data-stu-id="4e484-110">If the action is available, the apps are connected.</span></span>   

## <a name="video-example"></a><span data-ttu-id="4e484-111">Video Example</span><span class="sxs-lookup"><span data-stu-id="4e484-111">Video Example</span></span>

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a><span data-ttu-id="4e484-112">To couple a record</span><span class="sxs-lookup"><span data-stu-id="4e484-112">To couple a record</span></span>  
1.  <span data-ttu-id="4e484-113">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="4e484-113">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="4e484-114">For example, the Customer or Contact card.</span><span class="sxs-lookup"><span data-stu-id="4e484-114">For example, the Customer or Contact card.</span></span>  

    <span data-ttu-id="4e484-115">You can also just open the list page and select the record that you want to couple.</span><span class="sxs-lookup"><span data-stu-id="4e484-115">You can also just open the list page and select the record that you want to couple.</span></span>  

2.  <span data-ttu-id="4e484-116">Choose the **Set Up Coupling** action.</span><span class="sxs-lookup"><span data-stu-id="4e484-116">Choose the **Set Up Coupling** action.</span></span>  
3.  <span data-ttu-id="4e484-117">Fill in the fields, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="4e484-117">Fill in the fields, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record"></a><span data-ttu-id="4e484-118">To synchronise a single record</span><span class="sxs-lookup"><span data-stu-id="4e484-118">To synchronize a single record</span></span>  
1.  <span data-ttu-id="4e484-119">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="4e484-119">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="4e484-120">For example, the Customer or Contact card.</span><span class="sxs-lookup"><span data-stu-id="4e484-120">For example, the Customer or Contact card.</span></span>  
2.  <span data-ttu-id="4e484-121">Choose the **Synchronise Now** action.</span><span class="sxs-lookup"><span data-stu-id="4e484-121">Choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="4e484-122">If a record can be synchronised in one direction, select the option that specifies the direction of data update, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="4e484-122">If a record can be synchronized in one direction, select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record-from-crm_md"></a><span data-ttu-id="4e484-123">To synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)]</span><span class="sxs-lookup"><span data-stu-id="4e484-123">To synchronize a single record from [!INCLUDE[crm_md](includes/crm_md.md)]</span></span>  
1.  <span data-ttu-id="4e484-124">In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="4e484-124">In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple.</span></span> <span data-ttu-id="4e484-125">For example, the Account card or Contact card form.</span><span class="sxs-lookup"><span data-stu-id="4e484-125">For example, the Account card or Contact card form.</span></span>  
2.  <span data-ttu-id="4e484-126">Choose the **[!INCLUDE[d365fin](includes/d365fin_md.md)]** action in the ribbon to open and couple record automatically.</span><span class="sxs-lookup"><span data-stu-id="4e484-126">Choose the **[!INCLUDE[d365fin](includes/d365fin_md.md)]** action in the ribbon to open and couple record automatically.</span></span>

> [!Note]
> <span data-ttu-id="4e484-127">You can synchronise a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronisation direction is set to Bidirectional or From Integration Table on the **Integration Table Mapping** page for the record.</span><span class="sxs-lookup"><span data-stu-id="4e484-127">You can synchronize a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronization direction is set to Bidirectional or From Integration Table on the **Integration Table Mapping** page for the record.</span></span> <span data-ttu-id="4e484-128">For more information, see [Mapping the Tables and Fields to Synchronise](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).</span><span class="sxs-lookup"><span data-stu-id="4e484-128">For more information, see [Mapping the Tables and Fields to Synchronize](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).</span></span>     

## <a name="to-synchronize-multiple-records"></a><span data-ttu-id="4e484-129">To synchronise multiple records</span><span class="sxs-lookup"><span data-stu-id="4e484-129">To synchronize multiple records</span></span>  
1.  <span data-ttu-id="4e484-130">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span><span class="sxs-lookup"><span data-stu-id="4e484-130">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span></span>  
2.  <span data-ttu-id="4e484-131">Select the records that you want to synchronise, and then choose the **Synchronise Now** action.</span><span class="sxs-lookup"><span data-stu-id="4e484-131">Select the records that you want to synchronize, and then choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="4e484-132">If records can be synchronised in one direction, select the option that specifies the direction, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="4e484-132">If records can be synchronized in one direction, select the option that specifies the direction, and then choose **OK**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4e484-133">See Also</span><span class="sxs-lookup"><span data-stu-id="4e484-133">See Also</span></span>  
[<span data-ttu-id="4e484-134">Using Dynamics 365 Sales from Business Central</span><span class="sxs-lookup"><span data-stu-id="4e484-134">Using Dynamics 365 Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
