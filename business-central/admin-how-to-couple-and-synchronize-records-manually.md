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
ms.openlocfilehash: 6d1248ac77208e382c5594af57335df6ff824630
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/04/2019
ms.locfileid: "1726774"
---
# <a name="couple-and-synchronize-records-manually"></a><span data-ttu-id="efe5a-103">Couple and Synchronise Records Manually</span><span class="sxs-lookup"><span data-stu-id="efe5a-103">Couple and Synchronize Records Manually</span></span>
<span data-ttu-id="efe5a-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="efe5a-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="efe5a-105">Coupling records lets you view [!INCLUDE[crm_md](includes/crm_md.md)] information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span><span class="sxs-lookup"><span data-stu-id="efe5a-105">Coupling records lets you view [!INCLUDE[crm_md](includes/crm_md.md)] information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span></span> <span data-ttu-id="efe5a-106">The coupling also enables you to synchronise data between the records.</span><span class="sxs-lookup"><span data-stu-id="efe5a-106">The coupling also enables you to synchronize data between the records.</span></span> <span data-ttu-id="efe5a-107">You can couple existing records, or create and couple new records.</span><span class="sxs-lookup"><span data-stu-id="efe5a-107">You can couple existing records, or create and couple new records.</span></span>

> [!Note]
> <span data-ttu-id="efe5a-108">Coupling and synchronising data with [!INCLUDE[crm_md](includes/crm_md.md)] is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="efe5a-108">Coupling and synchronizing data with [!INCLUDE[crm_md](includes/crm_md.md)] is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="efe5a-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span><span class="sxs-lookup"><span data-stu-id="efe5a-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span></span> <span data-ttu-id="efe5a-110">If the action is available, the apps are connected.</span><span class="sxs-lookup"><span data-stu-id="efe5a-110">If the action is available, the apps are connected.</span></span>   

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a><span data-ttu-id="efe5a-111">To couple a record</span><span class="sxs-lookup"><span data-stu-id="efe5a-111">To couple a record</span></span>  
1.  <span data-ttu-id="efe5a-112">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="efe5a-112">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="efe5a-113">For example, the Customer or Contact card.</span><span class="sxs-lookup"><span data-stu-id="efe5a-113">For example, the Customer or Contact card.</span></span>  

    <span data-ttu-id="efe5a-114">You can also just open the list page and select the record that you want to couple.</span><span class="sxs-lookup"><span data-stu-id="efe5a-114">You can also just open the list page and select the record that you want to couple.</span></span>  

2.  <span data-ttu-id="efe5a-115">Choose the **Set Up Coupling** action.</span><span class="sxs-lookup"><span data-stu-id="efe5a-115">Choose the **Set Up Coupling** action.</span></span>  
3.  <span data-ttu-id="efe5a-116">Fill in the fields, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="efe5a-116">Fill in the fields, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record"></a><span data-ttu-id="efe5a-117">To synchronise a single record</span><span class="sxs-lookup"><span data-stu-id="efe5a-117">To synchronize a single record</span></span>  
1.  <span data-ttu-id="efe5a-118">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span><span class="sxs-lookup"><span data-stu-id="efe5a-118">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="efe5a-119">For example, the Customer or Contact card.</span><span class="sxs-lookup"><span data-stu-id="efe5a-119">For example, the Customer or Contact card.</span></span>  
2.  <span data-ttu-id="efe5a-120">Choose the **Synchronise Now** action.</span><span class="sxs-lookup"><span data-stu-id="efe5a-120">Choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="efe5a-121">If a record can be synchronised either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="efe5a-121">If a record can be synchronized either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="to-synchronize-multiple-records"></a><span data-ttu-id="efe5a-122">To synchronise multiple records</span><span class="sxs-lookup"><span data-stu-id="efe5a-122">To synchronize multiple records</span></span>  
1.  <span data-ttu-id="efe5a-123">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span><span class="sxs-lookup"><span data-stu-id="efe5a-123">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span></span>  
2.  <span data-ttu-id="efe5a-124">Select the records that you want to synchronise, and then choose the **Synchronise Now** action.</span><span class="sxs-lookup"><span data-stu-id="efe5a-124">Select the records that you want to synchronize, and then choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="efe5a-125">If records can be synchronised either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span><span class="sxs-lookup"><span data-stu-id="efe5a-125">If records can be synchronized either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="efe5a-126">See Also</span><span class="sxs-lookup"><span data-stu-id="efe5a-126">See Also</span></span>  
[<span data-ttu-id="efe5a-127">Using Dynamics 365 for Sales from Business Central</span><span class="sxs-lookup"><span data-stu-id="efe5a-127">Using Dynamics 365 for Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
