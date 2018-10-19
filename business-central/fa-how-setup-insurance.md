---
title: Set Up FA Insurance| Microsoft Docs
description: You set up an insurance card and general insurance policy information to manage fixed asset insurance coverage.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: policy, coverage
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 16098723fed40fbe26b9ba238e7fe5bf339003f5
ms.contentlocale: en-gb
ms.lasthandoff: 09/28/2018

---
# <a name="set-up-fixed-asset-insurance"></a>Set Up Fixed Asset Insurance
To manage fixed asset insurance coverage, you must first set up some general insurance information and an insurance card per policy.

## <a name="to-set-up-general-insurance-information"></a>To set up general insurance information
To use the insurance features in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must set up some general insurance information.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Setups**, and then choose the related link.  
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-insurance-types"></a>To set up insurance types
You can group your insurance policies into categories, such as insurance against theft or fire insurance. The insurance types are used on the insurance card.

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Types**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="to-set-up-insurance-cards"></a>To set up insurance cards
You may accumulate information about each insurance policy on the insurance card.  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance**, and then choose the related link.  
2. In the **Insurance** window, choose the **New** action to create a  new insurance card.  
3. Fill in the fields as necessary.

## <a name="to-set-up-insurance-journal-templates"></a>To set up insurance journal templates
[!INCLUDE[d365fin](includes/d365fin_md.md)] automatically creates an insurance journal template the first time that you open the **Insurance Journal** window, but you can set up additional journal templates. For more information, see [Working with General Journals](ui-work-general-journals.md).  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journal Templates**, and then choose the related link.  
2. Fill in the fields as necessary.

## <a name="to-set-up-insurance-journal-batches"></a>To set up insurance journal batches
You can set up batches in an insurance journal template. The values in the journal batch are used as default values if the fields are not filled in on the journal lines. For more information, see [Work with General Journals](ui-work-general-journals.md)  

1. Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Insurance Journal Templates**, and then choose the related link.  
2. Select an insurance journal template, and then choose the **Batches** action.
3. In the **Insurance Journal Batches** window, fill in the fields as necessary.

> [!NOTE]  
>   Numbers have a special function in journal names. If a journal template name or journal batch name contains a number, the number automatically advances by one every time that the journal is posted. For example, if HH1 is entered in the **Name** field, the journal name will change to HH2 after the journal named HH1 has been posted.

## <a name="see-also"></a>See Also
[Setting Up Fixed Assets](fa-setup.md)  
[Fixed Assets](fa-manage.md)  
[Finance](finance.md)  
[Getting Started](product-get-started.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

