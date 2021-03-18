---
title: Expose objects as web services
description: Publish objects as web services to make them immediately available for your Business Central solution.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 10/08/2020
ms.author: edupont
ms.openlocfilehash: 94a4752abc133e59169209b94a145d2195ce783d
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 02/15/2021
ms.locfileid: "5384631"
---
# <a name="publish-a-web-service"></a><span data-ttu-id="e1a6e-103">Publish a Web Service</span><span class="sxs-lookup"><span data-stu-id="e1a6e-103">Publish a Web Service</span></span>

<span data-ttu-id="e1a6e-104">Web services are a lightweight way to make application functionality available to different kinds of external systems and users.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-104">Web services are a lightweight way to make application functionality available to different kinds of external systems and users.</span></span> <span data-ttu-id="e1a6e-105">By default, [!INCLUDE[prod_short](includes/prod_short.md)] exposes a number of objects as web services for better integration with other Microsoft services.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-105">By default, [!INCLUDE[prod_short](includes/prod_short.md)] exposes a number of objects as web services for better integration with other Microsoft services.</span></span> <span data-ttu-id="e1a6e-106">You can add other web services as your business requires.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-106">You can add other web services as your business requires.</span></span>  

<span data-ttu-id="e1a6e-107">Set up a web service in [!INCLUDE[prod_short](includes/prod_short.md)], and then publish the web service so that it is available to authenticated users.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-107">Set up a web service in [!INCLUDE[prod_short](includes/prod_short.md)], and then publish the web service so that it is available to authenticated users.</span></span> <span data-ttu-id="e1a6e-108">All authorised users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-108">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>  

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="e1a6e-109">Creating and Publishing a Web Service</span><span class="sxs-lookup"><span data-stu-id="e1a6e-109">Creating and Publishing a Web Service</span></span>

<span data-ttu-id="e1a6e-110">The following steps explain how to create and publish a web service.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-110">The following steps explain how to create and publish a web service.</span></span>  

### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="e1a6e-111">To create and publish a web service</span><span class="sxs-lookup"><span data-stu-id="e1a6e-111">To create and publish a web service</span></span>  

1. <span data-ttu-id="e1a6e-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Web Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e1a6e-113">On the **Web Services** page, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-113">On the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    > <span data-ttu-id="e1a6e-114">**Codeunit** and **Page** are valid types for SOAP web services.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-114">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="e1a6e-115">**Page** and **Query** are valid types for OData web services.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-115">**Page** and **Query** are valid types for OData web services.</span></span> <span data-ttu-id="e1a6e-116">Starting with version 16.3, **Codeunit** is also a valid type for OData v4 web services, but then no URL is shown in the user interface.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-116">Starting with version 16.3, **Codeunit** is also a valid type for OData v4 web services, but then no URL is shown in the user interface.</span></span> <span data-ttu-id="e1a6e-117">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-117">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    > <span data-ttu-id="e1a6e-118">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-118">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3. <span data-ttu-id="e1a6e-119">Select the check box in the **Published** column.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-119">Select the check box in the **Published** column.</span></span>  

<span data-ttu-id="e1a6e-120">When you publish the web service, the **OData URL** and **SOAP URL** fields show the new URLs.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-120">When you publish the web service, the **OData URL** and **SOAP URL** fields show the new URLs.</span></span> <span data-ttu-id="e1a6e-121">However, for codeunits that are exposed as OData v4 unbound actions, the URL fields are not shown.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-121">However, for codeunits that are exposed as OData v4 unbound actions, the URL fields are not shown.</span></span>  

<span data-ttu-id="e1a6e-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="e1a6e-123">Optionally, copy the value of the field and save it for later use.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-123">Optionally, copy the value of the field and save it for later use.</span></span> <span data-ttu-id="e1a6e-124">To test codeunits that are exposed as OData v4 unbound actions, follow the instructions in the [Verifying web service availability](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) section in the developer content.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-124">To test codeunits that are exposed as OData v4 unbound actions, follow the instructions in the [Verifying web service availability](/dynamics365/business-central/dev-itpro/developer/devenv-creating-and-interacting-with-odatav4-unbound-action#verifying-web-service-availability) section in the developer content.</span></span>

