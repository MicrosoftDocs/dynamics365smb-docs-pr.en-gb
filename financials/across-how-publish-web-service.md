---
title: Expose objects as web services | Microsoft Docs
description: Publish [!INCLUDE[d365fin](includes/d365fin_md.md)] objects as web services, they are immediately available on the network.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 278515fc479a72957fb52dad71ce2f98d354ee32
ms.contentlocale: en-gb
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-publish-a-web-service"></a><span data-ttu-id="17ace-103">How to: Publish a Web Service</span><span class="sxs-lookup"><span data-stu-id="17ace-103">How to: Publish a Web Service</span></span>
<span data-ttu-id="17ace-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span><span class="sxs-lookup"><span data-stu-id="17ace-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="17ace-105"> includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span><span class="sxs-lookup"><span data-stu-id="17ace-105"> includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="17ace-106">You can set up a web service in the Windows client or in the Web client.</span><span class="sxs-lookup"><span data-stu-id="17ace-106">You can set up a web service in the Windows client or in the Web client.</span></span> <span data-ttu-id="17ace-107">You must then publish the web service so that it is available to service requests over the network.</span><span class="sxs-lookup"><span data-stu-id="17ace-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="17ace-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span><span class="sxs-lookup"><span data-stu-id="17ace-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="17ace-109">When you publish a web service, it is immediately available over the network for authenticated users.</span><span class="sxs-lookup"><span data-stu-id="17ace-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="17ace-110">All authorised users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span><span class="sxs-lookup"><span data-stu-id="17ace-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="17ace-111">Creating and Publishing a Web Service</span><span class="sxs-lookup"><span data-stu-id="17ace-111">Creating and Publishing a Web Service</span></span>  
 <span data-ttu-id="17ace-112">The following steps explain how to create and publish a web service.</span><span class="sxs-lookup"><span data-stu-id="17ace-112">The following steps explain how to create and publish a web service.</span></span>  

#### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="17ace-113">To create and publish a web service</span><span class="sxs-lookup"><span data-stu-id="17ace-113">To create and publish a web service</span></span>  

1.  <span data-ttu-id="17ace-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Services**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="17ace-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Services**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="17ace-115">In the **Web Services** page, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="17ace-115">In the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    >  <span data-ttu-id="17ace-116">**Codeunit** and **Page** are valid types for SOAP web services.</span><span class="sxs-lookup"><span data-stu-id="17ace-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="17ace-117">**Page** and **Query** are valid types for OData web services.</span><span class="sxs-lookup"><span data-stu-id="17ace-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    <span data-ttu-id="17ace-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span><span class="sxs-lookup"><span data-stu-id="17ace-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    <span data-ttu-id="17ace-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span><span class="sxs-lookup"><span data-stu-id="17ace-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3.  <span data-ttu-id="17ace-120">Select the check box in the **Published** column.</span><span class="sxs-lookup"><span data-stu-id="17ace-120">Select the check box in the **Published** column.</span></span>  

     <span data-ttu-id="17ace-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span><span class="sxs-lookup"><span data-stu-id="17ace-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="17ace-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span><span class="sxs-lookup"><span data-stu-id="17ace-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="17ace-123">Optionally, you can copy the value of the field and save it for later use.</span><span class="sxs-lookup"><span data-stu-id="17ace-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

<span data-ttu-id="17ace-124">After you publish a web service, it is available to external parties.</span><span class="sxs-lookup"><span data-stu-id="17ace-124">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="17ace-125">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields in the **Web Services** window.</span><span class="sxs-lookup"><span data-stu-id="17ace-125">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields in the **Web Services** window.</span></span> <span data-ttu-id="17ace-126">The following procedure illustrates how you can verify the availability of the web service for later use.</span><span class="sxs-lookup"><span data-stu-id="17ace-126">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

#### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="17ace-127">To verify the availability of a web service</span><span class="sxs-lookup"><span data-stu-id="17ace-127">To verify the availability of a web service</span></span>  

1.  <span data-ttu-id="17ace-128">In your browser, enter the relevant URL.</span><span class="sxs-lookup"><span data-stu-id="17ace-128">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="17ace-129">The following table illustrates the types of URLs that you can enter.</span><span class="sxs-lookup"><span data-stu-id="17ace-129">The following table illustrates the types of URLs that you can enter.</span></span> <span data-ttu-id="17ace-130">For SOAP web services, use the following format for your URI.</span><span class="sxs-lookup"><span data-stu-id="17ace-130">For SOAP web services, use the following format for your URI.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="17ace-131">Web service type</span><span class="sxs-lookup"><span data-stu-id="17ace-131">Web service type</span></span></th>
    <th><span data-ttu-id="17ace-132">Syntax</span><span class="sxs-lookup"><span data-stu-id="17ace-132">Syntax</span></span></th>
    <th><span data-ttu-id="17ace-133">Example</span><span class="sxs-lookup"><span data-stu-id="17ace-133">Example</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="17ace-134">SOAP</span><span class="sxs-lookup"><span data-stu-id="17ace-134">SOAP</span></span></td>
    <td><span data-ttu-id="17ace-135">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span><span class="sxs-lookup"><span data-stu-id="17ace-135">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span></span></td>
    <td><span data-ttu-id="17ace-136">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="17ace-136">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="17ace-137">OData</span><span class="sxs-lookup"><span data-stu-id="17ace-137">OData</span></span></td>
    <td><span data-ttu-id="17ace-138">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span><span class="sxs-lookup"><span data-stu-id="17ace-138">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span></span></td>
    <td><span data-ttu-id="17ace-139">https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="17ace-139">https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com</span></span>

         The company name is case-sensitive.</td>
    </tr>
    </table>

2.  <span data-ttu-id="17ace-140">Review the information that is displayed in the browser.</span><span class="sxs-lookup"><span data-stu-id="17ace-140">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="17ace-141">Verify that you can see the name of the web service that you have created.</span><span class="sxs-lookup"><span data-stu-id="17ace-141">Verify that you can see the name of the web service that you have created.</span></span>  

 <span data-ttu-id="17ace-142">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span><span class="sxs-lookup"><span data-stu-id="17ace-142">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="17ace-143">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span><span class="sxs-lookup"><span data-stu-id="17ace-143">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="17ace-144">For example, the following URIs point to the same OData web service and are both valid URIs.</span><span class="sxs-lookup"><span data-stu-id="17ace-144">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```  
https://localhost:7048/server/OData/Company('CRONUS International Ltd.')/Customer  
```  

```  
https://localhost:7048/server/OData/Customer?company='CRONUS International Ltd.'  
```  

## <a name="see-also"></a><span data-ttu-id="17ace-145">See Also</span><span class="sxs-lookup"><span data-stu-id="17ace-145">See Also</span></span>  
[<span data-ttu-id="17ace-146">Setup and Administration in Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="17ace-146">Setup and Administration in Dynamics 365 for Financials</span></span>](admin-setup-and-administration.md)  

