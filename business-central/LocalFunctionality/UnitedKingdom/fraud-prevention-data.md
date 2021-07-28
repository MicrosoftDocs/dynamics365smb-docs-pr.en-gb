---
title: Send Fraud Prevention Data (UK)
description: Business Central supports the British requirement to submit fraud prevention data to HMRC as part of Making Tax Digital. This article describes how to set up the required headers.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: fraud prevention, making tax digital, making tax digital software, hmrc, tax
ms.date: 06/30/2021
ms.author: edupont
ms.openlocfilehash: 9e787bb646951a986173bb2e0592fbe8ebbd8831
ms.sourcegitcommit: c7e084f9822796e75491f5950d97d41dd7c05aef
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 07/01/2021
ms.locfileid: "6330996"
---
# <a name="send-fraud-prevention-data-in-the-united-kingdom"></a>Send Fraud Prevention Data in the United Kingdom

Communication with Her Majesty's Revenue and Customs (HMRC) without fraud prevention headers is not allowed, starting in 2021. [!INCLUDE [prod_short](../../includes/prod_short.md)] communicates with HMRC through Making Tax Digital and supports the requirement to submit data that can help prevent fraud.  

> [!IMPORTANT]
> Make sure that you have the latest version of the Making Tax Digital app. For more information, see [Making Tax Digital in the United Kingdom](making-tax-digital-submit-vat-return.md).

The admin of the company that transmits VAT data together with fraud prevention parameters must consent one time for each web application that is used for interoperation with the HMRC VAT APIs. Otherwise, data that is collected from the user devices that are used to submit the VAT requests cannot be transmitted.

> [!NOTE]
> We recommend that it's always the same person who submits data to HMRC from the same device. This way, the fraud prevention headers contain consistent information about the device.

## <a name="fraud-prevention-headers"></a>Fraud prevention headers

