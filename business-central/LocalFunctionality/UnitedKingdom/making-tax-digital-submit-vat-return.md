---
title: Making Tax Digital - Submitting VAT Returns
description: Business Central includes features to manage your VAT and comply with Making Tax Digital. This article describes how to set up and use these features.
author: sorenfriisalexandersen
ms.topic: conceptual
ms.search.keywords: 'making tax digital, vat, vat return, submit vat, making tax digital software, hmrc, tax'
ms.search.form: '743, 10530, 10531, 10532, 10537, 10538, 10539,'
ms.date: 09/28/2023
ms.author: bholtorf
ms.reviewer: soalex
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# <a name="making-tax-digital-in-the-united-kingdom"></a>Making Tax Digital in the United Kingdom

His Majesty's Revenue and Customs (HMRC) has implemented the first steps of *Making Tax Digital*, which imposes new requirements on VAT registered businesses above the VAT threshold. [!INCLUDE [prod_short](../../includes/prod_short.md)] supports the first rounds of *Making Tax Digital*, which took effect in April 2019:

* Keeping records digitally

  Businesses must now keep all their records digitally. For users of finance systems, such as [!INCLUDE [prod_short](../../includes/prod_short.md)], this requirement is already met because they already keep their records digitally.  
* Submit VAT return electronically using [software recognized by HMRC](https://www.gov.uk/guidance/software-for-sending-income-tax-updates).  

Since 2021, the electronic statements must also include information that helps prevent fraud. For more information, see [Send Fraud Prevention Data](fraud-prevention-data.md).  

[!INCLUDE[prod_short](../../includes/prod_short.md)] supports Making Tax Digital and the GovTalk service.

## <a name="making-tax-digital-for-vat-capabilities-in-dynamics-365-business-central"></a>Making Tax Digital for VAT capabilities in Dynamics 365 Business Central

In [!INCLUDE[prod_short](../../includes/prod_short.md)], you can use the VAT Return report for creating VAT reports. The Making Tax Digital VAT features extend this capability to communicate with HMRC. For example, the Making Tax Digital VAT extension lets you:

* Retrieve VAT obligations from HMRC
* Get reminded about VAT obligations that are approaching or already past due
* Submit VAT returns to HMRC  
* View the VAT return  
* View VAT payments with HMRC  
* View VAT liabilities with HMRC  

## <a name="set-up-making-tax-digital-for-vat"></a>Set up Making Tax Digital for VAT

The *Making Tax Digital* integration uses a service connection to communicate with HMRC. To make it easy to establish communications, [!INCLUDE[prod_short](../../includes/prod_short.md)] provides the **HMRC VAT Setup** service connection, which contains most of the information needed to communicate with HMRC. To finish the connection, you must give the **Dynamics 365 Business Central MTD VAT** application the authority to interact with HMRC on your behalf. Microsoft manages the **Dynamics 365 Business Central MTD VAT** application on the HMRC web site, and the application is a requirement for the connection. You give permission by requesting an authorization code from HMRC, and then copying the code to the service connection. The following steps describe how to set up the service connection.  
  
> [!NOTE]
> The following procedure describes the steps to set up Making Tax Digital in [!INCLUDE [prod_short](../../includes/prod_short.md)] online. If you're using [!INCLUDE [prod_short](../../includes/prod_short.md)] on-premises, there are some additional steps. For more information, see the [Setup requirements for on-premises versions](#setup-requirements-for-on-premises-versions) section before you start to set up the service connection.

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose the related link.  
2. On the **Service Connections** page, choose **HMRC VAT Setup**.
3. To open a GOV.UK website and request an authorisation code, choose **Process**, then **Request Authorisation Code**, and then choose **Continue**.  
4. Sign in with your HMRC credentials. To allow the **Dynamics 365 Business Central MTD VAT** application to interact with HMRC on your behalf, choose **Grant authority**.
5. A confirmation page displays "Authorization granted" and an authorization code. To copy the authorization code, choose **Copy**.
6. Return to the service connection you are setting up, and paste the authorisation code in the **Enter Authorisation Code** field. Then choose **Enter**. Note that the authorisation code is valid for 10 minutes. To set up the connection, you must enter the code in [!INCLUDE[prod_short](../../includes/prod_short.md)] before it expires.

    > [!NOTE]
    > [!INCLUDE[prod_short](../../includes/prod_short.md)] will use the authorisation code to test whether the service connection can communicate with HMRC. If the connection is successful, a confirmation page prompts you to verify your VAT registration number. To open the **Company Information** page and verify the number is correct, and the one you have used to register with HMRC, choose **Yes**.

You must also fill in the fields on the **VAT Report Setup** page. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)] For more information, see [Set up VAT reporting](../../finance-setup-vat.md#set-up-vat-reporting).  

> [!IMPORTANT]
> Starting in March 2022, the **User IP Address Service** must specify an endpoint for the service that your company uses to extract and submit the IP address of the user who sends the VAT report. For more information, see [IP addresses](fraud-prevention-data.md#ip-addresses).

### <a name="setup-requirements-for-on-premises-versions"></a>Setup requirements for on-premises versions

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

3. Create an application registration for Business Central in Azure portal. For more information, see [Registering Business Central On-Premises in Microsoft Entra ID for Integrating with Other Services](/dynamics365/business-central/dev-itpro/administration/register-app-azure). When you set up the service connection in [!INCLUDE [prod_short](../../includes/prod_short.md)], you'll need the following information from the registration:

    * Client ID
    * Client Secret
    * Redirect URL

## <a name="vat-obligations"></a>VAT obligations

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

Use this report to submit VAT for sales and purchase documents. For example, purchase and sales orders, invoices, and credit memos.

### <a name="to-create-and-submit-a-vat-return"></a>To create and submit a VAT return

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Return Periods**, and then choose the related link.  
2. On the **VAT Return Periods** page, choose the relevant period, and then choose the **Create VAT Return** action.
3. If you want to open the VAT return, on the confirmation page, choose **Yes**.
4. On the **VAT Return** page, to calculate and prepare the amounts for the VAT return, choose **Process**, and then choose the **Suggest Lines** action.  
5. Fill in the fields as necessary, and then choose the **OK** button. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

    VAT amounts display in the **Report Lines** section on the **VAT Return** page.  
6. To release the VAT return and prepare it for submission, choose **Process**, and then choose the **Release** action. After you release a VAT return, you cannot edit it. If you need to change something, you must reopen the return. Releasing the VAT return does not submit it.
7. To submit the VAT return to HMRC, choose **Process**, and then choose the **Submit** action.  

A successful submission of the VAT Return will result in a status of *Accepted* on the VAT Return. This status is based on the submission result at the HMRC. If the status after submission is not set to *Approved*, a previously submitted VAT Return can be retrieved from the HMRC.

### <a name="to-receive-previously-submitted-vat-returns-from-hmrc"></a>To receive previously submitted VAT returns from HMRC

1. Choose the ![Lightbulb that opens the Tell Me feature.](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Return Periods**, and then choose the related link.  
2. On the **VAT Return Periods** page, choose the relevant VAT return period.
3. On the **VAT Return Period Card** page, choose the **Receive Submitted VAT Returns** action.

### <a name="vat-return-statuses"></a>VAT Return Statuses

Dependding on where they are in the process, VAT returns can have one of the following statuses:

| Status | Description |
|------------|-------------------------|
| Open | When you create a new **VAT Return**. This status lets you run the **Suggest Lines** action. If you need to correct values, run the **Suggest Lines** action again. You can't submit a **VAT Return** with this status. |
| Released | Status will be changed when you manually run the **Release** action. The **Errors and Warnings** FastTab is available. You can't make changes or run the **Suggest Lines** action. To make changes, you must reopen this **VAT Return**. |
| Rejected | If your submission was not successful (for example, if authentication failed), the **VAT Return** status will be changed to **Rejected**. You Can't reopen the **VAT Return** from this status. |
| Submitted | **VAT Return** is submitted using the **Submit** action or it is marked as submitted using the **Mark as Submitted** action. |
| Accepted | **VAT Return** will get this status if the report is marked with the **Mark as Accepted** action. The **Accepted** status can be assigned automatically after user sends the VAT Return to the tax authority (Business Central calls the **Get VAT Returns** method and checks whether the VAT return is in the response). If the **VAT Return** report is marked as **Accepted**, you can run the **Calculate and Post VAT Settlement** action. |
| Partially Accepted | Business Central can assign the **Partially Accepted** status related to GovTalk information that was collected using the **Get VAT Returns** method.
| Closed | When request called Get VAT obligations check whether the obligation for which the user created the VAT return is closed. Business Central automatically marks the **VAT Return** as **Closed**. |

## <a name="vat-liabilities-and-payments"></a>VAT liabilities and payments

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

  If you submit VAT on behalf of a group of companies that share a VAT registration number (Group VAT), there isn't a built-in way to retrieve VAT entries from companies in the group. There are currently no plans to support Group VAT, and we refer to Microsoft partners to add this functionality.
* Agent services

  Agents can submit VAT returns on behalf of their customers, and HMRC has agent services. [!INCLUDE[prod_short](../../includes/prod_short.md)] does not support agent services.

## <a name="connection-errors-with-hmrc"></a>Connection errors with HMRC

If you experience "The operation has timed out" errors on an on-premises installation of [!INCLUDE[prod_short](../../includes/prod_short.md)], check any firewall settings that may be blocking the communication to and from HMRC.

## <a name="testing-the-integration-to-hmrc-in-a-sandbox"></a>Testing the integration to HMRC in a sandbox

Due to a limitation at HMRC, it is not possible to send test submissions of VAT Returns and test the integration in non-production scenarios. You can only send real VAT returns.  

Some online documentation at HMRC uses the term *Sandbox*. A sandbox is an environment that software developers, such as Microsoft and others, can use to test features during development. This environment is not intended for customer testing, and it isn't related to [!INCLUDE[prod_short](../../includes/prod_short.md)] sandboxes.

## <a name="see-also"></a>See also

[Send Fraud Prevention Data](fraud-prevention-data.md)  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  
[Set Up Calculations and Posting Methods for Value-Added Tax](../../finance-setup-vat.md)  
[The GetAddress.io UK Postcodes Extension](ui-extensions-getaddressio.md)  
[The VAT Group Management Extension](../../ui-extensions-vat-group.md)  
[Customising [!INCLUDE[prod_short](../../includes/prod_short.md)] Using Extensions](../../ui-extensions.md)  
[Work with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
