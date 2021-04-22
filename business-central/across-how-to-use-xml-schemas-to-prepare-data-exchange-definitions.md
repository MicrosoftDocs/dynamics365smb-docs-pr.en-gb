---
title: Use XML Schemas to Prepare Data Exchange Definitions
description: Use XML schemas to set up the document exchange framework.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 70e80403175c6a77d120a3b405b1b5758410c227
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781369"
---
# <a name="use-xml-schemas-to-prepare-data-exchange-definitions"></a><span data-ttu-id="300a5-103">Use XML Schemas to Prepare Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="300a5-103">Use XML Schemas to Prepare Data Exchange Definitions</span></span>

<span data-ttu-id="300a5-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[prod_short](includes/prod_short.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="300a5-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[prod_short](includes/prod_short.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="300a5-105">You perform this work on the **XML Schema Viewer** page by loading the XML schema file, selecting the relevant data elements, and then initialising a data exchange definition.</span><span class="sxs-lookup"><span data-stu-id="300a5-105">You perform this work on the **XML Schema Viewer** page by loading the XML schema file, selecting the relevant data elements, and then initializing a data exchange definition.</span></span>  

 <span data-ttu-id="300a5-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate Data Exchange Definition** action to initialise a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span><span class="sxs-lookup"><span data-stu-id="300a5-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate Data Exchange Definition** action to initialize a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span></span> <span data-ttu-id="300a5-107">This creates a record on the **Posting Exchange Definition** page where you continue by defining which elements in the file map to which fields in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="300a5-107">This creates a record on the **Posting Exchange Definition** page where you continue by defining which elements in the file map to which fields in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="300a5-108">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="300a5-108">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

 <span data-ttu-id="300a5-109">This topic contains the following procedures:</span><span class="sxs-lookup"><span data-stu-id="300a5-109">This topic contains the following procedures:</span></span>  

- <span data-ttu-id="300a5-110">To load an XML schema file</span><span class="sxs-lookup"><span data-stu-id="300a5-110">To load an XML schema file</span></span>  

- <span data-ttu-id="300a5-111">To select or clear nodes in an XML schema</span><span class="sxs-lookup"><span data-stu-id="300a5-111">To select or clear nodes in an XML schema</span></span>  

- <span data-ttu-id="300a5-112">To generate a data exchange definition that is based on an XML schema</span><span class="sxs-lookup"><span data-stu-id="300a5-112">To generate a data exchange definition that is based on an XML schema</span></span>  

## <a name="to-load-an-xml-schema-file"></a><span data-ttu-id="300a5-113">To load an XML schema file</span><span class="sxs-lookup"><span data-stu-id="300a5-113">To load an XML schema file</span></span>

1. <span data-ttu-id="300a5-114">Make sure that the relevant XML schema file is available.</span><span class="sxs-lookup"><span data-stu-id="300a5-114">Make sure that the relevant XML schema file is available.</span></span> <span data-ttu-id="300a5-115">The file extension is .xsd.</span><span class="sxs-lookup"><span data-stu-id="300a5-115">The file extension is .xsd.</span></span>  

2. <span data-ttu-id="300a5-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schemas**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="300a5-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schemas**, and then choose the related link.</span></span>  

3. <span data-ttu-id="300a5-117">Choose the **New** action.</span><span class="sxs-lookup"><span data-stu-id="300a5-117">Choose the **New** action.</span></span>  

4. <span data-ttu-id="300a5-118">Fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="300a5-118">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="300a5-119">Field</span><span class="sxs-lookup"><span data-stu-id="300a5-119">Field</span></span>|<span data-ttu-id="300a5-120">Description</span><span class="sxs-lookup"><span data-stu-id="300a5-120">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="300a5-121">**Code**</span><span class="sxs-lookup"><span data-stu-id="300a5-121">**Code**</span></span>|<span data-ttu-id="300a5-122">Specify a code to identify the XML schema.</span><span class="sxs-lookup"><span data-stu-id="300a5-122">Specify a code to identify the XML schema.</span></span>|  
    |<span data-ttu-id="300a5-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="300a5-123">**Description**</span></span>|<span data-ttu-id="300a5-124">Specify a description of the XML schema.</span><span class="sxs-lookup"><span data-stu-id="300a5-124">Specify a description of the XML schema.</span></span>|  

     <span data-ttu-id="300a5-125">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span><span class="sxs-lookup"><span data-stu-id="300a5-125">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span></span>  

5. <span data-ttu-id="300a5-126">Choose the **Load Schema** action, and then select the XML schema file.</span><span class="sxs-lookup"><span data-stu-id="300a5-126">Choose the **Load Schema** action, and then select the XML schema file.</span></span>  

     <span data-ttu-id="300a5-127">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="300a5-127">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="300a5-128">The tree of the loaded XML schema is collapsed by default.</span><span class="sxs-lookup"><span data-stu-id="300a5-128">The tree of the loaded XML schema is collapsed by default.</span></span> <span data-ttu-id="300a5-129">You expand each node by choosing the **+** button on the node.</span><span class="sxs-lookup"><span data-stu-id="300a5-129">You expand each node by choosing the **+** button on the node.</span></span> <span data-ttu-id="300a5-130">To expand all nodes, choose **Expand All** on the ribbon.</span><span class="sxs-lookup"><span data-stu-id="300a5-130">To expand all nodes, choose **Expand All** on the ribbon.</span></span>  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a><span data-ttu-id="300a5-131">To select or clear nodes in an XML schema</span><span class="sxs-lookup"><span data-stu-id="300a5-131">To select or clear nodes in an XML schema</span></span>  

1. <span data-ttu-id="300a5-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schema Viewer**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="300a5-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **XML Schema Viewer**, and then choose the related link.</span></span>  

2. <span data-ttu-id="300a5-133">Fill the fields on the header as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="300a5-133">Fill the fields on the header as described in the following table.</span></span>  

    |<span data-ttu-id="300a5-134">Field</span><span class="sxs-lookup"><span data-stu-id="300a5-134">Field</span></span>|<span data-ttu-id="300a5-135">Description</span><span class="sxs-lookup"><span data-stu-id="300a5-135">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="300a5-136">**XML Schema Code**</span><span class="sxs-lookup"><span data-stu-id="300a5-136">**XML Schema Code**</span></span>|<span data-ttu-id="300a5-137">Specify the XML schema file that you loaded in step 5 in the "To load an XML schema file" section.</span><span class="sxs-lookup"><span data-stu-id="300a5-137">Specify the XML schema file that you loaded in step 5 in the "To load an XML schema file" section.</span></span>|  
    |<span data-ttu-id="300a5-138">**New XMLport No.**</span><span class="sxs-lookup"><span data-stu-id="300a5-138">**New XMLport No.**</span></span>|<span data-ttu-id="300a5-139">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span><span class="sxs-lookup"><span data-stu-id="300a5-139">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span></span>|  

     <span data-ttu-id="300a5-140">The lines are now filled with nodes representing all elements in the XML schema.</span><span class="sxs-lookup"><span data-stu-id="300a5-140">The lines are now filled with nodes representing all elements in the XML schema.</span></span> <span data-ttu-id="300a5-141">Nodes for elements that are mandatory according to the XML schema are selected by default.</span><span class="sxs-lookup"><span data-stu-id="300a5-141">Nodes for elements that are mandatory according to the XML schema are selected by default.</span></span>  

3. <span data-ttu-id="300a5-142">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span><span class="sxs-lookup"><span data-stu-id="300a5-142">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span></span>  

     <span data-ttu-id="300a5-143">Alternatively, right-click on a node and then choose **Expand All**.</span><span class="sxs-lookup"><span data-stu-id="300a5-143">Alternatively, right-click on a node and then choose **Expand All**.</span></span>  

4. <span data-ttu-id="300a5-144">Choose either of the following actions to change which nodes are displayed.</span><span class="sxs-lookup"><span data-stu-id="300a5-144">Choose either of the following actions to change which nodes are displayed.</span></span>  

    |<span data-ttu-id="300a5-145">**Action**</span><span class="sxs-lookup"><span data-stu-id="300a5-145">**Action**</span></span>|<span data-ttu-id="300a5-146">Description</span><span class="sxs-lookup"><span data-stu-id="300a5-146">Description</span></span>|  
    |----------------|---------------------------------------|  
    |<span data-ttu-id="300a5-147">**Show All**</span><span class="sxs-lookup"><span data-stu-id="300a5-147">**Show All**</span></span>|<span data-ttu-id="300a5-148">All nodes are shown.</span><span class="sxs-lookup"><span data-stu-id="300a5-148">All nodes are shown.</span></span>|  
    |<span data-ttu-id="300a5-149">**Hide Non-Mandatory**</span><span class="sxs-lookup"><span data-stu-id="300a5-149">**Hide Non-Mandatory**</span></span>|<span data-ttu-id="300a5-150">Only nodes representing elements that are required according to the XML schema are shown.</span><span class="sxs-lookup"><span data-stu-id="300a5-150">Only nodes representing elements that are required according to the XML schema are shown.</span></span> <span data-ttu-id="300a5-151">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span><span class="sxs-lookup"><span data-stu-id="300a5-151">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span></span><br /><br /> <span data-ttu-id="300a5-152">Choose **Show All** to reverse the view.</span><span class="sxs-lookup"><span data-stu-id="300a5-152">Choose **Show All** to reverse the view.</span></span>|  
    |<span data-ttu-id="300a5-153">**Hide Non-Selected**</span><span class="sxs-lookup"><span data-stu-id="300a5-153">**Hide Non-Selected**</span></span>|<span data-ttu-id="300a5-154">Only nodes where the **Selected** check box is selected are shown.</span><span class="sxs-lookup"><span data-stu-id="300a5-154">Only nodes where the **Selected** check box is selected are shown.</span></span><br /><br /> <span data-ttu-id="300a5-155">Choose **Show All** to reverse the view.</span><span class="sxs-lookup"><span data-stu-id="300a5-155">Choose **Show All** to reverse the view.</span></span>|  

5. <span data-ttu-id="300a5-156">Choose the **Edit** action.</span><span class="sxs-lookup"><span data-stu-id="300a5-156">Choose the **Edit** action.</span></span>  

6. <span data-ttu-id="300a5-157">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span><span class="sxs-lookup"><span data-stu-id="300a5-157">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="300a5-158">When you select a mandatory child node, all parent nodes above it are also selected.</span><span class="sxs-lookup"><span data-stu-id="300a5-158">When you select a mandatory child node, all parent nodes above it are also selected.</span></span>  

7. <span data-ttu-id="300a5-159">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span><span class="sxs-lookup"><span data-stu-id="300a5-159">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span></span>  

8. <span data-ttu-id="300a5-160">Choose the **Deselect All** action to clear all selections.</span><span class="sxs-lookup"><span data-stu-id="300a5-160">Choose the **Deselect All** action to clear all selections.</span></span>  

     <span data-ttu-id="300a5-161">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span><span class="sxs-lookup"><span data-stu-id="300a5-161">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span></span>  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a><span data-ttu-id="300a5-162">To generate a data exchange definition that is based on an XML schema</span><span class="sxs-lookup"><span data-stu-id="300a5-162">To generate a data exchange definition that is based on an XML schema</span></span>  

1. <span data-ttu-id="300a5-163">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter  **XML Schemas**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="300a5-163">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter  **XML Schemas**, and then choose the related link.</span></span>  

2. <span data-ttu-id="300a5-164">Select the relevant XML schema, and then choose the **Open XML Schema Viewer** action.</span><span class="sxs-lookup"><span data-stu-id="300a5-164">Select the relevant XML schema, and then choose the **Open XML Schema Viewer** action.</span></span>  

3. <span data-ttu-id="300a5-165">Make sure the relevant nodes are selected.</span><span class="sxs-lookup"><span data-stu-id="300a5-165">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="300a5-166">For more information, see the "To select or clear nodes in an XML schema" section.</span><span class="sxs-lookup"><span data-stu-id="300a5-166">For more information, see the "To select or clear nodes in an XML schema" section.</span></span>  

4. <span data-ttu-id="300a5-167">On the **XML Schema Viewer** page, choose the **Generate Data Exchange Definition** action.</span><span class="sxs-lookup"><span data-stu-id="300a5-167">On the **XML Schema Viewer** page, choose the **Generate Data Exchange Definition** action.</span></span>  

 <span data-ttu-id="300a5-168">A data exchange definition is created on the **Posting Exchange Definition** page, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="300a5-168">A data exchange definition is created on the **Posting Exchange Definition** page, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="300a5-169">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="300a5-169">For more information, see [Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

> [!NOTE]  
> <span data-ttu-id="300a5-170">You can also use the **Get File Structure** function from the **Posting Exchange Definition** page, which uses the functionality of the **XML Schema Viewer** page to prefill the **Column Definitions** TastTab.</span><span class="sxs-lookup"><span data-stu-id="300a5-170">You can also use the **Get File Structure** function from the **Posting Exchange Definition** page, which uses the functionality of the **XML Schema Viewer** page to prefill the **Column Definitions** TastTab.</span></span>  

> [!NOTE]
> <span data-ttu-id="300a5-171">In 2019 release wave 1 and earlier versions, you could generate an XMLport that was based on the schema and then import that into your solution.</span><span class="sxs-lookup"><span data-stu-id="300a5-171">In 2019 release wave 1 and earlier versions, you could generate an XMLport that was based on the schema and then import that into your solution.</span></span> <span data-ttu-id="300a5-172">This is no longer supported.</span><span class="sxs-lookup"><span data-stu-id="300a5-172">This is no longer supported.</span></span>

## <a name="see-also"></a><span data-ttu-id="300a5-173">See Also</span><span class="sxs-lookup"><span data-stu-id="300a5-173">See Also</span></span>

[<span data-ttu-id="300a5-174">Set Up Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="300a5-174">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="300a5-175">Export Payments to a Bank File</span><span class="sxs-lookup"><span data-stu-id="300a5-175">Export Payments to a Bank File</span></span>](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file)  
[<span data-ttu-id="300a5-176">Collect Payments with SEPA Direct Debit</span><span class="sxs-lookup"><span data-stu-id="300a5-176">Collect Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)  
[<span data-ttu-id="300a5-177">About the Data Exchange Framework</span><span class="sxs-lookup"><span data-stu-id="300a5-177">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]