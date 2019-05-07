---
title: Couple and Synchronise Records Manually| Microsoft Docs
description: Synchronising an integration table mapping enables data syncing in all records in a table in Business Central and Dynamics 365 for Sales entity that are coupled.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 36f1a0fe8c50744d9ce13d1e6c3c899f4ceaf5e4
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "940409"
---
# <a name="couple-and-synchronize-records-manually"></a><span data-ttu-id="cf564-103">Couple and Synchronise Records Manually</span><span class="sxs-lookup"><span data-stu-id="cf564-103">Couple and Synchronize Records Manually</span></span>
<span data-ttu-id="cf564-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="cf564-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="cf564-105">Coupling records lets you view [!INCLUDE[crm_md](includes/crm_md.md)] information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span><span class="sxs-lookup"><span data-stu-id="cf564-105">Coupling records lets you view [!INCLUDE[crm_md](includes/crm_md.md)] information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span></span> <span data-ttu-id="cf564-106">The coupling also enables you to synchronise data between the records.</span><span class="sxs-lookup"><span data-stu-id="cf564-106">The coupling also enables you to synchronize data between the records.</span></span> <span data-ttu-id="cf564-107">You can couple existing records, or create and couple new records.</span><span class="sxs-lookup"><span data-stu-id="cf564-107">You can couple existing records, or create and couple new records.</span></span>

> [!Note]
> <span data-ttu-id="cf564-108">Coupling and synchronising data with [!INCLUDE[crm_md](includes/crm_md.md)] is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="cf564-108">Coupling and synchronizing data with [!INCLUDE[crm_md](includes/crm_md.md)] is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="cf564-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span><span class="sxs-lookup"><span data-stu-id="cf564-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span></span> <span data-ttu-id="cf564-110">If the action is available, the apps are connected.</span><span class="sxs-lookup"><span data-stu-id="cf564-110">If the action is available, the apps are connected.</span></span>   

## <a name="to-couple-a-record"></a><span data-ttu-id="cf564-111">To couple a record</span><span class="sxs-lookup"><span data-stu-id="cf564-111">To couple a record</span></span>  
1.  <span data-ttu-id="cf564-112">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="cf564-112">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="cf564-113">For example, the Customer or Contact card.</span><span class="sxs-lookup"><span data-stu-id="cf564-113">For example, the Customer or Contact card.</span></span>  

    <span data-ttu-id="cf564-114">You can also just open the list page and select the record that you want to couple.</span><span class="sxs-lookup"><span data-stu-id="cf564-114">You can also just open the list page and select the record that you want to couple.</span></span>  

2.  <span data-ttu-id="cf564-115">Choose the **Set Up Coupling** action.</span><span class="sxs-lookup"><span data-stu-id="cf564-115">Choose the **Set Up Coupling** action.</span></span>  
3.  <span data-ttu-id="cf564-116">Fill in the fields, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="cf564-116">Fill in the fields, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record"></a><span data-ttu-id="cf564-117">To synchronise a single record</span><span class="sxs-lookup"><span data-stu-id="cf564-117">To synchronize a single record</span></span>  
1.  <span data-ttu-id="cf564-118">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="cf564-118">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="cf564-119">For example, the Customer or Contact card.</span><span class="sxs-lookup"><span data-stu-id="cf564-119">For example, the Customer or Contact card.</span></span>  
2.  <span data-ttu-id="cf564-120">Choose the **Synchronise Now** action.</span><span class="sxs-lookup"><span data-stu-id="cf564-120">Choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="cf564-121">If a record can be synchronised either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="cf564-121">If a record can be synchronized either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="to-synchronize-multiple-records"></a><span data-ttu-id="cf564-122">To synchronise multiple records</span><span class="sxs-lookup"><span data-stu-id="cf564-122">To synchronize multiple records</span></span>  
1.  <span data-ttu-id="cf564-123">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span><span class="sxs-lookup"><span data-stu-id="cf564-123">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span></span>  
2.  <span data-ttu-id="cf564-124">Select the records that you want to synchronise, and then choose the **Synchronise Now** action.</span><span class="sxs-lookup"><span data-stu-id="cf564-124">Select the records that you want to synchronize, and then choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="cf564-125">If records can be synchronised either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="cf564-125">If records can be synchronized either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cf564-126">See Also</span><span class="sxs-lookup"><span data-stu-id="cf564-126">See Also</span></span>  
[<span data-ttu-id="cf564-127">Using Dynamics 365 for Sales from Business Central</span><span class="sxs-lookup"><span data-stu-id="cf564-127">Using Dynamics 365 for Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