> [!NOTE]
> <span data-ttu-id="e1a6e-125">If the objects that you expose as web services must not be accessible from [!INCLUDE[prod_short](includes/prod_short.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-125">If the objects that you expose as web services must not be accessible from [!INCLUDE[prod_short](includes/prod_short.md)] online, you must mark the methods exposed in the code as `[Scope('OnPrem')]`.</span></span> <span data-ttu-id="e1a6e-126">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span><span class="sxs-lookup"><span data-stu-id="e1a6e-126">For more information, see [Scope Attribute](/dynamics365/business-central/dev-itpro/developer/methods/devenv-scope-attribute).</span></span>

<span data-ttu-id="e1a6e-127">After you publish a web service, it is available to external parties.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-127">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="e1a6e-128">You can verify the availability of that web service by using a browser, or choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-128">You can verify the availability of that web service by using a browser, or choose the link in the **OData URL** and **SOAP URL** fields on the **Web Services** page.</span></span> <span data-ttu-id="e1a6e-129">The following procedure illustrates how you can verify the availability of the web service for later use.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-129">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="e1a6e-130">To verify the availability of a web service</span><span class="sxs-lookup"><span data-stu-id="e1a6e-130">To verify the availability of a web service</span></span>  

1. <span data-ttu-id="e1a6e-131">In your browser, enter the relevant URL.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-131">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="e1a6e-132">The following table illustrates the types of URLs that you can enter for different web service types.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-132">The following table illustrates the types of URLs that you can enter for different web service types.</span></span>  

    > [!div class="mx-tdBreakAll"]
    > |<span data-ttu-id="e1a6e-133">Type</span><span class="sxs-lookup"><span data-stu-id="e1a6e-133">Type</span></span>|<span data-ttu-id="e1a6e-134">Syntax</span><span class="sxs-lookup"><span data-stu-id="e1a6e-134">Syntax</span></span>|<span data-ttu-id="e1a6e-135">Example</span><span class="sxs-lookup"><span data-stu-id="e1a6e-135">Example</span></span>|
    > |----------------|------|-------|
    > |<span data-ttu-id="e1a6e-136">SOAP</span><span class="sxs-lookup"><span data-stu-id="e1a6e-136">SOAP</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/WS/*CompanyName*/*entity*/` |`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/WS/CRONUS%20USA%2C%20Inc./Page/InvoiceDocument`|
    > |<span data-ttu-id="e1a6e-137">OData V4</span><span class="sxs-lookup"><span data-stu-id="e1a6e-137">OData V4</span></span>|`https://api.businesscentral.dynamics.com/*version*/*tenant*/Production/ODataV4/Company('*CompanyName*')/*entity*`|`https://api.businesscentral.dynamics.com/v2.0/7acc9d3d-d354-4616-8bbd-c4fc9f2b15b3/Production/ODataV4/Company('CRONUS%20USA%2C%20Inc.')/InvoiceDocument`<br/>    <span data-ttu-id="e1a6e-138">The company name is case-sensitive.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-138">The company name is case-sensitive.</span></span>|

2. <span data-ttu-id="e1a6e-139">Review the information that is displayed in the browser.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-139">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="e1a6e-140">Verify that you can see the name of the web service that you have created.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-140">Verify that you can see the name of the web service that you have created.</span></span>  

<span data-ttu-id="e1a6e-141">When you access a web service, and you want to write data back to [!INCLUDE[prod_short](includes/prod_short.md)], you must specify the company name.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-141">When you access a web service, and you want to write data back to [!INCLUDE[prod_short](includes/prod_short.md)], you must specify the company name.</span></span> <span data-ttu-id="e1a6e-142">You can specify the company as part of the URI as shown in the examples; alternatively, specify the company as part of the query parameters.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-142">You can specify the company as part of the URI as shown in the examples; alternatively, specify the company as part of the query parameters.</span></span> <span data-ttu-id="e1a6e-143">For example, the following URIs point to the same OData web service and are both valid URIs.</span><span class="sxs-lookup"><span data-stu-id="e1a6e-143">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```
https://api.businesscentral.dynamics.com/v1.0/OData/Company('CRONUS International Ltd.')/Customer  
```

```
https://api.businesscentral.dynamics.com/v1.0/OData/Customer?company='CRONUS International Ltd.'  
```

## <a name="see-also"></a><span data-ttu-id="e1a6e-144">See Also</span><span class="sxs-lookup"><span data-stu-id="e1a6e-144">See Also</span></span>

[<span data-ttu-id="e1a6e-145">Administration</span><span class="sxs-lookup"><span data-stu-id="e1a6e-145">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="e1a6e-146">Business Central Web Services for developers</span><span class="sxs-lookup"><span data-stu-id="e1a6e-146">Business Central Web Services for developers</span></span>](/dynamics365/business-central/dev-itpro/webservices/web-services)  
[<span data-ttu-id="e1a6e-147">OData request limits</span><span class="sxs-lookup"><span data-stu-id="e1a6e-147">OData request limits</span></span>](/dynamics365/business-central/dev-itpro/administration/operational-limits-online#ODataServices)  


[!INCLUDE[footer-include](includes/footer-banner.md)]