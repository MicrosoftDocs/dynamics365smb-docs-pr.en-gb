---
title: Create XMLports based on XML schemas | Microsoft Docs
description: Use XML schemas to set yup the document exchange framework.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 5b10eaff0d412ee26ead2137a353054c41d05113
ms.contentlocale: en-gb
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-use-xml-schemas-to-prepare-data-exchange-definitions"></a><span data-ttu-id="b0c8d-103">How to: Use XML Schemas to Prepare Data Exchange Definitions</span><span class="sxs-lookup"><span data-stu-id="b0c8d-103">How to: Use XML Schemas to Prepare Data Exchange Definitions</span></span>
<span data-ttu-id="b0c8d-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b0c8d-104">To enable import/export of data in XML files through the data exchange framework in [!INCLUDE[d365fin](includes/d365fin_md.md)], you can use XML schemas to define which data elements you want to exchange with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b0c8d-105">You perform this work in the **XML Schema Viewer** window by loading the XML schema file, selecting the relevant data elements, and then initialising either a data exchange definition or an XMLport.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-105">You perform this work in the **XML Schema Viewer** window by loading the XML schema file, selecting the relevant data elements, and then initializing either a data exchange definition or an XMLport.</span></span>  

 <span data-ttu-id="b0c8d-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate XMLport** action to create the XMLport object.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-106">When you have defined which data elements to include based on the XML schema, you can use the **Generate XMLport** action to create the XMLport object.</span></span>  

 <span data-ttu-id="b0c8d-107">Alternatively, you can use the **Generate Data Exchange Definition** action to initialise a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-107">Alternatively, you can use the **Generate Data Exchange Definition** action to initialize a data exchange definition based on the selected data elements, which you then complete in the Data Exchange Framework.</span></span> <span data-ttu-id="b0c8d-108">This creates a record in the **Posting Exchange Definition** window where you continue by defining which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b0c8d-108">This creates a record in the **Posting Exchange Definition** window where you continue by defining which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b0c8d-109">For more information, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="b0c8d-109">For more information, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

 <span data-ttu-id="b0c8d-110">This topic contains the following procedures:</span><span class="sxs-lookup"><span data-stu-id="b0c8d-110">This topic contains the following procedures:</span></span>  

-   <span data-ttu-id="b0c8d-111">To load an XML schema file</span><span class="sxs-lookup"><span data-stu-id="b0c8d-111">To load an XML schema file</span></span>  

-   <span data-ttu-id="b0c8d-112">To select or clear nodes in an XML schema</span><span class="sxs-lookup"><span data-stu-id="b0c8d-112">To select or clear nodes in an XML schema</span></span>  

-   <span data-ttu-id="b0c8d-113">To generate a data exchange definition that is based on an XML schema</span><span class="sxs-lookup"><span data-stu-id="b0c8d-113">To generate a data exchange definition that is based on an XML schema</span></span>  

-   <span data-ttu-id="b0c8d-114">To generate an XMLport for the file that is based on an XML schema</span><span class="sxs-lookup"><span data-stu-id="b0c8d-114">To generate an XMLport for the file that is based on an XML schema</span></span>  

-   <span data-ttu-id="b0c8d-115">To import an XMLport into the Object Designer</span><span class="sxs-lookup"><span data-stu-id="b0c8d-115">To import an XMLport into the Object Designer</span></span>  

### <a name="to-load-an-xml-schema-file"></a><span data-ttu-id="b0c8d-116">To load an XML schema file</span><span class="sxs-lookup"><span data-stu-id="b0c8d-116">To load an XML schema file</span></span>  

1.  <span data-ttu-id="b0c8d-117">Make sure that the relevant XML schema file is available.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-117">Make sure that the relevant XML schema file is available.</span></span> <span data-ttu-id="b0c8d-118">The file extension is .xsd.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-118">The file extension is .xsd.</span></span>  

2.  <span data-ttu-id="b0c8d-119">In the **Search** box, enter **XML Schemas**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-119">In the **Search** box, enter **XML Schemas**, and then choose the related link.</span></span>  

3.  <span data-ttu-id="b0c8d-120">On the **Home** tab, in the **New** group, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-120">On the **Home** tab, in the **New** group, choose **New**.</span></span>  

