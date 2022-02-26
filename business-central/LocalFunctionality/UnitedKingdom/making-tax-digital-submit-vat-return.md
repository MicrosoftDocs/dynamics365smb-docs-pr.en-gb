---
title: Making Tax Digital - Submitting VAT Returns
description: Business Central includes features to manage your VAT and comply with Making Tax Digital. This article describes how to set up and use these features.
author: sorenfriisalexandersen
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: making tax digital, vat, vat return, submit vat, making tax digital software, hmrc, tax
ms.date: 01/31/2022
ms.author: soalex
ms.openlocfilehash: 525e03830b88460ce57e5a7d1ca1699f76f847a1
ms.sourcegitcommit: 189bf08d7ddf6c8b7ef2c09058c6847aa6e590d3
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 01/31/2022
ms.locfileid: "8060136"
---
# <a name="making-tax-digital-in-the-united-kingdom"></a>Making Tax Digital in the United Kingdom

Her Majesty's Revenue and Customs (HMRC) has implemented the first step of Making Tax Digital, which imposes new requirements on VAT registered businesses above the VAT threshold. Requirements will be implemented in phases. In the first phase, with a deadline in April 2019, the following requirements took effect:

* Keeping records digitally

  Businesses must now keep all their records digitally. For users of ERP systems, this requirement will not have any impact since they already keep their records digitally in these systems.  
* Submit VAT return electronically using [software recognized by HMRC](https://www.gov.uk/guidance/software-for-sending-income-tax-updates).  

Starting in 2021, the electronic statements must also include information that helps prevent fraud. For more information, see [Send Fraud Prevention Data](fraud-prevention-data.md).  

[!INCLUDE[prod_short](../../includes/prod_short.md)] supports Making Tax Digital and the GovTalk service.

## <a name="making-tax-digital-for-vat-capabilities-in-dynamics-365-business-central"></a>Making Tax Digital for VAT Capabilities in Dynamics 365 Business Central

In [!INCLUDE[prod_short](../../includes/prod_short.md)] you can use the VAT Return report for creating VAT reports. The Making Tax Digital VAT features extend this capability to communicate with HMRC. For example, the Making Tax Digital VAT extension lets you:

* Retrieve VAT obligations from HMRC
* Get reminded about VAT obligations that are approaching or already past due
* Submit VAT returns to HMRC  
* View the VAT return  
* View VAT payments with HMRC  
* View VAT liabilities with HMRC  

## <a name="set-up-making-tax-digital-for-vat"></a>Set up Making Tax Digital for VAT

The Making Tax Digital feature uses a service connection to communicate with HMRC. To make it easy to establish communications, [!INCLUDE[prod_short](../../includes/prod_short.md)] provides the **HMRC VAT Setup** service connection, which contains most of the information needed to communicate with HMRC. To finish the connection, you must give the **Dynamics 365 Business Central MTD VAT** application the authority to interact with HMRC on your behalf. Microsoft manages the **Dynamics 365 Business Central MTD VAT** application on the HMRC web site, and the application is a requirement for the connection. You give permission by requesting an authorization code from HMRC, and then copying the code to the service connection. The following steps describe how to set up the service connection.  
  
> [!Note]
> If you are using [!INCLUDE [prod_short](../../includes/prod_short.md)] on-premises, there are some additional steps to set up the features for Making Tax Digital. In [!INCLUDE [prod_short](../../includes/prod_short.md)] online, these happen automatically. For more information, see the [Additional Setup Requirements for On-Premises Versions](#additional-setup-requirements-for-on-premises-versions) section.

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose the related link.  
2. On the **Service Connections** page, choose **HMRC VAT Setup**.

    > [!Note]
    > If you use [!INCLUDE[prod_short](../../includes/prod_short.md)] on-premises, you must also provide a client ID and client secret. If you are not sure what these are, contact your partner.  

3. To open a GOV.UK website and request an authorisation code, choose **Process**, then **Request Authorisation Code**, and then choose **Continue**.  
4. Sign in with your HMRC credentials. To allow the **Dynamics 365 Business Central MTD VAT** application to interact with HMRC on your behalf, choose **Grant authority**.
5. A confirmation page displays "Authorization granted" and an authorization code. To copy the authorization code, choose **Copy**.
6. Return to the service connection you are setting up, and paste the authorisation code in the **Enter Authorisation Code** field. Then choose **Enter**. Note, that the authorisation code is valid for 10 minutes and must be entered into [!INCLUDE[prod_short](../../includes/prod_short.md)] before expiry in order to set up the connection correctly.

    > [!Note]
    > [!INCLUDE[prod_short](../../includes/prod_short.md)] will use the authorisation code to test whether the service connection can communicate with HMRC. If the connection is successful, a confirmation page prompts you to verify your VAT registration number. To open the **Company Information** page and verify the number is correct, and the one you have used to register with HMRC, choose **Yes**.

### <a name="additional-setup-requirements-for-on-premises-versions"></a>Additional Setup Requirements for On-Premises Versions

1. You must add a VAT report configuration on the **VAT Reports Configuration** page.  
  
    a. Create a new configuration, and choose the VAT Return type.  
    b. Give the configuration a descriptive name, such as **HMRC MTD**.  
    c. In the **Suggest Lines Codeunit ID** field, choose codeunit **745**.  
    d. In the **Content Codeunit ID** field, choose codeunit **10531**.  
    e. In the **Submission Codeunit ID** field, choose codeunit **10532**.  
    f. In the **Validate Codeunit ID** field, choose codeunit **10533**.  
    g. Fill in the remaining fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]

2. You must edit the VAT report setup on the **VAT Report Setup** page.  
  
    a. Expand the **Return Period** FastTab.  
    b. In the **Report Version** field, choose the VAT report configuration that you created in the previous step.  
    c. In the **Manual Receive Codeunit ID** field, choose codeunit **10534**.  
    d. In the **Receive Submitted Return Codeunit ID** field, choose codeunit **10536**.  
    e. Optional: If you want to automatically update the information about VAT obligations, specify how often to do so in the **Update Period Job Frequency** field, and then specify codeunit **10535** in the **Auto Receive Codeunit ID** field.  
    f. Fill in the remaining fields as necessary. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]