[!INCLUDE [prod_short](../../includes/prod_short.md)] online generates fraud prevention headers for you. For on-premises, you can verify the headers in the **HMRC Fraud Prevention Headers Setup** page. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)] Choose the **Get Current Headers** action to see which headers cannot be retrieved automatically. Find tips for how to find the missing information in the [Identify values for missing headers](#identify-values-for-missing-headers) section.  

Fraud prevention headers are sent to HMRC whenever there is communication with the APIs at HMRC. In other words, this information is sent when one of the following actions are chosen in [!INCLUDE [prod_short](../../includes/prod_short.md)]:

* Get VAT return periods
* Submit VAT return
* Get status of submitted VAT return

When you start one of these processes, you are presented with the current header content and asked for consent before the any data is sent. If you choose to cancel, no information is sent to HMRC.

> [!NOTE]
> The **Get Current Headers** action fetches data based on the current user. That means that if you are not the user who will submit the final data to HMRC, you will see different data for those headers that include person identifiable information (PII).

### <a name="headers"></a>Headers

In this section, we provide a list of fraud prevention headers. The content is intended to help you identify any issues with fraud prevention headers for your company.  

The set of HTTP headers that must be transmitted for fraud prevention varies, depending on the architecture of the environment that is used by the company that is interoperating with MTD for VAT. The **Gov-Client-Connection-Method** header must represent the connection method that is used for the request that the company makes. It's assumed that most companies that use [!INCLUDE [prod_short](../../includes/prod_short.md)] online use the **WEB\_APP\_VIA\_SERVER** connection method.  

The **WEB\_APP\_VIA\_SERVER** connection method assumes transmission of headers as outlined in the following table.

| HTTP header | Description |
|--|--|
| Gov-Client-Public-IP | The public IP address (IPv4 or IPv6) that the originating device makes the request from. |
| Gov-Client-Public-Port | The public TCP port that the originating device uses when it initiates the request. |
| Gov-Client-Device-ID | An identifier that is unique to an originating device. |
| Gov-Client-User-IDs | A key-value data structure that contains the user identifiers. |
| Gov-Client-Timezone | The local time zone of the originating device. |
| Gov-Client-Local-IPs | A list of all local IP addresses (IPv4 and IPv6) that are available to the originating device. |
| Gov-Client-Screens | Information that is related to the originating device's screens. The following fields are included:<ul><li><strong>width</strong> – The reported width of the screen, in pixels</li><li><strong>height</strong> – The reported height of the screen, in pixels</li><li><strong>scaling-factor</strong> – The reported scaling factor of the screen. For example, a high-pixel density screen could have a scaling factor of 2, while a standard definition screen could have a scaling factor of 1.</li><li><strong>colour-depth</strong> – The colour depth of the screen, in bits.</li></ul> |
| Gov-Client-Window-Size | The number of pixels of the window on the originating device where the user initiated (directly or indirectly) the API call to HMRC. |
| Gov-Client-Browser-Plugins | A list of browser plug-ins on the originating device. |
| Gov-Client-Browser-JS-User-Agent | The JavaScript-reported user agent string from the originating device. |
| Gov-Client-Browser-Do-Not-Track | A value that indicates whether the **Do Not Track** option is turned on in the browser. |
| Gov-Client-Multi-Factor | A list of key-value data structures that contains details of the multifactor authentication (MFA) statuses that are related to the API call. |
| Gov-Supplier-Version | A key-value data structure of the software versions that are involved in handling a request. |
| Gov-Supplier-licence-IDs | A key-value data structure of hashed licence keys that are related to the supplier software that initiated the API request on the originating device. |
| Gov-Supplier-Public-IP | The public IP address of the servers that the originating device sent its requests to. |
| Gov-Supplier-Forwarded | A list that details the hops over the internet between services that terminate Transport Layer Security (TLS). |

## <a name="identify-values-for-missing-headers"></a>Identify values for missing headers

When you run the **Get Current Headers** process in the **HMRC Fraud Prevention Headers Setup** page, some headers may return an error that values are missing. The following table proposes how you can identify values for such missing headers. The guidance is based on an example from one of our reselling partners in the UK. The content is intended to help you set up fraud prevention headers for your company.  

|Header|Description  |Example  |Notes  |
|---------|---------|---------|---------|
|Gov-Client-Browser-Do-Not-Track |`true` or `false`, depending on your browser's setting for tracking.         | `Gov-Client-Browser-Do-Not-Track: false`        | `false` by default. Check the value in your browser's settings. You can also search online for *do not track option in (name of browser)*.       |
|Gov-Client-Browser-JS-User-Agent | JavaScript-reported user agent string from the originating device. Pass the value as reported by the browser, usually in this format:`product / product-version (system-information) platform (platform-details) extensions`|`Gov-Client-Browser-JS-User-Agent: Mozilla/5.0 (iPad; U; CPU OS 3 2_1 like Mac OS X; en-us) (KHTML, like Gecko) Mobile/7B405`| Search for *device information online* to get the information about the device and the browser. Combine the values using the described format. |
|Gov-Client-Browser-Plugins| A list of browser plugins on the originating device. Every value in the list must be percent encoded (opens in a new tab), not percent encode separators (commas).  |`Gov-Client-Browser-P1ugins: Shockwave%20F1ash Chromium%20PDF%20Viewer`| Search for *device information online* to get the information about the device and the browser. Separate all the values with commas. Then search for *encode url online*.        |
|Gov-Client-Local-Ips |  IP addresses.       |<ul><li>`Gov-Client-Local-IPs:  10 .1. 2.3`</li><li>`Gov-Client-Local-IPs: 10.1. 2. 3,10.3.4. 2`</li><li>`Gov-Client-Local-IPs: 65f466e3-1f39-4ca5-957f-65e231804f91.local`</li></ul>| If you don't know your IP address, search for *how to identify my local IP*. Alternatively, use a PowerShell command such as the following: <br>`Test-Connection -ComputerName (hostname) -Count 1 \| Select IPV4Address`|
|Gov-Client-Public-Port|The public TCP port used by the originating device when initiating the request. This must not be a server port, such as 80 for http connections or 443 for https connections. The valid range is between 0 and 65535.|`57961`|Run ```netstat -a``` and see the TCP connection. For example, if your IP address is 192.168.45.2 and you see an entry for 192.168.45.2:57961, it means that port number 57961 is open and possibly in use. You can choose this value.|
|Gov-Client-Screens|Information about the originating device's screen. These fields should be submitted as a list of key-value data structures, and you can see a description of the keys in the table in the [Headers](#headers) section. |`Gov-Client-Screens: width=1920&height=1080&sca1ing-factor=1.25&colour-depth=16`|Find the details about your monitor in the display settings. Combine the values using the format.|
|Gov-Supplier-Public-IP|The public IP address of the servers the originating device sent their requests to.|`Gov -Vendor-Public-IP: 203.0.113.6`|Search for *what is my public ip address?*.|
|Gov-Supplier-Forwarded|A list that details bops over the internet between services that terminate Transport Layer Security (TLS).|`Gov-vendor-Forwarded:by=203.0.113.6&for=198.51.100.0`|`by` = public ID. `for` = local IP.|

## <a name="see-also"></a>See Also

[Making Tax Digital](making-tax-digital-submit-vat-return.md)  
[United Kingdom Local Functionality](united-kingdom-local-functionality.md)  
[Customising [!INCLUDE[prod_short](../../includes/prod_short.md)] Using Extensions](../../ui-extensions.md)  
[Working with [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