4.  <span data-ttu-id="b0c8d-121">Fill the fields as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-121">Fill the fields as described in the following table.</span></span>  

    |<span data-ttu-id="b0c8d-122">Field</span><span class="sxs-lookup"><span data-stu-id="b0c8d-122">Field</span></span>|<span data-ttu-id="b0c8d-123">Description</span><span class="sxs-lookup"><span data-stu-id="b0c8d-123">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="b0c8d-124">**Code**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-124">**Code**</span></span>|<span data-ttu-id="b0c8d-125">Specify a code to identify the XML schema.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-125">Specify a code to identify the XML schema.</span></span>|  
    |<span data-ttu-id="b0c8d-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-126">**Description**</span></span>|<span data-ttu-id="b0c8d-127">Specify a description of the XML schema.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-127">Specify a description of the XML schema.</span></span>|  

     <span data-ttu-id="b0c8d-128">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-128">The **Target Namespace** field specifies any namespace in the XML schema file that has been loaded for the line.</span></span>  

5.  <span data-ttu-id="b0c8d-129">On the **Home** tab, in the **Process** group, choose **Load Schema**, and then select the XML schema file.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-129">On the **Home** tab, in the **Process** group, choose **Load Schema**, and then select the XML schema file.</span></span>  

     <span data-ttu-id="b0c8d-130">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-130">When the file is loaded, the rest of the fields on the line are filled with information from the file, and the **Schema is Loaded** check box is selected.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b0c8d-131">The tree of the loaded XML schema is collapsed by default.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-131">The tree of the loaded XML schema is collapsed by default.</span></span> <span data-ttu-id="b0c8d-132">You expand each node by choosing the **+** button on the node.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-132">You expand each node by choosing the **+** button on the node.</span></span> <span data-ttu-id="b0c8d-133">To expand all nodes, choose **Expand All** on the ribbon.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-133">To expand all nodes, choose **Expand All** on the ribbon.</span></span>  

### <a name="to-select-or-clear-nodes-in-an-xml-schema"></a><span data-ttu-id="b0c8d-134">To select or clear nodes in an XML schema</span><span class="sxs-lookup"><span data-stu-id="b0c8d-134">To select or clear nodes in an XML schema</span></span>  

1.  <span data-ttu-id="b0c8d-135">In the **Search** box, enter **XML Schema Viewer**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-135">In the **Search** box, enter **XML Schema Viewer**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="b0c8d-136">Fill the fields on the header as described in the following table.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-136">Fill the fields on the header as described in the following table.</span></span>  

    |<span data-ttu-id="b0c8d-137">Field</span><span class="sxs-lookup"><span data-stu-id="b0c8d-137">Field</span></span>|<span data-ttu-id="b0c8d-138">Description</span><span class="sxs-lookup"><span data-stu-id="b0c8d-138">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="b0c8d-139">**XML Schema Code**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-139">**XML Schema Code**</span></span>|<span data-ttu-id="b0c8d-140">Specify the XML schema file that you loaded in step 5 in the “To load an XML schema file” section.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-140">Specify the XML schema file that you loaded in step 5 in the “To load an XML schema file” section.</span></span>|  
    |<span data-ttu-id="b0c8d-141">**New XMLport No.**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-141">**New XMLport No.**</span></span>|<span data-ttu-id="b0c8d-142">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-142">Specify the number of the XMLport that is created from this XML schema when you choose the **Generate XMLport** action.</span></span>|  

     <span data-ttu-id="b0c8d-143">The lines are now filled with nodes representing all elements in the XML schema.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-143">The lines are now filled with nodes representing all elements in the XML schema.</span></span> <span data-ttu-id="b0c8d-144">Nodes for elements that are mandatory according to the XML schema are selected by default.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-144">Nodes for elements that are mandatory according to the XML schema are selected by default.</span></span>  

3.  <span data-ttu-id="b0c8d-145">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-145">On the first line, in the **Node Name** column, expand the **Document** node, and then gradually expand underlying nodes that you want to review.</span></span>  

     <span data-ttu-id="b0c8d-146">Alternatively, right-click on a node and then choose **Expand All**.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-146">Alternatively, right-click on a node and then choose **Expand All**.</span></span>  