## <a name="vat-obligations"></a>VAT Obligations

HMRC maintains a list of VAT obligations for companies, which are the periods for which they must report VAT and the due date for the report. HMRC exposes this information through their APIs, which enables [!INCLUDE[prod_short](../../includes/prod_short.md)] to retrieve the obligations. [!INCLUDE[prod_short](../../includes/prod_short.md)] stores VAT obligations as **VAT Return Periods**, and uses them to:

* Remind you about VAT returns that are due or overdue.
* Automatically enter start and end dates when you create VAT returns.

### <a name="to-retrieve-the-vat-return-periods-from-hmrc"></a>To retrieve the VAT return periods from HMRC

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Return Periods**, and then choose the related link.  
2. On the **VAT Return Periods** page, choose the **Get VAT Return Periods** action.
3. Enter the **Start Date** and **End Date** to specify the period for which to get the VAT return periods, and then choose **OK**.  

The VAT obligations are now retrieved from HMRC and you can view them on the **VAT Return Periods** page. A confirmation page shows how many obligations were retrieved.

  > [!NOTE]  
  > Do not create VAT return periods manually when submitting VAT Returns to HMRC. VAT return periods must be retrieved from HMRC using the steps above. Creating them manually will result in inability to submit VAT Returns.  

## <a name="vat-returns"></a>VAT Returns

Use this report to submit VAT for sales and purchase documents, such as purchase and sales orders,invoices, and credit memos.

### <a name="to-create-and-submit-a-vat-return"></a>To create and submit a VAT return

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Return Periods**, and then choose the related link.  
2. On the **VAT Return Periods** page, choose the relvant period, and then choose the **Create VAT Return** action.
3. If you want to open the VAT return, on the confirmation page, choose **Yes**.
4. On the **VAT Return** page, to calculate and prepare the amounts for the VAT return, choose **Process**, and then choose the **Suggest Lines** action.  
5. Fill in the fields as necessary, and then choose the **OK** button. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    VAT amounts display in the **Report Lines** section on the **VAT Return** page.  
6. To release the VAT return and prepare it for submission, choose **Process**, and then choose the **Release** action. After you release a VAT return, you cannot edit it. If you need to change something, you must reopen the return. Releasing the VAT return does not submit it.
7. To submit the VAT return to HMRC, choose **Process**, and then choose the **Submit** action.  

