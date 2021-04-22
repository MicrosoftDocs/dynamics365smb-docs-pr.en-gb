---
title: Set Up FA Insurance| Microsoft Docs
description: You set up an insurance card and general insurance policy information to manage fixed asset insurance coverage.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: policy, coverage
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 0ebb62a4ef9ea84ec5bfddc099dfb6120a4e6405
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774048"
---
# <a name="set-up-fixed-asset-insurance"></a>Set Up Fixed Asset Insurance
To manage fixed asset insurance coverage, you must first set up some general insurance information and an insurance card per policy.

## <a name="to-set-up-general-insurance-information"></a>To set up general insurance information
To use the insurance features in [!INCLUDE[prod_short](includes/prod_short.md)], you must set up some general insurance information.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Setups**, and then choose the related link.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-insurance-types"></a>To set up insurance types
You can group your insurance policies into categories, such as insurance against theft or fire insurance. The insurance types are used on the insurance card.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Types**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="to-set-up-insurance-cards"></a>To set up insurance cards
You may accumulate information about each insurance policy on the insurance card.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance**, and then choose the related link.  
2. On the **Insurance** page, choose the **New** action to create a  new insurance card.  
3. Fill in the fields as necessary.

## <a name="to-set-up-insurance-journal-templates"></a>To set up insurance journal templates
[!INCLUDE[prod_short](includes/prod_short.md)] automatically creates an insurance journal template the first time that you open the **Insurance Journal** page, but you can set up additional journal templates. For more information, see [Working with General Journals](ui-work-general-journals.md).  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journal Templates**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="to-set-up-insurance-journal-batches"></a>To set up insurance journal batches
You can set up batches in an insurance journal template. The values in the journal batch are used as default values if the fields are not filled in on the journal lines. For more information, see [Work with General Journals](ui-work-general-journals.md)  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journal Templates**, and then choose the related link.  
2. Select an insurance journal template, and then choose the **Batches** action.
3. On the **Insurance Journal Batches** page, fill in the fields as necessary.

> [!NOTE]  
>   Numbers have a special function in journal names. If a journal template name or journal batch name contains a number, the number automatically advances by one every time that the journal is posted. For example, if HH1 is entered in the **Name** field, the journal name will change to HH2 after the journal named HH1 has been posted.

## <a name="see-also"></a>See Also
[Setting Up Fixed Assets](fa-setup.md)  
[Fixed Assets](fa-manage.md)  
[Finance](finance.md)  
[Getting Ready for Doing Business](ui-get-ready-business.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]