4.  <span data-ttu-id="b0c8d-147">On the **Home** tab, in the **View** group, choose either of the following actions to change which nodes are displayed.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-147">On the **Home** tab, in the **View** group, choose either of the following actions to change which nodes are displayed.</span></span>  

    |<span data-ttu-id="b0c8d-148">**Action**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-148">**Action**</span></span>|<span data-ttu-id="b0c8d-149">Description</span><span class="sxs-lookup"><span data-stu-id="b0c8d-149">Description</span></span>|  
    |----------------|---------------------------------------|  
    |<span data-ttu-id="b0c8d-150">**Show All**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-150">**Show All**</span></span>|<span data-ttu-id="b0c8d-151">All nodes are shown.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-151">All nodes are shown.</span></span>|  
    |<span data-ttu-id="b0c8d-152">**Hide Non-Mandatory**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-152">**Hide Non-Mandatory**</span></span>|<span data-ttu-id="b0c8d-153">Only nodes representing elements that are required according to the XML schema are shown.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-153">Only nodes representing elements that are required according to the XML schema are shown.</span></span> <span data-ttu-id="b0c8d-154">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-154">These nodes are typically indicated by a **1** in the **MinOccurs** field.</span></span><br /><br /> <span data-ttu-id="b0c8d-155">Choose **Show All** to reverse the view.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-155">Choose **Show All** to reverse the view.</span></span>|  
    |<span data-ttu-id="b0c8d-156">**Hide Non-Selected**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-156">**Hide Non-Selected**</span></span>|<span data-ttu-id="b0c8d-157">Only nodes where the **Selected** check box is selected are shown.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-157">Only nodes where the **Selected** check box is selected are shown.</span></span><br /><br /> <span data-ttu-id="b0c8d-158">Choose **Show All** to reverse the view.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-158">Choose **Show All** to reverse the view.</span></span>|  

5.  <span data-ttu-id="b0c8d-159">On the **Home** tab, in the **Manage** group, choose **Edit**.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-159">On the **Home** tab, in the **Manage** group, choose **Edit**.</span></span>  

6.  <span data-ttu-id="b0c8d-160">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-160">In the **Selected** check box, specify for each node if you want the element to be supported in the data exchange definition for the related SEPA bank file.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b0c8d-161">When you select a mandatory child node, all parent nodes above it are also selected.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-161">When you select a mandatory child node, all parent nodes above it are also selected.</span></span>  

7.  <span data-ttu-id="b0c8d-162">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-162">Choose the **Select All Mandatory Elements** action to reselect all nodes that represent elements that are mandatory according to the XML schema.</span></span>  

8.  <span data-ttu-id="b0c8d-163">Choose the **Deselect All** action to clear all selections.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-163">Choose the **Deselect All** action to clear all selections.</span></span>  

     <span data-ttu-id="b0c8d-164">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-164">The **Choice** field specifies that the node has two or more sibling nodes that function as options.</span></span>  

### <a name="to-generate-a-data-exchange-definition-that-is-based-on-an-xml-schema"></a><span data-ttu-id="b0c8d-165">To generate a data exchange definition that is based on an XML schema</span><span class="sxs-lookup"><span data-stu-id="b0c8d-165">To generate a data exchange definition that is based on an XML schema</span></span>  

1.  <span data-ttu-id="b0c8d-166">In the **Search** box, enter  **XML Schemas**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-166">In the **Search** box, enter  **XML Schemas**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="b0c8d-167">Select the relevant XML schema, and then on the on the **Home** tab, in the **Process** group, choose **Open XML Schema Viewer**.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-167">Select the relevant XML schema, and then on the on the **Home** tab, in the **Process** group, choose **Open XML Schema Viewer**.</span></span>  

3.  <span data-ttu-id="b0c8d-168">Make sure the relevant nodes are selected.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-168">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="b0c8d-169">For more information, see the “To select or clear nodes in an XML schema” section.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-169">For more information, see the “To select or clear nodes in an XML schema” section.</span></span>  

