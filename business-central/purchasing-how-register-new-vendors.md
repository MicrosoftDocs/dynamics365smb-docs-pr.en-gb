---
title: Create a Supplier Card to Register a New Supplier
description: In this topic learn how to create a supplier card to register a new supplier or supplier and save supplier cards as a template.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 06/23/2021
ms.author: edupont
ms.openlocfilehash: 2d4943415af6f5cd91ac35c68a9d8433e024b6be
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/08/2021
ms.locfileid: "6445383"
---
# <a name="register-new-vendors"></a>Register New Suppliers

Suppliers provide the products that you sell. Each supplier that you purchase from must be registered as a supplier card.

Before you can register new suppliers, you must set up various purchase codes that you can select from when you fill supplier cards. When all of the required master data is created, you can perform additional configuration of the supplier, such as prioritise the supplier for payment purposes and list items that the supplier and other suppliers can supply. Another group of setup tasks for suppliers is to record your agreements concerning discounts, prices, and payment methods. For more information, see [Setting Up Purchasing](purchasing-setup-purchasing.md).

Supplier cards hold the information that is required to buy products from the supplier. For more information, see [Record Purchases](purchasing-how-record-purchases.md) and [Register New Items](inventory-how-register-new-items.md).

> [!NOTE]  
> If supplier templates exist for different supplier types, then a page appears when you create a new supplier card from where you can select an appropriate template. If only one supplier template exists, then new supplier cards always use that template.
<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE3PZtd?rel=0]

## <a name="adding-new-vendors"></a>Adding new suppliers

To register a new supplier, you must fill in a supplier card. You can establish templates for different supplier profiles, or you can add suppliers without templates. You can also create a supplier from a contact. For more information, see [To create a customer, supplier, employee, or bank account from a contact](marketing-create-contact-companies.md#to-create-a-customer-vendor-employee-or-bank-account-from-a-contact).  

> [!NOTE]  
> If supplier templates exist for different supplier types, then a page appears when you create a new supplier card from where you can select an appropriate template. If only one supplier template exists, then new supplier cards always use that template.  

### <a name="to-create-a-new-vendor-card"></a>To create a new supplier card

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suppliers**, and then choose the related link.  
2. On the **Suppliers** page, Choose **New**.

    If more than one supplier template exists, then a page opens from which you can select a supplier template. In that case, follow the next two steps.
    1. On the **Select a template for a new supplier** page, choose the template that you want to use for the new supplier card.
    2. Choose the **OK** button. A new supplier card opens with some fields filled with information from the template.
3. Proceed to fill or change fields on the supplier card as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!TIP]  
    > If you do not know the invoicing address that will be used for every invoice from a supplier, do not fill in the **Supplier No.** field. Instead, choose the pay-to supplier number after you have set up a purchase quote, order, or invoice header.

The supplier is now registered, and the supplier card is ready to be used on purchase documents.

If you want to use this supplier card as a template when you create new supplier cards, you can save it as a supplier template. For more information, see the [To save the supplier card as a template](#to-save-the-vendor-card-as-a-template) section.

### <a name="deleting-vendor-cards"></a>Deleting supplier cards

If you have posted a transaction for a supplier, you cannot delete the card because the ledger entries may be needed for auditing. To delete supplier cards with ledger entries, contact your Microsoft partner to do so through code.

## <a name="to-save-the-vendor-card-as-a-template"></a>To save the supplier card as a template

1. On the **Supplier Card** page, choose the **Save as Template** action. The **Supplier Template** page opens showing the supplier card as a template.
2. Fill in the fields as necessary. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. To reuse dimensions in templates, choose the **Dimensions** action. The **Dimension Templates** page opens showing any dimension codes that are set up for the supplier.
4. Edit or enter dimension codes that will apply to new supplier cards created by using the template.
5. When you have completed the new supplier template, choose the **OK** button.  
   The supplier template is added to the list of supplier templates, so that you can use it to create new supplier cards.

## <a name="see-also"></a>See Also

[Merge Duplicate Records](sales-how-merge-duplicate-records.md)  
[Create Number Series](ui-create-number-series.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Record Purchases](purchasing-how-record-purchases.md)  
[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]