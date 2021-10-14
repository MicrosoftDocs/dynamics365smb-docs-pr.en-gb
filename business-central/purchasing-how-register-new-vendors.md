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
ms.date: 09/29/2021
ms.author: edupont
ms.openlocfilehash: 662239446426cf64ac20d766e21aee55b92f9809
ms.sourcegitcommit: 6ad0a834fc225cc27dfdbee4a83cf06bbbcbc1c9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 10/01/2021
ms.locfileid: "7587691"
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
You can add new suppliers manually, by filling out the fields on the **Supplier Card** page, or you can use templates that contain predefined information. For example, you can create a templates for different types of supplier profiles. Using templates saves time when adding new suppliers, and helps ensure that the information is correct each time. If you create templates for more than one type of supplier, you can choose the template to use when you add a supplier. If you create only one template it will be used for all new suppliers. After you create a template, you can use the **Apply Template** action to apply it to one or more selected suppliers. To create a template, you fill in the information that you want to reuse on the Supplier Card page, and then save it as a template. For more information, see [To save the Supplier Card page as a template](purchasing-how-register-new-vendors.md#to-save-the-vendor-card-as-a-template).

> [!TIP]
> It can be helpful to personalise the **supplier Template** page when you create a template. For example, you might want to add a field that is not already displayed on the page. For more information, see [Personalise Your Workspace](/dynamics365/business-central/ui-personalization-user#to-start-personalizing-a-page-through-the-personalizing-banner).

You can also create a supplier from a contact. For more information, see [To create a customer, supplier, employee, or bank account from a contact](marketing-create-contact-companies.md#to-create-a-customer-vendor-employee-or-bank-account-from-a-contact). 

### <a name="to-create-a-new-vendor"></a>To create a new supplier

[!INCLUDE[create_new_vendor](includes/create_new_vendor.md)]

> [!TIP]  
> If you do not know the invoicing address that will be used for every invoice from a supplier, do not fill in the **Supplier No.** field. Instead, choose the pay-to supplier number after you have set up a purchase quote, order, or invoice header.

The supplier is now registered, and the supplier card is ready to be used on purchase documents.

If you want to use this supplier card as a template when you create new supplier cards, you can save it as a supplier template. For more information, see the [To save the supplier card as a template](#to-save-the-vendor-card-as-a-template) section.

### <a name="deleting-and-editing-vendor-information"></a>Deleting and editing supplier information

You can edit the information on supplier cards at any time. However, if you have posted a transaction for a supplier, you cannot delete the card because the ledger entries may be needed for auditing. To delete supplier cards with ledger entries, contact your Microsoft partner to do so through code.

> [!TIP]
> You can change the IBAN on a supplier bank account without the change affecting your historical credit transfer register entries. Credit transfer register entries store the Recipient IBAN, Recepient Bank Account No. that were specified in the Supplier Bank Account and Recipient Name fields from the Supplier Card page when the entries were created.


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