A successful submission of the VAT Return will result in a status of *Accepted* on the VAT Return. This status is based on the submission result at the HMRC. If the status after submission is not set to *Approved*, a previously submitted VAT Return can be retrieved from the HMRC.

### <a name="to-receive-previously-submitted-vat-returns-from-hmrc"></a>To receive previously submitted VAT Returns from HMRC

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Return Periods**, and then choose the related link.  
2. On the **VAT Return Periods** page, choose the relevant VAT return period.
3. On the **VAT Return Period Card** page, choose the **Receive Submitted VAT Returns** action.

## <a name="vat-liabilities-and-payments"></a>VAT Liabilities and Payments

If you want to check the status of your VAT, you can retrieve information from HMRC about your VAT liabilities and payments. VAT liabilities are the amounts that you owed to HMRC, and show if there are outstanding amounts to be paid. VAT payments are the actual payments your company has made to HMRC.

To retrieve VAT liabilities:

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Liabilities**, and then choose the related link.  
2. On the **VAT Liabilities** page, choose **Process**, and then select **Get Liabilities**.
3. Enter the **Start Date** and **End Date** of the period to retrieve VAT liabilities for, and then choose **OK**.

The VAT liabilities are now retrieved from HMRC and you can view them on the **VAT Liabilities** page. A confirmation page shows how many liabilities were retrieved.

To retrieve VAT payments from HMRC:

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Payments**, and then choose the related link.  
2. On the **VAT Payments** page, choose **Process**, and then choose **Get Payments**.
3. Enter the **Start Date** and **End Date** of the period to retrieve VAT payments for, and then choose **OK**.

The VAT payments are now retrieved from HMRC and you can view them on the **VAT Payments** page. A confirmation page shows how many VAT payments were retrieved.

## <a name="not-in-scope-of-this-feature"></a>Not in scope of this feature

This integration to HMRC and support of Making Tax Digital for VAT does not include support for:

* Group VAT scenarios

  If your [!INCLUDE[prod_short](../../includes/prod_short.md)] submits VAT on behalf of a group of companies that share a VAT registration number (Group VAT), there is no built in mechanism for retrieving VAT entries from other companies in the group. There are currently no plans to support Group VAT, and we refer to Microsoft partners to add this functionality.
* Agent services

  Agents can submit VAT returns on behalf of their customers and HMRC has solutions for that. This is currently not supported by [!INCLUDE[prod_short](../../includes/prod_short.md)].

## <a name="connection-errors-with-hmrc"></a>Connection errors with HMRC

If you experience "The operation has timed out" errors on an on-premises installation of [!INCLUDE[prod_short](../../includes/prod_short.md)], check any firewall settings that may be blocking the communication to and from HMRC.

## <a name="testing-the-integration-to-hmrc-in-a-sandbox"></a>Testing the integration to HMRC in a sandbox

Due to a limitation at HMRC, it is not possible to send test submissions of VAT Returns and test the integration in non-production scenarios. You can only send real VAT returns.  

Certain online documentation at HMRC refers to the term *Sandbox*. This term refers to an environment for software developers such as Microsoft and others for testing their features during development. This environment is not intended for customer testing, and it is unrelated to [!INCLUDE[prod_short](../../includes/prod_short.md)] sandboxes.

## <a name="see-also"></a>See Also

[Send Fraud Prevention Data](fraud-prevention-data.md)  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  
[The GetAddress.io UK Postcodes Extension](ui-extensions-getaddressio.md)  
[The VAT Group Management Extension](../../ui-extensions-vat-group.md)  
[Customising [!INCLUDE[prod_short](../../includes/prod_short.md)] Using Extensions](../../ui-extensions.md)  
[Working with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]