4.  <span data-ttu-id="b0c8d-170">In the **XML Schema Viewer** window, on the **Home** tab, in the **Process** group, choose **Generate Data Exchange Definition**.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-170">In the **XML Schema Viewer** window, on the **Home** tab, in the **Process** group, choose **Generate Data Exchange Definition**.</span></span>  

 <span data-ttu-id="b0c8d-171">A data exchange definition is created in the **Posting Exchange Definition** window, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b0c8d-171">A data exchange definition is created in the **Posting Exchange Definition** window, which you can complete by specifying which elements in the file map to which fields in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b0c8d-172">For more information, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="b0c8d-172">For more information, see [How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="b0c8d-173">You can also use the **Get File Structure** function from the **Posting Exchange Definition** window, which uses the functionality of the **XML Schema Viewer** window to prefill the **Column Definitions** TastTab.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-173">You can also use the **Get File Structure** function from the **Posting Exchange Definition** window, which uses the functionality of the **XML Schema Viewer** window to prefill the **Column Definitions** TastTab.</span></span>  

### <a name="to-generate-an-xmlport-that-is-based-on-an-xml-schema"></a><span data-ttu-id="b0c8d-174">To generate an XMLport that is based on an XML schema</span><span class="sxs-lookup"><span data-stu-id="b0c8d-174">To generate an XMLport that is based on an XML schema</span></span>  

1.  <span data-ttu-id="b0c8d-175">In the **Search** box, enter  **XML Schemas**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-175">In the **Search** box, enter  **XML Schemas**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="b0c8d-176">Select the relevant XML schema, and then on the on the **Home** tab, in the **Process** group, choose **Open XML Schema Viewer**.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-176">Select the relevant XML schema, and then on the on the **Home** tab, in the **Process** group, choose **Open XML Schema Viewer**.</span></span>  

3.  <span data-ttu-id="b0c8d-177">In the **New XMLport No.**</span><span class="sxs-lookup"><span data-stu-id="b0c8d-177">In the **New XMLport No.**</span></span> <span data-ttu-id="b0c8d-178">field, specify the number that the new XMLport object will be given when it is generated.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-178">field, specify the number that the new XMLport object will be given when it is generated.</span></span>  

4.  <span data-ttu-id="b0c8d-179">Make sure the relevant nodes are selected.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-179">Make sure the relevant nodes are selected.</span></span> <span data-ttu-id="b0c8d-180">For more information, see the “To select or clear nodes in an XML schema” section.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-180">For more information, see the “To select or clear nodes in an XML schema” section.</span></span>  

5.  <span data-ttu-id="b0c8d-181">On the **Home** tab, in the **Process** group, choose **Generate XMLport**, and then save the object as a .txt file in an appropriate location.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-181">On the **Home** tab, in the **Process** group, choose **Generate XMLport**, and then save the object as a .txt file in an appropriate location.</span></span>  

6. <span data-ttu-id="b0c8d-182">Import the new XMLport into the [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment and compile it.</span><span class="sxs-lookup"><span data-stu-id="b0c8d-182">Import the new XMLport into the [!INCLUDE[d365fin](includes/d365fin_md.md)] development environment and compile it.</span></span>

## <a name="see-also"></a><span data-ttu-id="b0c8d-183">See Also</span><span class="sxs-lookup"><span data-stu-id="b0c8d-183">See Also</span></span>  
<span data-ttu-id="b0c8d-184">[How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) </span><span class="sxs-lookup"><span data-stu-id="b0c8d-184">[How to: Set Up Data Exchange Definitions](across-how-to-set-up-data-exchange-definitions.md) </span></span>  
<span data-ttu-id="b0c8d-185">[How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md) </span><span class="sxs-lookup"><span data-stu-id="b0c8d-185">[How to: Export Payments to a Bank File](payables-how-export-payments-bank-file.md) </span></span>  
<span data-ttu-id="b0c8d-186">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="b0c8d-186">[Collecting Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
[<span data-ttu-id="b0c8d-187">About the Data Exchange Framework</span><span class="sxs-lookup"><span data-stu-id="b0c8d-187">About the Data Exchange Framework</span></span>](across-about-the-data-exchange-framework.md)

